# Comparing `tmp/design.plone.contenttypes-6.2.1.tar.gz` & `tmp/design.plone.contenttypes-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.contenttypes-6.2.1.tar", last modified: Thu Mar  7 14:37:25 2024, max compression
+gzip compressed data, was "design.plone.contenttypes-6.2.2.tar", last modified: Tue Mar 19 08:35:45 2024, max compression
```

## Comparing `design.plone.contenttypes-6.2.1.tar` & `design.plone.contenttypes-6.2.2.tar`

### file list

```diff
@@ -1,374 +1,374 @@
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.275576 design.plone.contenttypes-6.2.1/
--rw-r--r--   0 filippocampi   (501) staff       (20)    23124 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/CHANGES.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)       67 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/CONTRIBUTORS.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)      585 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/DEVELOP.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)    18092 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/LICENSE.GPL
--rw-r--r--   0 filippocampi   (501) staff       (20)      665 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/LICENSE.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)      158 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/MANIFEST.in
--rw-r--r--   0 filippocampi   (501) staff       (20)    41226 2024-03-07 14:37:25.275323 design.plone.contenttypes-6.2.1/PKG-INFO
--rw-r--r--   0 filippocampi   (501) staff       (20)    15960 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/README.md
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.107640 design.plone.contenttypes-6.2.1/docs/
--rw-r--r--   0 filippocampi   (501) staff       (20)     7993 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/docs/conf.py
--rw-r--r--   0 filippocampi   (501) staff       (20)       98 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/docs/index.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)       62 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/requirements.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      383 2024-03-07 14:37:25.276711 design.plone.contenttypes-6.2.1/setup.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     3005 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/setup.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.088385 design.plone.contenttypes-6.2.1/src/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.108179 design.plone.contenttypes-6.2.1/src/design/
--rw-r--r--   0 filippocampi   (501) staff       (20)       80 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.112367 design.plone.contenttypes-6.2.1/src/design/plone/
--rw-r--r--   0 filippocampi   (501) staff       (20)       80 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.115694 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/
--rw-r--r--   0 filippocampi   (501) staff       (20)      668 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.119198 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      892 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      421 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/interfaces.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      930 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/query.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1755 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      231 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/servizi_correlati.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.134969 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1354 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/additional_help_infos.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2403 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/address.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     8986 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/argomenti.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    11818 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     6469 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/contatti.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1589 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/dataset_correlati.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2679 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6212 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/evento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1060 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/exclude_from_search.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1657 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/geolocation.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2388 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/info_testata.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2739 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6540 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/luogo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1606 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/multi_file.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4439 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/news_additional_fields.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1787 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/servizi_correlati.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1357 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/show_modified.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1648 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/strutture_correlate.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    10452 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/trasparenza.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1165 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/update_note.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.136536 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1333 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.137100 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/overrides/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/overrides/.gitkeep
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.091592 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/static/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.137571 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/static/js/
--rw-r--r--   0 filippocampi   (501) staff       (20)      262 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/static/js/move_content.js
--rw-r--r--   0 filippocampi   (501) staff       (20)      469 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/trasparenza.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.143757 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3813 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/change_news_type.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     8270 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_documenti.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     7290 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_eventi.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     7550 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_luoghi.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     8729 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_notizie.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     8573 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_persone.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    10794 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_servizi.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     7594 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_uo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3467 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1571 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/export_incarichi.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2796 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/move_news_items.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.148579 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/
--rw-r--r--   0 filippocampi   (501) staff       (20)     3360 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     6399 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     6372 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     6388 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     8600 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     6167 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     9179 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     6177 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     4760 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     3797 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/utils.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     3122 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.158284 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      315 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/cartella_modulistica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      238 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/dataset.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      246 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/documento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      283 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/documento_personale.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      210 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/evento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      242 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/incarico.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      215 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/luogo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      275 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/messaggio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      229 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/modulo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      271 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/pagina_argomento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      238 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/persona.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      238 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/pratica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      272 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/punto_di_contatto.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      279 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/ricevuta_pagamento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      242 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/servizio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      283 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/content/unita_organizzativa.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.160204 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      737 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1382 2024-03-07 14:37:23.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3865 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/settings.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.162745 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5779 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/common.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1189 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      618 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/document.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      536 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/incarico.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      969 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/pagina_argomento.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.167564 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      458 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/bando.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1119 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/common.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1803 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      411 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/events.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      921 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/news.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      621 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/pagina_argomento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      829 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/persona.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      741 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/punto_di_contatto.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      470 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/servizio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      445 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/uo.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.175364 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/
--rw-r--r--   0 filippocampi   (501) staff       (20)      419 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6263 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/bando.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      699 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      857 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/dataset.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     8557 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/documento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4702 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/documento_personale.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5442 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/incarico.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1483 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/messaggio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      205 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/modulo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2560 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/pagina_argomento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5024 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/persona.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1781 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/pratica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2850 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1838 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    18229 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/servizio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     7904 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.178195 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/
--rw-r--r--   0 filippocampi   (501) staff       (20)      611 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/README.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.094152 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/__pycache__/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.178641 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
--rw-r--r--   0 filippocampi   (501) staff       (20)    83688 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 filippocampi   (501) staff       (20)    83643 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.094624 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/en/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.179239 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
--rw-r--r--   0 filippocampi   (501) staff       (20)    83808 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.095101 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.180898 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
--rw-r--r--   0 filippocampi   (501) staff       (20)     1243 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
--rw-r--r--   0 filippocampi   (501) staff       (20)    84783 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 filippocampi   (501) staff       (20)     7287 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/plone.pot
--rw-r--r--   0 filippocampi   (501) staff       (20)     1597 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/update.py
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      512 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/update.sh
--rw-r--r--   0 filippocampi   (501) staff       (20)      712 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/overrides.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.182605 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/
--rw-r--r--   0 filippocampi   (501) staff       (20)      516 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3700 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/baseserializer.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      483 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      343 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/patches.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2751 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/permissions.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.097614 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.096059 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.200322 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
--rw-r--r--   0 filippocampi   (501) staff       (20)      314 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     3401 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      331 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     4370 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      286 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2870 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      372 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     8078 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      300 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2156 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      313 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)    13732 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      398 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     5133 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      292 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     1042 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      303 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2196 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      265 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)    15346 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      322 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     1015 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      355 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     3138 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      342 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2275 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      344 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2275 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.205261 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/
--rw-r--r--   0 filippocampi   (501) staff       (20)      799 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/actions.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      193 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2919 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/catalog.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1040 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/controlpanel.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1219 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      595 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/metadata.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.206515 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/registry/
--rw-r--r--   0 filippocampi   (501) staff       (20)    19836 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      618 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/registry/settings.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1139 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/repositorytool.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     4491 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.217485 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/
--rw-r--r--   0 filippocampi   (501) staff       (20)     1155 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Bando.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      503 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3563 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3327 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1001 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3747 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Documento.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3321 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2501 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      345 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Folder.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3427 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      506 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3199 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2908 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1194 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3456 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3430 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Persona.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3178 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3342 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3149 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3829 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3775 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2212 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Venue.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1194 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.218208 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/fix_syndication/
--rw-r--r--   0 filippocampi   (501) staff       (20)      520 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.219338 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/to_3000/
--rw-r--r--   0 filippocampi   (501) staff       (20)      377 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      275 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/to_3000/registry.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.220105 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/uninstall/
--rw-r--r--   0 filippocampi   (501) staff       (20)      128 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.222350 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      663 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      504 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/converters.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      702 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/correlati.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.227299 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      760 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     5795 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/documento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6050 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5743 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/news.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1658 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/persona.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5844 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/servizio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5999 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6016 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/venue.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.234742 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1548 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/bando.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2086 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1976 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2102 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/documento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2837 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     7597 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/dxfields.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1407 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/modulo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2360 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/persona.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3726 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1763 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2502 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/relationfield.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1660 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/servizio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    16924 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/summary.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5316 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3769 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/venue.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.236051 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      601 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.237610 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/content/
--rw-r--r--   0 filippocampi   (501) staff       (20)       24 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/content/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      664 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/content/add.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      368 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/content/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      653 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/controlpanel.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.239238 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/modulistica_items/
--rw-r--r--   0 filippocampi   (501) staff       (20)       24 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      605 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2915 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.240723 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/navigation/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/navigation/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      558 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1254 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/navigation/get.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.242052 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/scadenziario/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1200 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)    11504 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.243353 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/trasparenza/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      884 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3351 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.244860 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/types/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/types/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      404 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/types/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)    11265 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/types/get.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.246331 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/types/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/types/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3805 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/types/adapters.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      394 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/types/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1628 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/schema_overrides.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2315 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/setuphandlers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4083 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/testing.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.264936 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    11218 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/example.pdf
--rw-r--r--   0 filippocampi   (501) staff       (20)    10503 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/example.png
--rw-r--r--   0 filippocampi   (501) staff       (20)     1997 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_argomenti.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2330 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_base_serializer.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1564 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4707 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3169 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_luogo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2563 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1755 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_update_note.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1893 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_change_news_type.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     7543 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_bando.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5613 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6203 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_document.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    11615 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_documento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    13149 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_event.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1640 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_folder.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    14852 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_luogo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4225 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_modulo.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    12271 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_news.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5903 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     9850 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_persona.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    19255 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_servizio.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    17028 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2926 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_custom_service_navigation.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2708 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2526 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_move_news_items_view.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6638 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2798 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_service_scadenziario.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1381 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3533 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_setup.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    13785 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_substructure_creation.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    11753 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_summary_serializer.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4714 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6351 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_vocabularies.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.267718 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    24799 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     5033 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/draftjs_converter.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    12517 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/to_7001.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6007 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/to_7002.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    57526 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/upgrades.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      862 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/utils.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.272547 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1308 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1573 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1694 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1466 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1895 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1704 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/mockup.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2223 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1623 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4225 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2024-03-07 14:37:25.273419 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/
--rw-r--r--   0 filippocampi   (501) staff       (20)    41226 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 filippocampi   (501) staff       (20)    19380 2024-03-07 14:37:25.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        1 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      130 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/entry_points.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)       20 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        1 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 filippocampi   (501) staff       (20)      451 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/requires.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        7 2024-03-07 14:37:24.000000 design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.234902 design.plone.contenttypes-6.2.2/
+-rw-r--r--   0 lucabel    (501) staff       (20)    23315 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      585 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      665 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      158 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    40572 2024-03-19 08:35:45.235042 design.plone.contenttypes-6.2.2/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    15960 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/README.md
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.151550 design.plone.contenttypes-6.2.2/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7993 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       98 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      383 2024-03-19 08:35:45.235491 design.plone.contenttypes-6.2.2/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3005 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.140193 design.plone.contenttypes-6.2.2/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.151820 design.plone.contenttypes-6.2.2/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.154555 design.plone.contenttypes-6.2.2/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.156800 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/
+-rw-r--r--   0 lucabel    (501) staff       (20)      668 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.158434 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      892 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      421 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/interfaces.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      930 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/query.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      231 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/servizi_correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.164226 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1354 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/additional_help_infos.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2403 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/address.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8986 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11818 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     6469 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/contatti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1589 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/dataset_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2679 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6212 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1060 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/exclude_from_search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1657 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/geolocation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2388 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/info_testata.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2739 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6540 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1606 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/multi_file.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4439 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/news_additional_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1787 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/servizi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1357 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1648 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/strutture_correlate.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10452 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1165 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/update_note.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.165079 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1333 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.165368 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/overrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/overrides/.gitkeep
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.141591 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/static/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.165589 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/static/js/
+-rw-r--r--   0 lucabel    (501) staff       (20)      262 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/static/js/move_content.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      469 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/trasparenza.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.168892 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3813 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8270 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_documenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7290 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_eventi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7550 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_luoghi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8729 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_notizie.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8573 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_persone.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    14304 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_servizi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7594 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_uo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3467 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1571 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/export_incarichi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2796 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/move_news_items.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.171673 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3360 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6399 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6372 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6388 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     8600 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6167 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     9903 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6177 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     4760 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     3797 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/utils.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     3122 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.176248 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      315 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      246 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      210 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      215 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      229 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      271 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      272 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/content/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.177308 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      737 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1382 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3865 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/settings.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.178911 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5779 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      536 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      969 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/pagina_argomento.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.181911 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      458 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1119 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1803 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      411 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      921 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      621 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      829 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      741 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      470 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      445 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/uo.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.186613 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/
+-rw-r--r--   0 lucabel    (501) staff       (20)      419 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6263 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      699 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      857 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8557 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4702 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5442 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1483 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      205 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2560 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5024 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1781 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2850 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1838 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    18229 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7946 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.188340 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.143602 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/__pycache__/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.188629 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    82355 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    82310 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.144000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.189034 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    82335 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.144309 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.190096 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1243 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    83275 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     7287 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/plone.pot
+-rw-r--r--   0 lucabel    (501) staff       (20)     1597 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/overrides.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.191393 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/
+-rw-r--r--   0 lucabel    (501) staff       (20)      516 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3700 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/baseserializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      483 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      343 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/patches.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2751 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.145873 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.144883 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.199508 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
+-rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3401 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      331 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     4370 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      286 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2870 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      372 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     8078 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      300 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2156 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      313 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    13732 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      398 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     5133 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      292 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1042 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      303 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2196 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      265 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    15346 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      322 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1015 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      355 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3138 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      342 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.201733 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      799 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/actions.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      193 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2919 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1040 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1219 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      595 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.202241 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)    19836 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/registry/settings.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1139 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/repositorytool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4491 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.207609 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1155 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Bando.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3563 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3327 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3747 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3321 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2501 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      345 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Folder.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3427 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      506 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3199 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2908 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3456 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3430 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Persona.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3178 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3342 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3149 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3829 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3775 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2212 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Venue.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.207903 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/fix_syndication/
+-rw-r--r--   0 lucabel    (501) staff       (20)      520 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.208412 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/to_3000/
+-rw-r--r--   0 lucabel    (501) staff       (20)      377 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/to_3000/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.208728 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      128 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.209776 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      663 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      504 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/converters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      702 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.211909 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      760 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5795 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6050 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5743 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1658 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5844 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5999 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6016 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.215996 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1548 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2086 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1976 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2102 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2837 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7597 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1407 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2360 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3726 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1763 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2502 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/relationfield.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1660 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    16924 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/summary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5316 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3769 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.216760 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      601 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.217484 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      664 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/content/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      368 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/content/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      653 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/controlpanel.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.218209 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/modulistica_items/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      605 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2915 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.218903 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/navigation/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/navigation/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      558 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1254 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/navigation/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.219549 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/scadenziario/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1200 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    11504 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.220212 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/trasparenza/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      884 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3351 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.220852 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    11265 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/types/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.221499 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3805 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/types/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      394 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1628 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/schema_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2315 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4083 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.230763 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11218 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/example.pdf
+-rw-r--r--   0 lucabel    (501) staff       (20)    10503 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/example.png
+-rw-r--r--   0 lucabel    (501) staff       (20)     1997 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2330 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_base_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1564 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4707 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2563 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_update_note.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1893 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7543 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5613 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6203 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11615 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13149 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_event.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1640 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_folder.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    14852 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    12271 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5903 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     9850 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    19255 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    17028 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2926 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_custom_service_navigation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2708 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2526 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_move_news_items_view.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6638 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2798 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_service_scadenziario.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1381 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3533 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13785 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_substructure_creation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11753 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4714 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6351 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.232153 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    24799 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5033 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/draftjs_converter.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    12517 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/to_7001.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6007 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/to_7002.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    57526 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      862 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/utils.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.234704 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1308 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1573 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1694 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1466 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1895 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1704 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/mockup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2223 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1623 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-03-19 08:35:43.000000 design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:35:45.154281 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    40572 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    19380 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      130 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      451 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-03-19 08:35:44.000000 design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/top_level.txt
```

### Comparing `design.plone.contenttypes-6.2.1/CHANGES.rst` & `design.plone.contenttypes-6.2.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+6.2.2 (2024-03-19)
+------------------
+
+- @@check-servizi: provides also the full list of servizi.
+  [daniele]
+- UnitaOrganizzativa.assessore_riferimento title internationalize.
+  [folix-01]
+
 6.2.1 (2024-03-07)
 ------------------
 
 - Added check for blocks field in check_luoghi view.
   [eikichi18]
```

### Comparing `design.plone.contenttypes-6.2.1/DEVELOP.rst` & `design.plone.contenttypes-6.2.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/LICENSE.GPL` & `design.plone.contenttypes-6.2.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/LICENSE.rst` & `design.plone.contenttypes-6.2.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/PKG-INFO` & `design.plone.contenttypes-6.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.2.1
+Version: 6.2.2
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,37 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
-Requires-Dist: setuptools
-Requires-Dist: z3c.jbot
-Requires-Dist: plone.api>=1.8.4
-Requires-Dist: plone.app.dexterity>2.6.9
-Requires-Dist: collective.venue[geolocation]
-Requires-Dist: collective.volto.blocksfield
-Requires-Dist: collective.z3cform.datagridfield
-Requires-Dist: plone.formwidget.geolocation
-Requires-Dist: redturtle.volto>=5.0.0
-Requires-Dist: redturtle.bandi
-Requires-Dist: z3c.unconfigure
-Requires-Dist: eea.api.taxonomy
-Requires-Dist: openpyxl
-Requires-Dist: collective.volto.enhancedlinks
-Provides-Extra: test
-Requires-Dist: plone.app.testing; extra == "test"
-Requires-Dist: collective.volto.blocksfield; extra == "test"
-Requires-Dist: plone.testing>=5.0.0; extra == "test"
-Requires-Dist: plone.app.contenttypes; extra == "test"
-Requires-Dist: plone.app.robotframework[debug]; extra == "test"
-Requires-Dist: collective.MockMailHost; extra == "test"
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Tests](https://github.com/RedTurtle/design.plone.contenttypes/actions/workflows/tests.yml/badge.svg)](https://github.com/RedTurtle/design.plone.contenttypes/actions)
 [![Coverage](https://coveralls.io/repos/github/RedTurtle/design.plone.contenttypes/badge.svg?branch=main)](https://coveralls.io/github/RedTurtle/design.plone.contenttypes?branch=main)
@@ -518,14 +498,22 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.2.2 (2024-03-19)
+------------------
+
+- @@check-servizi: provides also the full list of servizi.
+  [daniele]
+- UnitaOrganizzativa.assessore_riferimento title internationalize.
+  [folix-01]
+
 6.2.1 (2024-03-07)
 ------------------
 
 - Added check for blocks field in check_luoghi view.
   [eikichi18]
```

### Comparing `design.plone.contenttypes-6.2.1/README.md` & `design.plone.contenttypes-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/docs/conf.py` & `design.plone.contenttypes-6.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/setup.py` & `design.plone.contenttypes-6.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.contenttypes",
-    version="6.2.1",
+    version="6.2.2",
     description="DesignItalia contenty types",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/__init__.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/query.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/query.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/adapters/searchabletext_indexers.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/adapters/searchabletext_indexers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/additional_help_infos.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/additional_help_infos.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/address.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/address.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/argomenti.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/contatti.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/contatti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/dataset_correlati.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/dataset_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/descrizione_estesa.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/evento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/exclude_from_search.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/exclude_from_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/geolocation.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/geolocation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/info_testata.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/info_testata.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/luoghi_correlati.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/luoghi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/luogo.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/multi_file.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/multi_file.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/news_additional_fields.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/news_additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/servizi_correlati.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/servizi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/show_modified.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/strutture_correlate.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/strutture_correlate.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/trasparenza.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/behaviors/update_note.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/behaviors/update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/change_news_type.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_documenti.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_documenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_eventi.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_eventi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_luoghi.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_luoghi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_notizie.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_notizie.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_persone.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_persone.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_servizi.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_servizi.py`

 * *Files 22% similar despite different names*

```diff
@@ -87,15 +87,23 @@
         frontend_domain = api.portal.get_registry_record(
             "volto.frontend_domain", default=""
         )
         if frontend_domain and url.startswith(portal_url):
             return url.replace(portal_url, frontend_domain, 1)
         return url
 
-    def get_servizi(self):
+    def get_relation_title(self, information_dict, label):
+        result = ""
+        for item in information_dict[label]:
+            if not item:
+                continue
+            result = result + " " + item.to_object.title
+        return result
+
+    def get_servizi(self, full_report=False):
         if self.is_anonymous():
             return []
         pc = api.portal.get_tool("portal_catalog")
 
         # show_inactive ha sempre avuto una gestione... particolare! aggiungo ai
         # kw effectiveRange = DateTime() che è quello che fa Products.CMFPlone
         # nel CatalogTool.py
@@ -125,57 +133,90 @@
             parent = servizio.aq_inner.aq_parent
             if parent.title not in results:
                 results[parent.title] = {
                     "url": self.plone2volto(parent.absolute_url()),
                     "children": [],
                 }
 
-            results[parent.title]["children"].append(
-                {
-                    "title": servizio.title,
-                    "url": self.plone2volto(servizio.absolute_url()),
-                    "data": {
-                        "title": information_dict.get("title") and FLAG or "",
-                        "description": information_dict.get("description")
-                        and FLAG
-                        or "",
-                        "condizioni_di_servizio": information_dict.get(
-                            "condizioni_di_servizio"
-                        )
-                        and FLAG
-                        or "",
-                        "tassonomia_argomenti": information_dict.get(
-                            "tassonomia_argomenti"
-                        )
-                        and FLAG
-                        or "",
-                        "a_chi_si_rivolge": information_dict.get("a_chi_si_rivolge")
-                        and FLAG
-                        or "",
-                        "come_si_fa": information_dict.get("come_si_fa") and FLAG or "",
-                        "cosa_si_ottiene": information_dict.get("cosa_si_ottiene")
-                        and FLAG
-                        or "",
-                        "canale_accesso": information_dict.get("canale_accesso") or "",
-                        "cosa_serve": information_dict.get("cosa_serve") and FLAG or "",
-                        "tempi_e_scadenze": information_dict.get("tempi_e_scadenze")
-                        and FLAG
-                        or "",
-                        "ufficio_responsabile": information_dict.get(
-                            "ufficio_responsabile"
-                        )
-                        and FLAG
-                        or "",
-                        "contact_info": information_dict.get("contact_info")
-                        and FLAG
-                        or "",
-                    },
-                }
+            tassonomia_argomenti = self.get_relation_title(
+                information_dict, "tassonomia_argomenti"
+            )
+            ufficio_responsabile = self.get_relation_title(
+                information_dict, "ufficio_responsabile"
             )
 
+            contatti = self.get_relation_title(information_dict, "contact_info")
+
+            if full_report:
+                results[parent.title]["children"].append(
+                    {
+                        "title": servizio.title,
+                        "url": self.plone2volto(servizio.absolute_url()),
+                        "data": {
+                            "title": information_dict.get("title") or "",
+                            "description": information_dict.get("description") or "",
+                            "condizioni_di_servizio": information_dict.get(
+                                "condizioni_di_servizio"
+                            )
+                            or "",
+                            "tassonomia_argomenti": tassonomia_argomenti or "",
+                            "a_chi_si_rivolge": information_dict.get("a_chi_si_rivolge")
+                            or "",
+                            "come_si_fa": information_dict.get("come_si_fa") or "",
+                            "cosa_si_ottiene": information_dict.get("cosa_si_ottiene")
+                            or "",
+                            "canale_accesso": information_dict.get("canale_accesso")
+                            or "",
+                            "cosa_serve": information_dict.get("cosa_serve") or "",
+                            "tempi_e_scadenze": information_dict.get("tempi_e_scadenze")
+                            or "",
+                            "ufficio_responsabile": ufficio_responsabile or "",
+                            "contact_info": contatti or "",
+                        },
+                    }
+                )
+            else:
+                results[parent.title]["children"].append(
+                    {
+                        "title": servizio.title,
+                        "url": self.plone2volto(servizio.absolute_url()),
+                        "data": {
+                            "title": information_dict.get("title") and FLAG or "",
+                            "description": information_dict.get("description")
+                            and FLAG
+                            or "",
+                            "condizioni_di_servizio": information_dict.get(
+                                "condizioni_di_servizio"
+                            )
+                            and FLAG
+                            or "",
+                            "tassonomia_argomenti": tassonomia_argomenti and FLAG or "",
+                            "a_chi_si_rivolge": information_dict.get("a_chi_si_rivolge")
+                            and FLAG
+                            or "",
+                            "come_si_fa": information_dict.get("come_si_fa")
+                            and FLAG
+                            or "",
+                            "cosa_si_ottiene": information_dict.get("cosa_si_ottiene")
+                            and FLAG
+                            or "",
+                            "canale_accesso": information_dict.get("canale_accesso")
+                            or "",
+                            "cosa_serve": information_dict.get("cosa_serve")
+                            and FLAG
+                            or "",
+                            "tempi_e_scadenze": information_dict.get("tempi_e_scadenze")
+                            and FLAG
+                            or "",
+                            "ufficio_responsabile": ufficio_responsabile and FLAG or "",
+                            "contact_info": contatti and FLAG or "",
+                        },
+                    }
+                )
+
         results = dict(sorted(results.items()))
         for key in results:
             results[key]["children"].sort(key=lambda x: x["title"])
         return results
 
 
 class DownloadCheckServizi(CheckServizi):
@@ -199,40 +240,66 @@
         cds = self.request.form.get("condizioni_di_servizio", None)
         if cds:
             EMPTY_ROW = [""] * 12
             HEADER.insert(2, "Condizioni di servizio")
         else:
             EMPTY_ROW = [""] * 11
 
-        servizi = self.get_servizi()
+        full_report = self.request.form.get("full", False)
+        servizi = self.get_servizi(full_report)
+
         data = []
         for category in servizi:
             data.append([category] + [""] * 10 + [servizi[category]["url"]])
             data.append(HEADER)
-            for servizio in servizi[category]["children"]:
-                dati_servizio = [
-                    servizio["title"],
-                    servizio["data"]["description"] and "V" or "",
-                    servizio["data"]["tassonomia_argomenti"] and "V" or "",
-                    servizio["data"]["a_chi_si_rivolge"] and "V" or "",
-                    servizio["data"]["come_si_fa"] and "V" or "",
-                    servizio["data"]["cosa_si_ottiene"] and "V" or "",
-                    servizio["data"]["canale_accesso"] and "V" or "",
-                    servizio["data"]["cosa_serve"] and "V" or "",
-                    servizio["data"]["tempi_e_scadenze"] and "V" or "",
-                    servizio["data"]["ufficio_responsabile"] and "V" or "",
-                    servizio["data"]["contact_info"] and "V" or "",
-                    servizio["url"],
-                ]
-                if cds:
-                    condizioni_di_servizio = (
-                        servizio["data"]["condizioni_di_servizio"] and "V" or ""
-                    )
-                    dati_servizio.insert(2, condizioni_di_servizio)
-                data.append(dati_servizio)
+
+            if full_report:
+                for servizio in servizi[category]["children"]:
+                    dati_servizio = [
+                        servizio["title"],
+                        servizio["data"]["description"] or "",
+                        servizio["data"]["tassonomia_argomenti"] or "",
+                        servizio["data"]["a_chi_si_rivolge"] or "",
+                        servizio["data"]["come_si_fa"] or "",
+                        servizio["data"]["cosa_si_ottiene"] or "",
+                        servizio["data"]["canale_accesso"] or "",
+                        servizio["data"]["cosa_serve"] or "",
+                        servizio["data"]["tempi_e_scadenze"] or "",
+                        servizio["data"]["ufficio_responsabile"] or "",
+                        servizio["data"]["contact_info"] or "",
+                        servizio["url"],
+                    ]
+                    if cds:
+                        condizioni_di_servizio = (
+                            servizio["data"]["condizioni_di_servizio"] or ""
+                        )
+                        dati_servizio.insert(2, condizioni_di_servizio)
+                    data.append(dati_servizio)
+            else:
+                for servizio in servizi[category]["children"]:
+                    dati_servizio = [
+                        servizio["title"],
+                        servizio["data"]["description"] and "V" or "",
+                        servizio["data"]["tassonomia_argomenti"] and "V" or "",
+                        servizio["data"]["a_chi_si_rivolge"] and "V" or "",
+                        servizio["data"]["come_si_fa"] and "V" or "",
+                        servizio["data"]["cosa_si_ottiene"] and "V" or "",
+                        servizio["data"]["canale_accesso"] and "V" or "",
+                        servizio["data"]["cosa_serve"] and "V" or "",
+                        servizio["data"]["tempi_e_scadenze"] and "V" or "",
+                        servizio["data"]["ufficio_responsabile"] and "V" or "",
+                        servizio["data"]["contact_info"] and "V" or "",
+                        servizio["url"],
+                    ]
+                    if cds:
+                        condizioni_di_servizio = (
+                            servizio["data"]["condizioni_di_servizio"] or ""
+                        )
+                        dati_servizio.insert(2, condizioni_di_servizio)
+                    data.append(dati_servizio)
             data.append(EMPTY_ROW)
             data.append(EMPTY_ROW)
 
         workbook = Workbook()
         sheet = workbook.active
         sheet.title = "Servizi"
         link_font = Font(underline="single", color="0563C1")
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/check_uo.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/check_uo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/export_incarichi.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/export_incarichi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/move_news_items.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/move_news_items.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,33 @@
                         type="submit"
                 >
                   <i class="fas fa-download"></i>
                    Download servizi
                 </button>
               </form>
             </div>
+            <div class="download_button">
+              <form action="${context/absolute_url}/@@download-check-servizi">
+                <!-- <input type="Submit" value="Download" /> -->
+                <input name="condizioni_di_servizio"
+                       type="hidden"
+                       value="True"
+                />
+                <input name="full"
+                       type="hidden"
+                       value="True"
+                />
+                <button class="download-button"
+                        type="submit"
+                >
+                  <i class="fas fa-download"></i>
+                   Download tutti i servizi
+                </button>
+              </form>
+            </div>
           </div>
 
 
 
           <ul>
             <li class="categoria"
                 tal:repeat="categoria servizi"
```

#### html2text {}

```diff
@@ -16,14 +16,15 @@
 tutti i campi relativi al canale di accesso.
 Si fa notare, infine, che la seguente lista di servizi presenta tutti quei
 servizi in stato pubblicato e nnoonn ssccaadduuttii secondo le logiche di pubblicazione
 del CMS Plone, ovvero con una data di scadenza ancora da raggiugnere.
 [Cerca senza condizioni di servizio]
 [Cerca con condizioni di servizio]
 Download servizi
+Download tutti i servizi
     * ********** _$$_{{_cc_aa_tt_ee_gg_oo_rr_ii_aa_}} **********
           o **** _$$_{{_ss_ee_rr_vv_ii_zz_ii_oo_//_tt_ii_tt_ll_ee_}} ****
                              CCoonnddiizziioonnii           AA cchhii ?è CCoommee CCoossaa ssii CCaannaallee  CCoossaa  TTeemmppii ee  UUnniitt?à oorrgg..
       TTiittoolloo     DDeessccrriizziioonnee ddii         AArrggoommeennttii rriivvoollttoo ffaarree oottttiieennee ddii      sseerrvvee ssccaaddeennzzee rreessppoonnssaabbiillee CCoonnttaattttii
                              sseerrvviizziioo                     ppeerr          aacccceessssoo
       _$
       _{_s_e_r_v_i_z_i_o_/
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/browser/utils/templates/utils.pt` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/browser/utils/templates/utils.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/controlpanels/settings.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/controlpanels/settings.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/common.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/document.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/incarico.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/events/pagina_argomento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/events/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/common.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/news.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/pagina_argomento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/persona.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/indexers/punto_di_contatto.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/indexers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/bando.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/cartella_modulistica.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/dataset.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/dataset.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/documento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/documento_personale.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/incarico.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/messaggio.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/messaggio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/pagina_argomento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/persona.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/pratica.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/punto_di_contatto.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/servizio.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/interfaces/unita_organizzativa.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/interfaces/unita_organizzativa.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             default="Selezionare il/i responsabile/i della struttura.",
         ),
         default=[],
         required=False,
     )
 
     assessore_riferimento = RelationList(
-        title="Assessore di riferimento",
+        title=_("assessore_riferimento_title", default="Assessore di riferimento"),
         # vocabolario di riferimento sara' dinamico con i content type
         # persona presenti all'interno della macro Amministrazione"
         value_type=RelationChoice(
             title=_("Assessore di riferimento"),
             vocabulary="plone.app.vocabularies.Catalog",
         ),
         description=_(
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/README.rst` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,506 +1,495 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # Language  translations for PACKAGE package.
 # Roman Kysil <roman@folix.local>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-01-13 13:15+0000\n"
+"POT-Creation-Date: 2024-03-18 13:30+0000\n"
 "PO-Revision-Date: 2023-01-03 18:01+0100\n"
 "Last-Translator: Roman Kysil <roman@folix.local>\n"
 "Language-Team: Language\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: design.plone.contenttypes\n"
 "Language: __pycache__\n"
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
-msgid "Abitazione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:36
-msgid "Accesso al trasporto pubblico"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:59
-msgid "Accesso luoghi della cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:18
+msgid "Accesso all'informazione"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:33
 msgid "Accettare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:34
-msgid "Accordo tra enti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:19
 msgid "Acqua"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
+#: design/plone/contenttypes/behaviors/configure.zcml:223
 msgid "Address Event"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Address UO"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:186
+#: design/plone/contenttypes/behaviors/configure.zcml:215
 msgid "Address Venue"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:19
 msgid "Adds fields."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:28
-msgid "Agricoltura, pesca, silvicoltura e prodotti alimentari"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "After Plone6 migration syndication is broken"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:22
-msgid "All the already existing News Types"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:20
+msgid "Agricoltura"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:63
-msgid "All the selected items will be moved to indicated path"
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:30
+msgid "All the already existing News Types"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:36
-msgid "Ambiente"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:113
+msgid "All the selected items will be moved to indicated path"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:21
 msgid "Animale domestico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
-msgid "Anziano"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/bando.py:134
-#: design/plone/contenttypes/interfaces/documento.py:67
-#: design/plone/contenttypes/interfaces/servizio.py:239
+#: design/plone/contenttypes/interfaces/bando.py:135
+#: design/plone/contenttypes/interfaces/documento.py:97
+#: design/plone/contenttypes/interfaces/servizio.py:328
 msgid "Area"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
-msgid "Area di parcheggio"
-msgstr ""
-
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Argomenti"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:76
+#: design/plone/contenttypes/behaviors/configure.zcml:94
 msgid "Argomenti Bando"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:58
+#: design/plone/contenttypes/behaviors/configure.zcml:76
 msgid "Argomenti Document"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:67
+#: design/plone/contenttypes/behaviors/configure.zcml:85
 msgid "Argomenti Documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:28
+#: design/plone/contenttypes/behaviors/configure.zcml:112
+msgid "Argomenti Link"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/argomenti.py:32
 msgid "Argomenti correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
 msgid "Argomento"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:73
+#: design/plone/contenttypes/behaviors/configure.zcml:103
+msgid "Argomento Servizio"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:22
+msgid "Aria"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:65
 msgid "Assessore di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
-msgid "Associazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:23
+msgid "Assistenza agli invalidi"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:24
+msgid "Assistenza sociale"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
+msgid "Associazioni"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:29
 msgid "Attivare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:33
-msgid "Atto normativo"
+#: design/plone/contenttypes/interfaces/incarico.py:121
+msgid "Atto di nomina"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:86
 msgid "Autore"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:30
 msgid "Autorizzare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:65
-msgid "Avvio impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:66
-msgid "Avvio nuova attività professionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:69
-msgid "Avvio/registrazione filiale"
+#: design/plone/contenttypes/behaviors/configure.zcml:223
+msgid "Behavior address per Event."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:78
-msgid "Bancarotta"
+#: design/plone/contenttypes/behaviors/configure.zcml:215
+msgid "Behavior address per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
-msgid "Behavior address per Event."
+#: design/plone/contenttypes/behaviors/configure.zcml:263
+msgid "Behavior contatti per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Behavior address per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:255
+msgid "Behavior contatti per Persona."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:186
-msgid "Behavior address per Venue."
+#: design/plone/contenttypes/behaviors/configure.zcml:247
+msgid "Behavior contatti per Servizio."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
 msgid "Behavior contatti per UO."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:210
+#: design/plone/contenttypes/behaviors/configure.zcml:239
 msgid "Behavior contatti per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:234
+#: design/plone/contenttypes/behaviors/configure.zcml:279
 msgid "Behavior geolocatable per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
-msgid "Behavior geolocatable per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:271
+msgid "Behavior geolocatable per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:226
-msgid "Behavior geolocatable per Venue."
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
+msgid "Bilancio"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:18
 msgid "CAP"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:43
-msgid "Cambio di residenza/domicilio"
+#: design/plone/contenttypes/behaviors/configure.zcml:306
+msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:261
-msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Campo per escludere un contenuto dalle ricerche del sito."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
+#: design/plone/contenttypes/behaviors/configure.zcml:315
 msgid "Campo per le note di aggiornamento."
 msgstr ""
 
+#: design/plone/contenttypes/interfaces/servizio.py:183
+msgid "Canale fisico"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:26
 msgid "Canon 5D IV"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 msgid "Cartella Modulistica"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:11
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:13
 msgid "Change News Type"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:75
-msgid "Chiusura filiale"
+#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
+msgid "Città"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:74
-msgid "Chiusura impresa e attività professionale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
+msgid "Commercio al minuto"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
-msgid "Città"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
+msgid "Commercio all'ingrosso"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:39
-msgid "Compravendita/affitto casa/edifici/terreni, costruzione o ristrutturazione casa/edificio	"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
+msgid "Commercio ambulante"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
-msgid "Comunicazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
+msgid "Comunicazione istituzionale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
-msgid "Condizioni e organizzazione del lavoro"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+msgid "Comunicazione politica"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
+msgid "Concorsi"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:57
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:104
 msgid "Contained by"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
+#: design/plone/contenttypes/behaviors/contatti.py:112
 msgid "Contatti"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:33
 msgid "Coordinate"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:42
+#: design/plone/contenttypes/behaviors/argomenti.py:46
 msgid "Correlato in evidenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
-msgid "Cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+msgid "Covid - 19"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:130
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 msgid "Dataset"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:134
 msgid "Dataset collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:104
+#: design/plone/contenttypes/behaviors/configure.zcml:141
 msgid "Dataset correlati"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:31
 msgid "Delegare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:52
-msgid "Denuncia crimini"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:143
+#: design/plone/contenttypes/behaviors/configure.zcml:180
 msgid "Descrizione estesa"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:160
+#: design/plone/contenttypes/behaviors/configure.zcml:197
 msgid "Descrizione estesa documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:152
+#: design/plone/contenttypes/behaviors/configure.zcml:189
 msgid "Descrizione estesa servizio"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Design Plone: Content-types"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Design Plone: Content-types (behaviors)"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Design Plone: Content-types (uninstall)"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Design Plone: Content-types to 3000"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:55
-msgid "Dichiarazione dei redditi, versamento e riscossione tributi/imposte e contributi"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "Design Plone: Fix Syndication after Plone6 Migration"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:145
+#: design/plone/contenttypes/behaviors/trasparenza.py:146
 msgid "Dirigente"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:27
-msgid "Documenti albo pretorio"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:134
+msgid "Documenti pubblici"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/servizio.py:252
+#: design/plone/contenttypes/interfaces/servizio.py:341
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Documento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:41
-msgid "Documento (tecnico) di supporto"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
 msgid "Documento Personale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:37
-msgid "Documento attivita politica"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:31
-msgid "Documento funzionamento interno"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:30
-msgid "Economia e Finanze"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Edit"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
-msgid "Elezione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:35
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
-msgid "Energia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+msgid "Elezioni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
-msgid "Famiglia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
+msgid "Energie rinnovabili"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
-msgid "Fanciullo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
+msgid "Estero"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:70
-msgid "Finanziamento impresa"
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Exclude from search"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:28
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:51
 msgid "Find news with the indicated Path, put attention than generaly sites have the root name \"/Plone/\""
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:21
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:29
 msgid "Find news with this News Type"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Fix control panel of design.plone.contenttypes add-on."
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
+msgid "Foreste"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/tags_vocabulary.py:38
 msgid "Formazione professionale"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:39
+msgid "Gemellaggi"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:271
 msgid "Geolocatable"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:43
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Geolocation default"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
-msgid "Gestione dei rifiuti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:71
-msgid "Gestione personale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
-msgid "Giovane"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:40
+msgid "Gestione rifiuti"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:30
 msgid "Giovanni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:42
-msgid "Giustizia, sistema giuridico e sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
+msgid "Giustizia"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:37
-msgid "Governo e settore pubblico"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:42
+msgid "Igiene pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+#: design/plone/contenttypes/browser/utils/change_news_type.py:32
+#: design/plone/contenttypes/browser/utils/move_news_items.py:74
+msgid "Il vocabolario dei valori non è stato trovato"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
 msgid "Immigrazione"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/settings.py:154
+#: design/plone/contenttypes/controlpanels/settings.py:106
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Impostazioni Design Plone"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+msgid "Imposte"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
+msgid "Imprese"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/persona.py:68
+msgid "Incarichi"
+msgstr ""
+
+#: design/plone/contenttypes/profiles/default/types/Incarico.xml
+msgid "Incarico"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/move_news_items.py:34
 msgid "Indicated path is not valid"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:170
+#: design/plone/contenttypes/behaviors/configure.zcml:207
 msgid "Info per la testata"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:32
 msgid "Informare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
-msgid "Informatica e trattamento dei dati"
+#: design/plone/contenttypes/behaviors/contatti.py:34
+msgid "Informazioni di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
 msgid "Inquinamento"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Installs the design.plone.contenttypes add-on."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
 msgid "Integrazione sociale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:28
-msgid "Invalidità"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:26
 msgid "Iscriversi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:26
-msgid "Iscrizione scuola/università e/o richiesta borsa di studio"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:43
-msgid "Istanza"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+msgid "Isolamento termico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
 msgid "Istruzione"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:33
-msgid "Istruzione, cultura e sport"
+#: design/plone/contenttypes/browser/utils/move_news_items.py:48
+msgid "Items moved with success"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:47
-msgid "Items moved with success"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
+msgid "Lavoro"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:28
 msgid "Leggere"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:85
+#: design/plone/contenttypes/behaviors/configure.zcml:122
 msgid "Luoghi correlati"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
 msgid "Matrimonio"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:49
-msgid "Matrimonio e/o cambio stato civile"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+msgid "Mercato"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Messaggio.xml
 msgid "Messaggio"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:29
@@ -511,529 +500,536 @@
 msgid "Metadati luogo"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:39
 msgid "Metadati news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:28
-msgid "Modulistica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
+msgid "Mobilità sostenibile"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Modulo"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:50
-msgid "Morte ed eredità"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
+msgid "Morte"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Mostra la data di modifica."
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:70
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:124
 msgid "Move"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:11
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:13
 msgid "Move News Items"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:62
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:110
 msgid "Move to Path"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Multi File"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:48
-msgid "Nascita di un bambino, richiesta adozioni"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
+msgid "Nascita"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:28
 msgid "Nazione"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:21
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:20
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:26
 msgid "News Type"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:30
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:48
 msgid "News Type to substitute"
 msgstr ""
 
 #. Default: "Nome e cognome"
-#: design/plone/contenttypes/restapi/services/types/get.py:152
+#: design/plone/contenttypes/restapi/services/types/get.py:163
 msgid "Nome e Cognome"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:73
-msgid "Notifiche autorità"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/persona.py:48
+#: design/plone/contenttypes/interfaces/persona.py:51
 msgid "Organizzazione di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:72
-msgid "Pagamento tasse, iva e dogane"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:25
 msgid "Pagare"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:29
 msgid "Paperino"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:81
-msgid "Partecipazione ad appalti pubblici nazionali e trasfrontalieri"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
+msgid "Parcheggi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:33
-msgid "Pensionamento"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
+msgid "Patrimonio culturale"
 msgstr ""
 
-#: design/plone/contenttypes/profiles/default/types/Persona.xml
+#: design/plone/contenttypes/interfaces/incarico.py:54
 msgid "Persona"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/evento.py:50
-msgid "Persona dell'amministrazione"
+#: design/plone/contenttypes/profiles/default/types/Persona.xml
+msgid "Persona pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:92
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:84
 msgid "Persone della struttura"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+msgid "Pesca"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
+msgid "Piano di sviluppo"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:27
 msgid "Pippo"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+msgid "Pista ciclabile"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:28
 msgid "Pluto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:45
-msgid "Popolazione e società"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
+msgid "Politica commerciale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:60
-msgid "Possesso, cura, smarrimento animale da compagnia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:62
+msgid "Polizia"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pratica.xml
 msgid "Pratica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:51
-msgid "Prenotazione e disdetta visite/esami"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:63
+msgid "Prodotti alimentari"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
-msgid "Protezione sociale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
+msgid "Protezione civile"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:13
-msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
+#: design/plone/contenttypes/behaviors/contatti.py:78
+msgid "Punti di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:13
-msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
+#: design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+msgid "Punto di Contatto"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:15
+msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:44
-msgid "Regioni e città"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:15
+msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:68
-msgid "Registrazione impresa transfrontalier"
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Registers taxonomies."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:35
-msgid "Registrazione/possesso veicolo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:65
+msgid "Residenza"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:45
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:49
 msgid "Responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:129
-msgid "Responsabile procedimento"
+#: design/plone/contenttypes/interfaces/incarico.py:89
+msgid "Responsabile della struttura"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:31
-msgid "Ricerca di lavoro, avvio nuovo lavoro, disoccupazione"
+#: design/plone/contenttypes/behaviors/trasparenza.py:130
+msgid "Responsabile procedimento"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
 msgid "RicevutaPagamento"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:27
 msgid "Richiedere"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:67
-msgid "Richiesta licenze/permessi/certificati"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:34
-msgid "Richiesta o rinnovo patente"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:46
-msgid "Richiesta passaporto, visto e assistenza viaggi internazionali"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:66
+msgid "Risposta alle emergenze"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:76
-msgid "Ristrutturazione impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:38
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
-msgid "Salute"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:46
-msgid "Scienza e tecnologia"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:47
 msgid "Search Path"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:114
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:104
 msgid "Sede"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:114
+#: design/plone/contenttypes/behaviors/configure.zcml:151
 msgid "Servizi correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Servizio.xml
 msgid "Servizio"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:101
 msgid "Servizio collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Show modified"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
-msgid "Sicurezza internazionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
-msgid "Sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:67
+msgid "Sistema giuridico"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:25
 msgid "Sony Aplha 7R III"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
-msgid "Spazio verde"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:68
+msgid "Spazio Verde"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:69
 msgid "Sport"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:37
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:41
 msgid "Struttura"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:20
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:21
 msgid "Struttura politica coinvolta"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/luogo.py:74
+#: design/plone/contenttypes/behaviors/luogo.py:75
 msgid "Struttura responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:124
+#: design/plone/contenttypes/behaviors/configure.zcml:161
 msgid "Strutture correlate"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
-msgid "Studente"
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:74
+msgid "Substitute"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:43
-msgid "Substitute"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:70
+msgid "Sviluppo sostenibile"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:71
+msgid "Tassa sui servizi"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Tassonomia argomenti"
 msgstr ""
 
+#: design/plone/contenttypes/behaviors/configure.zcml:67
+msgid "Tassonomia argomenti evento"
+msgstr ""
+
 #: design/plone/contenttypes/behaviors/configure.zcml:58
-msgid "Tassonomia argomenti per i Document"
+msgid "Tassonomia argomenti news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:39
-msgid "Tematiche internazionali"
+#: design/plone/contenttypes/behaviors/configure.zcml:76
+msgid "Tassonomia argomenti per i Document"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:72
 msgid "Tempo libero"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:31
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:52
 msgid "The News Type selected above will be substituted by the selected value"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:97
+#: design/plone/contenttypes/browser/utils/change_news_type.py:108
 msgid "The News Types was changed with success"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:55
+#: design/plone/contenttypes/browser/utils/change_news_type.py:64
 msgid "The new News Type was not found between available values"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:49
+#: design/plone/contenttypes/browser/utils/change_news_type.py:58
 msgid "The new type field was not populated"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:61
+#: design/plone/contenttypes/browser/utils/change_news_type.py:70
 msgid "The old News Type was not found between available values"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:43
+#: design/plone/contenttypes/browser/utils/change_news_type.py:52
 msgid "The old type field was not populated"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:51
+#: design/plone/contenttypes/browser/utils/move_news_items.py:52
 msgid "The path was not indicated"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
-msgid "Traffico urbano"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:261
+#: design/plone/contenttypes/behaviors/configure.zcml:306
 msgid "Trasparenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
-msgid "Trasporto"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:73
+msgid "Trasparenza amministrativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
-msgid "Trasporto stradale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:74
+msgid "Trasporto pubblico"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Tre campi file aggiuntivi."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:75
 msgid "Turismo"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:117
-#: design/plone/contenttypes/interfaces/documento.py:50
-#: design/plone/contenttypes/interfaces/servizio.py:225
+#: design/plone/contenttypes/interfaces/bando.py:118
+#: design/plone/contenttypes/interfaces/documento.py:80
 msgid "Ufficio responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:134
+#: design/plone/contenttypes/behaviors/configure.zcml:171
 msgid "Ulteriori campi aiuto testuali"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Un modulo compilabile."
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:15
+msgid "Una raccolta di utility per i contenuti agid"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Uninstalls the design.plone.contenttypes add-on."
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
 msgid "Unita Organizzativa"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:45
 msgid "Unità amministrative responsabili"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
-msgid "Update note"
+#: design/plone/contenttypes/interfaces/incarico.py:71
+msgid "Unità organizzativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
-msgid "Urbanistica ed edilizia"
+#: design/plone/contenttypes/interfaces/servizio.py:314
+msgid "Unità organizzativa responsabile"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:315
+msgid "Update note"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:77
-msgid "Vendita impresa"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:76
+msgid "Urbanizzazione"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:13
 msgid "Via"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:77
+msgid "Viaggi"
+msgstr ""
+
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "View"
 msgstr ""
 
-#. Default: "A chi si rivolge questo servizio e chi può usufruirne."
-#: design/plone/contenttypes/interfaces/servizio.py:53
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:13
+msgid "Viste di utility per Design Plone Contenttypes"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:79
+msgid "ZTL"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:78
+msgid "Zone pedonali"
+msgstr ""
+
+#. Default: "Descrizione testuale dei principali destinatari dell'Evento"
+#: design/plone/contenttypes/behaviors/evento.py:43
+#: design/plone/contenttypes/interfaces/servizio.py:98
 msgid "a_chi_si_rivolge_help"
 msgstr ""
 
-#. Default: "A chi si rivolge"
-#: design/plone/contenttypes/interfaces/servizio.py:51
+#. Default: "A chi è rivolto"
+#: design/plone/contenttypes/behaviors/evento.py:41
+#: design/plone/contenttypes/interfaces/servizio.py:96
 msgid "a_chi_si_rivolge_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio di comunicazione responsabile di questa notizia/comunicato stampa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:47
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:39
 msgid "a_cura_di_help"
 msgstr ""
 
 #. Default: "A cura di"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:46
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
 msgid "a_cura_di_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di persone dell'amministrazione citate in questa notizia/comunicato stampa. Questa informazione verrà mostrata nella sezione \"A cura di\"."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:59
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:51
 msgid "a_cura_di_persone_help"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:58
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:50
 msgid "a_cura_di_persone_label"
 msgstr ""
 
 #. Default: "Accedere al servizio"
-#: design/plone/contenttypes/interfaces/servizio.py:370
+#: design/plone/contenttypes/interfaces/servizio.py:481
 msgid "accedi_al_servizio_label"
 msgstr ""
 
 #. Default: "Modalità di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:171
+#: design/plone/contenttypes/behaviors/luogo.py:140
 msgid "accesso_label"
 msgstr ""
 
 #. Default: "Allegato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:56
 msgid "allegato"
 msgstr ""
 
 #. Default: "Indicare, se esistono, altre modalità di invio."
-#: design/plone/contenttypes/behaviors/trasparenza.py:189
+#: design/plone/contenttypes/behaviors/trasparenza.py:190
 msgid "altre_modalita_invio_help"
 msgstr ""
 
 #. Default: "Altre modalità di invio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:185
+#: design/plone/contenttypes/behaviors/trasparenza.py:186
 msgid "altre_modalita_invio_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei documenti di supporto collegati a questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:246
+#: design/plone/contenttypes/interfaces/servizio.py:335
 msgid "altri_documenti_help"
 msgstr ""
 
 #. Default: "Date and time of the opening of the announcement. Use this field if you want to set a specific opening date. If not set, the announcement will be open immediately."
-#: design/plone/contenttypes/interfaces/bando.py:56
+#: design/plone/contenttypes/interfaces/bando.py:57
 msgid "apertura_bando_help"
 msgstr ""
 
 #. Default: "Opening date"
-#: design/plone/contenttypes/interfaces/bando.py:55
+#: design/plone/contenttypes/interfaces/bando.py:56
 msgid "apertura_bando_label"
 msgstr ""
 
 #. Default: "Area"
-#: design/plone/contenttypes/interfaces/servizio.py:231
+#: design/plone/contenttypes/interfaces/servizio.py:320
 msgid "area"
 msgstr ""
 
 #. Default: "Seleziona l'area da cui dipende questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:234
+#: design/plone/contenttypes/interfaces/servizio.py:323
 msgid "area_help"
 msgstr ""
 
 #. Default: "Area responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:73
 msgid "area_responsabile_documento_personale"
 msgstr ""
 
 #. Default: "Seleziona l'area amministrativa responsabile del documento."
-#: design/plone/contenttypes/interfaces/bando.py:127
-#: design/plone/contenttypes/interfaces/documento.py:60
+#: design/plone/contenttypes/interfaces/bando.py:128
+#: design/plone/contenttypes/interfaces/documento.py:90
 msgid "area_responsabile_help"
 msgstr ""
 
 #. Default: "Area responsabile del documento"
-#: design/plone/contenttypes/interfaces/bando.py:123
-#: design/plone/contenttypes/interfaces/documento.py:56
+#: design/plone/contenttypes/interfaces/bando.py:124
+#: design/plone/contenttypes/interfaces/documento.py:86
 msgid "area_responsabile_label"
 msgstr ""
 
 #. Default: "Argomenti utenti"
 #: design/plone/contenttypes/interfaces/documento_personale.py:42
 msgid "argomenti_utenti"
 msgstr ""
 
 #. Default: "Inserire l'assessore di riferimento della struttura, se esiste."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:76
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:68
 msgid "assessore_riferimento_help"
 msgstr ""
 
+#. Default: "Assessore di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:61
+msgid "assessore_riferimento_title"
+msgstr ""
+
 #. Default: "Indicare, se la esistono, atti e documenti a corredo dell'istanza."
-#: design/plone/contenttypes/behaviors/trasparenza.py:200
+#: design/plone/contenttypes/behaviors/trasparenza.py:201
 msgid "atti_documenti_corredo_help"
 msgstr ""
 
 #. Default: "Atti e documenti a corredo dell'istanza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:196
+#: design/plone/contenttypes/behaviors/trasparenza.py:197
 msgid "atti_documenti_corredo_label"
 msgstr ""
 
-#. Default: "Inserire un file contenente l'atto di nomina della persona."
-#: design/plone/contenttypes/interfaces/persona.py:160
-msgid "atto_nomina_help"
+#. Default: "Inserire riferimento all'atto di nomina della persona"
+#: design/plone/contenttypes/interfaces/incarico.py:114
+msgid "atto_nomina_incarico_help"
 msgstr ""
 
 #. Default: "Atto di nomina"
-#: design/plone/contenttypes/interfaces/persona.py:158
-msgid "atto_nomina_label"
-msgstr ""
-
-#. Default: "Autenticazione"
-#: design/plone/contenttypes/interfaces/servizio.py:121
-msgid "autenticazione"
-msgstr ""
-
-#. Default: "Indicare, se previste, le modalità di autenticazione necessarie per poter accedere al servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:122
-msgid "autenticazione_help"
+#: design/plone/contenttypes/interfaces/incarico.py:110
+msgid "atto_nomina_incarico_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di autori che hanno pubblicato il documento. Possono essere Persone o Unità Organizzative."
-#: design/plone/contenttypes/interfaces/documento.py:76
+#: design/plone/contenttypes/interfaces/documento.py:106
 msgid "autori_help"
 msgstr ""
 
 #. Default: "Autore/i"
-#: design/plone/contenttypes/interfaces/documento.py:72
+#: design/plone/contenttypes/interfaces/documento.py:102
 msgid "autori_label"
 msgstr ""
 
 #. Default: "Azioni"
 #: design/plone/contenttypes/interfaces/messaggio.py:28
 msgid "azioni_pratica"
 msgstr ""
@@ -1045,660 +1041,686 @@
 
 #. Default: "Azioni utente"
 #: design/plone/contenttypes/interfaces/pratica.py:47
 msgid "azioni_utente"
 msgstr ""
 
 #. Default: "Solo per persona politica: testo descrittivo che riporta la biografia della persona."
-#: design/plone/contenttypes/interfaces/persona.py:107
+#: design/plone/contenttypes/interfaces/persona.py:94
 msgid "biografia_help"
 msgstr ""
 
 #. Default: "Biografia"
-#: design/plone/contenttypes/interfaces/persona.py:106
+#: design/plone/contenttypes/interfaces/persona.py:93
 msgid "biografia_label"
 msgstr ""
 
 #. Default: "Canale digitale"
-#: design/plone/contenttypes/interfaces/servizio.py:111
+#: design/plone/contenttypes/interfaces/servizio.py:156
 msgid "canale_digitale"
 msgstr ""
 
-#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:112
+#. Default: "Testo di introduzione del canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:157
 msgid "canale_digitale_help"
 msgstr ""
 
+#. Default: "Link al canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:165
+msgid "canale_digitale_link"
+msgstr ""
+
+#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
+#: design/plone/contenttypes/interfaces/servizio.py:166
+msgid "canale_digitale_link_help"
+msgstr ""
+
 #. Default: "Canale digitale servizio collegato"
 #: design/plone/contenttypes/interfaces/documento_personale.py:108
 msgid "canale_digitale_servizio"
 msgstr ""
 
+#. Default: "Canale fisico"
+#: design/plone/contenttypes/interfaces/servizio.py:175
+msgid "canale_fisico"
+msgstr ""
+
+#. Default: "Unità organizzative per la fruizione del servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:176
+msgid "canale_fisico_help"
+msgstr ""
+
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:205
+#: design/plone/contenttypes/interfaces/servizio.py:291
 msgid "casi_particolari"
 msgstr ""
 
 #. Default: "Descrizione degli evetuali casi particolari riferiti alla fruibilità di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:207
+#: design/plone/contenttypes/interfaces/servizio.py:293
 msgid "casi_particolari_help"
 msgstr ""
 
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:401
+#: design/plone/contenttypes/interfaces/servizio.py:514
 msgid "casi_particolari_label"
 msgstr ""
 
 #. Default: "Descrizione di chi può presentare domanda per usufruire del servizio e delle diverse casistiche."
-#: design/plone/contenttypes/interfaces/servizio.py:62
+#: design/plone/contenttypes/interfaces/servizio.py:107
 msgid "chi_puo_presentare_help"
 msgstr ""
 
 #. Default: "Chi può presentare"
-#: design/plone/contenttypes/interfaces/servizio.py:60
+#: design/plone/contenttypes/interfaces/servizio.py:105
 msgid "chi_puo_presentare_label"
 msgstr ""
 
 #. Default: "Circoscrizione"
 #: design/plone/contenttypes/behaviors/address.py:37
 msgid "circoscrizione"
 msgstr ""
 
 #. Default: "Codice dell'ente erogatore (ipa)"
-#: design/plone/contenttypes/interfaces/servizio.py:268
+#: design/plone/contenttypes/interfaces/servizio.py:357
 msgid "codice_ipa"
 msgstr ""
 
 #. Default: "Specificare il nome dell’organizzazione, come indicato nell’Indice della Pubblica Amministrazione (IPA), che esercita uno specifico ruolo sul Servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:270
+#: design/plone/contenttypes/interfaces/servizio.py:359
 msgid "codice_ipa_help"
 msgstr ""
 
-#. Default: "Come si fa"
-#: design/plone/contenttypes/interfaces/servizio.py:80
+#. Default: "Come fare"
+#: design/plone/contenttypes/interfaces/servizio.py:125
 msgid "come_si_fa"
 msgstr ""
 
 #. Default: "Descrizione della procedura da seguire per poter usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:82
+#: design/plone/contenttypes/interfaces/servizio.py:127
 msgid "come_si_fa_help"
 msgstr ""
 
+#. Default: "Solo per incarico politico: compensi di qualsiasi natura connessi all'assunzione della carica."
+#: design/plone/contenttypes/interfaces/incarico.py:21
+msgid "compensi_incarico_help"
+msgstr ""
+
+#. Default: "Compensi"
+#: design/plone/contenttypes/interfaces/incarico.py:17
+msgid "compensi_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione del ruolo e dei compiti della persona."
-#: design/plone/contenttypes/interfaces/persona.py:69
+#: design/plone/contenttypes/interfaces/persona.py:77
 msgid "competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/persona.py:68
+#: design/plone/contenttypes/interfaces/persona.py:76
 msgid "competenze_label"
 msgstr ""
 
-#. Default: "Informazioni di contatto generiche"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:137
+#. Default: "Condizioni di servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:388
+msgid "condizioni_di_servizio"
+msgstr ""
+
+#. Default: "Contatti dell'unità organizzativa."
+#: design/plone/contenttypes/behaviors/contatti.py:27
+msgid "contact_info_help"
+msgstr ""
+
+#. Default: "Punti di contatto dell'unità organizzativa"
+#: design/plone/contenttypes/behaviors/contatti.py:23
 msgid "contact_info_label"
 msgstr ""
 
 #. Default: "Contatti"
 #: design/plone/contenttypes/interfaces/pratica.py:44
 msgid "contatti"
 msgstr ""
 
 #. Default: "Contatti"
-#: design/plone/contenttypes/behaviors/address.py:52
-#: design/plone/contenttypes/behaviors/contatti.py:76
-#: design/plone/contenttypes/behaviors/evento.py:215
+#: design/plone/contenttypes/behaviors/contatti.py:57
+#: design/plone/contenttypes/behaviors/evento.py:170
+#: design/plone/contenttypes/behaviors/geolocation.py:18
 msgid "contatti_label"
 msgstr ""
 
 #. Default: "Contenuto"
 #: design/plone/contenttypes/interfaces/pratica.py:42
 msgid "contenuto"
 msgstr ""
 
 #. Default: "Indicare se il servizio si riferisce ad una particolare area geografica o all'intero territorio di riferimento."
-#: design/plone/contenttypes/interfaces/servizio.py:72
+#: design/plone/contenttypes/interfaces/servizio.py:117
 msgid "copertura_geografica_help"
 msgstr ""
 
 #. Default: "Copertura geografica"
-#: design/plone/contenttypes/interfaces/servizio.py:70
+#: design/plone/contenttypes/interfaces/servizio.py:115
 msgid "copertura_geografica_label"
 msgstr ""
 
 #. Default: "Contenuti collegati"
-#: design/plone/contenttypes/behaviors/argomenti.py:74
+#: design/plone/contenttypes/behaviors/argomenti.py:108
 #: design/plone/contenttypes/behaviors/dataset_correlati.py:40
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:43
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:120
 msgid "correlati_label"
 msgstr ""
 
 #. Default: "Seleziona un correlato da mettere in evidenza per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:36
+#: design/plone/contenttypes/behaviors/argomenti.py:40
 msgid "correlato_in_evidenza_help"
 msgstr ""
 
 #. Default: "Correlato in evidenza"
-#: design/plone/contenttypes/behaviors/argomenti.py:35
+#: design/plone/contenttypes/behaviors/argomenti.py:39
 msgid "correlato_in_evidenza_label"
 msgstr ""
 
-#. Default: "Cosa fa"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
+#. Default: "Competenze"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:201
 msgid "cosa_fa_label"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:177
+#: design/plone/contenttypes/interfaces/servizio.py:263
 msgid "cosa_serve"
 msgstr ""
 
 #. Default: "Descrizione delle istruzioni per usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:179
+#: design/plone/contenttypes/interfaces/servizio.py:265
 msgid "cosa_serve_help"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:384
+#: design/plone/contenttypes/interfaces/servizio.py:497
 msgid "cosa_serve_label"
 msgstr ""
 
 #. Default: "Cosa si ottiene"
-#: design/plone/contenttypes/interfaces/servizio.py:90
+#: design/plone/contenttypes/interfaces/servizio.py:135
 msgid "cosa_si_ottiene"
 msgstr ""
 
 #. Default: "Indicare cosa si può ottenere dal servizio, ad esempio 'carta di identità elettronica', 'certificato di residenza'."
-#: design/plone/contenttypes/interfaces/servizio.py:91
+#: design/plone/contenttypes/interfaces/servizio.py:136
 msgid "cosa_si_ottiene_help"
 msgstr ""
 
 #. Default: "Cos'è"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:40
-#: design/plone/contenttypes/behaviors/evento.py:200
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:52
+#: design/plone/contenttypes/behaviors/evento.py:155
 msgid "cose_label"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/interfaces/servizio.py:186
+#: design/plone/contenttypes/interfaces/servizio.py:272
 msgid "costi"
 msgstr ""
 
 #. Default: "Costi e vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:389
+#: design/plone/contenttypes/interfaces/servizio.py:502
 msgid "costi_e_vincoli_label"
 msgstr ""
 
 #. Default: "Descrizione delle condizioni e dei termini economici per completare la procedura di richiesta del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:188
+#: design/plone/contenttypes/interfaces/servizio.py:274
 msgid "costi_help"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/behaviors/evento.py:212
+#: design/plone/contenttypes/behaviors/evento.py:167
 msgid "costi_label"
 msgstr ""
 
 #. Default: "Allega un file contenente il curriculum vitae della persona. Se ha più file da allegare, utilizza questo campo per quello principale e gli altri mettili dentro alla cartella \"Curriculum vitae\" che troverai dentro alla Persona."
-#: design/plone/contenttypes/interfaces/persona.py:149
+#: design/plone/contenttypes/interfaces/persona.py:105
 msgid "curriculum_vitae_help"
 msgstr ""
 
 #. Default: "Curriculum vitae"
-#: design/plone/contenttypes/interfaces/persona.py:147
+#: design/plone/contenttypes/interfaces/persona.py:103
 msgid "curriculum_vitae_label"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction."
-#: design/plone/contenttypes/behaviors/trasparenza.py:254
+#: design/plone/contenttypes/behaviors/trasparenza.py:255
 msgid "customer_satisfaction_help"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction"
-#: design/plone/contenttypes/behaviors/trasparenza.py:249
+#: design/plone/contenttypes/behaviors/trasparenza.py:250
 msgid "customer_satisfaction_label"
 msgstr ""
 
-#. Default: "Data di conclusione dell'incarico."
-#: design/plone/contenttypes/interfaces/persona.py:60
-msgid "data_conclusione_incarico_help"
-msgstr ""
-
 #. Default: "Data conclusione incarico"
-#: design/plone/contenttypes/interfaces/persona.py:56
-msgid "data_conclusione_incarico_label"
+#: design/plone/contenttypes/interfaces/incarico.py:100
+msgid "data_conclusione_incarico"
 msgstr ""
 
 #. Default: "Data e fasi intermedie"
 #: design/plone/contenttypes/interfaces/documento_personale.py:120
 msgid "data_e_fasi_intermedie"
 msgstr ""
 
 #. Default: "Data di inizio"
 #: design/plone/contenttypes/interfaces/documento_personale.py:116
 msgid "data_inizio"
 msgstr ""
 
-#. Default: "Solo per persona politica: specificare la data di insediamento."
-#: design/plone/contenttypes/interfaces/persona.py:97
-msgid "data_insediamento_help"
+#. Default: "Data inizio incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:95
+msgid "data_inizio_incarico"
 msgstr ""
 
 #. Default: "Data insediamento"
-#: design/plone/contenttypes/interfaces/persona.py:96
-msgid "data_insediamento_label"
+#: design/plone/contenttypes/interfaces/incarico.py:105
+msgid "data_insediamento"
 msgstr ""
 
 #. Default: "Data del messaggio"
 #: design/plone/contenttypes/interfaces/messaggio.py:12
 msgid "data_messaggio"
 msgstr ""
 
 #. Default: "Data pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:21
 msgid "data_pagamento"
 msgstr ""
 
 #. Default: "Data del protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:41
 #: design/plone/contenttypes/interfaces/documento_personale.py:19
 msgid "data_protocollo"
 msgstr ""
 
+#. Default: "Data scadenza"
+#: design/plone/contenttypes/interfaces/servizio.py:49
+msgid "data_scadenza_label"
+msgstr ""
+
 #. Default: "Data di scadenza della procedura"
 #: design/plone/contenttypes/interfaces/messaggio.py:40
 msgid "data_scadenza_procedura"
 msgstr ""
 
 #. Default: "Dataset"
-#: design/plone/contenttypes/interfaces/dataset.py:27
+#: design/plone/contenttypes/interfaces/dataset.py:20
 msgid "dataset"
 msgstr ""
 
+#. Default: "Schede dataset collegate al documento"
+#: design/plone/contenttypes/interfaces/documento.py:150
+msgid "dataset_collegati_help"
+msgstr ""
+
 #. Default: "Seleziona una lista di schede dataset collegate a questo contenuto."
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:20
 msgid "dataset_correlati_help"
 msgstr ""
 
 #. Default: "Dataset correlati"
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:18
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
 msgid "dataset_correlati_label"
 msgstr ""
 
+#. Default: "Dataset collegati"
+#: design/plone/contenttypes/interfaces/documento.py:146
+msgid "dataset_label"
+msgstr ""
+
+#. Default: "Date e informazioni"
+#: design/plone/contenttypes/interfaces/incarico.py:175
+msgid "date_e_informazioni_label"
+msgstr ""
+
 #. Default: "Date e orari"
-#: design/plone/contenttypes/behaviors/evento.py:209
-#: design/plone/contenttypes/schema_overrides.py:34
+#: design/plone/contenttypes/behaviors/evento.py:164
+#: design/plone/contenttypes/schema_overrides.py:33
 msgid "date_e_orari_label"
 msgstr ""
 
 #. Default: "Inserisci la decorrenza termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:69
+#: design/plone/contenttypes/behaviors/trasparenza.py:70
 msgid "decorrenza_termini_help"
 msgstr ""
 
 #. Default: "Decorrenza termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:64
+#: design/plone/contenttypes/behaviors/trasparenza.py:65
 msgid "decorrenza_termini_label"
 msgstr ""
 
 #. Default: "Elenco delle deleghe a capo della persona."
-#: design/plone/contenttypes/interfaces/persona.py:77
+#: design/plone/contenttypes/interfaces/persona.py:85
 msgid "deleghe_help"
 msgstr ""
 
 #. Default: "Deleghe"
-#: design/plone/contenttypes/interfaces/persona.py:76
+#: design/plone/contenttypes/interfaces/persona.py:84
 msgid "deleghe_label"
 msgstr ""
 
 #. Default: "Descrizione completa"
-#: design/plone/contenttypes/behaviors/luogo.py:23
+#: design/plone/contenttypes/behaviors/luogo.py:24
 msgid "descrizione_completa"
 msgstr ""
 
-#. Default: "Descrizione destinatari"
-#: design/plone/contenttypes/behaviors/evento.py:38
-msgid "descrizione_destinatari"
-msgstr ""
-
-#. Default: "Descrizione dei principali interlocutori dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:40
-msgid "descrizione_destinatari_help"
-msgstr ""
-
 #. Default: "Descrizione estesa"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:16
-#: design/plone/contenttypes/behaviors/evento.py:30
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:19
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:17
+#: design/plone/contenttypes/behaviors/evento.py:32
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
 msgid "descrizione_estesa"
 msgstr ""
 
 #. Default: "Descrizione dettagliata e completa."
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:18
-#: design/plone/contenttypes/behaviors/evento.py:32
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:19
+#: design/plone/contenttypes/behaviors/evento.py:34
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:23
 msgid "descrizione_estesa_help"
 msgstr ""
 
 #. Default: "Descrizione"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:51
-#: design/plone/contenttypes/behaviors/luogo.py:166
-#: design/plone/contenttypes/interfaces/documento.py:162
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:72
+#: design/plone/contenttypes/behaviors/luogo.py:135
+#: design/plone/contenttypes/interfaces/documento.py:242
 msgid "descrizione_label"
 msgstr ""
 
 #. Default: "Inserisci eventuale testo descrittivo del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:37
+#: design/plone/contenttypes/behaviors/trasparenza.py:38
 msgid "descrizione_procedimento_help"
 msgstr ""
 
 #. Default: "Descrizione del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:32
+#: design/plone/contenttypes/behaviors/trasparenza.py:33
 msgid "descrizione_procedimento_label"
 msgstr ""
 
 #. Default: "Dirigente"
-#: design/plone/contenttypes/behaviors/trasparenza.py:136
+#: design/plone/contenttypes/behaviors/trasparenza.py:137
 msgid "dirigente"
 msgstr ""
 
 #. Default: "Indicare il dirigente."
-#: design/plone/contenttypes/behaviors/trasparenza.py:140
+#: design/plone/contenttypes/behaviors/trasparenza.py:141
 msgid "dirigente_help"
 msgstr ""
 
 #. Default: "Distribuzione"
-#: design/plone/contenttypes/interfaces/dataset.py:22
+#: design/plone/contenttypes/interfaces/dataset.py:15
 msgid "distribuzione"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/messaggio.py:56
+#: design/plone/contenttypes/interfaces/messaggio.py:48
 msgid "documenti_allegati"
 msgstr ""
 
 #. Default: "Seleziona una serie di altri contenuti di tipo Documento che vanno allegati a questo."
-#: design/plone/contenttypes/interfaces/documento.py:113
+#: design/plone/contenttypes/interfaces/documento.py:194
 msgid "documenti_allegati_help"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/documento.py:109
+#: design/plone/contenttypes/interfaces/documento.py:190
 msgid "documenti_allegati_label"
 msgstr ""
 
 #. Default: "Documenti"
-#: design/plone/contenttypes/interfaces/persona.py:199
-#: design/plone/contenttypes/interfaces/servizio.py:412
+#: design/plone/contenttypes/interfaces/persona.py:146
+#: design/plone/contenttypes/interfaces/servizio.py:525
 msgid "documenti_label"
 msgstr ""
 
+#. Default: "Documenti pubblici importanti, collegati a questa Unità Organizzativa"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:129
+msgid "documenti_pubblici_help"
+msgstr ""
+
+#. Default: "Documenti pubblici"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:127
+msgid "documenti_pubblici_label"
+msgstr ""
+
 #. Default: "Dove"
-#: design/plone/contenttypes/behaviors/address.py:71
-#: design/plone/contenttypes/behaviors/geolocation.py:29
+#: design/plone/contenttypes/behaviors/address.py:53
+#: design/plone/contenttypes/behaviors/geolocation.py:26
 msgid "dove_label"
 msgstr ""
 
 #. Default: "Dove rivolgersi: informazioni aggiuntive"
-#: design/plone/contenttypes/interfaces/servizio.py:143
+#: design/plone/contenttypes/interfaces/servizio.py:212
 msgid "dove_rivolgersi_extra"
 msgstr ""
 
 #. Default: "Indicare eventuali informazioni aggiuntive riguardo al dove rivolgersi per questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:147
+#: design/plone/contenttypes/interfaces/servizio.py:216
 msgid "dove_rivolgersi_extra_help"
 msgstr ""
 
 #. Default: "Seleziona una lista delle sedi e dei luoghi in cui è presente questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:135
+#: design/plone/contenttypes/interfaces/servizio.py:204
 msgid "dove_rivolgersi_help"
 msgstr ""
 
 #. Default: "Elementi di interesse"
-#: design/plone/contenttypes/behaviors/luogo.py:44
+#: design/plone/contenttypes/behaviors/luogo.py:45
 msgid "elementi_di_interesse"
 msgstr ""
 
-#. Default: "Indicare un indirizzo mail per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:128
-msgid "email_event_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/evento.py:127
-msgid "email_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:35
-msgid "email_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/contatti.py:34
-msgid "email_label"
-msgstr ""
-
-#. Default: "Contatto mail della persona. E' possibile inserire più di un indirizzo. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:135
-msgid "email_persona_help"
-msgstr ""
-
-#. Default: "Indirizzo email"
-#: design/plone/contenttypes/interfaces/persona.py:134
-msgid "email_persona_label"
-msgstr ""
-
 #. Default: "Esito"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:51
 msgid "esito"
 msgstr ""
 
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/evento.py:113
-msgid "fax_event_help"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/evento.py:114
-msgid "fax_event_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/contatti.py:29
-msgid "fax_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/contatti.py:28
-msgid "fax_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/interfaces/persona.py:130
-msgid "fax_persona_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/interfaces/persona.py:129
-msgid "fax_persona_label"
+#. Default: "Escludi dalla ricerca"
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:17
+msgid "exclude_from_search_label"
 msgstr ""
 
 #. Default: "Inserisci il file correlato di questo pocedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:44
+#: design/plone/contenttypes/behaviors/trasparenza.py:45
 msgid "file_correlato_help"
 msgstr ""
 
 #. Default: "File correlato"
-#: design/plone/contenttypes/behaviors/trasparenza.py:43
+#: design/plone/contenttypes/behaviors/trasparenza.py:44
 msgid "file_correlato_label"
 msgstr ""
 
 #. Default: "Inserisci il file principale di questo contenuto."
-#: design/plone/contenttypes/behaviors/multi_file.py:16
+#: design/plone/contenttypes/behaviors/multi_file.py:17
 msgid "file_principale_help"
 msgstr ""
 
 #. Default: "File principale"
-#: design/plone/contenttypes/behaviors/multi_file.py:15
+#: design/plone/contenttypes/behaviors/multi_file.py:16
 msgid "file_principale_label"
 msgstr ""
 
 #. Default: "Inserisci la fine termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:80
+#: design/plone/contenttypes/behaviors/trasparenza.py:81
 msgid "fine_termine_help"
 msgstr ""
 
 #. Default: "Fine termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:75
+#: design/plone/contenttypes/behaviors/trasparenza.py:76
 msgid "fine_termine_label"
 msgstr ""
 
+#. Default: "Lista dei formati in cui è disponibile il documento"
+#: design/plone/contenttypes/interfaces/documento.py:117
+msgid "formati_disponibili_help"
+msgstr ""
+
+#. Default: "Formati disponibili"
+#: design/plone/contenttypes/interfaces/documento.py:116
+msgid "formati_disponibili_label"
+msgstr ""
+
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:25
+#: design/plone/contenttypes/behaviors/multi_file.py:26
 msgid "formato_alternativo_1_help"
 msgstr ""
 
 #. Default: "Formato alternativo 1"
-#: design/plone/contenttypes/behaviors/multi_file.py:24
+#: design/plone/contenttypes/behaviors/multi_file.py:25
 msgid "formato_alternativo_1_label"
 msgstr ""
 
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:35
+#: design/plone/contenttypes/behaviors/multi_file.py:36
 msgid "formato_alternativo_2_help"
 msgstr ""
 
 #. Default: "Formato alternativo 2"
-#: design/plone/contenttypes/behaviors/multi_file.py:34
+#: design/plone/contenttypes/behaviors/multi_file.py:35
 msgid "formato_alternativo_2_label"
 msgstr ""
 
-#. Default: "Foto da mostrare della persona. La dimensione suggerita è 180x100 px."
-#: design/plone/contenttypes/interfaces/persona.py:21
+#. Default: "Foto da mostrare della persona. La dimensione suggerita è 100x180px."
+#: design/plone/contenttypes/interfaces/persona.py:30
 msgid "foto_persona_help"
 msgstr ""
 
 #. Default: "Foto della persona"
-#: design/plone/contenttypes/interfaces/persona.py:19
+#: design/plone/contenttypes/interfaces/persona.py:28
 msgid "foto_persona_label"
 msgstr ""
 
 #. Default: "Frequenza di aggiornamento"
-#: design/plone/contenttypes/interfaces/dataset.py:32
+#: design/plone/contenttypes/interfaces/dataset.py:25
 msgid "frequenza_aggiornamento"
 msgstr ""
 
 #. Default: "Invalid geolocation data: ${value}. Provide latitude and longitude coordinates."
-#: design/plone/contenttypes/restapi/deserializers/dxfields.py:28
+#: design/plone/contenttypes/restapi/deserializers/dxfields.py:39
 msgid "geolocation_field_validator_label"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/address.py:38
 msgid "help_circoscrizione"
 msgstr ""
 
 #. Default: "Indicare una descrizione completa, inserendo tutte le informazioni rilevanti relative al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:24
+#: design/plone/contenttypes/behaviors/luogo.py:25
 msgid "help_descrizione_completa"
 msgstr ""
 
 #. Default: "Indicare eventuali elementi di interesse per il cittadino."
-#: design/plone/contenttypes/behaviors/luogo.py:45
+#: design/plone/contenttypes/behaviors/luogo.py:46
 msgid "help_elementi_di_interesse"
 msgstr ""
 
+#. Default: "Se selezionato, questo contenuto non verrà mostrato nelle ricerche del sito per gli utenti anonimi."
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:18
+msgid "help_exclude_from_search"
+msgstr ""
+
 #. Default: "Indicare tutte le informazioni relative alla modalità di accesso al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:54
+#: design/plone/contenttypes/behaviors/luogo.py:55
 msgid "help_modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare, se esiste, un nome alternativo per il luogo; questo sarà mostrato affianco al titolo della scheda"
-#: design/plone/contenttypes/behaviors/luogo.py:34
+#: design/plone/contenttypes/behaviors/luogo.py:35
 msgid "help_nome_alternativo"
 msgstr ""
 
 #. Default: "Inserisci il nome della sede, se non è presente tra i Luoghi del sito."
 #: design/plone/contenttypes/behaviors/address.py:17
 msgid "help_nome_sede"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/address.py:32
 msgid "help_quartiere"
 msgstr ""
 
-#. Default: "Indicare un numero di fax della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:108
-msgid "help_riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:119
-msgid "help_riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:132
-msgid "help_riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Indicare il riferimento telefonico per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:96
-msgid "help_riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato.Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
-#: design/plone/contenttypes/behaviors/update_note.py:17
+#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato. Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
+#: design/plone/contenttypes/behaviors/update_note.py:18
 msgid "help_update_note"
 msgstr ""
 
 #. Default: "Icona"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:27
 msgid "icona"
 msgstr ""
 
 #. Default: "Puoi selezionare un’icona fra quelle proposte nel menu a tendina oppure puoi scrivere/incollare nel campo di testo il nome di un’icona di fontawsome 5"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:28
 msgid "icona_help"
 msgstr ""
 
 #. Default: "Identificativo"
-#: design/plone/contenttypes/interfaces/servizio.py:290
+#: design/plone/contenttypes/interfaces/servizio.py:379
 msgid "identificativo"
 msgstr ""
 
 #. Default: "Un numero identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:21
 msgid "identificativo_documento_help"
 msgstr ""
 
 #. Default: "Identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:17
 msgid "identificativo_documento_label"
 msgstr ""
 
 #. Default: "Eventuale codice identificativo del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:292
+#: design/plone/contenttypes/interfaces/servizio.py:381
 msgid "identificativo_help"
 msgstr ""
 
+#. Default: "Identificativo"
+#: design/plone/contenttypes/behaviors/luogo.py:119
+msgid "identificativo_mibac"
+msgstr ""
+
+#. Default: "Codice identificativo del luogo. Nel MIBAC c'è il codice del DBUnico per i luoghi della cultura e il codice ISIL per le biblioteche. Non deve comparire nel frontend del sito."
+#: design/plone/contenttypes/behaviors/luogo.py:121
+msgid "identificativo_mibac_help"
+msgstr ""
+
 #. Default: "La dimensione dell'immagine dovrebbe essere di ${size} px"
-#: design/plone/contenttypes/restapi/types/adapters.py:31
+#: design/plone/contenttypes/restapi/types/adapters.py:43
 msgid "image_size_help"
 msgstr ""
 
 #. Default: "Immagine"
 #: design/plone/contenttypes/interfaces/documento_personale.py:23
 msgid "immagine"
 msgstr ""
 
+#. Default: "Solo per incarico politico: importi di viaggi di servizio  e missioni pagati con fondi pubblici."
+#: design/plone/contenttypes/interfaces/incarico.py:34
+msgid "importi_viaggio_servizio_incarico_help"
+msgstr ""
+
+#. Default: "Importi di viaggio e/o servizio"
+#: design/plone/contenttypes/interfaces/incarico.py:30
+msgid "importi_viaggio_servizio_incarico_label"
+msgstr ""
+
 #. Default: "Importo pagato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:25
 msgid "importo_pagato"
 msgstr ""
 
+#. Default: "Seleziona l'incarico corrente della persona."
+#: design/plone/contenttypes/interfaces/persona.py:63
+msgid "incarichi_help"
+msgstr ""
+
+#. Default: "Incarichi"
+#: design/plone/contenttypes/interfaces/persona.py:59
+msgid "incarichi_label"
+msgstr ""
+
 #. Default: "Inserisci eventuale testo informativo che verrà mostrato in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:23
 msgid "info_testata_help"
 msgstr ""
 
 #. Default: "Informazioni aggiuntive per la testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:18
@@ -1706,127 +1728,162 @@
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/interfaces/documento_personale.py:140
 msgid "informazioni"
 msgstr ""
 
+#. Default: "Compensi e trasparenza"
+#: design/plone/contenttypes/interfaces/incarico.py:170
+msgid "informazioni_compensi_label"
+msgstr ""
+
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/behaviors/additional_help_infos.py:28
-#: design/plone/contenttypes/behaviors/evento.py:229
 #: design/plone/contenttypes/behaviors/strutture_correlate.py:42
+#: design/plone/contenttypes/interfaces/documento.py:253
 msgid "informazioni_label"
 msgstr ""
 
+#. Default: "Intervallo della fase (es. 1)"
+#: design/plone/contenttypes/interfaces/servizio.py:32
+msgid "interval_qt_help"
+msgstr ""
+
+#. Default: "Intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:31
+msgid "interval_qt_label"
+msgstr ""
+
+#. Default: "Ad esempio: ore, giorni, settimane, mesi."
+#: design/plone/contenttypes/interfaces/servizio.py:41
+msgid "interval_type_help"
+msgstr ""
+
+#. Default: "Tipo intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:40
+msgid "interval_type_label"
+msgstr ""
+
 #. Default: "Se un content-type deve avere una dimensione della leadimage particolare, indicarle qui. Inserire le dimensioni nella forma di esempio PortalType|900x900"
-#: design/plone/contenttypes/controlpanels/settings.py:110
+#: design/plone/contenttypes/controlpanels/settings.py:52
 msgid "lead_image_dimension_help"
 msgstr ""
 
 #. Default: "Dimensioni lead image"
-#: design/plone/contenttypes/controlpanels/settings.py:106
+#: design/plone/contenttypes/controlpanels/settings.py:48
 msgid "lead_image_dimension_label"
 msgstr ""
 
-#. Default: "Servizi o uffici di riferimento"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:27
+#. Default: "Strutture o uffici di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
 msgid "legami_altre_strutture_label"
 msgstr ""
 
 #. Default: "Selezionare la lista di strutture e/o uffici collegati a questa unità organizzativa."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:35
 msgid "legami_con_altre_strutture_help"
 msgstr ""
 
 #. Default: "Licenza"
-#: design/plone/contenttypes/interfaces/dataset.py:25
+#: design/plone/contenttypes/interfaces/dataset.py:18
 msgid "licenza"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
 #: design/plone/contenttypes/interfaces/documento_personale.py:92
 msgid "licenza_distribuzione"
 msgstr ""
 
 #. Default: "La licenza con il quale viene distribuito questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:88
+#: design/plone/contenttypes/interfaces/documento.py:125
 msgid "licenza_distribuzione_help"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
-#: design/plone/contenttypes/interfaces/documento.py:87
+#: design/plone/contenttypes/interfaces/documento.py:124
 msgid "licenza_distribuzione_label"
 msgstr ""
 
 #. Default: "Link a siti esterni"
-#: design/plone/contenttypes/interfaces/servizio.py:258
+#: design/plone/contenttypes/interfaces/servizio.py:347
 msgid "link_siti_esterni"
 msgstr ""
 
 #. Default: "Eventuali collegamenti a pagine web, siti, servizi esterni all'ambito Comunale utili all'erogazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:260
+#: design/plone/contenttypes/interfaces/servizio.py:349
 msgid "link_siti_esterni_help"
 msgstr ""
 
 #. Default: "Link utili"
-#: design/plone/contenttypes/interfaces/servizio.py:417
+#: design/plone/contenttypes/interfaces/servizio.py:530
 msgid "link_utili_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati. Se il luogo dell'evento non è presente sul sito, inserisci le sue informazioni nei campi seguenti."
 #: design/plone/contenttypes/behaviors/luoghi_correlati.py:52
 msgid "luoghi_correlati_event_help"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati."
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:72
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:19
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:64
 msgid "luoghi_correlati_help"
 msgstr ""
 
 #. Default: "Luoghi correlati"
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:17
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:71
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:63
 msgid "luoghi_correlati_label"
 msgstr ""
 
 #. Default: "Luogo"
-#: design/plone/contenttypes/behaviors/address.py:89
-#: design/plone/contenttypes/behaviors/geolocation.py:38
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:74
+#: design/plone/contenttypes/behaviors/address.py:71
+#: design/plone/contenttypes/behaviors/geolocation.py:34
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:76
 msgid "luogo_label"
 msgstr ""
 
+#. Default: "Sottotitolo"
+#: design/plone/contenttypes/interfaces/servizio.py:26
+msgid "milestone_description_label"
+msgstr ""
+
+#. Default: "Titolo"
+#: design/plone/contenttypes/interfaces/servizio.py:21
+msgid "milestone_label"
+msgstr ""
+
 #. Default: "Modalita' di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:53
+#: design/plone/contenttypes/behaviors/luogo.py:54
 msgid "modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare la modalità di avvio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:25
+#: design/plone/contenttypes/behaviors/trasparenza.py:26
 msgid "modalita_avvio_help"
 msgstr ""
 
 #. Default: "Modalita di avvio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:24
+#: design/plone/contenttypes/behaviors/trasparenza.py:25
 msgid "modalita_avvio_label"
 msgstr ""
 
 #. Default: "Modalità pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:29
 msgid "modalita_pagamento"
 msgstr ""
 
 #. Default: "Indicare le modalità per richiedere informazioni riguardo a questo procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:168
+#: design/plone/contenttypes/behaviors/trasparenza.py:169
 msgid "modalita_richiesta_informazioni_help"
 msgstr ""
 
 #. Default: "Modalità per richiedere informazioni"
-#: design/plone/contenttypes/behaviors/trasparenza.py:163
+#: design/plone/contenttypes/behaviors/trasparenza.py:164
 msgid "modalita_richiesta_informazioni_label"
 msgstr ""
 
 #. Default: "Seleziona se mostrare o meno i bottoni con i link per la condivisione sui vari social, mail e stampa."
 #: design/plone/contenttypes/behaviors/info_testata.py:44
 msgid "mostra_bottoni_condivisione_help"
 msgstr ""
@@ -1842,46 +1899,46 @@
 msgstr ""
 
 #. Default: "Mostra la navigazione"
 #: design/plone/contenttypes/behaviors/info_testata.py:51
 msgid "mostra_navigazione_label"
 msgstr ""
 
-#. Default: "Descrizione del motivo per cui il servizio non è attivo."
-#: design/plone/contenttypes/interfaces/servizio.py:44
+#. Default: "Descrizione del motivo per cui il servizio non è attivo. È obbligatorio se il campo precedente è spuntato."
+#: design/plone/contenttypes/interfaces/servizio.py:89
 msgid "motivo_stato_servizio_help"
 msgstr ""
 
-#. Default: "Motivo dello stato del servizio nel caso non sia attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:39
+#. Default: "Motivo dello stato"
+#: design/plone/contenttypes/interfaces/servizio.py:84
 msgid "motivo_stato_servizio_label"
 msgstr ""
 
 #. Default: "Nome alternativo"
-#: design/plone/contenttypes/behaviors/luogo.py:33
+#: design/plone/contenttypes/behaviors/luogo.py:34
 msgid "nome_alternativo"
 msgstr ""
 
 #. Default: "Nome sede"
 #: design/plone/contenttypes/behaviors/address.py:16
 msgid "nome_sede"
 msgstr ""
 
 #. Default: "Seleziona una lista di notizie correlate a questa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:83
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:75
 msgid "notizie_correlate_help"
 msgstr ""
 
 #. Default: "Notizie correlate"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:82
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:74
 msgid "notizie_correlate_label"
 msgstr ""
 
 #. Default: "Numero progressivo del comunicato stampa"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:30
 msgid "numero_progressivo_cs_label"
 msgstr ""
 
 #. Default: "Numero protocollo"
 #: design/plone/contenttypes/interfaces/pratica.py:12
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:12
 msgid "numero_protocollo"
@@ -1889,125 +1946,163 @@
 
 #. Default: "Oggetto"
 #: design/plone/contenttypes/interfaces/documento_personale.py:48
 msgid "oggetto"
 msgstr ""
 
 #. Default: "Informazioni sugli orari"
-#: design/plone/contenttypes/behaviors/evento.py:62
+#: design/plone/contenttypes/behaviors/evento.py:50
 msgid "orari"
 msgstr ""
 
 #. Default: "Informazioni sugli orari di svolgimento dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:64
+#: design/plone/contenttypes/behaviors/evento.py:52
 msgid "orari_help"
 msgstr ""
 
 #. Default: "Orari di apertura"
-#: design/plone/contenttypes/behaviors/contatti.py:86
+#: design/plone/contenttypes/behaviors/luogo.py:151
 msgid "orari_label"
 msgstr ""
 
+#. Default: "Orario per il pubblico"
+#: design/plone/contenttypes/behaviors/luogo.py:93
+msgid "orario_pubblico"
+msgstr ""
+
 #. Default: "Indicare eventuali orari di accesso al pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:59
+#: design/plone/contenttypes/behaviors/contatti.py:40
+#: design/plone/contenttypes/behaviors/luogo.py:95
 msgid "orario_pubblico_help"
 msgstr ""
 
 #. Default: "Orario per il pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:58
+#: design/plone/contenttypes/behaviors/contatti.py:39
 msgid "orario_pubblico_label"
 msgstr ""
 
 #. Default: "Se l'evento non è organizzato direttamente dal comune oppure ha anche un organizzatore esterno, indicare il nome del contatto."
-#: design/plone/contenttypes/behaviors/evento.py:97
+#: design/plone/contenttypes/behaviors/evento.py:86
 msgid "organizzato_da_esterno_help"
 msgstr ""
 
 #. Default: "Organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:95
+#: design/plone/contenttypes/behaviors/evento.py:84
 msgid "organizzato_da_esterno_label"
 msgstr ""
 
 #. Default: "Se l'evento è organizzato direttamente dal comune, indicare l'ufficio/ente organizzatore. I dati di contatto verranno presi direttamente dall'ufficio selezionato. Se l'evento non è organizzato direttamente dal comune, o si vogliono sovrascrivere alcuni dati di contatto, utilizzare i seguenti campi."
-#: design/plone/contenttypes/behaviors/evento.py:84
+#: design/plone/contenttypes/behaviors/evento.py:74
 msgid "organizzato_da_interno_help"
 msgstr ""
 
 #. Default: "Organizzato da"
-#: design/plone/contenttypes/behaviors/evento.py:80
+#: design/plone/contenttypes/behaviors/evento.py:70
 msgid "organizzato_da_interno_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di organizzazioni a cui la persona appartiene."
-#: design/plone/contenttypes/interfaces/persona.py:42
+#: design/plone/contenttypes/interfaces/persona.py:45
 msgid "organizzazione_riferimento_help"
 msgstr ""
 
 #. Default: "Organizzazione di riferimento"
-#: design/plone/contenttypes/interfaces/persona.py:38
+#: design/plone/contenttypes/interfaces/persona.py:41
 msgid "organizzazione_riferimento_label"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:157
+#: design/plone/contenttypes/behaviors/trasparenza.py:158
 msgid "organo_competente_provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:152
+#: design/plone/contenttypes/behaviors/trasparenza.py:153
 msgid "organo_competente_provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Indicare le informazioni riguardanti i pagamenti previsti e modalità di pagamento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:222
+#: design/plone/contenttypes/behaviors/trasparenza.py:223
 msgid "pagamenti_help"
 msgstr ""
 
 #. Default: "Pagamenti previsti e modalità"
-#: design/plone/contenttypes/behaviors/trasparenza.py:218
+#: design/plone/contenttypes/behaviors/trasparenza.py:219
 msgid "pagamenti_label"
 msgstr ""
 
+#. Default: "Link a persone dell'amministrazione che interverranno all'evento"
+#: design/plone/contenttypes/behaviors/evento.py:118
+msgid "parteciperanno_help"
+msgstr ""
+
+#. Default: "Parteciperanno (Persone)"
+#: design/plone/contenttypes/behaviors/evento.py:114
+msgid "parteciperanno_label"
+msgstr ""
+
 #. Default: "Indicare l'ente che supporta l'evento, se presente."
-#: design/plone/contenttypes/behaviors/evento.py:160
+#: design/plone/contenttypes/behaviors/evento.py:107
 msgid "patrocinato_da_help"
 msgstr ""
 
 #. Default: "Patrocinato da"
-#: design/plone/contenttypes/behaviors/evento.py:158
+#: design/plone/contenttypes/behaviors/evento.py:105
 msgid "patrocinato_da_label"
 msgstr ""
 
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:44
-msgid "pec_help"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:27
+msgid "pdc_desc_help"
 msgstr ""
 
-#. Default: "Pec"
-#: design/plone/contenttypes/behaviors/contatti.py:43
-msgid "pec_label"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:26
+msgid "pdc_desc_label"
 msgstr ""
 
-#. Default: "Elenco delle persone dell'amministrazione che parteciperanno all'evento."
-#: design/plone/contenttypes/behaviors/evento.py:53
-msgid "persone_amministrazione_help"
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:16
+msgid "pdc_type_label"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:37
+msgid "pdc_value_help"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:36
+msgid "pdc_value_label"
+msgstr ""
+
+#. Default: "Seleziona la persona che ha questo incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:47
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:66
+msgid "persona_incarico_help"
+msgstr ""
+
+#. Default: "La persona che ha la carica e l'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:43
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:62
+msgid "persona_incarico_label"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:221
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:215
 msgid "persone_label"
 msgstr ""
 
 #. Default: "Seleziona la lista delle persone che compongono la struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
 msgid "persone_struttura_help"
 msgstr ""
 
 #. Default: "Persone che compongono la struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:79
 msgid "persone_struttura_label"
 msgstr ""
 
 #. Default: "Pratica associata"
 #: design/plone/contenttypes/interfaces/documento_personale.py:26
 #: design/plone/contenttypes/interfaces/messaggio.py:35
 msgid "pratica_associata"
@@ -2015,255 +2110,230 @@
 
 #. Default: "Pratica associata al pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:43
 msgid "pratica_associata_ricevuta"
 msgstr ""
 
 #. Default: "Prenota un appuntamento"
-#: design/plone/contenttypes/interfaces/servizio.py:156
+#: design/plone/contenttypes/interfaces/servizio.py:225
 msgid "prenota_appuntamento"
 msgstr ""
 
 #. Default: "Se è possibile prenotare un'appuntamento, indicare le informazioni necessarie e il collegamento al servizio di prenotazione appuntamenti del Comune."
-#: design/plone/contenttypes/interfaces/servizio.py:157
+#: design/plone/contenttypes/interfaces/servizio.py:226
 msgid "prenota_appuntamento_help"
 msgstr ""
 
-#. Default: "Prezzo"
-#: design/plone/contenttypes/behaviors/evento.py:71
+#. Default: "Costo"
+#: design/plone/contenttypes/behaviors/evento.py:59
 msgid "prezzo"
 msgstr ""
 
-#. Default: "Indicare il prezzo dell'evento, se presente, specificando se esistono formati diversi."
-#: design/plone/contenttypes/behaviors/evento.py:73
+#. Default: "Eventuale costo dell'evento (se ci sono uno o più biglietti), con link all'acquisto se disponibile"
+#: design/plone/contenttypes/behaviors/evento.py:61
 msgid "prezzo_help"
 msgstr ""
 
 #. Default: "Indicare, se la procedura è informatizzata online, il riferimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:178
+#: design/plone/contenttypes/behaviors/trasparenza.py:179
 msgid "procedura_online_help"
 msgstr ""
 
 #. Default: "Procedura informatizzata online"
-#: design/plone/contenttypes/behaviors/trasparenza.py:174
+#: design/plone/contenttypes/behaviors/trasparenza.py:175
 msgid "procedura_online_label"
 msgstr ""
 
 #. Default: "Procedure collegate all'esito"
-#: design/plone/contenttypes/interfaces/servizio.py:100
+#: design/plone/contenttypes/interfaces/servizio.py:145
 msgid "procedure_collegate"
 msgstr ""
 
 #. Default: "Indicare cosa deve fare l'utente del servizio per conoscere l'esito della procedura, e dove eventualmente poter ritirare l'esito."
-#: design/plone/contenttypes/interfaces/servizio.py:102
+#: design/plone/contenttypes/interfaces/servizio.py:147
 msgid "procedure_collegate_help"
 msgstr ""
 
 #. Default: "Protocollo"
 #: design/plone/contenttypes/interfaces/documento_personale.py:15
 msgid "protocollo"
 msgstr ""
 
+#. Default: "Il numero di protocollo del documento."
+#: design/plone/contenttypes/interfaces/documento.py:33
+msgid "protocollo_documento_help"
+msgstr ""
+
+#. Default: "Numero di protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:29
+msgid "protocollo_documento_label"
+msgstr ""
+
 #. Default: "Eventuale provvedimento finale del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:114
+#: design/plone/contenttypes/behaviors/trasparenza.py:115
 msgid "provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Provvedimento del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:109
+#: design/plone/contenttypes/behaviors/trasparenza.py:110
 msgid "provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Quartiere"
 #: design/plone/contenttypes/behaviors/address.py:31
 msgid "quartiere"
 msgstr ""
 
-#. Default: "Reperibilità organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:118
-msgid "reperibilita"
-msgstr ""
-
-#. Default: "Indicare gli orari in cui l'organizzatore è telefonicamente reperibile."
-#: design/plone/contenttypes/behaviors/evento.py:120
-msgid "reperibilita_help"
-msgstr ""
-
 #. Default: "Indicare dove è possibile reperre la modulistica per il procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:211
+#: design/plone/contenttypes/behaviors/trasparenza.py:212
 msgid "reperimento_modulistica_help"
 msgstr ""
 
 #. Default: "Dove reperire la modulistica"
-#: design/plone/contenttypes/behaviors/trasparenza.py:207
+#: design/plone/contenttypes/behaviors/trasparenza.py:208
 msgid "reperimento_modulistica_label"
 msgstr ""
 
 #. Default: "Selezionare il/i responsabile/i della struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:48
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:52
 msgid "responsabile_help"
 msgstr ""
 
 #. Default: "Responsabile"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:43
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:47
 msgid "responsabile_label"
 msgstr ""
 
 #. Default: "Responsabile del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:120
+#: design/plone/contenttypes/behaviors/trasparenza.py:121
 msgid "responsabile_procedimento"
 msgstr ""
 
 #. Default: "Indicare il responsabile del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:124
+#: design/plone/contenttypes/behaviors/trasparenza.py:125
 msgid "responsabile_procedimento_help"
 msgstr ""
 
+#. Default: "Se è un incarico di responsabilità, specificare l'organizzazione della quale è responsabile in base all'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:81
+msgid "responsabile_struttura_incarico_help"
+msgstr ""
+
+#. Default: "Responsabile della struttura"
+#: design/plone/contenttypes/interfaces/incarico.py:77
+msgid "responsabile_struttura_incarico_label"
+msgstr ""
+
 #. Default: "Seleziona se mostrare o meno il campo di ricerca in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:32
 msgid "ricerca_in_testata_help"
 msgstr ""
 
 #. Default: "Ricerca in testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:29
 msgid "ricerca_in_testata_label"
 msgstr ""
 
 #. Default: "Ulteriori informazioni non previste negli altri campi; si può trattare di contatti o note informative la cui conoscenza è indispensabile per la partecipazione al bando"
-#: design/plone/contenttypes/interfaces/bando.py:96
+#: design/plone/contenttypes/interfaces/bando.py:97
 msgid "riferimenti_bando_agid_help"
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
-#: design/plone/contenttypes/interfaces/bando.py:95
+#: design/plone/contenttypes/interfaces/bando.py:96
 msgid "riferimenti_bando_agid_label"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
 #: design/plone/contenttypes/interfaces/documento_personale.py:145
 msgid "riferimenti_normativi"
 msgstr ""
 
 #. Default: "Inserisici del testo di dettaglio per eventuali riferimenti normativi utili a questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:100
+#: design/plone/contenttypes/interfaces/documento.py:137
 msgid "riferimenti_normativi_documento_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/interfaces/documento.py:96
+#: design/plone/contenttypes/interfaces/documento.py:133
 msgid "riferimenti_normativi_documento_label"
 msgstr ""
 
 #. Default: "Indicare eventuali riferimenti normativi."
-#: design/plone/contenttypes/behaviors/trasparenza.py:265
+#: design/plone/contenttypes/behaviors/trasparenza.py:266
 msgid "riferimenti_normativi_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/behaviors/trasparenza.py:260
+#: design/plone/contenttypes/behaviors/trasparenza.py:261
 msgid "riferimenti_normativi_label"
 msgstr ""
 
-#. Default: "Fax della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:104
-msgid "riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "E-mail struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:115
-msgid "riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Pec della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:128
-msgid "riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Telefono della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:92
-msgid "riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per il ruolo di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:84
-msgid "ruoli_persona_help"
-msgstr ""
-
-#. Default: "Ruoli Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:83
-msgid "ruoli_persona_label"
-msgstr ""
-
-#. Default: "Seleziona il ruolo della persona tra quelli disponibili."
-#: design/plone/contenttypes/interfaces/persona.py:29
-msgid "ruolo_help"
-msgstr ""
-
 #. Default: "Ruolo"
-#: design/plone/contenttypes/interfaces/persona.py:28
+#: design/plone/contenttypes/interfaces/persona.py:135
 msgid "ruolo_label"
 msgstr ""
 
 #. Default: "Data entro la quale sarà possibile far pervenire domande e richieste di chiarimento a chi eroga il bando"
-#: design/plone/contenttypes/interfaces/bando.py:69
+#: design/plone/contenttypes/interfaces/bando.py:70
 msgid "scadenza_domande_bando_help"
 msgstr ""
 
 #. Default: "Termine per le richieste di chiarimenti"
-#: design/plone/contenttypes/interfaces/bando.py:65
+#: design/plone/contenttypes/interfaces/bando.py:66
 msgid "scadenza_domande_bando_label"
 msgstr ""
 
 #. Default: "Inserire una lista di sezioni per la ricerca."
-#: design/plone/contenttypes/controlpanels/settings.py:129
+#: design/plone/contenttypes/controlpanels/settings.py:71
 msgid "search_sections_help"
 msgstr ""
 
 #. Default: "Sezioni ricerca"
-#: design/plone/contenttypes/controlpanels/settings.py:128
+#: design/plone/contenttypes/controlpanels/settings.py:70
 msgid "search_sections_label"
 msgstr ""
 
-#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente un contenuto di tipo Luogo a cui far riferimento, puoi compilare i campi seguenti. Se selezioni un Luogo, puoi usare comunque i campi seguenti per sovrascrivere alcune informazioni."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:105
+#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente creare il Luogo nella sezione dedicata nell'alberatura del sito."
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:97
 msgid "sede_help"
 msgstr ""
 
 #. Default: "Sede principale"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:103
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
 msgid "sede_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di eventuali contenuti di tipo Luogo che sono sedi secondarie di questa struttura. Per queste sedi non sarà possibile sovrascrivere i dati. Nel caso servano informazioni diverse, è possibile usare il campo sottostante."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:122
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:112
 msgid "sedi_secondarie_help"
 msgstr ""
 
-#. Default: "Sedi secondarie"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:120
+#. Default: "Altre sedi"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:110
 msgid "sedi_secondarie_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei servizi collegati a questo."
-#: design/plone/contenttypes/interfaces/servizio.py:300
+#: design/plone/contenttypes/interfaces/servizio.py:394
 msgid "servizi_collegati_help"
 msgstr ""
 
 #. Default: "Servizi collegati"
-#: design/plone/contenttypes/interfaces/servizio.py:299
+#: design/plone/contenttypes/interfaces/servizio.py:393
 msgid "servizi_collegati_label"
 msgstr ""
 
 #. Default: "Questi servizi non verranno mostrati nel contenuto, ma permetteranno di vedere questo contenuto associato quando si visita il servizio"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:20
 msgid "servizi_correlati_description"
 msgstr ""
 
 #. Default: "Servizi correlati"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:18
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
 msgid "servizi_correlati_label"
 msgstr ""
 
 #. Default: "Servizio che genera il documento"
 #: design/plone/contenttypes/interfaces/documento_personale.py:31
 msgid "servizio_origine"
 msgstr ""
@@ -2275,367 +2345,292 @@
 
 #. Default: "Servizio che origina la pratica"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:35
 msgid "servizio_origine_ricevuta"
 msgstr ""
 
 #. Default: "Settore merceologico"
-#: design/plone/contenttypes/interfaces/servizio.py:280
+#: design/plone/contenttypes/interfaces/servizio.py:369
 msgid "settore_merceologico"
 msgstr ""
 
 #. Default: "Classificazione del servizio basata su catalogo dei servizi (Classificazione NACE)."
-#: design/plone/contenttypes/interfaces/servizio.py:282
+#: design/plone/contenttypes/interfaces/servizio.py:371
 msgid "settore_merceologico_help"
 msgstr ""
 
+#. Default: "Se selezionato, il footer verrà popolato automaticamente con i contenuti di primo livello non esclusi dalla navigazione."
+#: design/plone/contenttypes/controlpanels/settings.py:93
+msgid "show_dynamic_folders_in_footer_help"
+msgstr ""
+
+#. Default: "Footer dinamico"
+#: design/plone/contenttypes/controlpanels/settings.py:92
+msgid "show_dynamic_folders_in_footer_label"
+msgstr ""
+
 #. Default: "Questo è il valore di default per decidere se mostrare o meno la data di modifica nei contenuti che hanno la behavior abilitata. E' poi possibile sovrascrivere il default nei singoli contenuti (nel tab \"Impostazioni\")."
-#: design/plone/contenttypes/controlpanels/settings.py:139
+#: design/plone/contenttypes/controlpanels/settings.py:81
 msgid "show_modified_default_help"
 msgstr ""
 
 #. Default: "Mostra la data di modifica"
-#: design/plone/contenttypes/controlpanels/settings.py:138
+#: design/plone/contenttypes/controlpanels/settings.py:80
 msgid "show_modified_default_label"
 msgstr ""
 
 #. Default: "Se attivo, verrà mostrata la data di ultima modifica in visualizzazione del contenuto."
 #: design/plone/contenttypes/behaviors/show_modified.py:24
 msgid "show_modified_help"
 msgstr ""
 
 #. Default: "Mostra la data di ultima modifica"
 #: design/plone/contenttypes/behaviors/show_modified.py:23
 msgid "show_modified_label"
 msgstr ""
 
 #. Default: "Indicare se il procedimento prevede il silenzio assenso o la dichiarazione dell'interessato sostitutiva del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:103
+#: design/plone/contenttypes/behaviors/trasparenza.py:104
 msgid "silenzio_assenso_help"
 msgstr ""
 
 #. Default: "Silenzio assenso/Dichiarazione dell'interessato sostitutiva del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:97
+#: design/plone/contenttypes/behaviors/trasparenza.py:98
 msgid "silenzio_assenso_label"
 msgstr ""
 
 #. Default: "Inserisci eventuali soggetti esterni, nonché, strutture interne coinvolte nel procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:57
+#: design/plone/contenttypes/behaviors/trasparenza.py:58
 msgid "soggetti_eserni_help"
 msgstr ""
 
 #. Default: "Soggetti esterni, nonché, strutture interne coinvolte nel procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:52
+#: design/plone/contenttypes/behaviors/trasparenza.py:53
 msgid "soggetti_eserni_label"
 msgstr ""
 
 #. Default: "Indica un eventuale sottotitolo/titolo alternativo."
-#: design/plone/contenttypes/behaviors/evento.py:23
-#: design/plone/contenttypes/interfaces/servizio.py:19
+#: design/plone/contenttypes/behaviors/evento.py:24
+#: design/plone/contenttypes/interfaces/servizio.py:64
 msgid "sottotitolo_help"
 msgstr ""
 
 #. Default: "Sottotitolo"
-#: design/plone/contenttypes/behaviors/evento.py:22
-#: design/plone/contenttypes/interfaces/servizio.py:18
+#: design/plone/contenttypes/behaviors/evento.py:23
+#: design/plone/contenttypes/interfaces/servizio.py:63
 msgid "sottotitolo_label"
 msgstr ""
 
 #. Default: "Stampa ricevuta"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:17
 msgid "stampa_ricevuta"
 msgstr ""
 
 #. Default: "Stato della pratica"
 #: design/plone/contenttypes/interfaces/pratica.py:26
 msgid "stato_pratica"
 msgstr ""
 
-#. Default: "Indica se il servizio è effettivamente fruibile."
-#: design/plone/contenttypes/interfaces/servizio.py:32
+#. Default: "Indica se il servizio è effettivamente fruibile; spuntare se non è fruibile."
+#: design/plone/contenttypes/interfaces/servizio.py:77
 msgid "stato_servizio_help"
 msgstr ""
 
-#. Default: "Servizio non attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:30
+#. Default: "Servizio non fruibile"
+#: design/plone/contenttypes/interfaces/servizio.py:75
 msgid "stato_servizio_label"
 msgstr ""
 
 #. Default: "Indicare gli eventuali strumenti di tutela."
-#: design/plone/contenttypes/behaviors/trasparenza.py:230
+#: design/plone/contenttypes/behaviors/trasparenza.py:231
 msgid "strumenti_tutela_help"
 msgstr ""
 
 #. Default: "Strumenti di tutela"
-#: design/plone/contenttypes/behaviors/trasparenza.py:229
+#: design/plone/contenttypes/behaviors/trasparenza.py:230
 msgid "strumenti_tutela_label"
 msgstr ""
 
 #. Default: "Struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:211
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
 msgid "struttura_label"
 msgstr ""
 
 #. Default: "Struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:82
+#: design/plone/contenttypes/behaviors/luogo.py:83
 msgid "struttura_responsabile"
 msgstr ""
 
 #. Default: "Struttura responsabile del luogo."
-#: design/plone/contenttypes/behaviors/luogo.py:63
+#: design/plone/contenttypes/behaviors/luogo.py:64
 msgid "struttura_responsabile_correlati"
 msgstr ""
 
 #. Default: "Indicare la struttura responsabile del luogo qualora sia fra unità organizzative del comune inserite nel sito; altrimenti compilare i campi testuali relativi alla struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:67
+#: design/plone/contenttypes/behaviors/luogo.py:68
 msgid "struttura_responsabile_correlati_help"
 msgstr ""
 
 #. Default: "Nome/link al sito web della struttura che gestisce il luogo, se questa non è comunale."
-#: design/plone/contenttypes/behaviors/luogo.py:84
+#: design/plone/contenttypes/behaviors/luogo.py:85
 msgid "struttura_responsabile_help"
 msgstr ""
 
 #. Default: "Seleziona la lista delle strutture politiche coinvolte."
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:25
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:26
 msgid "strutture_politiche_help"
 msgstr ""
 
 #. Default: "Indicare gli uffici/enti che supportano l'evento."
-#: design/plone/contenttypes/behaviors/evento.py:149
+#: design/plone/contenttypes/behaviors/evento.py:97
 msgid "supportato_da_help"
 msgstr ""
 
 #. Default: "Evento supportato da"
-#: design/plone/contenttypes/behaviors/evento.py:145
+#: design/plone/contenttypes/behaviors/evento.py:93
 msgid "supportato_da_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di argomenti d'interesse per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:22
+#: design/plone/contenttypes/behaviors/argomenti.py:26
 msgid "tassonomia_argomenti_help"
 msgstr ""
 
-#. Default: "Tassonomia argomenti"
-#: design/plone/contenttypes/behaviors/argomenti.py:21
+#. Default: "Argomenti"
+#: design/plone/contenttypes/behaviors/argomenti.py:25
 msgid "tassonomia_argomenti_label"
 msgstr ""
 
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/evento.py:104
-msgid "telefono_event_help"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:105
-msgid "telefono_event_label"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:19
-msgid "telefono_help"
-msgstr ""
-
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/contatti.py:18
-msgid "telefono_label"
-msgstr ""
-
-#. Default: "Contatto telefonico della persona. E' possibile inserire più di un numero. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:117
-msgid "telefono_persona_help"
-msgstr ""
-
-#. Default: "Numero di telefono"
-#: design/plone/contenttypes/interfaces/persona.py:116
-msgid "telefono_persona_label"
-msgstr ""
-
-#. Default: "Temi"
-#: design/plone/contenttypes/interfaces/dataset.py:14
-msgid "temi"
-msgstr ""
-
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:167
+#: design/plone/contenttypes/interfaces/servizio.py:236
 msgid "tempi_e_scadenze"
 msgstr ""
 
 #. Default: "Descrivere le informazioni dettagliate riguardo eventuali tempi e scadenze di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:169
+#: design/plone/contenttypes/interfaces/servizio.py:238
 msgid "tempi_e_scadenze_help"
 msgstr ""
 
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:395
+#: design/plone/contenttypes/interfaces/servizio.py:508
 msgid "tempi_e_scadenze_label"
 msgstr ""
 
 #. Default: "Inserisci il tempo medio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:91
+#: design/plone/contenttypes/behaviors/trasparenza.py:92
 msgid "tempo_medio_help"
 msgstr ""
 
 #. Default: "Tempo medio del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:86
+#: design/plone/contenttypes/behaviors/trasparenza.py:87
 msgid "tempo_medio_label"
 msgstr ""
 
 #. Default: "Testata"
-#: design/plone/contenttypes/behaviors/argomenti.py:104
+#: design/plone/contenttypes/behaviors/argomenti.py:232
 #: design/plone/contenttypes/behaviors/info_testata.py:62
 msgid "testata_fieldset_label"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:28
+#: design/plone/contenttypes/interfaces/bando.py:29
 msgid "text_help"
 msgstr ""
 
 #. Default: "Testo"
-#: design/plone/contenttypes/interfaces/bando.py:27
+#: design/plone/contenttypes/interfaces/bando.py:28
 msgid "text_label"
 msgstr ""
 
-#. Default: "Tipologia documento"
-#: design/plone/contenttypes/interfaces/messaggio.py:49
-msgid "tipologia_documento"
-msgstr ""
-
-#. Default: "Seleziona la tipologia del documento."
-#: design/plone/contenttypes/interfaces/documento.py:30
-msgid "tipologia_documento_help"
-msgstr ""
-
-#. Default: "Tipologia del documento"
-#: design/plone/contenttypes/interfaces/documento.py:29
-msgid "tipologia_documento_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia della notizia."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:29
-msgid "tipologia_notizia_help"
-msgstr ""
-
-#. Default: "Tipologia notizia"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:28
-msgid "tipologia_notizia_label"
-msgstr ""
-
-#. Default: "Specificare la tipologia di organizzazione: politica, amminsitrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:60
-msgid "tipologia_organizzazione_help"
-msgstr ""
-
-#. Default: "Tipologia organizzazione"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:57
-msgid "tipologia_organizzazione_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia di persona: politica, amministrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/persona.py:86
-msgid "tipologia_persona_help"
-msgstr ""
-
-#. Default: "Tipologia persona"
-#: design/plone/contenttypes/interfaces/persona.py:85
-msgid "tipologia_persona_label"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per le tipologie di un Documento. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:46
-msgid "tipologie_documento_help"
+#. Default: "Timeline tempi e scadenze"
+#: design/plone/contenttypes/interfaces/servizio.py:246
+msgid "timeline_tempi_scadenze"
 msgstr ""
 
-#. Default: "Tipologie Documento"
-#: design/plone/contenttypes/controlpanels/settings.py:45
-msgid "tipologie_documento_label"
+#. Default: "Timeline tempi e scadenze del servizio: indicare per ogni scadenza un titolo descrittivo ed un eventuale sottotitolo. Per ogni scadenza, selezionare opzionalmente o l'intervallo (Campi \"Intervallo\" e \"Tipo Intervallo\", es. \"1\" e \"settimana\"), oppure direttamente una data di scadenza (campo: \"Data Scadenza\", esempio 31/12/2023). Se vengono compilati entrambi, ha priorità il campo \"Data Scadenza\"."
+#: design/plone/contenttypes/interfaces/servizio.py:249
+msgid "timeline_tempi_scadenze_help"
 msgstr ""
 
 #. Default: "Inserisci i valori utilizzabili per le tipologie di una Notizia. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:19
+#: design/plone/contenttypes/controlpanels/settings.py:22
 msgid "tipologie_notizia_help"
 msgstr ""
 
 #. Default: "Tipologie Notizia"
-#: design/plone/contenttypes/controlpanels/settings.py:18
+#: design/plone/contenttypes/controlpanels/settings.py:21
 msgid "tipologie_notizia_label"
 msgstr ""
 
-#. Default: "Inserisci i valori utilizzabili per le tipologie di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:72
-msgid "tipologie_persona_help"
-msgstr ""
-
-#. Default: "Tipologie Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:71
-msgid "tipologie_persona_label"
-msgstr ""
-
 #. Default: "Inserisci i valori utilizzabili per le tipologie di un' Unità Organizzativa. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:34
+#: design/plone/contenttypes/controlpanels/settings.py:37
 msgid "tipologie_unita_organizzativa_help"
 msgstr ""
 
 #. Default: "Tipologie Unità Organizzativa"
-#: design/plone/contenttypes/controlpanels/settings.py:30
+#: design/plone/contenttypes/controlpanels/settings.py:33
 msgid "tipologie_unita_organizzativa_label"
 msgstr ""
 
 #. Default: "Titolare"
-#: design/plone/contenttypes/interfaces/dataset.py:29
+#: design/plone/contenttypes/interfaces/dataset.py:22
 msgid "titolare"
 msgstr ""
 
 #. Default: "Eventuale titolare del potere sostitutivo."
-#: design/plone/contenttypes/behaviors/trasparenza.py:243
+#: design/plone/contenttypes/behaviors/trasparenza.py:244
 msgid "titolare_potere_sostitutivo_help"
 msgstr ""
 
 #. Default: "Titolare del potere sostitutivo"
-#: design/plone/contenttypes/behaviors/trasparenza.py:238
+#: design/plone/contenttypes/behaviors/trasparenza.py:239
 msgid "titolare_potere_sostitutivo_label"
 msgstr ""
 
 #. Default: "Trasparenza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:292
+#: design/plone/contenttypes/behaviors/trasparenza.py:291
 msgid "trasparenza_fieldset_label"
 msgstr ""
 
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:17
+msgid "type_help"
+msgstr ""
+
 #. Default: "Seleziona l'ufficio responsabile di questo bando."
-#: design/plone/contenttypes/interfaces/bando.py:110
+#: design/plone/contenttypes/interfaces/bando.py:111
 msgid "ufficio_responsabile_bando_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del bando"
-#: design/plone/contenttypes/interfaces/bando.py:106
+#: design/plone/contenttypes/interfaces/bando.py:107
 msgid "ufficio_responsabile_bando_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio responsabile di questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:43
+#: design/plone/contenttypes/interfaces/documento.py:73
 msgid "ufficio_responsabile_documento_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del documento"
-#: design/plone/contenttypes/interfaces/documento.py:39
+#: design/plone/contenttypes/interfaces/documento.py:69
 msgid "ufficio_responsabile_documento_label"
 msgstr ""
 
 #. Default: "Ufficio responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:62
 msgid "ufficio_responsabile_documento_personale"
 msgstr ""
 
-#. Default: "Uffici responsabili"
-#: design/plone/contenttypes/interfaces/servizio.py:216
+#. Default: "Unità organizzativa responsabile"
+#: design/plone/contenttypes/interfaces/servizio.py:302
 msgid "ufficio_responsabile_erogazione"
 msgstr ""
 
 #. Default: "Seleziona gli uffici responsabili dell'erogazione di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:217
+#: design/plone/contenttypes/interfaces/servizio.py:306
 msgid "ufficio_responsabile_help"
 msgstr ""
 
 #. Default: "Ufficio di riferimento"
 #: design/plone/contenttypes/interfaces/pratica.py:17
 msgid "ufficio_riferimento"
 msgstr ""
@@ -2658,56 +2653,56 @@
 msgstr ""
 
 #. Default: "Seleziona la lista delle unità amministrative responsabili di questo argomento."
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:48
 msgid "unita_amministrative_responsabili_help"
 msgstr ""
 
+#. Default: "Seleziona l'organizzazione presso la quale svolge l'incarico."
+#: design/plone/contenttypes/interfaces/incarico.py:64
+msgid "unita_organizzativa_incarico_help"
+msgstr ""
+
+#. Default: "Unità organizzativa"
+#: design/plone/contenttypes/interfaces/incarico.py:60
+msgid "unita_organizzativa_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione dei compiti assegnati alla struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:19
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:23
 msgid "uo_competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:18
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:22
 msgid "uo_competenze_label"
 msgstr ""
 
-#. Default: "Inserisci eventuali informazioni di contatto aggiuntive non contemplate nei campi precedenti. Utilizza questo campo se ci sono dei contatti aggiuntivi rispetto ai contatti della sede principale. Se inserisci un collegamento con un indirizzo email, aggiungi \"mailto:\" prima dell'indirizzo, per farlo aprire direttamente nel client di posta."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:139
-msgid "uo_contact_info_description"
-msgstr ""
-
 #. Default: "Note di aggiornamento"
-#: design/plone/contenttypes/behaviors/update_note.py:16
+#: design/plone/contenttypes/behaviors/update_note.py:17
 msgid "update_note_label"
 msgstr ""
 
+#. Default: "Il valore del punto di contatto: il numero compreso di prefisso internazionale (se telefono), l'account (se social network), l'URL (se sito o pagina web), l'indirizzo email (se email)."
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:54
+msgid "value_punto_contatto_help"
+msgstr ""
+
 #. Default: "Vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:196
+#: design/plone/contenttypes/interfaces/servizio.py:282
 msgid "vincoli"
 msgstr ""
 
 #. Default: "Descrizione degli eventuali vincoli presenti."
-#: design/plone/contenttypes/interfaces/servizio.py:198
+#: design/plone/contenttypes/interfaces/servizio.py:284
 msgid "vincoli_help"
 msgstr ""
 
-#. Default: "Indicare un indirizzo web di riferimento a questo evento."
-#: design/plone/contenttypes/behaviors/evento.py:138
-msgid "web_event_help"
-msgstr ""
-
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/evento.py:137
-msgid "web_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo web di riferimento."
-#: design/plone/contenttypes/behaviors/contatti.py:53
-msgid "web_help"
+#. Default: "Mostra i PDF in anteprima"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:12
+msgid "visualize_files_title"
 msgstr ""
 
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/contatti.py:52
-msgid "web_label"
+#. Default: "Permette di aprire l'anteprima di tutti i PDF di questa cartella in una tab separata, altrimenti i PDF vengono scaricati"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:13
+msgid "visulize_files_description"
 msgstr ""
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot`

 * *Files 2% similar despite different names*

```diff
@@ -1,505 +1,494 @@
 #--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 #SOME DESCRIPTIVE TITLE.
 #FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-01-13 13:15+0000\n"
+"POT-Creation-Date: 2024-03-18 13:30+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: design.plone.contenttypes\n"
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
-msgid "Abitazione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:36
-msgid "Accesso al trasporto pubblico"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:59
-msgid "Accesso luoghi della cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:18
+msgid "Accesso all'informazione"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:33
 msgid "Accettare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:34
-msgid "Accordo tra enti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:19
 msgid "Acqua"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
+#: design/plone/contenttypes/behaviors/configure.zcml:223
 msgid "Address Event"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Address UO"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:186
+#: design/plone/contenttypes/behaviors/configure.zcml:215
 msgid "Address Venue"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:19
 msgid "Adds fields."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:28
-msgid "Agricoltura, pesca, silvicoltura e prodotti alimentari"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "After Plone6 migration syndication is broken"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:22
-msgid "All the already existing News Types"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:20
+msgid "Agricoltura"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:63
-msgid "All the selected items will be moved to indicated path"
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:30
+msgid "All the already existing News Types"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:36
-msgid "Ambiente"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:113
+msgid "All the selected items will be moved to indicated path"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:21
 msgid "Animale domestico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
-msgid "Anziano"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/bando.py:134
-#: design/plone/contenttypes/interfaces/documento.py:67
-#: design/plone/contenttypes/interfaces/servizio.py:239
+#: design/plone/contenttypes/interfaces/bando.py:135
+#: design/plone/contenttypes/interfaces/documento.py:97
+#: design/plone/contenttypes/interfaces/servizio.py:328
 msgid "Area"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
-msgid "Area di parcheggio"
-msgstr ""
-
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Argomenti"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:76
+#: design/plone/contenttypes/behaviors/configure.zcml:94
 msgid "Argomenti Bando"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:58
+#: design/plone/contenttypes/behaviors/configure.zcml:76
 msgid "Argomenti Document"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:67
+#: design/plone/contenttypes/behaviors/configure.zcml:85
 msgid "Argomenti Documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:28
+#: design/plone/contenttypes/behaviors/configure.zcml:112
+msgid "Argomenti Link"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/argomenti.py:32
 msgid "Argomenti correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
 msgid "Argomento"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:73
+#: design/plone/contenttypes/behaviors/configure.zcml:103
+msgid "Argomento Servizio"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:22
+msgid "Aria"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:65
 msgid "Assessore di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
-msgid "Associazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:23
+msgid "Assistenza agli invalidi"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:24
+msgid "Assistenza sociale"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
+msgid "Associazioni"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:29
 msgid "Attivare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:33
-msgid "Atto normativo"
+#: design/plone/contenttypes/interfaces/incarico.py:121
+msgid "Atto di nomina"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:86
 msgid "Autore"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:30
 msgid "Autorizzare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:65
-msgid "Avvio impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:66
-msgid "Avvio nuova attività professionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:69
-msgid "Avvio/registrazione filiale"
+#: design/plone/contenttypes/behaviors/configure.zcml:223
+msgid "Behavior address per Event."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:78
-msgid "Bancarotta"
+#: design/plone/contenttypes/behaviors/configure.zcml:215
+msgid "Behavior address per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
-msgid "Behavior address per Event."
+#: design/plone/contenttypes/behaviors/configure.zcml:263
+msgid "Behavior contatti per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Behavior address per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:255
+msgid "Behavior contatti per Persona."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:186
-msgid "Behavior address per Venue."
+#: design/plone/contenttypes/behaviors/configure.zcml:247
+msgid "Behavior contatti per Servizio."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
 msgid "Behavior contatti per UO."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:210
+#: design/plone/contenttypes/behaviors/configure.zcml:239
 msgid "Behavior contatti per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:234
+#: design/plone/contenttypes/behaviors/configure.zcml:279
 msgid "Behavior geolocatable per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
-msgid "Behavior geolocatable per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:271
+msgid "Behavior geolocatable per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:226
-msgid "Behavior geolocatable per Venue."
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
+msgid "Bilancio"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:18
 msgid "CAP"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:43
-msgid "Cambio di residenza/domicilio"
+#: design/plone/contenttypes/behaviors/configure.zcml:306
+msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:261
-msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Campo per escludere un contenuto dalle ricerche del sito."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
+#: design/plone/contenttypes/behaviors/configure.zcml:315
 msgid "Campo per le note di aggiornamento."
 msgstr ""
 
+#: design/plone/contenttypes/interfaces/servizio.py:183
+msgid "Canale fisico"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:26
 msgid "Canon 5D IV"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 msgid "Cartella Modulistica"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:11
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:13
 msgid "Change News Type"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:75
-msgid "Chiusura filiale"
+#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
+msgid "Città"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:74
-msgid "Chiusura impresa e attività professionale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
+msgid "Commercio al minuto"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
-msgid "Città"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
+msgid "Commercio all'ingrosso"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:39
-msgid "Compravendita/affitto casa/edifici/terreni, costruzione o ristrutturazione casa/edificio	"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
+msgid "Commercio ambulante"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
-msgid "Comunicazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
+msgid "Comunicazione istituzionale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
-msgid "Condizioni e organizzazione del lavoro"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+msgid "Comunicazione politica"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
+msgid "Concorsi"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:57
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:104
 msgid "Contained by"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
+#: design/plone/contenttypes/behaviors/contatti.py:112
 msgid "Contatti"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:33
 msgid "Coordinate"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:42
+#: design/plone/contenttypes/behaviors/argomenti.py:46
 msgid "Correlato in evidenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
-msgid "Cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+msgid "Covid - 19"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:130
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 msgid "Dataset"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:134
 msgid "Dataset collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:104
+#: design/plone/contenttypes/behaviors/configure.zcml:141
 msgid "Dataset correlati"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:31
 msgid "Delegare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:52
-msgid "Denuncia crimini"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:143
+#: design/plone/contenttypes/behaviors/configure.zcml:180
 msgid "Descrizione estesa"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:160
+#: design/plone/contenttypes/behaviors/configure.zcml:197
 msgid "Descrizione estesa documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:152
+#: design/plone/contenttypes/behaviors/configure.zcml:189
 msgid "Descrizione estesa servizio"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Design Plone: Content-types"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Design Plone: Content-types (behaviors)"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Design Plone: Content-types (uninstall)"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Design Plone: Content-types to 3000"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:55
-msgid "Dichiarazione dei redditi, versamento e riscossione tributi/imposte e contributi"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "Design Plone: Fix Syndication after Plone6 Migration"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:145
+#: design/plone/contenttypes/behaviors/trasparenza.py:146
 msgid "Dirigente"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:27
-msgid "Documenti albo pretorio"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:134
+msgid "Documenti pubblici"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/servizio.py:252
+#: design/plone/contenttypes/interfaces/servizio.py:341
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Documento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:41
-msgid "Documento (tecnico) di supporto"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
 msgid "Documento Personale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:37
-msgid "Documento attivita politica"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:31
-msgid "Documento funzionamento interno"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:30
-msgid "Economia e Finanze"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Edit"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
-msgid "Elezione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:35
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
-msgid "Energia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+msgid "Elezioni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
-msgid "Famiglia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
+msgid "Energie rinnovabili"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
-msgid "Fanciullo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
+msgid "Estero"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:70
-msgid "Finanziamento impresa"
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Exclude from search"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:28
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:51
 msgid "Find news with the indicated Path, put attention than generaly sites have the root name \"/Plone/\""
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:21
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:29
 msgid "Find news with this News Type"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Fix control panel of design.plone.contenttypes add-on."
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
+msgid "Foreste"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/tags_vocabulary.py:38
 msgid "Formazione professionale"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:39
+msgid "Gemellaggi"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:271
 msgid "Geolocatable"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:43
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Geolocation default"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
-msgid "Gestione dei rifiuti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:71
-msgid "Gestione personale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
-msgid "Giovane"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:40
+msgid "Gestione rifiuti"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:30
 msgid "Giovanni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:42
-msgid "Giustizia, sistema giuridico e sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
+msgid "Giustizia"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:37
-msgid "Governo e settore pubblico"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:42
+msgid "Igiene pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+#: design/plone/contenttypes/browser/utils/change_news_type.py:32
+#: design/plone/contenttypes/browser/utils/move_news_items.py:74
+msgid "Il vocabolario dei valori non è stato trovato"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
 msgid "Immigrazione"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/settings.py:154
+#: design/plone/contenttypes/controlpanels/settings.py:106
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Impostazioni Design Plone"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+msgid "Imposte"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
+msgid "Imprese"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/persona.py:68
+msgid "Incarichi"
+msgstr ""
+
+#: design/plone/contenttypes/profiles/default/types/Incarico.xml
+msgid "Incarico"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/move_news_items.py:34
 msgid "Indicated path is not valid"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:170
+#: design/plone/contenttypes/behaviors/configure.zcml:207
 msgid "Info per la testata"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:32
 msgid "Informare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
-msgid "Informatica e trattamento dei dati"
+#: design/plone/contenttypes/behaviors/contatti.py:34
+msgid "Informazioni di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
 msgid "Inquinamento"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Installs the design.plone.contenttypes add-on."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
 msgid "Integrazione sociale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:28
-msgid "Invalidità"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:26
 msgid "Iscriversi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:26
-msgid "Iscrizione scuola/università e/o richiesta borsa di studio"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:43
-msgid "Istanza"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+msgid "Isolamento termico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
 msgid "Istruzione"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:33
-msgid "Istruzione, cultura e sport"
+#: design/plone/contenttypes/browser/utils/move_news_items.py:48
+msgid "Items moved with success"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:47
-msgid "Items moved with success"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
+msgid "Lavoro"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:28
 msgid "Leggere"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:85
+#: design/plone/contenttypes/behaviors/configure.zcml:122
 msgid "Luoghi correlati"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
 msgid "Matrimonio"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:49
-msgid "Matrimonio e/o cambio stato civile"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+msgid "Mercato"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Messaggio.xml
 msgid "Messaggio"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:29
@@ -510,529 +499,536 @@
 msgid "Metadati luogo"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:39
 msgid "Metadati news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:28
-msgid "Modulistica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
+msgid "Mobilità sostenibile"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Modulo"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:50
-msgid "Morte ed eredità"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
+msgid "Morte"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Mostra la data di modifica."
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:70
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:124
 msgid "Move"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:11
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:13
 msgid "Move News Items"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:62
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:110
 msgid "Move to Path"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Multi File"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:48
-msgid "Nascita di un bambino, richiesta adozioni"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
+msgid "Nascita"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:28
 msgid "Nazione"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:21
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:20
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:26
 msgid "News Type"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:30
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:48
 msgid "News Type to substitute"
 msgstr ""
 
 #. Default: "Nome e cognome"
-#: design/plone/contenttypes/restapi/services/types/get.py:152
+#: design/plone/contenttypes/restapi/services/types/get.py:163
 msgid "Nome e Cognome"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:73
-msgid "Notifiche autorità"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/persona.py:48
+#: design/plone/contenttypes/interfaces/persona.py:51
 msgid "Organizzazione di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:72
-msgid "Pagamento tasse, iva e dogane"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:25
 msgid "Pagare"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:29
 msgid "Paperino"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:81
-msgid "Partecipazione ad appalti pubblici nazionali e trasfrontalieri"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
+msgid "Parcheggi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:33
-msgid "Pensionamento"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
+msgid "Patrimonio culturale"
 msgstr ""
 
-#: design/plone/contenttypes/profiles/default/types/Persona.xml
+#: design/plone/contenttypes/interfaces/incarico.py:54
 msgid "Persona"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/evento.py:50
-msgid "Persona dell'amministrazione"
+#: design/plone/contenttypes/profiles/default/types/Persona.xml
+msgid "Persona pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:92
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:84
 msgid "Persone della struttura"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+msgid "Pesca"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
+msgid "Piano di sviluppo"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:27
 msgid "Pippo"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+msgid "Pista ciclabile"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:28
 msgid "Pluto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:45
-msgid "Popolazione e società"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
+msgid "Politica commerciale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:60
-msgid "Possesso, cura, smarrimento animale da compagnia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:62
+msgid "Polizia"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pratica.xml
 msgid "Pratica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:51
-msgid "Prenotazione e disdetta visite/esami"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:63
+msgid "Prodotti alimentari"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
-msgid "Protezione sociale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
+msgid "Protezione civile"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:13
-msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
+#: design/plone/contenttypes/behaviors/contatti.py:78
+msgid "Punti di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:13
-msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
+#: design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+msgid "Punto di Contatto"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:15
+msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:44
-msgid "Regioni e città"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:15
+msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:68
-msgid "Registrazione impresa transfrontalier"
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Registers taxonomies."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:35
-msgid "Registrazione/possesso veicolo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:65
+msgid "Residenza"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:45
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:49
 msgid "Responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:129
-msgid "Responsabile procedimento"
+#: design/plone/contenttypes/interfaces/incarico.py:89
+msgid "Responsabile della struttura"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:31
-msgid "Ricerca di lavoro, avvio nuovo lavoro, disoccupazione"
+#: design/plone/contenttypes/behaviors/trasparenza.py:130
+msgid "Responsabile procedimento"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
 msgid "RicevutaPagamento"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:27
 msgid "Richiedere"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:67
-msgid "Richiesta licenze/permessi/certificati"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:34
-msgid "Richiesta o rinnovo patente"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:46
-msgid "Richiesta passaporto, visto e assistenza viaggi internazionali"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:66
+msgid "Risposta alle emergenze"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:76
-msgid "Ristrutturazione impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:38
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
-msgid "Salute"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:46
-msgid "Scienza e tecnologia"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:47
 msgid "Search Path"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:114
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:104
 msgid "Sede"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:114
+#: design/plone/contenttypes/behaviors/configure.zcml:151
 msgid "Servizi correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Servizio.xml
 msgid "Servizio"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:101
 msgid "Servizio collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Show modified"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
-msgid "Sicurezza internazionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
-msgid "Sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:67
+msgid "Sistema giuridico"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:25
 msgid "Sony Aplha 7R III"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
-msgid "Spazio verde"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:68
+msgid "Spazio Verde"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:69
 msgid "Sport"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:37
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:41
 msgid "Struttura"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:20
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:21
 msgid "Struttura politica coinvolta"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/luogo.py:74
+#: design/plone/contenttypes/behaviors/luogo.py:75
 msgid "Struttura responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:124
+#: design/plone/contenttypes/behaviors/configure.zcml:161
 msgid "Strutture correlate"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
-msgid "Studente"
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:74
+msgid "Substitute"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:43
-msgid "Substitute"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:70
+msgid "Sviluppo sostenibile"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:71
+msgid "Tassa sui servizi"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Tassonomia argomenti"
 msgstr ""
 
+#: design/plone/contenttypes/behaviors/configure.zcml:67
+msgid "Tassonomia argomenti evento"
+msgstr ""
+
 #: design/plone/contenttypes/behaviors/configure.zcml:58
-msgid "Tassonomia argomenti per i Document"
+msgid "Tassonomia argomenti news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:39
-msgid "Tematiche internazionali"
+#: design/plone/contenttypes/behaviors/configure.zcml:76
+msgid "Tassonomia argomenti per i Document"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:72
 msgid "Tempo libero"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:31
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:52
 msgid "The News Type selected above will be substituted by the selected value"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:97
+#: design/plone/contenttypes/browser/utils/change_news_type.py:108
 msgid "The News Types was changed with success"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:55
+#: design/plone/contenttypes/browser/utils/change_news_type.py:64
 msgid "The new News Type was not found between available values"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:49
+#: design/plone/contenttypes/browser/utils/change_news_type.py:58
 msgid "The new type field was not populated"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:61
+#: design/plone/contenttypes/browser/utils/change_news_type.py:70
 msgid "The old News Type was not found between available values"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:43
+#: design/plone/contenttypes/browser/utils/change_news_type.py:52
 msgid "The old type field was not populated"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:51
+#: design/plone/contenttypes/browser/utils/move_news_items.py:52
 msgid "The path was not indicated"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
-msgid "Traffico urbano"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:261
+#: design/plone/contenttypes/behaviors/configure.zcml:306
 msgid "Trasparenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
-msgid "Trasporto"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:73
+msgid "Trasparenza amministrativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
-msgid "Trasporto stradale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:74
+msgid "Trasporto pubblico"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Tre campi file aggiuntivi."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:75
 msgid "Turismo"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:117
-#: design/plone/contenttypes/interfaces/documento.py:50
-#: design/plone/contenttypes/interfaces/servizio.py:225
+#: design/plone/contenttypes/interfaces/bando.py:118
+#: design/plone/contenttypes/interfaces/documento.py:80
 msgid "Ufficio responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:134
+#: design/plone/contenttypes/behaviors/configure.zcml:171
 msgid "Ulteriori campi aiuto testuali"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Un modulo compilabile."
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:15
+msgid "Una raccolta di utility per i contenuti agid"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Uninstalls the design.plone.contenttypes add-on."
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
 msgid "Unita Organizzativa"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:45
 msgid "Unità amministrative responsabili"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
-msgid "Update note"
+#: design/plone/contenttypes/interfaces/incarico.py:71
+msgid "Unità organizzativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
-msgid "Urbanistica ed edilizia"
+#: design/plone/contenttypes/interfaces/servizio.py:314
+msgid "Unità organizzativa responsabile"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:315
+msgid "Update note"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:77
-msgid "Vendita impresa"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:76
+msgid "Urbanizzazione"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:13
 msgid "Via"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:77
+msgid "Viaggi"
+msgstr ""
+
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "View"
 msgstr ""
 
-#. Default: "A chi si rivolge questo servizio e chi può usufruirne."
-#: design/plone/contenttypes/interfaces/servizio.py:53
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:13
+msgid "Viste di utility per Design Plone Contenttypes"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:79
+msgid "ZTL"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:78
+msgid "Zone pedonali"
+msgstr ""
+
+#. Default: "Descrizione testuale dei principali destinatari dell'Evento"
+#: design/plone/contenttypes/behaviors/evento.py:43
+#: design/plone/contenttypes/interfaces/servizio.py:98
 msgid "a_chi_si_rivolge_help"
 msgstr ""
 
-#. Default: "A chi si rivolge"
-#: design/plone/contenttypes/interfaces/servizio.py:51
+#. Default: "A chi è rivolto"
+#: design/plone/contenttypes/behaviors/evento.py:41
+#: design/plone/contenttypes/interfaces/servizio.py:96
 msgid "a_chi_si_rivolge_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio di comunicazione responsabile di questa notizia/comunicato stampa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:47
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:39
 msgid "a_cura_di_help"
 msgstr ""
 
 #. Default: "A cura di"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:46
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
 msgid "a_cura_di_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di persone dell'amministrazione citate in questa notizia/comunicato stampa. Questa informazione verrà mostrata nella sezione \"A cura di\"."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:59
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:51
 msgid "a_cura_di_persone_help"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:58
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:50
 msgid "a_cura_di_persone_label"
 msgstr ""
 
 #. Default: "Accedere al servizio"
-#: design/plone/contenttypes/interfaces/servizio.py:370
+#: design/plone/contenttypes/interfaces/servizio.py:481
 msgid "accedi_al_servizio_label"
 msgstr ""
 
 #. Default: "Modalità di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:171
+#: design/plone/contenttypes/behaviors/luogo.py:140
 msgid "accesso_label"
 msgstr ""
 
 #. Default: "Allegato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:56
 msgid "allegato"
 msgstr ""
 
 #. Default: "Indicare, se esistono, altre modalità di invio."
-#: design/plone/contenttypes/behaviors/trasparenza.py:189
+#: design/plone/contenttypes/behaviors/trasparenza.py:190
 msgid "altre_modalita_invio_help"
 msgstr ""
 
 #. Default: "Altre modalità di invio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:185
+#: design/plone/contenttypes/behaviors/trasparenza.py:186
 msgid "altre_modalita_invio_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei documenti di supporto collegati a questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:246
+#: design/plone/contenttypes/interfaces/servizio.py:335
 msgid "altri_documenti_help"
 msgstr ""
 
 #. Default: "Date and time of the opening of the announcement. Use this field if you want to set a specific opening date. If not set, the announcement will be open immediately."
-#: design/plone/contenttypes/interfaces/bando.py:56
+#: design/plone/contenttypes/interfaces/bando.py:57
 msgid "apertura_bando_help"
 msgstr ""
 
 #. Default: "Opening date"
-#: design/plone/contenttypes/interfaces/bando.py:55
+#: design/plone/contenttypes/interfaces/bando.py:56
 msgid "apertura_bando_label"
 msgstr ""
 
 #. Default: "Area"
-#: design/plone/contenttypes/interfaces/servizio.py:231
+#: design/plone/contenttypes/interfaces/servizio.py:320
 msgid "area"
 msgstr ""
 
 #. Default: "Seleziona l'area da cui dipende questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:234
+#: design/plone/contenttypes/interfaces/servizio.py:323
 msgid "area_help"
 msgstr ""
 
 #. Default: "Area responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:73
 msgid "area_responsabile_documento_personale"
 msgstr ""
 
 #. Default: "Seleziona l'area amministrativa responsabile del documento."
-#: design/plone/contenttypes/interfaces/bando.py:127
-#: design/plone/contenttypes/interfaces/documento.py:60
+#: design/plone/contenttypes/interfaces/bando.py:128
+#: design/plone/contenttypes/interfaces/documento.py:90
 msgid "area_responsabile_help"
 msgstr ""
 
 #. Default: "Area responsabile del documento"
-#: design/plone/contenttypes/interfaces/bando.py:123
-#: design/plone/contenttypes/interfaces/documento.py:56
+#: design/plone/contenttypes/interfaces/bando.py:124
+#: design/plone/contenttypes/interfaces/documento.py:86
 msgid "area_responsabile_label"
 msgstr ""
 
 #. Default: "Argomenti utenti"
 #: design/plone/contenttypes/interfaces/documento_personale.py:42
 msgid "argomenti_utenti"
 msgstr ""
 
 #. Default: "Inserire l'assessore di riferimento della struttura, se esiste."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:76
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:68
 msgid "assessore_riferimento_help"
 msgstr ""
 
+#. Default: "Assessore di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:61
+msgid "assessore_riferimento_title"
+msgstr ""
+
 #. Default: "Indicare, se la esistono, atti e documenti a corredo dell'istanza."
-#: design/plone/contenttypes/behaviors/trasparenza.py:200
+#: design/plone/contenttypes/behaviors/trasparenza.py:201
 msgid "atti_documenti_corredo_help"
 msgstr ""
 
 #. Default: "Atti e documenti a corredo dell'istanza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:196
+#: design/plone/contenttypes/behaviors/trasparenza.py:197
 msgid "atti_documenti_corredo_label"
 msgstr ""
 
-#. Default: "Inserire un file contenente l'atto di nomina della persona."
-#: design/plone/contenttypes/interfaces/persona.py:160
-msgid "atto_nomina_help"
+#. Default: "Inserire riferimento all'atto di nomina della persona"
+#: design/plone/contenttypes/interfaces/incarico.py:114
+msgid "atto_nomina_incarico_help"
 msgstr ""
 
 #. Default: "Atto di nomina"
-#: design/plone/contenttypes/interfaces/persona.py:158
-msgid "atto_nomina_label"
-msgstr ""
-
-#. Default: "Autenticazione"
-#: design/plone/contenttypes/interfaces/servizio.py:121
-msgid "autenticazione"
-msgstr ""
-
-#. Default: "Indicare, se previste, le modalità di autenticazione necessarie per poter accedere al servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:122
-msgid "autenticazione_help"
+#: design/plone/contenttypes/interfaces/incarico.py:110
+msgid "atto_nomina_incarico_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di autori che hanno pubblicato il documento. Possono essere Persone o Unità Organizzative."
-#: design/plone/contenttypes/interfaces/documento.py:76
+#: design/plone/contenttypes/interfaces/documento.py:106
 msgid "autori_help"
 msgstr ""
 
 #. Default: "Autore/i"
-#: design/plone/contenttypes/interfaces/documento.py:72
+#: design/plone/contenttypes/interfaces/documento.py:102
 msgid "autori_label"
 msgstr ""
 
 #. Default: "Azioni"
 #: design/plone/contenttypes/interfaces/messaggio.py:28
 msgid "azioni_pratica"
 msgstr ""
@@ -1044,660 +1040,686 @@
 
 #. Default: "Azioni utente"
 #: design/plone/contenttypes/interfaces/pratica.py:47
 msgid "azioni_utente"
 msgstr ""
 
 #. Default: "Solo per persona politica: testo descrittivo che riporta la biografia della persona."
-#: design/plone/contenttypes/interfaces/persona.py:107
+#: design/plone/contenttypes/interfaces/persona.py:94
 msgid "biografia_help"
 msgstr ""
 
 #. Default: "Biografia"
-#: design/plone/contenttypes/interfaces/persona.py:106
+#: design/plone/contenttypes/interfaces/persona.py:93
 msgid "biografia_label"
 msgstr ""
 
 #. Default: "Canale digitale"
-#: design/plone/contenttypes/interfaces/servizio.py:111
+#: design/plone/contenttypes/interfaces/servizio.py:156
 msgid "canale_digitale"
 msgstr ""
 
-#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:112
+#. Default: "Testo di introduzione del canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:157
 msgid "canale_digitale_help"
 msgstr ""
 
+#. Default: "Link al canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:165
+msgid "canale_digitale_link"
+msgstr ""
+
+#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
+#: design/plone/contenttypes/interfaces/servizio.py:166
+msgid "canale_digitale_link_help"
+msgstr ""
+
 #. Default: "Canale digitale servizio collegato"
 #: design/plone/contenttypes/interfaces/documento_personale.py:108
 msgid "canale_digitale_servizio"
 msgstr ""
 
+#. Default: "Canale fisico"
+#: design/plone/contenttypes/interfaces/servizio.py:175
+msgid "canale_fisico"
+msgstr ""
+
+#. Default: "Unità organizzative per la fruizione del servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:176
+msgid "canale_fisico_help"
+msgstr ""
+
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:205
+#: design/plone/contenttypes/interfaces/servizio.py:291
 msgid "casi_particolari"
 msgstr ""
 
 #. Default: "Descrizione degli evetuali casi particolari riferiti alla fruibilità di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:207
+#: design/plone/contenttypes/interfaces/servizio.py:293
 msgid "casi_particolari_help"
 msgstr ""
 
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:401
+#: design/plone/contenttypes/interfaces/servizio.py:514
 msgid "casi_particolari_label"
 msgstr ""
 
 #. Default: "Descrizione di chi può presentare domanda per usufruire del servizio e delle diverse casistiche."
-#: design/plone/contenttypes/interfaces/servizio.py:62
+#: design/plone/contenttypes/interfaces/servizio.py:107
 msgid "chi_puo_presentare_help"
 msgstr ""
 
 #. Default: "Chi può presentare"
-#: design/plone/contenttypes/interfaces/servizio.py:60
+#: design/plone/contenttypes/interfaces/servizio.py:105
 msgid "chi_puo_presentare_label"
 msgstr ""
 
 #. Default: "Circoscrizione"
 #: design/plone/contenttypes/behaviors/address.py:37
 msgid "circoscrizione"
 msgstr ""
 
 #. Default: "Codice dell'ente erogatore (ipa)"
-#: design/plone/contenttypes/interfaces/servizio.py:268
+#: design/plone/contenttypes/interfaces/servizio.py:357
 msgid "codice_ipa"
 msgstr ""
 
 #. Default: "Specificare il nome dell’organizzazione, come indicato nell’Indice della Pubblica Amministrazione (IPA), che esercita uno specifico ruolo sul Servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:270
+#: design/plone/contenttypes/interfaces/servizio.py:359
 msgid "codice_ipa_help"
 msgstr ""
 
-#. Default: "Come si fa"
-#: design/plone/contenttypes/interfaces/servizio.py:80
+#. Default: "Come fare"
+#: design/plone/contenttypes/interfaces/servizio.py:125
 msgid "come_si_fa"
 msgstr ""
 
 #. Default: "Descrizione della procedura da seguire per poter usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:82
+#: design/plone/contenttypes/interfaces/servizio.py:127
 msgid "come_si_fa_help"
 msgstr ""
 
+#. Default: "Solo per incarico politico: compensi di qualsiasi natura connessi all'assunzione della carica."
+#: design/plone/contenttypes/interfaces/incarico.py:21
+msgid "compensi_incarico_help"
+msgstr ""
+
+#. Default: "Compensi"
+#: design/plone/contenttypes/interfaces/incarico.py:17
+msgid "compensi_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione del ruolo e dei compiti della persona."
-#: design/plone/contenttypes/interfaces/persona.py:69
+#: design/plone/contenttypes/interfaces/persona.py:77
 msgid "competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/persona.py:68
+#: design/plone/contenttypes/interfaces/persona.py:76
 msgid "competenze_label"
 msgstr ""
 
-#. Default: "Informazioni di contatto generiche"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:137
+#. Default: "Condizioni di servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:388
+msgid "condizioni_di_servizio"
+msgstr ""
+
+#. Default: "Contatti dell'unità organizzativa."
+#: design/plone/contenttypes/behaviors/contatti.py:27
+msgid "contact_info_help"
+msgstr ""
+
+#. Default: "Punti di contatto dell'unità organizzativa"
+#: design/plone/contenttypes/behaviors/contatti.py:23
 msgid "contact_info_label"
 msgstr ""
 
 #. Default: "Contatti"
 #: design/plone/contenttypes/interfaces/pratica.py:44
 msgid "contatti"
 msgstr ""
 
 #. Default: "Contatti"
-#: design/plone/contenttypes/behaviors/address.py:52
-#: design/plone/contenttypes/behaviors/contatti.py:76
-#: design/plone/contenttypes/behaviors/evento.py:215
+#: design/plone/contenttypes/behaviors/contatti.py:57
+#: design/plone/contenttypes/behaviors/evento.py:170
+#: design/plone/contenttypes/behaviors/geolocation.py:18
 msgid "contatti_label"
 msgstr ""
 
 #. Default: "Contenuto"
 #: design/plone/contenttypes/interfaces/pratica.py:42
 msgid "contenuto"
 msgstr ""
 
 #. Default: "Indicare se il servizio si riferisce ad una particolare area geografica o all'intero territorio di riferimento."
-#: design/plone/contenttypes/interfaces/servizio.py:72
+#: design/plone/contenttypes/interfaces/servizio.py:117
 msgid "copertura_geografica_help"
 msgstr ""
 
 #. Default: "Copertura geografica"
-#: design/plone/contenttypes/interfaces/servizio.py:70
+#: design/plone/contenttypes/interfaces/servizio.py:115
 msgid "copertura_geografica_label"
 msgstr ""
 
 #. Default: "Contenuti collegati"
-#: design/plone/contenttypes/behaviors/argomenti.py:74
+#: design/plone/contenttypes/behaviors/argomenti.py:108
 #: design/plone/contenttypes/behaviors/dataset_correlati.py:40
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:43
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:120
 msgid "correlati_label"
 msgstr ""
 
 #. Default: "Seleziona un correlato da mettere in evidenza per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:36
+#: design/plone/contenttypes/behaviors/argomenti.py:40
 msgid "correlato_in_evidenza_help"
 msgstr ""
 
 #. Default: "Correlato in evidenza"
-#: design/plone/contenttypes/behaviors/argomenti.py:35
+#: design/plone/contenttypes/behaviors/argomenti.py:39
 msgid "correlato_in_evidenza_label"
 msgstr ""
 
-#. Default: "Cosa fa"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
+#. Default: "Competenze"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:201
 msgid "cosa_fa_label"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:177
+#: design/plone/contenttypes/interfaces/servizio.py:263
 msgid "cosa_serve"
 msgstr ""
 
 #. Default: "Descrizione delle istruzioni per usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:179
+#: design/plone/contenttypes/interfaces/servizio.py:265
 msgid "cosa_serve_help"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:384
+#: design/plone/contenttypes/interfaces/servizio.py:497
 msgid "cosa_serve_label"
 msgstr ""
 
 #. Default: "Cosa si ottiene"
-#: design/plone/contenttypes/interfaces/servizio.py:90
+#: design/plone/contenttypes/interfaces/servizio.py:135
 msgid "cosa_si_ottiene"
 msgstr ""
 
 #. Default: "Indicare cosa si può ottenere dal servizio, ad esempio 'carta di identità elettronica', 'certificato di residenza'."
-#: design/plone/contenttypes/interfaces/servizio.py:91
+#: design/plone/contenttypes/interfaces/servizio.py:136
 msgid "cosa_si_ottiene_help"
 msgstr ""
 
 #. Default: "Cos'è"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:40
-#: design/plone/contenttypes/behaviors/evento.py:200
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:52
+#: design/plone/contenttypes/behaviors/evento.py:155
 msgid "cose_label"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/interfaces/servizio.py:186
+#: design/plone/contenttypes/interfaces/servizio.py:272
 msgid "costi"
 msgstr ""
 
 #. Default: "Costi e vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:389
+#: design/plone/contenttypes/interfaces/servizio.py:502
 msgid "costi_e_vincoli_label"
 msgstr ""
 
 #. Default: "Descrizione delle condizioni e dei termini economici per completare la procedura di richiesta del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:188
+#: design/plone/contenttypes/interfaces/servizio.py:274
 msgid "costi_help"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/behaviors/evento.py:212
+#: design/plone/contenttypes/behaviors/evento.py:167
 msgid "costi_label"
 msgstr ""
 
 #. Default: "Allega un file contenente il curriculum vitae della persona. Se ha più file da allegare, utilizza questo campo per quello principale e gli altri mettili dentro alla cartella \"Curriculum vitae\" che troverai dentro alla Persona."
-#: design/plone/contenttypes/interfaces/persona.py:149
+#: design/plone/contenttypes/interfaces/persona.py:105
 msgid "curriculum_vitae_help"
 msgstr ""
 
 #. Default: "Curriculum vitae"
-#: design/plone/contenttypes/interfaces/persona.py:147
+#: design/plone/contenttypes/interfaces/persona.py:103
 msgid "curriculum_vitae_label"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction."
-#: design/plone/contenttypes/behaviors/trasparenza.py:254
+#: design/plone/contenttypes/behaviors/trasparenza.py:255
 msgid "customer_satisfaction_help"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction"
-#: design/plone/contenttypes/behaviors/trasparenza.py:249
+#: design/plone/contenttypes/behaviors/trasparenza.py:250
 msgid "customer_satisfaction_label"
 msgstr ""
 
-#. Default: "Data di conclusione dell'incarico."
-#: design/plone/contenttypes/interfaces/persona.py:60
-msgid "data_conclusione_incarico_help"
-msgstr ""
-
 #. Default: "Data conclusione incarico"
-#: design/plone/contenttypes/interfaces/persona.py:56
-msgid "data_conclusione_incarico_label"
+#: design/plone/contenttypes/interfaces/incarico.py:100
+msgid "data_conclusione_incarico"
 msgstr ""
 
 #. Default: "Data e fasi intermedie"
 #: design/plone/contenttypes/interfaces/documento_personale.py:120
 msgid "data_e_fasi_intermedie"
 msgstr ""
 
 #. Default: "Data di inizio"
 #: design/plone/contenttypes/interfaces/documento_personale.py:116
 msgid "data_inizio"
 msgstr ""
 
-#. Default: "Solo per persona politica: specificare la data di insediamento."
-#: design/plone/contenttypes/interfaces/persona.py:97
-msgid "data_insediamento_help"
+#. Default: "Data inizio incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:95
+msgid "data_inizio_incarico"
 msgstr ""
 
 #. Default: "Data insediamento"
-#: design/plone/contenttypes/interfaces/persona.py:96
-msgid "data_insediamento_label"
+#: design/plone/contenttypes/interfaces/incarico.py:105
+msgid "data_insediamento"
 msgstr ""
 
 #. Default: "Data del messaggio"
 #: design/plone/contenttypes/interfaces/messaggio.py:12
 msgid "data_messaggio"
 msgstr ""
 
 #. Default: "Data pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:21
 msgid "data_pagamento"
 msgstr ""
 
 #. Default: "Data del protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:41
 #: design/plone/contenttypes/interfaces/documento_personale.py:19
 msgid "data_protocollo"
 msgstr ""
 
+#. Default: "Data scadenza"
+#: design/plone/contenttypes/interfaces/servizio.py:49
+msgid "data_scadenza_label"
+msgstr ""
+
 #. Default: "Data di scadenza della procedura"
 #: design/plone/contenttypes/interfaces/messaggio.py:40
 msgid "data_scadenza_procedura"
 msgstr ""
 
 #. Default: "Dataset"
-#: design/plone/contenttypes/interfaces/dataset.py:27
+#: design/plone/contenttypes/interfaces/dataset.py:20
 msgid "dataset"
 msgstr ""
 
+#. Default: "Schede dataset collegate al documento"
+#: design/plone/contenttypes/interfaces/documento.py:150
+msgid "dataset_collegati_help"
+msgstr ""
+
 #. Default: "Seleziona una lista di schede dataset collegate a questo contenuto."
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:20
 msgid "dataset_correlati_help"
 msgstr ""
 
 #. Default: "Dataset correlati"
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:18
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
 msgid "dataset_correlati_label"
 msgstr ""
 
+#. Default: "Dataset collegati"
+#: design/plone/contenttypes/interfaces/documento.py:146
+msgid "dataset_label"
+msgstr ""
+
+#. Default: "Date e informazioni"
+#: design/plone/contenttypes/interfaces/incarico.py:175
+msgid "date_e_informazioni_label"
+msgstr ""
+
 #. Default: "Date e orari"
-#: design/plone/contenttypes/behaviors/evento.py:209
-#: design/plone/contenttypes/schema_overrides.py:34
+#: design/plone/contenttypes/behaviors/evento.py:164
+#: design/plone/contenttypes/schema_overrides.py:33
 msgid "date_e_orari_label"
 msgstr ""
 
 #. Default: "Inserisci la decorrenza termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:69
+#: design/plone/contenttypes/behaviors/trasparenza.py:70
 msgid "decorrenza_termini_help"
 msgstr ""
 
 #. Default: "Decorrenza termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:64
+#: design/plone/contenttypes/behaviors/trasparenza.py:65
 msgid "decorrenza_termini_label"
 msgstr ""
 
 #. Default: "Elenco delle deleghe a capo della persona."
-#: design/plone/contenttypes/interfaces/persona.py:77
+#: design/plone/contenttypes/interfaces/persona.py:85
 msgid "deleghe_help"
 msgstr ""
 
 #. Default: "Deleghe"
-#: design/plone/contenttypes/interfaces/persona.py:76
+#: design/plone/contenttypes/interfaces/persona.py:84
 msgid "deleghe_label"
 msgstr ""
 
 #. Default: "Descrizione completa"
-#: design/plone/contenttypes/behaviors/luogo.py:23
+#: design/plone/contenttypes/behaviors/luogo.py:24
 msgid "descrizione_completa"
 msgstr ""
 
-#. Default: "Descrizione destinatari"
-#: design/plone/contenttypes/behaviors/evento.py:38
-msgid "descrizione_destinatari"
-msgstr ""
-
-#. Default: "Descrizione dei principali interlocutori dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:40
-msgid "descrizione_destinatari_help"
-msgstr ""
-
 #. Default: "Descrizione estesa"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:16
-#: design/plone/contenttypes/behaviors/evento.py:30
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:19
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:17
+#: design/plone/contenttypes/behaviors/evento.py:32
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
 msgid "descrizione_estesa"
 msgstr ""
 
 #. Default: "Descrizione dettagliata e completa."
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:18
-#: design/plone/contenttypes/behaviors/evento.py:32
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:19
+#: design/plone/contenttypes/behaviors/evento.py:34
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:23
 msgid "descrizione_estesa_help"
 msgstr ""
 
 #. Default: "Descrizione"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:51
-#: design/plone/contenttypes/behaviors/luogo.py:166
-#: design/plone/contenttypes/interfaces/documento.py:162
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:72
+#: design/plone/contenttypes/behaviors/luogo.py:135
+#: design/plone/contenttypes/interfaces/documento.py:242
 msgid "descrizione_label"
 msgstr ""
 
 #. Default: "Inserisci eventuale testo descrittivo del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:37
+#: design/plone/contenttypes/behaviors/trasparenza.py:38
 msgid "descrizione_procedimento_help"
 msgstr ""
 
 #. Default: "Descrizione del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:32
+#: design/plone/contenttypes/behaviors/trasparenza.py:33
 msgid "descrizione_procedimento_label"
 msgstr ""
 
 #. Default: "Dirigente"
-#: design/plone/contenttypes/behaviors/trasparenza.py:136
+#: design/plone/contenttypes/behaviors/trasparenza.py:137
 msgid "dirigente"
 msgstr ""
 
 #. Default: "Indicare il dirigente."
-#: design/plone/contenttypes/behaviors/trasparenza.py:140
+#: design/plone/contenttypes/behaviors/trasparenza.py:141
 msgid "dirigente_help"
 msgstr ""
 
 #. Default: "Distribuzione"
-#: design/plone/contenttypes/interfaces/dataset.py:22
+#: design/plone/contenttypes/interfaces/dataset.py:15
 msgid "distribuzione"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/messaggio.py:56
+#: design/plone/contenttypes/interfaces/messaggio.py:48
 msgid "documenti_allegati"
 msgstr ""
 
 #. Default: "Seleziona una serie di altri contenuti di tipo Documento che vanno allegati a questo."
-#: design/plone/contenttypes/interfaces/documento.py:113
+#: design/plone/contenttypes/interfaces/documento.py:194
 msgid "documenti_allegati_help"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/documento.py:109
+#: design/plone/contenttypes/interfaces/documento.py:190
 msgid "documenti_allegati_label"
 msgstr ""
 
 #. Default: "Documenti"
-#: design/plone/contenttypes/interfaces/persona.py:199
-#: design/plone/contenttypes/interfaces/servizio.py:412
+#: design/plone/contenttypes/interfaces/persona.py:146
+#: design/plone/contenttypes/interfaces/servizio.py:525
 msgid "documenti_label"
 msgstr ""
 
+#. Default: "Documenti pubblici importanti, collegati a questa Unità Organizzativa"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:129
+msgid "documenti_pubblici_help"
+msgstr ""
+
+#. Default: "Documenti pubblici"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:127
+msgid "documenti_pubblici_label"
+msgstr ""
+
 #. Default: "Dove"
-#: design/plone/contenttypes/behaviors/address.py:71
-#: design/plone/contenttypes/behaviors/geolocation.py:29
+#: design/plone/contenttypes/behaviors/address.py:53
+#: design/plone/contenttypes/behaviors/geolocation.py:26
 msgid "dove_label"
 msgstr ""
 
 #. Default: "Dove rivolgersi: informazioni aggiuntive"
-#: design/plone/contenttypes/interfaces/servizio.py:143
+#: design/plone/contenttypes/interfaces/servizio.py:212
 msgid "dove_rivolgersi_extra"
 msgstr ""
 
 #. Default: "Indicare eventuali informazioni aggiuntive riguardo al dove rivolgersi per questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:147
+#: design/plone/contenttypes/interfaces/servizio.py:216
 msgid "dove_rivolgersi_extra_help"
 msgstr ""
 
 #. Default: "Seleziona una lista delle sedi e dei luoghi in cui è presente questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:135
+#: design/plone/contenttypes/interfaces/servizio.py:204
 msgid "dove_rivolgersi_help"
 msgstr ""
 
 #. Default: "Elementi di interesse"
-#: design/plone/contenttypes/behaviors/luogo.py:44
+#: design/plone/contenttypes/behaviors/luogo.py:45
 msgid "elementi_di_interesse"
 msgstr ""
 
-#. Default: "Indicare un indirizzo mail per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:128
-msgid "email_event_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/evento.py:127
-msgid "email_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:35
-msgid "email_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/contatti.py:34
-msgid "email_label"
-msgstr ""
-
-#. Default: "Contatto mail della persona. E' possibile inserire più di un indirizzo. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:135
-msgid "email_persona_help"
-msgstr ""
-
-#. Default: "Indirizzo email"
-#: design/plone/contenttypes/interfaces/persona.py:134
-msgid "email_persona_label"
-msgstr ""
-
 #. Default: "Esito"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:51
 msgid "esito"
 msgstr ""
 
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/evento.py:113
-msgid "fax_event_help"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/evento.py:114
-msgid "fax_event_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/contatti.py:29
-msgid "fax_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/contatti.py:28
-msgid "fax_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/interfaces/persona.py:130
-msgid "fax_persona_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/interfaces/persona.py:129
-msgid "fax_persona_label"
+#. Default: "Escludi dalla ricerca"
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:17
+msgid "exclude_from_search_label"
 msgstr ""
 
 #. Default: "Inserisci il file correlato di questo pocedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:44
+#: design/plone/contenttypes/behaviors/trasparenza.py:45
 msgid "file_correlato_help"
 msgstr ""
 
 #. Default: "File correlato"
-#: design/plone/contenttypes/behaviors/trasparenza.py:43
+#: design/plone/contenttypes/behaviors/trasparenza.py:44
 msgid "file_correlato_label"
 msgstr ""
 
 #. Default: "Inserisci il file principale di questo contenuto."
-#: design/plone/contenttypes/behaviors/multi_file.py:16
+#: design/plone/contenttypes/behaviors/multi_file.py:17
 msgid "file_principale_help"
 msgstr ""
 
 #. Default: "File principale"
-#: design/plone/contenttypes/behaviors/multi_file.py:15
+#: design/plone/contenttypes/behaviors/multi_file.py:16
 msgid "file_principale_label"
 msgstr ""
 
 #. Default: "Inserisci la fine termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:80
+#: design/plone/contenttypes/behaviors/trasparenza.py:81
 msgid "fine_termine_help"
 msgstr ""
 
 #. Default: "Fine termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:75
+#: design/plone/contenttypes/behaviors/trasparenza.py:76
 msgid "fine_termine_label"
 msgstr ""
 
+#. Default: "Lista dei formati in cui è disponibile il documento"
+#: design/plone/contenttypes/interfaces/documento.py:117
+msgid "formati_disponibili_help"
+msgstr ""
+
+#. Default: "Formati disponibili"
+#: design/plone/contenttypes/interfaces/documento.py:116
+msgid "formati_disponibili_label"
+msgstr ""
+
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:25
+#: design/plone/contenttypes/behaviors/multi_file.py:26
 msgid "formato_alternativo_1_help"
 msgstr ""
 
 #. Default: "Formato alternativo 1"
-#: design/plone/contenttypes/behaviors/multi_file.py:24
+#: design/plone/contenttypes/behaviors/multi_file.py:25
 msgid "formato_alternativo_1_label"
 msgstr ""
 
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:35
+#: design/plone/contenttypes/behaviors/multi_file.py:36
 msgid "formato_alternativo_2_help"
 msgstr ""
 
 #. Default: "Formato alternativo 2"
-#: design/plone/contenttypes/behaviors/multi_file.py:34
+#: design/plone/contenttypes/behaviors/multi_file.py:35
 msgid "formato_alternativo_2_label"
 msgstr ""
 
-#. Default: "Foto da mostrare della persona. La dimensione suggerita è 180x100 px."
-#: design/plone/contenttypes/interfaces/persona.py:21
+#. Default: "Foto da mostrare della persona. La dimensione suggerita è 100x180px."
+#: design/plone/contenttypes/interfaces/persona.py:30
 msgid "foto_persona_help"
 msgstr ""
 
 #. Default: "Foto della persona"
-#: design/plone/contenttypes/interfaces/persona.py:19
+#: design/plone/contenttypes/interfaces/persona.py:28
 msgid "foto_persona_label"
 msgstr ""
 
 #. Default: "Frequenza di aggiornamento"
-#: design/plone/contenttypes/interfaces/dataset.py:32
+#: design/plone/contenttypes/interfaces/dataset.py:25
 msgid "frequenza_aggiornamento"
 msgstr ""
 
 #. Default: "Invalid geolocation data: ${value}. Provide latitude and longitude coordinates."
-#: design/plone/contenttypes/restapi/deserializers/dxfields.py:28
+#: design/plone/contenttypes/restapi/deserializers/dxfields.py:39
 msgid "geolocation_field_validator_label"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/address.py:38
 msgid "help_circoscrizione"
 msgstr ""
 
 #. Default: "Indicare una descrizione completa, inserendo tutte le informazioni rilevanti relative al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:24
+#: design/plone/contenttypes/behaviors/luogo.py:25
 msgid "help_descrizione_completa"
 msgstr ""
 
 #. Default: "Indicare eventuali elementi di interesse per il cittadino."
-#: design/plone/contenttypes/behaviors/luogo.py:45
+#: design/plone/contenttypes/behaviors/luogo.py:46
 msgid "help_elementi_di_interesse"
 msgstr ""
 
+#. Default: "Se selezionato, questo contenuto non verrà mostrato nelle ricerche del sito per gli utenti anonimi."
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:18
+msgid "help_exclude_from_search"
+msgstr ""
+
 #. Default: "Indicare tutte le informazioni relative alla modalità di accesso al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:54
+#: design/plone/contenttypes/behaviors/luogo.py:55
 msgid "help_modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare, se esiste, un nome alternativo per il luogo; questo sarà mostrato affianco al titolo della scheda"
-#: design/plone/contenttypes/behaviors/luogo.py:34
+#: design/plone/contenttypes/behaviors/luogo.py:35
 msgid "help_nome_alternativo"
 msgstr ""
 
 #. Default: "Inserisci il nome della sede, se non è presente tra i Luoghi del sito."
 #: design/plone/contenttypes/behaviors/address.py:17
 msgid "help_nome_sede"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/address.py:32
 msgid "help_quartiere"
 msgstr ""
 
-#. Default: "Indicare un numero di fax della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:108
-msgid "help_riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:119
-msgid "help_riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:132
-msgid "help_riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Indicare il riferimento telefonico per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:96
-msgid "help_riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato.Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
-#: design/plone/contenttypes/behaviors/update_note.py:17
+#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato. Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
+#: design/plone/contenttypes/behaviors/update_note.py:18
 msgid "help_update_note"
 msgstr ""
 
 #. Default: "Icona"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:27
 msgid "icona"
 msgstr ""
 
 #. Default: "Puoi selezionare un’icona fra quelle proposte nel menu a tendina oppure puoi scrivere/incollare nel campo di testo il nome di un’icona di fontawsome 5"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:28
 msgid "icona_help"
 msgstr ""
 
 #. Default: "Identificativo"
-#: design/plone/contenttypes/interfaces/servizio.py:290
+#: design/plone/contenttypes/interfaces/servizio.py:379
 msgid "identificativo"
 msgstr ""
 
 #. Default: "Un numero identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:21
 msgid "identificativo_documento_help"
 msgstr ""
 
 #. Default: "Identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:17
 msgid "identificativo_documento_label"
 msgstr ""
 
 #. Default: "Eventuale codice identificativo del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:292
+#: design/plone/contenttypes/interfaces/servizio.py:381
 msgid "identificativo_help"
 msgstr ""
 
+#. Default: "Identificativo"
+#: design/plone/contenttypes/behaviors/luogo.py:119
+msgid "identificativo_mibac"
+msgstr ""
+
+#. Default: "Codice identificativo del luogo. Nel MIBAC c'è il codice del DBUnico per i luoghi della cultura e il codice ISIL per le biblioteche. Non deve comparire nel frontend del sito."
+#: design/plone/contenttypes/behaviors/luogo.py:121
+msgid "identificativo_mibac_help"
+msgstr ""
+
 #. Default: "La dimensione dell'immagine dovrebbe essere di ${size} px"
-#: design/plone/contenttypes/restapi/types/adapters.py:31
+#: design/plone/contenttypes/restapi/types/adapters.py:43
 msgid "image_size_help"
 msgstr ""
 
 #. Default: "Immagine"
 #: design/plone/contenttypes/interfaces/documento_personale.py:23
 msgid "immagine"
 msgstr ""
 
+#. Default: "Solo per incarico politico: importi di viaggi di servizio  e missioni pagati con fondi pubblici."
+#: design/plone/contenttypes/interfaces/incarico.py:34
+msgid "importi_viaggio_servizio_incarico_help"
+msgstr ""
+
+#. Default: "Importi di viaggio e/o servizio"
+#: design/plone/contenttypes/interfaces/incarico.py:30
+msgid "importi_viaggio_servizio_incarico_label"
+msgstr ""
+
 #. Default: "Importo pagato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:25
 msgid "importo_pagato"
 msgstr ""
 
+#. Default: "Seleziona l'incarico corrente della persona."
+#: design/plone/contenttypes/interfaces/persona.py:63
+msgid "incarichi_help"
+msgstr ""
+
+#. Default: "Incarichi"
+#: design/plone/contenttypes/interfaces/persona.py:59
+msgid "incarichi_label"
+msgstr ""
+
 #. Default: "Inserisci eventuale testo informativo che verrà mostrato in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:23
 msgid "info_testata_help"
 msgstr ""
 
 #. Default: "Informazioni aggiuntive per la testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:18
@@ -1705,127 +1727,162 @@
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/interfaces/documento_personale.py:140
 msgid "informazioni"
 msgstr ""
 
+#. Default: "Compensi e trasparenza"
+#: design/plone/contenttypes/interfaces/incarico.py:170
+msgid "informazioni_compensi_label"
+msgstr ""
+
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/behaviors/additional_help_infos.py:28
-#: design/plone/contenttypes/behaviors/evento.py:229
 #: design/plone/contenttypes/behaviors/strutture_correlate.py:42
+#: design/plone/contenttypes/interfaces/documento.py:253
 msgid "informazioni_label"
 msgstr ""
 
+#. Default: "Intervallo della fase (es. 1)"
+#: design/plone/contenttypes/interfaces/servizio.py:32
+msgid "interval_qt_help"
+msgstr ""
+
+#. Default: "Intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:31
+msgid "interval_qt_label"
+msgstr ""
+
+#. Default: "Ad esempio: ore, giorni, settimane, mesi."
+#: design/plone/contenttypes/interfaces/servizio.py:41
+msgid "interval_type_help"
+msgstr ""
+
+#. Default: "Tipo intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:40
+msgid "interval_type_label"
+msgstr ""
+
 #. Default: "Se un content-type deve avere una dimensione della leadimage particolare, indicarle qui. Inserire le dimensioni nella forma di esempio PortalType|900x900"
-#: design/plone/contenttypes/controlpanels/settings.py:110
+#: design/plone/contenttypes/controlpanels/settings.py:52
 msgid "lead_image_dimension_help"
 msgstr ""
 
 #. Default: "Dimensioni lead image"
-#: design/plone/contenttypes/controlpanels/settings.py:106
+#: design/plone/contenttypes/controlpanels/settings.py:48
 msgid "lead_image_dimension_label"
 msgstr ""
 
-#. Default: "Servizi o uffici di riferimento"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:27
+#. Default: "Strutture o uffici di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
 msgid "legami_altre_strutture_label"
 msgstr ""
 
 #. Default: "Selezionare la lista di strutture e/o uffici collegati a questa unità organizzativa."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:35
 msgid "legami_con_altre_strutture_help"
 msgstr ""
 
 #. Default: "Licenza"
-#: design/plone/contenttypes/interfaces/dataset.py:25
+#: design/plone/contenttypes/interfaces/dataset.py:18
 msgid "licenza"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
 #: design/plone/contenttypes/interfaces/documento_personale.py:92
 msgid "licenza_distribuzione"
 msgstr ""
 
 #. Default: "La licenza con il quale viene distribuito questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:88
+#: design/plone/contenttypes/interfaces/documento.py:125
 msgid "licenza_distribuzione_help"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
-#: design/plone/contenttypes/interfaces/documento.py:87
+#: design/plone/contenttypes/interfaces/documento.py:124
 msgid "licenza_distribuzione_label"
 msgstr ""
 
 #. Default: "Link a siti esterni"
-#: design/plone/contenttypes/interfaces/servizio.py:258
+#: design/plone/contenttypes/interfaces/servizio.py:347
 msgid "link_siti_esterni"
 msgstr ""
 
 #. Default: "Eventuali collegamenti a pagine web, siti, servizi esterni all'ambito Comunale utili all'erogazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:260
+#: design/plone/contenttypes/interfaces/servizio.py:349
 msgid "link_siti_esterni_help"
 msgstr ""
 
 #. Default: "Link utili"
-#: design/plone/contenttypes/interfaces/servizio.py:417
+#: design/plone/contenttypes/interfaces/servizio.py:530
 msgid "link_utili_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati. Se il luogo dell'evento non è presente sul sito, inserisci le sue informazioni nei campi seguenti."
 #: design/plone/contenttypes/behaviors/luoghi_correlati.py:52
 msgid "luoghi_correlati_event_help"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati."
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:72
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:19
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:64
 msgid "luoghi_correlati_help"
 msgstr ""
 
 #. Default: "Luoghi correlati"
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:17
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:71
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:63
 msgid "luoghi_correlati_label"
 msgstr ""
 
 #. Default: "Luogo"
-#: design/plone/contenttypes/behaviors/address.py:89
-#: design/plone/contenttypes/behaviors/geolocation.py:38
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:74
+#: design/plone/contenttypes/behaviors/address.py:71
+#: design/plone/contenttypes/behaviors/geolocation.py:34
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:76
 msgid "luogo_label"
 msgstr ""
 
+#. Default: "Sottotitolo"
+#: design/plone/contenttypes/interfaces/servizio.py:26
+msgid "milestone_description_label"
+msgstr ""
+
+#. Default: "Titolo"
+#: design/plone/contenttypes/interfaces/servizio.py:21
+msgid "milestone_label"
+msgstr ""
+
 #. Default: "Modalita' di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:53
+#: design/plone/contenttypes/behaviors/luogo.py:54
 msgid "modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare la modalità di avvio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:25
+#: design/plone/contenttypes/behaviors/trasparenza.py:26
 msgid "modalita_avvio_help"
 msgstr ""
 
 #. Default: "Modalita di avvio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:24
+#: design/plone/contenttypes/behaviors/trasparenza.py:25
 msgid "modalita_avvio_label"
 msgstr ""
 
 #. Default: "Modalità pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:29
 msgid "modalita_pagamento"
 msgstr ""
 
 #. Default: "Indicare le modalità per richiedere informazioni riguardo a questo procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:168
+#: design/plone/contenttypes/behaviors/trasparenza.py:169
 msgid "modalita_richiesta_informazioni_help"
 msgstr ""
 
 #. Default: "Modalità per richiedere informazioni"
-#: design/plone/contenttypes/behaviors/trasparenza.py:163
+#: design/plone/contenttypes/behaviors/trasparenza.py:164
 msgid "modalita_richiesta_informazioni_label"
 msgstr ""
 
 #. Default: "Seleziona se mostrare o meno i bottoni con i link per la condivisione sui vari social, mail e stampa."
 #: design/plone/contenttypes/behaviors/info_testata.py:44
 msgid "mostra_bottoni_condivisione_help"
 msgstr ""
@@ -1841,46 +1898,46 @@
 msgstr ""
 
 #. Default: "Mostra la navigazione"
 #: design/plone/contenttypes/behaviors/info_testata.py:51
 msgid "mostra_navigazione_label"
 msgstr ""
 
-#. Default: "Descrizione del motivo per cui il servizio non è attivo."
-#: design/plone/contenttypes/interfaces/servizio.py:44
+#. Default: "Descrizione del motivo per cui il servizio non è attivo. È obbligatorio se il campo precedente è spuntato."
+#: design/plone/contenttypes/interfaces/servizio.py:89
 msgid "motivo_stato_servizio_help"
 msgstr ""
 
-#. Default: "Motivo dello stato del servizio nel caso non sia attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:39
+#. Default: "Motivo dello stato"
+#: design/plone/contenttypes/interfaces/servizio.py:84
 msgid "motivo_stato_servizio_label"
 msgstr ""
 
 #. Default: "Nome alternativo"
-#: design/plone/contenttypes/behaviors/luogo.py:33
+#: design/plone/contenttypes/behaviors/luogo.py:34
 msgid "nome_alternativo"
 msgstr ""
 
 #. Default: "Nome sede"
 #: design/plone/contenttypes/behaviors/address.py:16
 msgid "nome_sede"
 msgstr ""
 
 #. Default: "Seleziona una lista di notizie correlate a questa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:83
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:75
 msgid "notizie_correlate_help"
 msgstr ""
 
 #. Default: "Notizie correlate"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:82
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:74
 msgid "notizie_correlate_label"
 msgstr ""
 
 #. Default: "Numero progressivo del comunicato stampa"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:30
 msgid "numero_progressivo_cs_label"
 msgstr ""
 
 #. Default: "Numero protocollo"
 #: design/plone/contenttypes/interfaces/pratica.py:12
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:12
 msgid "numero_protocollo"
@@ -1888,125 +1945,163 @@
 
 #. Default: "Oggetto"
 #: design/plone/contenttypes/interfaces/documento_personale.py:48
 msgid "oggetto"
 msgstr ""
 
 #. Default: "Informazioni sugli orari"
-#: design/plone/contenttypes/behaviors/evento.py:62
+#: design/plone/contenttypes/behaviors/evento.py:50
 msgid "orari"
 msgstr ""
 
 #. Default: "Informazioni sugli orari di svolgimento dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:64
+#: design/plone/contenttypes/behaviors/evento.py:52
 msgid "orari_help"
 msgstr ""
 
 #. Default: "Orari di apertura"
-#: design/plone/contenttypes/behaviors/contatti.py:86
+#: design/plone/contenttypes/behaviors/luogo.py:151
 msgid "orari_label"
 msgstr ""
 
+#. Default: "Orario per il pubblico"
+#: design/plone/contenttypes/behaviors/luogo.py:93
+msgid "orario_pubblico"
+msgstr ""
+
 #. Default: "Indicare eventuali orari di accesso al pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:59
+#: design/plone/contenttypes/behaviors/contatti.py:40
+#: design/plone/contenttypes/behaviors/luogo.py:95
 msgid "orario_pubblico_help"
 msgstr ""
 
 #. Default: "Orario per il pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:58
+#: design/plone/contenttypes/behaviors/contatti.py:39
 msgid "orario_pubblico_label"
 msgstr ""
 
 #. Default: "Se l'evento non è organizzato direttamente dal comune oppure ha anche un organizzatore esterno, indicare il nome del contatto."
-#: design/plone/contenttypes/behaviors/evento.py:97
+#: design/plone/contenttypes/behaviors/evento.py:86
 msgid "organizzato_da_esterno_help"
 msgstr ""
 
 #. Default: "Organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:95
+#: design/plone/contenttypes/behaviors/evento.py:84
 msgid "organizzato_da_esterno_label"
 msgstr ""
 
 #. Default: "Se l'evento è organizzato direttamente dal comune, indicare l'ufficio/ente organizzatore. I dati di contatto verranno presi direttamente dall'ufficio selezionato. Se l'evento non è organizzato direttamente dal comune, o si vogliono sovrascrivere alcuni dati di contatto, utilizzare i seguenti campi."
-#: design/plone/contenttypes/behaviors/evento.py:84
+#: design/plone/contenttypes/behaviors/evento.py:74
 msgid "organizzato_da_interno_help"
 msgstr ""
 
 #. Default: "Organizzato da"
-#: design/plone/contenttypes/behaviors/evento.py:80
+#: design/plone/contenttypes/behaviors/evento.py:70
 msgid "organizzato_da_interno_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di organizzazioni a cui la persona appartiene."
-#: design/plone/contenttypes/interfaces/persona.py:42
+#: design/plone/contenttypes/interfaces/persona.py:45
 msgid "organizzazione_riferimento_help"
 msgstr ""
 
 #. Default: "Organizzazione di riferimento"
-#: design/plone/contenttypes/interfaces/persona.py:38
+#: design/plone/contenttypes/interfaces/persona.py:41
 msgid "organizzazione_riferimento_label"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:157
+#: design/plone/contenttypes/behaviors/trasparenza.py:158
 msgid "organo_competente_provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:152
+#: design/plone/contenttypes/behaviors/trasparenza.py:153
 msgid "organo_competente_provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Indicare le informazioni riguardanti i pagamenti previsti e modalità di pagamento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:222
+#: design/plone/contenttypes/behaviors/trasparenza.py:223
 msgid "pagamenti_help"
 msgstr ""
 
 #. Default: "Pagamenti previsti e modalità"
-#: design/plone/contenttypes/behaviors/trasparenza.py:218
+#: design/plone/contenttypes/behaviors/trasparenza.py:219
 msgid "pagamenti_label"
 msgstr ""
 
+#. Default: "Link a persone dell'amministrazione che interverranno all'evento"
+#: design/plone/contenttypes/behaviors/evento.py:118
+msgid "parteciperanno_help"
+msgstr ""
+
+#. Default: "Parteciperanno (Persone)"
+#: design/plone/contenttypes/behaviors/evento.py:114
+msgid "parteciperanno_label"
+msgstr ""
+
 #. Default: "Indicare l'ente che supporta l'evento, se presente."
-#: design/plone/contenttypes/behaviors/evento.py:160
+#: design/plone/contenttypes/behaviors/evento.py:107
 msgid "patrocinato_da_help"
 msgstr ""
 
 #. Default: "Patrocinato da"
-#: design/plone/contenttypes/behaviors/evento.py:158
+#: design/plone/contenttypes/behaviors/evento.py:105
 msgid "patrocinato_da_label"
 msgstr ""
 
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:44
-msgid "pec_help"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:27
+msgid "pdc_desc_help"
 msgstr ""
 
-#. Default: "Pec"
-#: design/plone/contenttypes/behaviors/contatti.py:43
-msgid "pec_label"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:26
+msgid "pdc_desc_label"
 msgstr ""
 
-#. Default: "Elenco delle persone dell'amministrazione che parteciperanno all'evento."
-#: design/plone/contenttypes/behaviors/evento.py:53
-msgid "persone_amministrazione_help"
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:16
+msgid "pdc_type_label"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:37
+msgid "pdc_value_help"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:36
+msgid "pdc_value_label"
+msgstr ""
+
+#. Default: "Seleziona la persona che ha questo incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:47
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:66
+msgid "persona_incarico_help"
+msgstr ""
+
+#. Default: "La persona che ha la carica e l'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:43
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:62
+msgid "persona_incarico_label"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:221
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:215
 msgid "persone_label"
 msgstr ""
 
 #. Default: "Seleziona la lista delle persone che compongono la struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
 msgid "persone_struttura_help"
 msgstr ""
 
 #. Default: "Persone che compongono la struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:79
 msgid "persone_struttura_label"
 msgstr ""
 
 #. Default: "Pratica associata"
 #: design/plone/contenttypes/interfaces/documento_personale.py:26
 #: design/plone/contenttypes/interfaces/messaggio.py:35
 msgid "pratica_associata"
@@ -2014,255 +2109,230 @@
 
 #. Default: "Pratica associata al pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:43
 msgid "pratica_associata_ricevuta"
 msgstr ""
 
 #. Default: "Prenota un appuntamento"
-#: design/plone/contenttypes/interfaces/servizio.py:156
+#: design/plone/contenttypes/interfaces/servizio.py:225
 msgid "prenota_appuntamento"
 msgstr ""
 
 #. Default: "Se è possibile prenotare un'appuntamento, indicare le informazioni necessarie e il collegamento al servizio di prenotazione appuntamenti del Comune."
-#: design/plone/contenttypes/interfaces/servizio.py:157
+#: design/plone/contenttypes/interfaces/servizio.py:226
 msgid "prenota_appuntamento_help"
 msgstr ""
 
-#. Default: "Prezzo"
-#: design/plone/contenttypes/behaviors/evento.py:71
+#. Default: "Costo"
+#: design/plone/contenttypes/behaviors/evento.py:59
 msgid "prezzo"
 msgstr ""
 
-#. Default: "Indicare il prezzo dell'evento, se presente, specificando se esistono formati diversi."
-#: design/plone/contenttypes/behaviors/evento.py:73
+#. Default: "Eventuale costo dell'evento (se ci sono uno o più biglietti), con link all'acquisto se disponibile"
+#: design/plone/contenttypes/behaviors/evento.py:61
 msgid "prezzo_help"
 msgstr ""
 
 #. Default: "Indicare, se la procedura è informatizzata online, il riferimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:178
+#: design/plone/contenttypes/behaviors/trasparenza.py:179
 msgid "procedura_online_help"
 msgstr ""
 
 #. Default: "Procedura informatizzata online"
-#: design/plone/contenttypes/behaviors/trasparenza.py:174
+#: design/plone/contenttypes/behaviors/trasparenza.py:175
 msgid "procedura_online_label"
 msgstr ""
 
 #. Default: "Procedure collegate all'esito"
-#: design/plone/contenttypes/interfaces/servizio.py:100
+#: design/plone/contenttypes/interfaces/servizio.py:145
 msgid "procedure_collegate"
 msgstr ""
 
 #. Default: "Indicare cosa deve fare l'utente del servizio per conoscere l'esito della procedura, e dove eventualmente poter ritirare l'esito."
-#: design/plone/contenttypes/interfaces/servizio.py:102
+#: design/plone/contenttypes/interfaces/servizio.py:147
 msgid "procedure_collegate_help"
 msgstr ""
 
 #. Default: "Protocollo"
 #: design/plone/contenttypes/interfaces/documento_personale.py:15
 msgid "protocollo"
 msgstr ""
 
+#. Default: "Il numero di protocollo del documento."
+#: design/plone/contenttypes/interfaces/documento.py:33
+msgid "protocollo_documento_help"
+msgstr ""
+
+#. Default: "Numero di protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:29
+msgid "protocollo_documento_label"
+msgstr ""
+
 #. Default: "Eventuale provvedimento finale del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:114
+#: design/plone/contenttypes/behaviors/trasparenza.py:115
 msgid "provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Provvedimento del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:109
+#: design/plone/contenttypes/behaviors/trasparenza.py:110
 msgid "provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Quartiere"
 #: design/plone/contenttypes/behaviors/address.py:31
 msgid "quartiere"
 msgstr ""
 
-#. Default: "Reperibilità organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:118
-msgid "reperibilita"
-msgstr ""
-
-#. Default: "Indicare gli orari in cui l'organizzatore è telefonicamente reperibile."
-#: design/plone/contenttypes/behaviors/evento.py:120
-msgid "reperibilita_help"
-msgstr ""
-
 #. Default: "Indicare dove è possibile reperre la modulistica per il procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:211
+#: design/plone/contenttypes/behaviors/trasparenza.py:212
 msgid "reperimento_modulistica_help"
 msgstr ""
 
 #. Default: "Dove reperire la modulistica"
-#: design/plone/contenttypes/behaviors/trasparenza.py:207
+#: design/plone/contenttypes/behaviors/trasparenza.py:208
 msgid "reperimento_modulistica_label"
 msgstr ""
 
 #. Default: "Selezionare il/i responsabile/i della struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:48
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:52
 msgid "responsabile_help"
 msgstr ""
 
 #. Default: "Responsabile"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:43
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:47
 msgid "responsabile_label"
 msgstr ""
 
 #. Default: "Responsabile del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:120
+#: design/plone/contenttypes/behaviors/trasparenza.py:121
 msgid "responsabile_procedimento"
 msgstr ""
 
 #. Default: "Indicare il responsabile del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:124
+#: design/plone/contenttypes/behaviors/trasparenza.py:125
 msgid "responsabile_procedimento_help"
 msgstr ""
 
+#. Default: "Se è un incarico di responsabilità, specificare l'organizzazione della quale è responsabile in base all'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:81
+msgid "responsabile_struttura_incarico_help"
+msgstr ""
+
+#. Default: "Responsabile della struttura"
+#: design/plone/contenttypes/interfaces/incarico.py:77
+msgid "responsabile_struttura_incarico_label"
+msgstr ""
+
 #. Default: "Seleziona se mostrare o meno il campo di ricerca in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:32
 msgid "ricerca_in_testata_help"
 msgstr ""
 
 #. Default: "Ricerca in testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:29
 msgid "ricerca_in_testata_label"
 msgstr ""
 
 #. Default: "Ulteriori informazioni non previste negli altri campi; si può trattare di contatti o note informative la cui conoscenza è indispensabile per la partecipazione al bando"
-#: design/plone/contenttypes/interfaces/bando.py:96
+#: design/plone/contenttypes/interfaces/bando.py:97
 msgid "riferimenti_bando_agid_help"
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
-#: design/plone/contenttypes/interfaces/bando.py:95
+#: design/plone/contenttypes/interfaces/bando.py:96
 msgid "riferimenti_bando_agid_label"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
 #: design/plone/contenttypes/interfaces/documento_personale.py:145
 msgid "riferimenti_normativi"
 msgstr ""
 
 #. Default: "Inserisici del testo di dettaglio per eventuali riferimenti normativi utili a questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:100
+#: design/plone/contenttypes/interfaces/documento.py:137
 msgid "riferimenti_normativi_documento_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/interfaces/documento.py:96
+#: design/plone/contenttypes/interfaces/documento.py:133
 msgid "riferimenti_normativi_documento_label"
 msgstr ""
 
 #. Default: "Indicare eventuali riferimenti normativi."
-#: design/plone/contenttypes/behaviors/trasparenza.py:265
+#: design/plone/contenttypes/behaviors/trasparenza.py:266
 msgid "riferimenti_normativi_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/behaviors/trasparenza.py:260
+#: design/plone/contenttypes/behaviors/trasparenza.py:261
 msgid "riferimenti_normativi_label"
 msgstr ""
 
-#. Default: "Fax della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:104
-msgid "riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "E-mail struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:115
-msgid "riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Pec della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:128
-msgid "riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Telefono della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:92
-msgid "riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per il ruolo di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:84
-msgid "ruoli_persona_help"
-msgstr ""
-
-#. Default: "Ruoli Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:83
-msgid "ruoli_persona_label"
-msgstr ""
-
-#. Default: "Seleziona il ruolo della persona tra quelli disponibili."
-#: design/plone/contenttypes/interfaces/persona.py:29
-msgid "ruolo_help"
-msgstr ""
-
 #. Default: "Ruolo"
-#: design/plone/contenttypes/interfaces/persona.py:28
+#: design/plone/contenttypes/interfaces/persona.py:135
 msgid "ruolo_label"
 msgstr ""
 
 #. Default: "Data entro la quale sarà possibile far pervenire domande e richieste di chiarimento a chi eroga il bando"
-#: design/plone/contenttypes/interfaces/bando.py:69
+#: design/plone/contenttypes/interfaces/bando.py:70
 msgid "scadenza_domande_bando_help"
 msgstr ""
 
 #. Default: "Termine per le richieste di chiarimenti"
-#: design/plone/contenttypes/interfaces/bando.py:65
+#: design/plone/contenttypes/interfaces/bando.py:66
 msgid "scadenza_domande_bando_label"
 msgstr ""
 
 #. Default: "Inserire una lista di sezioni per la ricerca."
-#: design/plone/contenttypes/controlpanels/settings.py:129
+#: design/plone/contenttypes/controlpanels/settings.py:71
 msgid "search_sections_help"
 msgstr ""
 
 #. Default: "Sezioni ricerca"
-#: design/plone/contenttypes/controlpanels/settings.py:128
+#: design/plone/contenttypes/controlpanels/settings.py:70
 msgid "search_sections_label"
 msgstr ""
 
-#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente un contenuto di tipo Luogo a cui far riferimento, puoi compilare i campi seguenti. Se selezioni un Luogo, puoi usare comunque i campi seguenti per sovrascrivere alcune informazioni."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:105
+#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente creare il Luogo nella sezione dedicata nell'alberatura del sito."
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:97
 msgid "sede_help"
 msgstr ""
 
 #. Default: "Sede principale"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:103
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
 msgid "sede_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di eventuali contenuti di tipo Luogo che sono sedi secondarie di questa struttura. Per queste sedi non sarà possibile sovrascrivere i dati. Nel caso servano informazioni diverse, è possibile usare il campo sottostante."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:122
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:112
 msgid "sedi_secondarie_help"
 msgstr ""
 
-#. Default: "Sedi secondarie"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:120
+#. Default: "Altre sedi"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:110
 msgid "sedi_secondarie_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei servizi collegati a questo."
-#: design/plone/contenttypes/interfaces/servizio.py:300
+#: design/plone/contenttypes/interfaces/servizio.py:394
 msgid "servizi_collegati_help"
 msgstr ""
 
 #. Default: "Servizi collegati"
-#: design/plone/contenttypes/interfaces/servizio.py:299
+#: design/plone/contenttypes/interfaces/servizio.py:393
 msgid "servizi_collegati_label"
 msgstr ""
 
 #. Default: "Questi servizi non verranno mostrati nel contenuto, ma permetteranno di vedere questo contenuto associato quando si visita il servizio"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:20
 msgid "servizi_correlati_description"
 msgstr ""
 
 #. Default: "Servizi correlati"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:18
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
 msgid "servizi_correlati_label"
 msgstr ""
 
 #. Default: "Servizio che genera il documento"
 #: design/plone/contenttypes/interfaces/documento_personale.py:31
 msgid "servizio_origine"
 msgstr ""
@@ -2274,367 +2344,292 @@
 
 #. Default: "Servizio che origina la pratica"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:35
 msgid "servizio_origine_ricevuta"
 msgstr ""
 
 #. Default: "Settore merceologico"
-#: design/plone/contenttypes/interfaces/servizio.py:280
+#: design/plone/contenttypes/interfaces/servizio.py:369
 msgid "settore_merceologico"
 msgstr ""
 
 #. Default: "Classificazione del servizio basata su catalogo dei servizi (Classificazione NACE)."
-#: design/plone/contenttypes/interfaces/servizio.py:282
+#: design/plone/contenttypes/interfaces/servizio.py:371
 msgid "settore_merceologico_help"
 msgstr ""
 
+#. Default: "Se selezionato, il footer verrà popolato automaticamente con i contenuti di primo livello non esclusi dalla navigazione."
+#: design/plone/contenttypes/controlpanels/settings.py:93
+msgid "show_dynamic_folders_in_footer_help"
+msgstr ""
+
+#. Default: "Footer dinamico"
+#: design/plone/contenttypes/controlpanels/settings.py:92
+msgid "show_dynamic_folders_in_footer_label"
+msgstr ""
+
 #. Default: "Questo è il valore di default per decidere se mostrare o meno la data di modifica nei contenuti che hanno la behavior abilitata. E' poi possibile sovrascrivere il default nei singoli contenuti (nel tab \"Impostazioni\")."
-#: design/plone/contenttypes/controlpanels/settings.py:139
+#: design/plone/contenttypes/controlpanels/settings.py:81
 msgid "show_modified_default_help"
 msgstr ""
 
 #. Default: "Mostra la data di modifica"
-#: design/plone/contenttypes/controlpanels/settings.py:138
+#: design/plone/contenttypes/controlpanels/settings.py:80
 msgid "show_modified_default_label"
 msgstr ""
 
 #. Default: "Se attivo, verrà mostrata la data di ultima modifica in visualizzazione del contenuto."
 #: design/plone/contenttypes/behaviors/show_modified.py:24
 msgid "show_modified_help"
 msgstr ""
 
 #. Default: "Mostra la data di ultima modifica"
 #: design/plone/contenttypes/behaviors/show_modified.py:23
 msgid "show_modified_label"
 msgstr ""
 
 #. Default: "Indicare se il procedimento prevede il silenzio assenso o la dichiarazione dell'interessato sostitutiva del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:103
+#: design/plone/contenttypes/behaviors/trasparenza.py:104
 msgid "silenzio_assenso_help"
 msgstr ""
 
 #. Default: "Silenzio assenso/Dichiarazione dell'interessato sostitutiva del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:97
+#: design/plone/contenttypes/behaviors/trasparenza.py:98
 msgid "silenzio_assenso_label"
 msgstr ""
 
 #. Default: "Inserisci eventuali soggetti esterni, nonché, strutture interne coinvolte nel procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:57
+#: design/plone/contenttypes/behaviors/trasparenza.py:58
 msgid "soggetti_eserni_help"
 msgstr ""
 
 #. Default: "Soggetti esterni, nonché, strutture interne coinvolte nel procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:52
+#: design/plone/contenttypes/behaviors/trasparenza.py:53
 msgid "soggetti_eserni_label"
 msgstr ""
 
 #. Default: "Indica un eventuale sottotitolo/titolo alternativo."
-#: design/plone/contenttypes/behaviors/evento.py:23
-#: design/plone/contenttypes/interfaces/servizio.py:19
+#: design/plone/contenttypes/behaviors/evento.py:24
+#: design/plone/contenttypes/interfaces/servizio.py:64
 msgid "sottotitolo_help"
 msgstr ""
 
 #. Default: "Sottotitolo"
-#: design/plone/contenttypes/behaviors/evento.py:22
-#: design/plone/contenttypes/interfaces/servizio.py:18
+#: design/plone/contenttypes/behaviors/evento.py:23
+#: design/plone/contenttypes/interfaces/servizio.py:63
 msgid "sottotitolo_label"
 msgstr ""
 
 #. Default: "Stampa ricevuta"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:17
 msgid "stampa_ricevuta"
 msgstr ""
 
 #. Default: "Stato della pratica"
 #: design/plone/contenttypes/interfaces/pratica.py:26
 msgid "stato_pratica"
 msgstr ""
 
-#. Default: "Indica se il servizio è effettivamente fruibile."
-#: design/plone/contenttypes/interfaces/servizio.py:32
+#. Default: "Indica se il servizio è effettivamente fruibile; spuntare se non è fruibile."
+#: design/plone/contenttypes/interfaces/servizio.py:77
 msgid "stato_servizio_help"
 msgstr ""
 
-#. Default: "Servizio non attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:30
+#. Default: "Servizio non fruibile"
+#: design/plone/contenttypes/interfaces/servizio.py:75
 msgid "stato_servizio_label"
 msgstr ""
 
 #. Default: "Indicare gli eventuali strumenti di tutela."
-#: design/plone/contenttypes/behaviors/trasparenza.py:230
+#: design/plone/contenttypes/behaviors/trasparenza.py:231
 msgid "strumenti_tutela_help"
 msgstr ""
 
 #. Default: "Strumenti di tutela"
-#: design/plone/contenttypes/behaviors/trasparenza.py:229
+#: design/plone/contenttypes/behaviors/trasparenza.py:230
 msgid "strumenti_tutela_label"
 msgstr ""
 
 #. Default: "Struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:211
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
 msgid "struttura_label"
 msgstr ""
 
 #. Default: "Struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:82
+#: design/plone/contenttypes/behaviors/luogo.py:83
 msgid "struttura_responsabile"
 msgstr ""
 
 #. Default: "Struttura responsabile del luogo."
-#: design/plone/contenttypes/behaviors/luogo.py:63
+#: design/plone/contenttypes/behaviors/luogo.py:64
 msgid "struttura_responsabile_correlati"
 msgstr ""
 
 #. Default: "Indicare la struttura responsabile del luogo qualora sia fra unità organizzative del comune inserite nel sito; altrimenti compilare i campi testuali relativi alla struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:67
+#: design/plone/contenttypes/behaviors/luogo.py:68
 msgid "struttura_responsabile_correlati_help"
 msgstr ""
 
 #. Default: "Nome/link al sito web della struttura che gestisce il luogo, se questa non è comunale."
-#: design/plone/contenttypes/behaviors/luogo.py:84
+#: design/plone/contenttypes/behaviors/luogo.py:85
 msgid "struttura_responsabile_help"
 msgstr ""
 
 #. Default: "Seleziona la lista delle strutture politiche coinvolte."
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:25
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:26
 msgid "strutture_politiche_help"
 msgstr ""
 
 #. Default: "Indicare gli uffici/enti che supportano l'evento."
-#: design/plone/contenttypes/behaviors/evento.py:149
+#: design/plone/contenttypes/behaviors/evento.py:97
 msgid "supportato_da_help"
 msgstr ""
 
 #. Default: "Evento supportato da"
-#: design/plone/contenttypes/behaviors/evento.py:145
+#: design/plone/contenttypes/behaviors/evento.py:93
 msgid "supportato_da_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di argomenti d'interesse per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:22
+#: design/plone/contenttypes/behaviors/argomenti.py:26
 msgid "tassonomia_argomenti_help"
 msgstr ""
 
-#. Default: "Tassonomia argomenti"
-#: design/plone/contenttypes/behaviors/argomenti.py:21
+#. Default: "Argomenti"
+#: design/plone/contenttypes/behaviors/argomenti.py:25
 msgid "tassonomia_argomenti_label"
 msgstr ""
 
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/evento.py:104
-msgid "telefono_event_help"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:105
-msgid "telefono_event_label"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:19
-msgid "telefono_help"
-msgstr ""
-
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/contatti.py:18
-msgid "telefono_label"
-msgstr ""
-
-#. Default: "Contatto telefonico della persona. E' possibile inserire più di un numero. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:117
-msgid "telefono_persona_help"
-msgstr ""
-
-#. Default: "Numero di telefono"
-#: design/plone/contenttypes/interfaces/persona.py:116
-msgid "telefono_persona_label"
-msgstr ""
-
-#. Default: "Temi"
-#: design/plone/contenttypes/interfaces/dataset.py:14
-msgid "temi"
-msgstr ""
-
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:167
+#: design/plone/contenttypes/interfaces/servizio.py:236
 msgid "tempi_e_scadenze"
 msgstr ""
 
 #. Default: "Descrivere le informazioni dettagliate riguardo eventuali tempi e scadenze di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:169
+#: design/plone/contenttypes/interfaces/servizio.py:238
 msgid "tempi_e_scadenze_help"
 msgstr ""
 
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:395
+#: design/plone/contenttypes/interfaces/servizio.py:508
 msgid "tempi_e_scadenze_label"
 msgstr ""
 
 #. Default: "Inserisci il tempo medio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:91
+#: design/plone/contenttypes/behaviors/trasparenza.py:92
 msgid "tempo_medio_help"
 msgstr ""
 
 #. Default: "Tempo medio del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:86
+#: design/plone/contenttypes/behaviors/trasparenza.py:87
 msgid "tempo_medio_label"
 msgstr ""
 
 #. Default: "Testata"
-#: design/plone/contenttypes/behaviors/argomenti.py:104
+#: design/plone/contenttypes/behaviors/argomenti.py:232
 #: design/plone/contenttypes/behaviors/info_testata.py:62
 msgid "testata_fieldset_label"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:28
+#: design/plone/contenttypes/interfaces/bando.py:29
 msgid "text_help"
 msgstr ""
 
 #. Default: "Testo"
-#: design/plone/contenttypes/interfaces/bando.py:27
+#: design/plone/contenttypes/interfaces/bando.py:28
 msgid "text_label"
 msgstr ""
 
-#. Default: "Tipologia documento"
-#: design/plone/contenttypes/interfaces/messaggio.py:49
-msgid "tipologia_documento"
-msgstr ""
-
-#. Default: "Seleziona la tipologia del documento."
-#: design/plone/contenttypes/interfaces/documento.py:30
-msgid "tipologia_documento_help"
-msgstr ""
-
-#. Default: "Tipologia del documento"
-#: design/plone/contenttypes/interfaces/documento.py:29
-msgid "tipologia_documento_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia della notizia."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:29
-msgid "tipologia_notizia_help"
-msgstr ""
-
-#. Default: "Tipologia notizia"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:28
-msgid "tipologia_notizia_label"
-msgstr ""
-
-#. Default: "Specificare la tipologia di organizzazione: politica, amminsitrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:60
-msgid "tipologia_organizzazione_help"
-msgstr ""
-
-#. Default: "Tipologia organizzazione"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:57
-msgid "tipologia_organizzazione_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia di persona: politica, amministrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/persona.py:86
-msgid "tipologia_persona_help"
-msgstr ""
-
-#. Default: "Tipologia persona"
-#: design/plone/contenttypes/interfaces/persona.py:85
-msgid "tipologia_persona_label"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per le tipologie di un Documento. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:46
-msgid "tipologie_documento_help"
+#. Default: "Timeline tempi e scadenze"
+#: design/plone/contenttypes/interfaces/servizio.py:246
+msgid "timeline_tempi_scadenze"
 msgstr ""
 
-#. Default: "Tipologie Documento"
-#: design/plone/contenttypes/controlpanels/settings.py:45
-msgid "tipologie_documento_label"
+#. Default: "Timeline tempi e scadenze del servizio: indicare per ogni scadenza un titolo descrittivo ed un eventuale sottotitolo. Per ogni scadenza, selezionare opzionalmente o l'intervallo (Campi \"Intervallo\" e \"Tipo Intervallo\", es. \"1\" e \"settimana\"), oppure direttamente una data di scadenza (campo: \"Data Scadenza\", esempio 31/12/2023). Se vengono compilati entrambi, ha priorità il campo \"Data Scadenza\"."
+#: design/plone/contenttypes/interfaces/servizio.py:249
+msgid "timeline_tempi_scadenze_help"
 msgstr ""
 
 #. Default: "Inserisci i valori utilizzabili per le tipologie di una Notizia. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:19
+#: design/plone/contenttypes/controlpanels/settings.py:22
 msgid "tipologie_notizia_help"
 msgstr ""
 
 #. Default: "Tipologie Notizia"
-#: design/plone/contenttypes/controlpanels/settings.py:18
+#: design/plone/contenttypes/controlpanels/settings.py:21
 msgid "tipologie_notizia_label"
 msgstr ""
 
-#. Default: "Inserisci i valori utilizzabili per le tipologie di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:72
-msgid "tipologie_persona_help"
-msgstr ""
-
-#. Default: "Tipologie Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:71
-msgid "tipologie_persona_label"
-msgstr ""
-
 #. Default: "Inserisci i valori utilizzabili per le tipologie di un' Unità Organizzativa. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:34
+#: design/plone/contenttypes/controlpanels/settings.py:37
 msgid "tipologie_unita_organizzativa_help"
 msgstr ""
 
 #. Default: "Tipologie Unità Organizzativa"
-#: design/plone/contenttypes/controlpanels/settings.py:30
+#: design/plone/contenttypes/controlpanels/settings.py:33
 msgid "tipologie_unita_organizzativa_label"
 msgstr ""
 
 #. Default: "Titolare"
-#: design/plone/contenttypes/interfaces/dataset.py:29
+#: design/plone/contenttypes/interfaces/dataset.py:22
 msgid "titolare"
 msgstr ""
 
 #. Default: "Eventuale titolare del potere sostitutivo."
-#: design/plone/contenttypes/behaviors/trasparenza.py:243
+#: design/plone/contenttypes/behaviors/trasparenza.py:244
 msgid "titolare_potere_sostitutivo_help"
 msgstr ""
 
 #. Default: "Titolare del potere sostitutivo"
-#: design/plone/contenttypes/behaviors/trasparenza.py:238
+#: design/plone/contenttypes/behaviors/trasparenza.py:239
 msgid "titolare_potere_sostitutivo_label"
 msgstr ""
 
 #. Default: "Trasparenza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:292
+#: design/plone/contenttypes/behaviors/trasparenza.py:291
 msgid "trasparenza_fieldset_label"
 msgstr ""
 
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:17
+msgid "type_help"
+msgstr ""
+
 #. Default: "Seleziona l'ufficio responsabile di questo bando."
-#: design/plone/contenttypes/interfaces/bando.py:110
+#: design/plone/contenttypes/interfaces/bando.py:111
 msgid "ufficio_responsabile_bando_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del bando"
-#: design/plone/contenttypes/interfaces/bando.py:106
+#: design/plone/contenttypes/interfaces/bando.py:107
 msgid "ufficio_responsabile_bando_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio responsabile di questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:43
+#: design/plone/contenttypes/interfaces/documento.py:73
 msgid "ufficio_responsabile_documento_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del documento"
-#: design/plone/contenttypes/interfaces/documento.py:39
+#: design/plone/contenttypes/interfaces/documento.py:69
 msgid "ufficio_responsabile_documento_label"
 msgstr ""
 
 #. Default: "Ufficio responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:62
 msgid "ufficio_responsabile_documento_personale"
 msgstr ""
 
-#. Default: "Uffici responsabili"
-#: design/plone/contenttypes/interfaces/servizio.py:216
+#. Default: "Unità organizzativa responsabile"
+#: design/plone/contenttypes/interfaces/servizio.py:302
 msgid "ufficio_responsabile_erogazione"
 msgstr ""
 
 #. Default: "Seleziona gli uffici responsabili dell'erogazione di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:217
+#: design/plone/contenttypes/interfaces/servizio.py:306
 msgid "ufficio_responsabile_help"
 msgstr ""
 
 #. Default: "Ufficio di riferimento"
 #: design/plone/contenttypes/interfaces/pratica.py:17
 msgid "ufficio_riferimento"
 msgstr ""
@@ -2657,56 +2652,56 @@
 msgstr ""
 
 #. Default: "Seleziona la lista delle unità amministrative responsabili di questo argomento."
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:48
 msgid "unita_amministrative_responsabili_help"
 msgstr ""
 
+#. Default: "Seleziona l'organizzazione presso la quale svolge l'incarico."
+#: design/plone/contenttypes/interfaces/incarico.py:64
+msgid "unita_organizzativa_incarico_help"
+msgstr ""
+
+#. Default: "Unità organizzativa"
+#: design/plone/contenttypes/interfaces/incarico.py:60
+msgid "unita_organizzativa_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione dei compiti assegnati alla struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:19
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:23
 msgid "uo_competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:18
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:22
 msgid "uo_competenze_label"
 msgstr ""
 
-#. Default: "Inserisci eventuali informazioni di contatto aggiuntive non contemplate nei campi precedenti. Utilizza questo campo se ci sono dei contatti aggiuntivi rispetto ai contatti della sede principale. Se inserisci un collegamento con un indirizzo email, aggiungi \"mailto:\" prima dell'indirizzo, per farlo aprire direttamente nel client di posta."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:139
-msgid "uo_contact_info_description"
-msgstr ""
-
 #. Default: "Note di aggiornamento"
-#: design/plone/contenttypes/behaviors/update_note.py:16
+#: design/plone/contenttypes/behaviors/update_note.py:17
 msgid "update_note_label"
 msgstr ""
 
+#. Default: "Il valore del punto di contatto: il numero compreso di prefisso internazionale (se telefono), l'account (se social network), l'URL (se sito o pagina web), l'indirizzo email (se email)."
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:54
+msgid "value_punto_contatto_help"
+msgstr ""
+
 #. Default: "Vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:196
+#: design/plone/contenttypes/interfaces/servizio.py:282
 msgid "vincoli"
 msgstr ""
 
 #. Default: "Descrizione degli eventuali vincoli presenti."
-#: design/plone/contenttypes/interfaces/servizio.py:198
+#: design/plone/contenttypes/interfaces/servizio.py:284
 msgid "vincoli_help"
 msgstr ""
 
-#. Default: "Indicare un indirizzo web di riferimento a questo evento."
-#: design/plone/contenttypes/behaviors/evento.py:138
-msgid "web_event_help"
-msgstr ""
-
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/evento.py:137
-msgid "web_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo web di riferimento."
-#: design/plone/contenttypes/behaviors/contatti.py:53
-msgid "web_help"
+#. Default: "Mostra i PDF in anteprima"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:12
+msgid "visualize_files_title"
 msgstr ""
 
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/contatti.py:52
-msgid "web_label"
+#. Default: "Permette di aprire l'anteprima di tutti i PDF di questa cartella in una tab separata, altrimenti i PDF vengono scaricati"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:13
+msgid "visulize_files_description"
 msgstr ""
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,506 +1,491 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-01-13 13:15+0000\n"
+"POT-Creation-Date: 2024-03-18 13:30+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
-msgid "Abitazione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:36
-msgid "Accesso al trasporto pubblico"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:59
-msgid "Accesso luoghi della cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:18
+msgid "Accesso all'informazione"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:33
 msgid "Accettare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:34
-msgid "Accordo tra enti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:19
 msgid "Acqua"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
+#: design/plone/contenttypes/behaviors/configure.zcml:223
 msgid "Address Event"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Address UO"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:186
+#: design/plone/contenttypes/behaviors/configure.zcml:215
 msgid "Address Venue"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:19
 msgid "Adds fields."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:28
-msgid "Agricoltura, pesca, silvicoltura e prodotti alimentari"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:22
-msgid "All the already existing News Types"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "After Plone6 migration syndication is broken"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:63
-msgid "All the selected items will be moved to indicated path"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:20
+msgid "Agricoltura"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:20
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:30
 msgid "All the already existing News Types"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:36
-msgid "Ambiente"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:113
+msgid "All the selected items will be moved to indicated path"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:21
 msgid "Animale domestico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
-msgid "Anziano"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/bando.py:134
-#: design/plone/contenttypes/interfaces/documento.py:67
-#: design/plone/contenttypes/interfaces/servizio.py:239
+#: design/plone/contenttypes/interfaces/bando.py:135
+#: design/plone/contenttypes/interfaces/documento.py:97
+#: design/plone/contenttypes/interfaces/servizio.py:328
 msgid "Area"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
-msgid "Area di parcheggio"
-msgstr ""
-
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Argomenti"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:76
+#: design/plone/contenttypes/behaviors/configure.zcml:94
 msgid "Argomenti Bando"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:58
+#: design/plone/contenttypes/behaviors/configure.zcml:76
 msgid "Argomenti Document"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:67
+#: design/plone/contenttypes/behaviors/configure.zcml:85
 msgid "Argomenti Documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:28
+#: design/plone/contenttypes/behaviors/configure.zcml:112
+msgid "Argomenti Link"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/argomenti.py:32
 msgid "Argomenti correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
 msgid "Argomento"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:73
+#: design/plone/contenttypes/behaviors/configure.zcml:103
+msgid "Argomento Servizio"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:22
+msgid "Aria"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:65
 msgid "Assessore di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
-msgid "Associazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:23
+msgid "Assistenza agli invalidi"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:24
+msgid "Assistenza sociale"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
+msgid "Associazioni"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:29
 msgid "Attivare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:33
-msgid "Atto normativo"
+#: design/plone/contenttypes/interfaces/incarico.py:121
+msgid "Atto di nomina"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:86
 msgid "Autore"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:30
 msgid "Autorizzare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:65
-msgid "Avvio impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:66
-msgid "Avvio nuova attività professionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:69
-msgid "Avvio/registrazione filiale"
+#: design/plone/contenttypes/behaviors/configure.zcml:223
+msgid "Behavior address per Event."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:78
-msgid "Bancarotta"
+#: design/plone/contenttypes/behaviors/configure.zcml:215
+msgid "Behavior address per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
-msgid "Behavior address per Event."
+#: design/plone/contenttypes/behaviors/configure.zcml:263
+msgid "Behavior contatti per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Behavior address per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:255
+msgid "Behavior contatti per Persona."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:186
-msgid "Behavior address per Venue."
+#: design/plone/contenttypes/behaviors/configure.zcml:247
+msgid "Behavior contatti per Servizio."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
 msgid "Behavior contatti per UO."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:210
+#: design/plone/contenttypes/behaviors/configure.zcml:239
 msgid "Behavior contatti per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:234
+#: design/plone/contenttypes/behaviors/configure.zcml:279
 msgid "Behavior geolocatable per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
-msgid "Behavior geolocatable per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:271
+msgid "Behavior geolocatable per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:226
-msgid "Behavior geolocatable per Venue."
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
+msgid "Bilancio"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:18
 msgid "CAP"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:43
-msgid "Cambio di residenza/domicilio"
+#: design/plone/contenttypes/behaviors/configure.zcml:306
+msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:261
-msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Campo per escludere un contenuto dalle ricerche del sito."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
+#: design/plone/contenttypes/behaviors/configure.zcml:315
 msgid "Campo per le note di aggiornamento."
 msgstr ""
 
+#: design/plone/contenttypes/interfaces/servizio.py:183
+msgid "Canale fisico"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:26
 msgid "Canon 5D IV"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 msgid "Cartella Modulistica"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:11
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:13
 msgid "Change News Type"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:75
-msgid "Chiusura filiale"
+#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
+msgid "Città"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:74
-msgid "Chiusura impresa e attività professionale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
+msgid "Commercio al minuto"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
-msgid "Città"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
+msgid "Commercio all'ingrosso"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:39
-msgid "Compravendita/affitto casa/edifici/terreni, costruzione o ristrutturazione casa/edificio	"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
+msgid "Commercio ambulante"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
-msgid "Comunicazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
+msgid "Comunicazione istituzionale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
-msgid "Condizioni e organizzazione del lavoro"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+msgid "Comunicazione politica"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:57
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
+msgid "Concorsi"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:104
 msgid "Contained by"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
+#: design/plone/contenttypes/behaviors/contatti.py:112
 msgid "Contatti"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:33
 msgid "Coordinate"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:42
+#: design/plone/contenttypes/behaviors/argomenti.py:46
 msgid "Correlato in evidenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
-msgid "Cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+msgid "Covid - 19"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:130
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 msgid "Dataset"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:134
 msgid "Dataset collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:104
+#: design/plone/contenttypes/behaviors/configure.zcml:141
 msgid "Dataset correlati"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:31
 msgid "Delegare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:52
-msgid "Denuncia crimini"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:143
+#: design/plone/contenttypes/behaviors/configure.zcml:180
 msgid "Descrizione estesa"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:160
+#: design/plone/contenttypes/behaviors/configure.zcml:197
 msgid "Descrizione estesa documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:152
+#: design/plone/contenttypes/behaviors/configure.zcml:189
 msgid "Descrizione estesa servizio"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Design Plone: Content-types"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Design Plone: Content-types (behaviors)"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Design Plone: Content-types (uninstall)"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Design Plone: Content-types to 3000"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:55
-msgid "Dichiarazione dei redditi, versamento e riscossione tributi/imposte e contributi"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "Design Plone: Fix Syndication after Plone6 Migration"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:145
+#: design/plone/contenttypes/behaviors/trasparenza.py:146
 msgid "Dirigente"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:27
-msgid "Documenti albo pretorio"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:134
+msgid "Documenti pubblici"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/servizio.py:252
+#: design/plone/contenttypes/interfaces/servizio.py:341
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Documento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:41
-msgid "Documento (tecnico) di supporto"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
 msgid "Documento Personale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:37
-msgid "Documento attivita politica"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:31
-msgid "Documento funzionamento interno"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:30
-msgid "Economia e Finanze"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Edit"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
-msgid "Elezione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:35
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
-msgid "Energia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+msgid "Elezioni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
-msgid "Famiglia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
+msgid "Energie rinnovabili"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
-msgid "Fanciullo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
+msgid "Estero"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:70
-msgid "Finanziamento impresa"
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Exclude from search"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:28
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:51
 msgid "Find news with the indicated Path, put attention than generaly sites have the root name \"/Plone/\""
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:21
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:29
 msgid "Find news with this News Type"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Fix control panel of design.plone.contenttypes add-on."
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
+msgid "Foreste"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/tags_vocabulary.py:38
 msgid "Formazione professionale"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:39
+msgid "Gemellaggi"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:271
 msgid "Geolocatable"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:43
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Geolocation default"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
-msgid "Gestione dei rifiuti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:71
-msgid "Gestione personale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
-msgid "Giovane"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:40
+msgid "Gestione rifiuti"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:30
 msgid "Giovanni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:42
-msgid "Giustizia, sistema giuridico e sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
+msgid "Giustizia"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:37
-msgid "Governo e settore pubblico"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:42
+msgid "Igiene pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+#: design/plone/contenttypes/browser/utils/change_news_type.py:32
+#: design/plone/contenttypes/browser/utils/move_news_items.py:74
+msgid "Il vocabolario dei valori non è stato trovato"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
 msgid "Immigrazione"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/settings.py:154
+#: design/plone/contenttypes/controlpanels/settings.py:106
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Impostazioni Design Plone"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+msgid "Imposte"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
+msgid "Imprese"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/persona.py:68
+msgid "Incarichi"
+msgstr ""
+
+#: design/plone/contenttypes/profiles/default/types/Incarico.xml
+msgid "Incarico"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/move_news_items.py:34
 msgid "Indicated path is not valid"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:170
+#: design/plone/contenttypes/behaviors/configure.zcml:207
 msgid "Info per la testata"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:32
 msgid "Informare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
-msgid "Informatica e trattamento dei dati"
+#: design/plone/contenttypes/behaviors/contatti.py:34
+msgid "Informazioni di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
 msgid "Inquinamento"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Installs the design.plone.contenttypes add-on."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
 msgid "Integrazione sociale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:28
-msgid "Invalidità"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:26
 msgid "Iscriversi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:26
-msgid "Iscrizione scuola/università e/o richiesta borsa di studio"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:43
-msgid "Istanza"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+msgid "Isolamento termico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
 msgid "Istruzione"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:33
-msgid "Istruzione, cultura e sport"
+#: design/plone/contenttypes/browser/utils/move_news_items.py:48
+msgid "Items moved with success"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:47
-msgid "Items moved with success"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
+msgid "Lavoro"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:28
 msgid "Leggere"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:85
+#: design/plone/contenttypes/behaviors/configure.zcml:122
 msgid "Luoghi correlati"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
 msgid "Matrimonio"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:49
-msgid "Matrimonio e/o cambio stato civile"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+msgid "Mercato"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Messaggio.xml
 msgid "Messaggio"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:29
@@ -511,529 +496,536 @@
 msgid "Metadati luogo"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:39
 msgid "Metadati news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:28
-msgid "Modulistica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
+msgid "Mobilità sostenibile"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Modulo"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:50
-msgid "Morte ed eredità"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
+msgid "Morte"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Mostra la data di modifica."
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:70
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:124
 msgid "Move"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:11
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:13
 msgid "Move News Items"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:62
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:110
 msgid "Move to Path"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Multi File"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:48
-msgid "Nascita di un bambino, richiesta adozioni"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
+msgid "Nascita"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:28
 msgid "Nazione"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:21
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:20
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:26
 msgid "News Type"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:30
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:48
 msgid "News Type to substitute"
 msgstr ""
 
 #. Default: "Nome e cognome"
-#: design/plone/contenttypes/restapi/services/types/get.py:152
+#: design/plone/contenttypes/restapi/services/types/get.py:163
 msgid "Nome e Cognome"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:73
-msgid "Notifiche autorità"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/persona.py:48
+#: design/plone/contenttypes/interfaces/persona.py:51
 msgid "Organizzazione di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:72
-msgid "Pagamento tasse, iva e dogane"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:25
 msgid "Pagare"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:29
 msgid "Paperino"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:81
-msgid "Partecipazione ad appalti pubblici nazionali e trasfrontalieri"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
+msgid "Parcheggi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:33
-msgid "Pensionamento"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
+msgid "Patrimonio culturale"
 msgstr ""
 
-#: design/plone/contenttypes/profiles/default/types/Persona.xml
+#: design/plone/contenttypes/interfaces/incarico.py:54
 msgid "Persona"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/evento.py:50
-msgid "Persona dell'amministrazione"
+#: design/plone/contenttypes/profiles/default/types/Persona.xml
+msgid "Persona pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:92
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:84
 msgid "Persone della struttura"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+msgid "Pesca"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
+msgid "Piano di sviluppo"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:27
 msgid "Pippo"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+msgid "Pista ciclabile"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:28
 msgid "Pluto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:45
-msgid "Popolazione e società"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
+msgid "Politica commerciale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:60
-msgid "Possesso, cura, smarrimento animale da compagnia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:62
+msgid "Polizia"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pratica.xml
 msgid "Pratica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:51
-msgid "Prenotazione e disdetta visite/esami"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:63
+msgid "Prodotti alimentari"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
-msgid "Protezione sociale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
+msgid "Protezione civile"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:13
-msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
+#: design/plone/contenttypes/behaviors/contatti.py:78
+msgid "Punti di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:13
-msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
+#: design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+msgid "Punto di Contatto"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:15
+msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:44
-msgid "Regioni e città"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:15
+msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:68
-msgid "Registrazione impresa transfrontalier"
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Registers taxonomies."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:35
-msgid "Registrazione/possesso veicolo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:65
+msgid "Residenza"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:45
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:49
 msgid "Responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:129
-msgid "Responsabile procedimento"
+#: design/plone/contenttypes/interfaces/incarico.py:89
+msgid "Responsabile della struttura"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:31
-msgid "Ricerca di lavoro, avvio nuovo lavoro, disoccupazione"
+#: design/plone/contenttypes/behaviors/trasparenza.py:130
+msgid "Responsabile procedimento"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
 msgid "RicevutaPagamento"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:27
 msgid "Richiedere"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:67
-msgid "Richiesta licenze/permessi/certificati"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:34
-msgid "Richiesta o rinnovo patente"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:46
-msgid "Richiesta passaporto, visto e assistenza viaggi internazionali"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:66
+msgid "Risposta alle emergenze"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:76
-msgid "Ristrutturazione impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:38
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
-msgid "Salute"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:46
-msgid "Scienza e tecnologia"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:47
 msgid "Search Path"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:114
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:104
 msgid "Sede"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:114
+#: design/plone/contenttypes/behaviors/configure.zcml:151
 msgid "Servizi correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Servizio.xml
 msgid "Servizio"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:101
 msgid "Servizio collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Show modified"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
-msgid "Sicurezza internazionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
-msgid "Sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:67
+msgid "Sistema giuridico"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:25
 msgid "Sony Aplha 7R III"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
-msgid "Spazio verde"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:68
+msgid "Spazio Verde"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:69
 msgid "Sport"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:37
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:41
 msgid "Struttura"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:20
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:21
 msgid "Struttura politica coinvolta"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/luogo.py:74
+#: design/plone/contenttypes/behaviors/luogo.py:75
 msgid "Struttura responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:124
+#: design/plone/contenttypes/behaviors/configure.zcml:161
 msgid "Strutture correlate"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
-msgid "Studente"
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:74
+msgid "Substitute"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:43
-msgid "Substitute"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:70
+msgid "Sviluppo sostenibile"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:71
+msgid "Tassa sui servizi"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Tassonomia argomenti"
 msgstr ""
 
+#: design/plone/contenttypes/behaviors/configure.zcml:67
+msgid "Tassonomia argomenti evento"
+msgstr ""
+
 #: design/plone/contenttypes/behaviors/configure.zcml:58
-msgid "Tassonomia argomenti per i Document"
+msgid "Tassonomia argomenti news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:39
-msgid "Tematiche internazionali"
+#: design/plone/contenttypes/behaviors/configure.zcml:76
+msgid "Tassonomia argomenti per i Document"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:72
 msgid "Tempo libero"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:31
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:52
 msgid "The News Type selected above will be substituted by the selected value"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:97
+#: design/plone/contenttypes/browser/utils/change_news_type.py:108
 msgid "The News Types was changed with success"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:55
+#: design/plone/contenttypes/browser/utils/change_news_type.py:64
 msgid "The new News Type was not found between available values"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:49
+#: design/plone/contenttypes/browser/utils/change_news_type.py:58
 msgid "The new type field was not populated"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:61
+#: design/plone/contenttypes/browser/utils/change_news_type.py:70
 msgid "The old News Type was not found between available values"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:43
+#: design/plone/contenttypes/browser/utils/change_news_type.py:52
 msgid "The old type field was not populated"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:51
+#: design/plone/contenttypes/browser/utils/move_news_items.py:52
 msgid "The path was not indicated"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
-msgid "Traffico urbano"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:261
+#: design/plone/contenttypes/behaviors/configure.zcml:306
 msgid "Trasparenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
-msgid "Trasporto"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:73
+msgid "Trasparenza amministrativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
-msgid "Trasporto stradale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:74
+msgid "Trasporto pubblico"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Tre campi file aggiuntivi."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:75
 msgid "Turismo"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:117
-#: design/plone/contenttypes/interfaces/documento.py:50
-#: design/plone/contenttypes/interfaces/servizio.py:225
+#: design/plone/contenttypes/interfaces/bando.py:118
+#: design/plone/contenttypes/interfaces/documento.py:80
 msgid "Ufficio responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:134
+#: design/plone/contenttypes/behaviors/configure.zcml:171
 msgid "Ulteriori campi aiuto testuali"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Un modulo compilabile."
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:15
+msgid "Una raccolta di utility per i contenuti agid"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Uninstalls the design.plone.contenttypes add-on."
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
 msgid "Unita Organizzativa"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:45
 msgid "Unità amministrative responsabili"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
-msgid "Update note"
+#: design/plone/contenttypes/interfaces/incarico.py:71
+msgid "Unità organizzativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
-msgid "Urbanistica ed edilizia"
+#: design/plone/contenttypes/interfaces/servizio.py:314
+msgid "Unità organizzativa responsabile"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:315
+msgid "Update note"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:77
-msgid "Vendita impresa"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:76
+msgid "Urbanizzazione"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:13
 msgid "Via"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:77
+msgid "Viaggi"
+msgstr ""
+
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "View"
 msgstr ""
 
-#. Default: "A chi si rivolge questo servizio e chi può usufruirne."
-#: design/plone/contenttypes/interfaces/servizio.py:53
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:13
+msgid "Viste di utility per Design Plone Contenttypes"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:79
+msgid "ZTL"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:78
+msgid "Zone pedonali"
+msgstr ""
+
+#. Default: "Descrizione testuale dei principali destinatari dell'Evento"
+#: design/plone/contenttypes/behaviors/evento.py:43
+#: design/plone/contenttypes/interfaces/servizio.py:98
 msgid "a_chi_si_rivolge_help"
 msgstr ""
 
-#. Default: "A chi si rivolge"
-#: design/plone/contenttypes/interfaces/servizio.py:51
+#. Default: "A chi è rivolto"
+#: design/plone/contenttypes/behaviors/evento.py:41
+#: design/plone/contenttypes/interfaces/servizio.py:96
 msgid "a_chi_si_rivolge_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio di comunicazione responsabile di questa notizia/comunicato stampa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:47
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:39
 msgid "a_cura_di_help"
 msgstr ""
 
 #. Default: "A cura di"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:46
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
 msgid "a_cura_di_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di persone dell'amministrazione citate in questa notizia/comunicato stampa. Questa informazione verrà mostrata nella sezione \"A cura di\"."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:59
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:51
 msgid "a_cura_di_persone_help"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:58
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:50
 msgid "a_cura_di_persone_label"
 msgstr ""
 
 #. Default: "Accedere al servizio"
-#: design/plone/contenttypes/interfaces/servizio.py:370
+#: design/plone/contenttypes/interfaces/servizio.py:481
 msgid "accedi_al_servizio_label"
 msgstr ""
 
 #. Default: "Modalità di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:171
+#: design/plone/contenttypes/behaviors/luogo.py:140
 msgid "accesso_label"
 msgstr ""
 
 #. Default: "Allegato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:56
 msgid "allegato"
 msgstr ""
 
 #. Default: "Indicare, se esistono, altre modalità di invio."
-#: design/plone/contenttypes/behaviors/trasparenza.py:189
+#: design/plone/contenttypes/behaviors/trasparenza.py:190
 msgid "altre_modalita_invio_help"
 msgstr ""
 
 #. Default: "Altre modalità di invio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:185
+#: design/plone/contenttypes/behaviors/trasparenza.py:186
 msgid "altre_modalita_invio_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei documenti di supporto collegati a questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:246
+#: design/plone/contenttypes/interfaces/servizio.py:335
 msgid "altri_documenti_help"
 msgstr ""
 
 #. Default: "Date and time of the opening of the announcement. Use this field if you want to set a specific opening date. If not set, the announcement will be open immediately."
-#: design/plone/contenttypes/interfaces/bando.py:56
+#: design/plone/contenttypes/interfaces/bando.py:57
 msgid "apertura_bando_help"
 msgstr ""
 
 #. Default: "Opening date"
-#: design/plone/contenttypes/interfaces/bando.py:55
+#: design/plone/contenttypes/interfaces/bando.py:56
 msgid "apertura_bando_label"
 msgstr ""
 
 #. Default: "Area"
-#: design/plone/contenttypes/interfaces/servizio.py:231
+#: design/plone/contenttypes/interfaces/servizio.py:320
 msgid "area"
 msgstr ""
 
 #. Default: "Seleziona l'area da cui dipende questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:234
+#: design/plone/contenttypes/interfaces/servizio.py:323
 msgid "area_help"
 msgstr ""
 
 #. Default: "Area responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:73
 msgid "area_responsabile_documento_personale"
 msgstr ""
 
 #. Default: "Seleziona l'area amministrativa responsabile del documento."
-#: design/plone/contenttypes/interfaces/bando.py:127
-#: design/plone/contenttypes/interfaces/documento.py:60
+#: design/plone/contenttypes/interfaces/bando.py:128
+#: design/plone/contenttypes/interfaces/documento.py:90
 msgid "area_responsabile_help"
 msgstr ""
 
 #. Default: "Area responsabile del documento"
-#: design/plone/contenttypes/interfaces/bando.py:123
-#: design/plone/contenttypes/interfaces/documento.py:56
+#: design/plone/contenttypes/interfaces/bando.py:124
+#: design/plone/contenttypes/interfaces/documento.py:86
 msgid "area_responsabile_label"
 msgstr ""
 
 #. Default: "Argomenti utenti"
 #: design/plone/contenttypes/interfaces/documento_personale.py:42
 msgid "argomenti_utenti"
 msgstr ""
 
 #. Default: "Inserire l'assessore di riferimento della struttura, se esiste."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:76
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:68
 msgid "assessore_riferimento_help"
 msgstr ""
 
+#. Default: "Assessore di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:61
+msgid "assessore_riferimento_title"
+msgstr ""
+
 #. Default: "Indicare, se la esistono, atti e documenti a corredo dell'istanza."
-#: design/plone/contenttypes/behaviors/trasparenza.py:200
+#: design/plone/contenttypes/behaviors/trasparenza.py:201
 msgid "atti_documenti_corredo_help"
 msgstr ""
 
 #. Default: "Atti e documenti a corredo dell'istanza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:196
+#: design/plone/contenttypes/behaviors/trasparenza.py:197
 msgid "atti_documenti_corredo_label"
 msgstr ""
 
-#. Default: "Inserire un file contenente l'atto di nomina della persona."
-#: design/plone/contenttypes/interfaces/persona.py:160
-msgid "atto_nomina_help"
+#. Default: "Inserire riferimento all'atto di nomina della persona"
+#: design/plone/contenttypes/interfaces/incarico.py:114
+msgid "atto_nomina_incarico_help"
 msgstr ""
 
 #. Default: "Atto di nomina"
-#: design/plone/contenttypes/interfaces/persona.py:158
-msgid "atto_nomina_label"
-msgstr ""
-
-#. Default: "Autenticazione"
-#: design/plone/contenttypes/interfaces/servizio.py:121
-msgid "autenticazione"
-msgstr ""
-
-#. Default: "Indicare, se previste, le modalità di autenticazione necessarie per poter accedere al servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:122
-msgid "autenticazione_help"
+#: design/plone/contenttypes/interfaces/incarico.py:110
+msgid "atto_nomina_incarico_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di autori che hanno pubblicato il documento. Possono essere Persone o Unità Organizzative."
-#: design/plone/contenttypes/interfaces/documento.py:76
+#: design/plone/contenttypes/interfaces/documento.py:106
 msgid "autori_help"
 msgstr ""
 
 #. Default: "Autore/i"
-#: design/plone/contenttypes/interfaces/documento.py:72
+#: design/plone/contenttypes/interfaces/documento.py:102
 msgid "autori_label"
 msgstr ""
 
 #. Default: "Azioni"
 #: design/plone/contenttypes/interfaces/messaggio.py:28
 msgid "azioni_pratica"
 msgstr ""
@@ -1045,662 +1037,688 @@
 
 #. Default: "Azioni utente"
 #: design/plone/contenttypes/interfaces/pratica.py:47
 msgid "azioni_utente"
 msgstr ""
 
 #. Default: "Solo per persona politica: testo descrittivo che riporta la biografia della persona."
-#: design/plone/contenttypes/interfaces/persona.py:107
+#: design/plone/contenttypes/interfaces/persona.py:94
 msgid "biografia_help"
 msgstr ""
 
 #. Default: "Biografia"
-#: design/plone/contenttypes/interfaces/persona.py:106
+#: design/plone/contenttypes/interfaces/persona.py:93
 msgid "biografia_label"
 msgstr ""
 
 #. Default: "Canale digitale"
-#: design/plone/contenttypes/interfaces/servizio.py:111
+#: design/plone/contenttypes/interfaces/servizio.py:156
 msgid "canale_digitale"
 msgstr ""
 
-#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:112
+#. Default: "Testo di introduzione del canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:157
 msgid "canale_digitale_help"
 msgstr ""
 
+#. Default: "Link al canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:165
+msgid "canale_digitale_link"
+msgstr ""
+
+#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
+#: design/plone/contenttypes/interfaces/servizio.py:166
+msgid "canale_digitale_link_help"
+msgstr ""
+
 #. Default: "Canale digitale servizio collegato"
 #: design/plone/contenttypes/interfaces/documento_personale.py:108
 msgid "canale_digitale_servizio"
 msgstr ""
 
+#. Default: "Canale fisico"
+#: design/plone/contenttypes/interfaces/servizio.py:175
+msgid "canale_fisico"
+msgstr ""
+
+#. Default: "Unità organizzative per la fruizione del servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:176
+msgid "canale_fisico_help"
+msgstr ""
+
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:205
+#: design/plone/contenttypes/interfaces/servizio.py:291
 msgid "casi_particolari"
 msgstr ""
 
 #. Default: "Descrizione degli evetuali casi particolari riferiti alla fruibilità di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:207
+#: design/plone/contenttypes/interfaces/servizio.py:293
 msgid "casi_particolari_help"
 msgstr ""
 
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:401
+#: design/plone/contenttypes/interfaces/servizio.py:514
 msgid "casi_particolari_label"
 msgstr ""
 
 #. Default: "Descrizione di chi può presentare domanda per usufruire del servizio e delle diverse casistiche."
-#: design/plone/contenttypes/interfaces/servizio.py:62
+#: design/plone/contenttypes/interfaces/servizio.py:107
 msgid "chi_puo_presentare_help"
 msgstr ""
 
 #. Default: "Chi può presentare"
-#: design/plone/contenttypes/interfaces/servizio.py:60
+#: design/plone/contenttypes/interfaces/servizio.py:105
 msgid "chi_puo_presentare_label"
 msgstr ""
 
 #. Default: "Circoscrizione"
 #: design/plone/contenttypes/behaviors/address.py:37
 msgid "circoscrizione"
 msgstr ""
 
 #. Default: "Codice dell'ente erogatore (ipa)"
-#: design/plone/contenttypes/interfaces/servizio.py:268
+#: design/plone/contenttypes/interfaces/servizio.py:357
 msgid "codice_ipa"
 msgstr ""
 
 #. Default: "Specificare il nome dell’organizzazione, come indicato nell’Indice della Pubblica Amministrazione (IPA), che esercita uno specifico ruolo sul Servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:270
+#: design/plone/contenttypes/interfaces/servizio.py:359
 msgid "codice_ipa_help"
 msgstr ""
 
-#. Default: "Come si fa"
-#: design/plone/contenttypes/interfaces/servizio.py:80
+#. Default: "Come fare"
+#: design/plone/contenttypes/interfaces/servizio.py:125
 msgid "come_si_fa"
 msgstr ""
 
 #. Default: "Descrizione della procedura da seguire per poter usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:82
+#: design/plone/contenttypes/interfaces/servizio.py:127
 msgid "come_si_fa_help"
 msgstr ""
 
+#. Default: "Solo per incarico politico: compensi di qualsiasi natura connessi all'assunzione della carica."
+#: design/plone/contenttypes/interfaces/incarico.py:21
+msgid "compensi_incarico_help"
+msgstr ""
+
+#. Default: "Compensi"
+#: design/plone/contenttypes/interfaces/incarico.py:17
+msgid "compensi_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione del ruolo e dei compiti della persona."
-#: design/plone/contenttypes/interfaces/persona.py:69
+#: design/plone/contenttypes/interfaces/persona.py:77
 msgid "competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/persona.py:68
+#: design/plone/contenttypes/interfaces/persona.py:76
 msgid "competenze_label"
 msgstr ""
 
-#. Default: "Informazioni di contatto generiche"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:137
+#. Default: "Condizioni di servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:388
+msgid "condizioni_di_servizio"
+msgstr ""
+
+#. Default: "Contatti dell'unità organizzativa."
+#: design/plone/contenttypes/behaviors/contatti.py:27
+msgid "contact_info_help"
+msgstr ""
+
+#. Default: "Punti di contatto dell'unità organizzativa"
+#: design/plone/contenttypes/behaviors/contatti.py:23
 msgid "contact_info_label"
 msgstr ""
 
 #. Default: "Contatti"
 #: design/plone/contenttypes/interfaces/pratica.py:44
 msgid "contatti"
 msgstr ""
 
 #. Default: "Contatti"
-#: design/plone/contenttypes/behaviors/address.py:52
-#: design/plone/contenttypes/behaviors/contatti.py:76
-#: design/plone/contenttypes/behaviors/evento.py:215
+#: design/plone/contenttypes/behaviors/contatti.py:57
+#: design/plone/contenttypes/behaviors/evento.py:170
+#: design/plone/contenttypes/behaviors/geolocation.py:18
 msgid "contatti_label"
 msgstr ""
 
 #. Default: "Contenuto"
 #: design/plone/contenttypes/interfaces/pratica.py:42
 msgid "contenuto"
 msgstr ""
 
 #. Default: "Indicare se il servizio si riferisce ad una particolare area geografica o all'intero territorio di riferimento."
-#: design/plone/contenttypes/interfaces/servizio.py:72
+#: design/plone/contenttypes/interfaces/servizio.py:117
 msgid "copertura_geografica_help"
 msgstr ""
 
 #. Default: "Copertura geografica"
-#: design/plone/contenttypes/interfaces/servizio.py:70
+#: design/plone/contenttypes/interfaces/servizio.py:115
 msgid "copertura_geografica_label"
 msgstr ""
 
 #. Default: "Contenuti collegati"
-#: design/plone/contenttypes/behaviors/argomenti.py:74
+#: design/plone/contenttypes/behaviors/argomenti.py:108
 #: design/plone/contenttypes/behaviors/dataset_correlati.py:40
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:43
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:120
 msgid "correlati_label"
 msgstr ""
 
 #. Default: "Seleziona un correlato da mettere in evidenza per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:36
+#: design/plone/contenttypes/behaviors/argomenti.py:40
 msgid "correlato_in_evidenza_help"
 msgstr ""
 
 #. Default: "Correlato in evidenza"
-#: design/plone/contenttypes/behaviors/argomenti.py:35
+#: design/plone/contenttypes/behaviors/argomenti.py:39
 msgid "correlato_in_evidenza_label"
 msgstr ""
 
-#. Default: "Cosa fa"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
+#. Default: "Competenze"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:201
 msgid "cosa_fa_label"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:177
+#: design/plone/contenttypes/interfaces/servizio.py:263
 msgid "cosa_serve"
 msgstr ""
 
 #. Default: "Descrizione delle istruzioni per usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:179
+#: design/plone/contenttypes/interfaces/servizio.py:265
 msgid "cosa_serve_help"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:384
+#: design/plone/contenttypes/interfaces/servizio.py:497
 msgid "cosa_serve_label"
 msgstr ""
 
 #. Default: "Cosa si ottiene"
-#: design/plone/contenttypes/interfaces/servizio.py:90
+#: design/plone/contenttypes/interfaces/servizio.py:135
 msgid "cosa_si_ottiene"
 msgstr ""
 
 #. Default: "Indicare cosa si può ottenere dal servizio, ad esempio 'carta di identità elettronica', 'certificato di residenza'."
-#: design/plone/contenttypes/interfaces/servizio.py:91
+#: design/plone/contenttypes/interfaces/servizio.py:136
 msgid "cosa_si_ottiene_help"
 msgstr ""
 
 #. Default: "Cos'è"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:40
-#: design/plone/contenttypes/behaviors/evento.py:200
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:52
+#: design/plone/contenttypes/behaviors/evento.py:155
 msgid "cose_label"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/interfaces/servizio.py:186
+#: design/plone/contenttypes/interfaces/servizio.py:272
 msgid "costi"
 msgstr ""
 
 #. Default: "Costi e vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:389
+#: design/plone/contenttypes/interfaces/servizio.py:502
 msgid "costi_e_vincoli_label"
 msgstr ""
 
 #. Default: "Descrizione delle condizioni e dei termini economici per completare la procedura di richiesta del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:188
+#: design/plone/contenttypes/interfaces/servizio.py:274
 msgid "costi_help"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/behaviors/evento.py:212
+#: design/plone/contenttypes/behaviors/evento.py:167
 msgid "costi_label"
 msgstr ""
 
 #. Default: "Allega un file contenente il curriculum vitae della persona. Se ha più file da allegare, utilizza questo campo per quello principale e gli altri mettili dentro alla cartella \"Curriculum vitae\" che troverai dentro alla Persona."
-#: design/plone/contenttypes/interfaces/persona.py:149
+#: design/plone/contenttypes/interfaces/persona.py:105
 msgid "curriculum_vitae_help"
 msgstr ""
 
 #. Default: "Curriculum vitae"
-#: design/plone/contenttypes/interfaces/persona.py:147
+#: design/plone/contenttypes/interfaces/persona.py:103
 msgid "curriculum_vitae_label"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction."
-#: design/plone/contenttypes/behaviors/trasparenza.py:254
+#: design/plone/contenttypes/behaviors/trasparenza.py:255
 msgid "customer_satisfaction_help"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction"
-#: design/plone/contenttypes/behaviors/trasparenza.py:249
+#: design/plone/contenttypes/behaviors/trasparenza.py:250
 msgid "customer_satisfaction_label"
 msgstr ""
 
-#. Default: "Data di conclusione dell'incarico."
-#: design/plone/contenttypes/interfaces/persona.py:60
-msgid "data_conclusione_incarico_help"
-msgstr ""
-
 #. Default: "Data conclusione incarico"
-#: design/plone/contenttypes/interfaces/persona.py:56
-msgid "data_conclusione_incarico_label"
+#: design/plone/contenttypes/interfaces/incarico.py:100
+msgid "data_conclusione_incarico"
 msgstr ""
 
 #. Default: "Data e fasi intermedie"
 #: design/plone/contenttypes/interfaces/documento_personale.py:120
 msgid "data_e_fasi_intermedie"
 msgstr ""
 
 #. Default: "Data di inizio"
 #: design/plone/contenttypes/interfaces/documento_personale.py:116
 msgid "data_inizio"
 msgstr ""
 
-#. Default: "Solo per persona politica: specificare la data di insediamento."
-#: design/plone/contenttypes/interfaces/persona.py:97
-msgid "data_insediamento_help"
+#. Default: "Data inizio incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:95
+msgid "data_inizio_incarico"
 msgstr ""
 
 #. Default: "Data insediamento"
-#: design/plone/contenttypes/interfaces/persona.py:96
-msgid "data_insediamento_label"
+#: design/plone/contenttypes/interfaces/incarico.py:105
+msgid "data_insediamento"
 msgstr ""
 
 #. Default: "Data del messaggio"
 #: design/plone/contenttypes/interfaces/messaggio.py:12
 msgid "data_messaggio"
 msgstr ""
 
 #. Default: "Data pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:21
 msgid "data_pagamento"
 msgstr ""
 
 #. Default: "Data del protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:41
 #: design/plone/contenttypes/interfaces/documento_personale.py:19
 msgid "data_protocollo"
 msgstr ""
 
+#. Default: "Data scadenza"
+#: design/plone/contenttypes/interfaces/servizio.py:49
+msgid "data_scadenza_label"
+msgstr ""
+
 #. Default: "Data di scadenza della procedura"
 #: design/plone/contenttypes/interfaces/messaggio.py:40
 msgid "data_scadenza_procedura"
 msgstr ""
 
 #. Default: "Dataset"
-#: design/plone/contenttypes/interfaces/dataset.py:27
+#: design/plone/contenttypes/interfaces/dataset.py:20
 msgid "dataset"
 msgstr ""
 
+#. Default: "Schede dataset collegate al documento"
+#: design/plone/contenttypes/interfaces/documento.py:150
+msgid "dataset_collegati_help"
+msgstr ""
+
 #. Default: "Seleziona una lista di schede dataset collegate a questo contenuto."
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:20
 msgid "dataset_correlati_help"
 msgstr ""
 
 #. Default: "Dataset correlati"
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:18
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
 msgid "dataset_correlati_label"
 msgstr ""
 
+#. Default: "Dataset collegati"
+#: design/plone/contenttypes/interfaces/documento.py:146
+msgid "dataset_label"
+msgstr ""
+
+#. Default: "Date e informazioni"
+#: design/plone/contenttypes/interfaces/incarico.py:175
+msgid "date_e_informazioni_label"
+msgstr ""
+
 #. Default: "Date e orari"
-#: design/plone/contenttypes/behaviors/evento.py:209
-#: design/plone/contenttypes/schema_overrides.py:34
+#: design/plone/contenttypes/behaviors/evento.py:164
+#: design/plone/contenttypes/schema_overrides.py:33
 msgid "date_e_orari_label"
 msgstr ""
 
 #. Default: "Inserisci la decorrenza termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:69
+#: design/plone/contenttypes/behaviors/trasparenza.py:70
 msgid "decorrenza_termini_help"
 msgstr ""
 
 #. Default: "Decorrenza termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:64
+#: design/plone/contenttypes/behaviors/trasparenza.py:65
 msgid "decorrenza_termini_label"
 msgstr ""
 
 #. Default: "Elenco delle deleghe a capo della persona."
-#: design/plone/contenttypes/interfaces/persona.py:77
+#: design/plone/contenttypes/interfaces/persona.py:85
 msgid "deleghe_help"
 msgstr ""
 
 #. Default: "Deleghe"
-#: design/plone/contenttypes/interfaces/persona.py:76
+#: design/plone/contenttypes/interfaces/persona.py:84
 msgid "deleghe_label"
 msgstr ""
 
 #. Default: "Descrizione completa"
-#: design/plone/contenttypes/behaviors/luogo.py:23
+#: design/plone/contenttypes/behaviors/luogo.py:24
 msgid "descrizione_completa"
 msgstr ""
 
-#. Default: "Descrizione destinatari"
-#: design/plone/contenttypes/behaviors/evento.py:38
-msgid "descrizione_destinatari"
-msgstr ""
-
-#. Default: "Descrizione dei principali interlocutori dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:40
-msgid "descrizione_destinatari_help"
-msgstr ""
-
 #. Default: "Descrizione estesa"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:16
-#: design/plone/contenttypes/behaviors/evento.py:30
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:19
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:17
+#: design/plone/contenttypes/behaviors/evento.py:32
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
 msgid "descrizione_estesa"
 msgstr ""
 
 #. Default: "Descrizione dettagliata e completa."
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:18
-#: design/plone/contenttypes/behaviors/evento.py:32
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:19
+#: design/plone/contenttypes/behaviors/evento.py:34
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:23
 msgid "descrizione_estesa_help"
 msgstr ""
 
 #. Default: "Descrizione"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:51
-#: design/plone/contenttypes/behaviors/luogo.py:166
-#: design/plone/contenttypes/interfaces/documento.py:162
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:72
+#: design/plone/contenttypes/behaviors/luogo.py:135
+#: design/plone/contenttypes/interfaces/documento.py:242
 msgid "descrizione_label"
 msgstr ""
 
 #. Default: "Inserisci eventuale testo descrittivo del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:37
+#: design/plone/contenttypes/behaviors/trasparenza.py:38
 msgid "descrizione_procedimento_help"
 msgstr ""
 
 #. Default: "Descrizione del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:32
+#: design/plone/contenttypes/behaviors/trasparenza.py:33
 msgid "descrizione_procedimento_label"
 msgstr ""
 
 #. Default: "Dirigente"
-#: design/plone/contenttypes/behaviors/trasparenza.py:136
+#: design/plone/contenttypes/behaviors/trasparenza.py:137
 msgid "dirigente"
 msgstr ""
 
 #. Default: "Indicare il dirigente."
-#: design/plone/contenttypes/behaviors/trasparenza.py:140
+#: design/plone/contenttypes/behaviors/trasparenza.py:141
 msgid "dirigente_help"
 msgstr ""
 
 #. Default: "Distribuzione"
-#: design/plone/contenttypes/interfaces/dataset.py:22
+#: design/plone/contenttypes/interfaces/dataset.py:15
 msgid "distribuzione"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/messaggio.py:56
+#: design/plone/contenttypes/interfaces/messaggio.py:48
 msgid "documenti_allegati"
 msgstr ""
 
 #. Default: "Seleziona una serie di altri contenuti di tipo Documento che vanno allegati a questo."
-#: design/plone/contenttypes/interfaces/documento.py:113
+#: design/plone/contenttypes/interfaces/documento.py:194
 msgid "documenti_allegati_help"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/documento.py:109
+#: design/plone/contenttypes/interfaces/documento.py:190
 msgid "documenti_allegati_label"
 msgstr ""
 
 #. Default: "Documenti"
-#: design/plone/contenttypes/interfaces/persona.py:199
-#: design/plone/contenttypes/interfaces/servizio.py:412
+#: design/plone/contenttypes/interfaces/persona.py:146
+#: design/plone/contenttypes/interfaces/servizio.py:525
 msgid "documenti_label"
 msgstr ""
 
+#. Default: "Documenti pubblici importanti, collegati a questa Unità Organizzativa"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:129
+msgid "documenti_pubblici_help"
+msgstr ""
+
+#. Default: "Documenti pubblici"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:127
+msgid "documenti_pubblici_label"
+msgstr ""
+
 #. Default: "Dove"
-#: design/plone/contenttypes/behaviors/address.py:71
-#: design/plone/contenttypes/behaviors/geolocation.py:29
+#: design/plone/contenttypes/behaviors/address.py:53
+#: design/plone/contenttypes/behaviors/geolocation.py:26
 msgid "dove_label"
 msgstr ""
 
 #. Default: "Dove rivolgersi: informazioni aggiuntive"
-#: design/plone/contenttypes/interfaces/servizio.py:143
+#: design/plone/contenttypes/interfaces/servizio.py:212
 msgid "dove_rivolgersi_extra"
 msgstr ""
 
 #. Default: "Indicare eventuali informazioni aggiuntive riguardo al dove rivolgersi per questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:147
+#: design/plone/contenttypes/interfaces/servizio.py:216
 msgid "dove_rivolgersi_extra_help"
 msgstr ""
 
 #. Default: "Seleziona una lista delle sedi e dei luoghi in cui è presente questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:135
+#: design/plone/contenttypes/interfaces/servizio.py:204
 msgid "dove_rivolgersi_help"
 msgstr ""
 
 #. Default: "Elementi di interesse"
-#: design/plone/contenttypes/behaviors/luogo.py:44
+#: design/plone/contenttypes/behaviors/luogo.py:45
 msgid "elementi_di_interesse"
 msgstr ""
 
-#. Default: "Indicare un indirizzo mail per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:128
-msgid "email_event_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/evento.py:127
-msgid "email_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:35
-msgid "email_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/contatti.py:34
-msgid "email_label"
-msgstr ""
-
-#. Default: "Contatto mail della persona. E' possibile inserire più di un indirizzo. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:135
-msgid "email_persona_help"
-msgstr ""
-
-#. Default: "Indirizzo email"
-#: design/plone/contenttypes/interfaces/persona.py:134
-msgid "email_persona_label"
-msgstr ""
-
 #. Default: "Esito"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:51
 msgid "esito"
 msgstr ""
 
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/evento.py:113
-msgid "fax_event_help"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/evento.py:114
-msgid "fax_event_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/contatti.py:29
-msgid "fax_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/contatti.py:28
-msgid "fax_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/interfaces/persona.py:130
-msgid "fax_persona_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/interfaces/persona.py:129
-msgid "fax_persona_label"
+#. Default: "Escludi dalla ricerca"
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:17
+msgid "exclude_from_search_label"
 msgstr ""
 
 #. Default: "Inserisci il file correlato di questo pocedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:44
+#: design/plone/contenttypes/behaviors/trasparenza.py:45
 msgid "file_correlato_help"
 msgstr ""
 
 #. Default: "File correlato"
-#: design/plone/contenttypes/behaviors/trasparenza.py:43
+#: design/plone/contenttypes/behaviors/trasparenza.py:44
 msgid "file_correlato_label"
 msgstr ""
 
 #. Default: "Inserisci il file principale di questo contenuto."
-#: design/plone/contenttypes/behaviors/multi_file.py:16
+#: design/plone/contenttypes/behaviors/multi_file.py:17
 msgid "file_principale_help"
 msgstr ""
 
 #. Default: "File principale"
-#: design/plone/contenttypes/behaviors/multi_file.py:15
+#: design/plone/contenttypes/behaviors/multi_file.py:16
 msgid "file_principale_label"
 msgstr ""
 
 #. Default: "Inserisci la fine termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:80
+#: design/plone/contenttypes/behaviors/trasparenza.py:81
 msgid "fine_termine_help"
 msgstr ""
 
 #. Default: "Fine termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:75
+#: design/plone/contenttypes/behaviors/trasparenza.py:76
 msgid "fine_termine_label"
 msgstr ""
 
+#. Default: "Lista dei formati in cui è disponibile il documento"
+#: design/plone/contenttypes/interfaces/documento.py:117
+msgid "formati_disponibili_help"
+msgstr ""
+
+#. Default: "Formati disponibili"
+#: design/plone/contenttypes/interfaces/documento.py:116
+msgid "formati_disponibili_label"
+msgstr ""
+
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:25
+#: design/plone/contenttypes/behaviors/multi_file.py:26
 msgid "formato_alternativo_1_help"
 msgstr ""
 
 #. Default: "Formato alternativo 1"
-#: design/plone/contenttypes/behaviors/multi_file.py:24
+#: design/plone/contenttypes/behaviors/multi_file.py:25
 msgid "formato_alternativo_1_label"
 msgstr ""
 
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:35
+#: design/plone/contenttypes/behaviors/multi_file.py:36
 msgid "formato_alternativo_2_help"
 msgstr ""
 
 #. Default: "Formato alternativo 2"
-#: design/plone/contenttypes/behaviors/multi_file.py:34
+#: design/plone/contenttypes/behaviors/multi_file.py:35
 msgid "formato_alternativo_2_label"
 msgstr ""
 
-#. Default: "Foto da mostrare della persona. La dimensione suggerita è 180x100 px."
-#: design/plone/contenttypes/interfaces/persona.py:21
+#. Default: "Foto da mostrare della persona. La dimensione suggerita è 100x180px."
+#: design/plone/contenttypes/interfaces/persona.py:30
 msgid "foto_persona_help"
 msgstr ""
 
 #. Default: "Foto della persona"
-#: design/plone/contenttypes/interfaces/persona.py:19
+#: design/plone/contenttypes/interfaces/persona.py:28
 msgid "foto_persona_label"
 msgstr ""
 
 #. Default: "Frequenza di aggiornamento"
-#: design/plone/contenttypes/interfaces/dataset.py:32
+#: design/plone/contenttypes/interfaces/dataset.py:25
 msgid "frequenza_aggiornamento"
 msgstr ""
 
 #. Default: "Invalid geolocation data: ${value}. Provide latitude and longitude coordinates."
-#: design/plone/contenttypes/restapi/deserializers/dxfields.py:28
+#: design/plone/contenttypes/restapi/deserializers/dxfields.py:39
 msgid "geolocation_field_validator_label"
 msgstr ""
 
 #. Default: "Indicare l'eventuale circoscrizione in cui si trova questo luogo"
 #: design/plone/contenttypes/behaviors/address.py:38
 msgid "help_circoscrizione"
 msgstr ""
 
 #. Default: "Indicare una descrizione completa, inserendo tutte le informazioni rilevanti relative al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:24
+#: design/plone/contenttypes/behaviors/luogo.py:25
 msgid "help_descrizione_completa"
 msgstr ""
 
 #. Default: "Indicare eventuali elementi di interesse per il cittadino."
-#: design/plone/contenttypes/behaviors/luogo.py:45
+#: design/plone/contenttypes/behaviors/luogo.py:46
 msgid "help_elementi_di_interesse"
 msgstr ""
 
+#. Default: "Se selezionato, questo contenuto non verrà mostrato nelle ricerche del sito per gli utenti anonimi."
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:18
+msgid "help_exclude_from_search"
+msgstr ""
+
 #. Default: "Indicare tutte le informazioni relative alla modalità di accesso al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:54
+#: design/plone/contenttypes/behaviors/luogo.py:55
 msgid "help_modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare, se esiste, un nome alternativo per il luogo; questo sarà mostrato affianco al titolo della scheda"
-#: design/plone/contenttypes/behaviors/luogo.py:34
+#: design/plone/contenttypes/behaviors/luogo.py:35
 msgid "help_nome_alternativo"
 msgstr ""
 
 #. Default: "Inserisci il nome della sede, se non è presente tra i Luoghi del sito."
 #: design/plone/contenttypes/behaviors/address.py:17
 msgid "help_nome_sede"
 msgstr ""
 
 #. Default: "Indicare l'eventuale quartiere in cui si trova questo luogo"
 #: design/plone/contenttypes/behaviors/address.py:32
 msgid "help_quartiere"
 msgstr ""
 
-#. Default: "Indicare un numero di fax della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:108
-msgid "help_riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:119
-msgid "help_riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:132
-msgid "help_riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Indicare il riferimento telefonico per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:96
-msgid "help_riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato.Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
-#: design/plone/contenttypes/behaviors/update_note.py:17
+#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato. Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
+#: design/plone/contenttypes/behaviors/update_note.py:18
 msgid "help_update_note"
 msgstr ""
 
 #. Default: "Icona"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:27
 msgid "icona"
 msgstr ""
 
 #. Default: "Puoi selezionare un’icona fra quelle proposte nel menu a tendina oppure puoi scrivere/incollare nel campo di testo il nome di un’icona di fontawsome 5"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:28
 msgid "icona_help"
 msgstr ""
 
 #. Default: "Identificativo"
-#: design/plone/contenttypes/interfaces/servizio.py:290
+#: design/plone/contenttypes/interfaces/servizio.py:379
 msgid "identificativo"
 msgstr ""
 
 #. Default: "Un numero identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:21
 msgid "identificativo_documento_help"
 msgstr ""
 
 #. Default: "Identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:17
 msgid "identificativo_documento_label"
 msgstr ""
 
 #. Default: "Eventuale codice identificativo del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:292
+#: design/plone/contenttypes/interfaces/servizio.py:381
 msgid "identificativo_help"
 msgstr ""
 
+#. Default: "Identificativo"
+#: design/plone/contenttypes/behaviors/luogo.py:119
+msgid "identificativo_mibac"
+msgstr ""
+
+#. Default: "Codice identificativo del luogo. Nel MIBAC c'è il codice del DBUnico per i luoghi della cultura e il codice ISIL per le biblioteche. Non deve comparire nel frontend del sito."
+#: design/plone/contenttypes/behaviors/luogo.py:121
+msgid "identificativo_mibac_help"
+msgstr ""
+
 #. Default: "La dimensione dell'immagine dovrebbe essere di ${size} px"
-#: design/plone/contenttypes/restapi/types/adapters.py:31
+#: design/plone/contenttypes/restapi/types/adapters.py:43
 msgid "image_size_help"
 msgstr ""
 
 #. Default: "Immagine"
 #: design/plone/contenttypes/interfaces/documento_personale.py:23
 msgid "immagine"
 msgstr ""
 
+#. Default: "Solo per incarico politico: importi di viaggi di servizio  e missioni pagati con fondi pubblici."
+#: design/plone/contenttypes/interfaces/incarico.py:34
+msgid "importi_viaggio_servizio_incarico_help"
+msgstr ""
+
+#. Default: "Importi di viaggio e/o servizio"
+#: design/plone/contenttypes/interfaces/incarico.py:30
+msgid "importi_viaggio_servizio_incarico_label"
+msgstr ""
+
 #. Default: "Importo pagato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:25
 msgid "importo_pagato"
 msgstr ""
 
+#. Default: "Seleziona l'incarico corrente della persona."
+#: design/plone/contenttypes/interfaces/persona.py:63
+msgid "incarichi_help"
+msgstr ""
+
+#. Default: "Incarichi"
+#: design/plone/contenttypes/interfaces/persona.py:59
+msgid "incarichi_label"
+msgstr ""
+
 #. Default: "Inserisci eventuale testo informativo che verrà mostrato in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:23
 msgid "info_testata_help"
 msgstr ""
 
 #. Default: "Informazioni aggiuntive per la testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:18
@@ -1708,127 +1726,162 @@
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/interfaces/documento_personale.py:140
 msgid "informazioni"
 msgstr ""
 
+#. Default: "Compensi e trasparenza"
+#: design/plone/contenttypes/interfaces/incarico.py:170
+msgid "informazioni_compensi_label"
+msgstr ""
+
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/behaviors/additional_help_infos.py:28
-#: design/plone/contenttypes/behaviors/evento.py:229
 #: design/plone/contenttypes/behaviors/strutture_correlate.py:42
+#: design/plone/contenttypes/interfaces/documento.py:253
 msgid "informazioni_label"
 msgstr ""
 
+#. Default: "Intervallo della fase (es. 1)"
+#: design/plone/contenttypes/interfaces/servizio.py:32
+msgid "interval_qt_help"
+msgstr ""
+
+#. Default: "Intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:31
+msgid "interval_qt_label"
+msgstr ""
+
+#. Default: "Ad esempio: ore, giorni, settimane, mesi."
+#: design/plone/contenttypes/interfaces/servizio.py:41
+msgid "interval_type_help"
+msgstr ""
+
+#. Default: "Tipo intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:40
+msgid "interval_type_label"
+msgstr ""
+
 #. Default: "Se un content-type deve avere una dimensione della leadimage particolare, indicarle qui. Inserire le dimensioni nella forma di esempio PortalType|900x900"
-#: design/plone/contenttypes/controlpanels/settings.py:110
+#: design/plone/contenttypes/controlpanels/settings.py:52
 msgid "lead_image_dimension_help"
 msgstr ""
 
 #. Default: "Dimensioni lead image"
-#: design/plone/contenttypes/controlpanels/settings.py:106
+#: design/plone/contenttypes/controlpanels/settings.py:48
 msgid "lead_image_dimension_label"
 msgstr ""
 
-#. Default: "Servizi o uffici di riferimento"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:27
+#. Default: "Strutture o uffici di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
 msgid "legami_altre_strutture_label"
 msgstr ""
 
 #. Default: "Selezionare la lista di strutture e/o uffici collegati a questa unità organizzativa."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:35
 msgid "legami_con_altre_strutture_help"
 msgstr ""
 
 #. Default: "Licenza"
-#: design/plone/contenttypes/interfaces/dataset.py:25
+#: design/plone/contenttypes/interfaces/dataset.py:18
 msgid "licenza"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
 #: design/plone/contenttypes/interfaces/documento_personale.py:92
 msgid "licenza_distribuzione"
 msgstr ""
 
 #. Default: "La licenza con il quale viene distribuito questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:88
+#: design/plone/contenttypes/interfaces/documento.py:125
 msgid "licenza_distribuzione_help"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
-#: design/plone/contenttypes/interfaces/documento.py:87
+#: design/plone/contenttypes/interfaces/documento.py:124
 msgid "licenza_distribuzione_label"
 msgstr ""
 
 #. Default: "Link a siti esterni"
-#: design/plone/contenttypes/interfaces/servizio.py:258
+#: design/plone/contenttypes/interfaces/servizio.py:347
 msgid "link_siti_esterni"
 msgstr ""
 
 #. Default: "Eventuali collegamenti a pagine web, siti, servizi esterni all'ambito Comunale utili all'erogazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:260
+#: design/plone/contenttypes/interfaces/servizio.py:349
 msgid "link_siti_esterni_help"
 msgstr ""
 
 #. Default: "Link utili"
-#: design/plone/contenttypes/interfaces/servizio.py:417
+#: design/plone/contenttypes/interfaces/servizio.py:530
 msgid "link_utili_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati. Se il luogo dell'evento non è presente sul sito, inserisci le sue informazioni nei campi seguenti."
 #: design/plone/contenttypes/behaviors/luoghi_correlati.py:52
 msgid "luoghi_correlati_event_help"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati."
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:72
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:19
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:64
 msgid "luoghi_correlati_help"
 msgstr ""
 
 #. Default: "Luoghi correlati"
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:17
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:71
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:63
 msgid "luoghi_correlati_label"
 msgstr ""
 
 #. Default: "Luogo"
-#: design/plone/contenttypes/behaviors/address.py:89
-#: design/plone/contenttypes/behaviors/geolocation.py:38
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:74
+#: design/plone/contenttypes/behaviors/address.py:71
+#: design/plone/contenttypes/behaviors/geolocation.py:34
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:76
 msgid "luogo_label"
 msgstr ""
 
+#. Default: "Sottotitolo"
+#: design/plone/contenttypes/interfaces/servizio.py:26
+msgid "milestone_description_label"
+msgstr ""
+
+#. Default: "Titolo"
+#: design/plone/contenttypes/interfaces/servizio.py:21
+msgid "milestone_label"
+msgstr ""
+
 #. Default: "Modalita' di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:53
+#: design/plone/contenttypes/behaviors/luogo.py:54
 msgid "modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare la modalità di avvio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:25
+#: design/plone/contenttypes/behaviors/trasparenza.py:26
 msgid "modalita_avvio_help"
 msgstr ""
 
 #. Default: "Modalita di avvio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:24
+#: design/plone/contenttypes/behaviors/trasparenza.py:25
 msgid "modalita_avvio_label"
 msgstr ""
 
 #. Default: "Modalità pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:29
 msgid "modalita_pagamento"
 msgstr ""
 
 #. Default: "Indicare le modalità per richiedere informazioni riguardo a questo procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:168
+#: design/plone/contenttypes/behaviors/trasparenza.py:169
 msgid "modalita_richiesta_informazioni_help"
 msgstr ""
 
 #. Default: "Modalità per richiedere informazioni"
-#: design/plone/contenttypes/behaviors/trasparenza.py:163
+#: design/plone/contenttypes/behaviors/trasparenza.py:164
 msgid "modalita_richiesta_informazioni_label"
 msgstr ""
 
 #. Default: "Seleziona se mostrare o meno i bottoni con i link per la condivisione sui vari social, mail e stampa."
 #: design/plone/contenttypes/behaviors/info_testata.py:44
 msgid "mostra_bottoni_condivisione_help"
 msgstr ""
@@ -1844,46 +1897,46 @@
 msgstr ""
 
 #. Default: "Mostra la navigazione"
 #: design/plone/contenttypes/behaviors/info_testata.py:51
 msgid "mostra_navigazione_label"
 msgstr ""
 
-#. Default: "Descrizione del motivo per cui il servizio non è attivo."
-#: design/plone/contenttypes/interfaces/servizio.py:44
+#. Default: "Descrizione del motivo per cui il servizio non è attivo. È obbligatorio se il campo precedente è spuntato."
+#: design/plone/contenttypes/interfaces/servizio.py:89
 msgid "motivo_stato_servizio_help"
 msgstr ""
 
-#. Default: "Motivo dello stato del servizio nel caso non sia attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:39
+#. Default: "Motivo dello stato"
+#: design/plone/contenttypes/interfaces/servizio.py:84
 msgid "motivo_stato_servizio_label"
 msgstr ""
 
 #. Default: "Nome alternativo"
-#: design/plone/contenttypes/behaviors/luogo.py:33
+#: design/plone/contenttypes/behaviors/luogo.py:34
 msgid "nome_alternativo"
 msgstr ""
 
 #. Default: "Nome sede"
 #: design/plone/contenttypes/behaviors/address.py:16
 msgid "nome_sede"
 msgstr ""
 
 #. Default: "Seleziona una lista di notizie correlate a questa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:83
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:75
 msgid "notizie_correlate_help"
 msgstr ""
 
 #. Default: "Notizie correlate"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:82
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:74
 msgid "notizie_correlate_label"
 msgstr ""
 
 #. Default: "Numero progressivo del comunicato stampa"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:30
 msgid "numero_progressivo_cs_label"
 msgstr ""
 
 #. Default: "Numero protocollo"
 #: design/plone/contenttypes/interfaces/pratica.py:12
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:12
 msgid "numero_protocollo"
@@ -1891,125 +1944,163 @@
 
 #. Default: "Oggetto"
 #: design/plone/contenttypes/interfaces/documento_personale.py:48
 msgid "oggetto"
 msgstr ""
 
 #. Default: "Informazioni sugli orari"
-#: design/plone/contenttypes/behaviors/evento.py:62
+#: design/plone/contenttypes/behaviors/evento.py:50
 msgid "orari"
 msgstr ""
 
 #. Default: "Informazioni sugli orari di svolgimento dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:64
+#: design/plone/contenttypes/behaviors/evento.py:52
 msgid "orari_help"
 msgstr ""
 
 #. Default: "Orari di apertura"
-#: design/plone/contenttypes/behaviors/contatti.py:86
+#: design/plone/contenttypes/behaviors/luogo.py:151
 msgid "orari_label"
 msgstr ""
 
+#. Default: "Orario per il pubblico"
+#: design/plone/contenttypes/behaviors/luogo.py:93
+msgid "orario_pubblico"
+msgstr ""
+
 #. Default: "Indicare eventuali orari di accesso al pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:59
+#: design/plone/contenttypes/behaviors/contatti.py:40
+#: design/plone/contenttypes/behaviors/luogo.py:95
 msgid "orario_pubblico_help"
 msgstr ""
 
 #. Default: "Orario per il pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:58
+#: design/plone/contenttypes/behaviors/contatti.py:39
 msgid "orario_pubblico_label"
 msgstr ""
 
 #. Default: "Se l'evento non è organizzato direttamente dal comune oppure ha anche un organizzatore esterno, indicare il nome del contatto."
-#: design/plone/contenttypes/behaviors/evento.py:97
+#: design/plone/contenttypes/behaviors/evento.py:86
 msgid "organizzato_da_esterno_help"
 msgstr ""
 
 #. Default: "Organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:95
+#: design/plone/contenttypes/behaviors/evento.py:84
 msgid "organizzato_da_esterno_label"
 msgstr ""
 
 #. Default: "Se l'evento è organizzato direttamente dal comune, indicare l'ufficio/ente organizzatore. I dati di contatto verranno presi direttamente dall'ufficio selezionato. Se l'evento non è organizzato direttamente dal comune, o si vogliono sovrascrivere alcuni dati di contatto, utilizzare i seguenti campi."
-#: design/plone/contenttypes/behaviors/evento.py:84
+#: design/plone/contenttypes/behaviors/evento.py:74
 msgid "organizzato_da_interno_help"
 msgstr ""
 
 #. Default: "Organizzato da"
-#: design/plone/contenttypes/behaviors/evento.py:80
+#: design/plone/contenttypes/behaviors/evento.py:70
 msgid "organizzato_da_interno_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di organizzazioni a cui la persona appartiene."
-#: design/plone/contenttypes/interfaces/persona.py:42
+#: design/plone/contenttypes/interfaces/persona.py:45
 msgid "organizzazione_riferimento_help"
 msgstr ""
 
 #. Default: "Organizzazione di riferimento"
-#: design/plone/contenttypes/interfaces/persona.py:38
+#: design/plone/contenttypes/interfaces/persona.py:41
 msgid "organizzazione_riferimento_label"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:157
+#: design/plone/contenttypes/behaviors/trasparenza.py:158
 msgid "organo_competente_provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:152
+#: design/plone/contenttypes/behaviors/trasparenza.py:153
 msgid "organo_competente_provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Indicare le informazioni riguardanti i pagamenti previsti e modalità di pagamento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:222
+#: design/plone/contenttypes/behaviors/trasparenza.py:223
 msgid "pagamenti_help"
 msgstr ""
 
 #. Default: "Pagamenti previsti e modalità"
-#: design/plone/contenttypes/behaviors/trasparenza.py:218
+#: design/plone/contenttypes/behaviors/trasparenza.py:219
 msgid "pagamenti_label"
 msgstr ""
 
+#. Default: "Link a persone dell'amministrazione che interverranno all'evento"
+#: design/plone/contenttypes/behaviors/evento.py:118
+msgid "parteciperanno_help"
+msgstr ""
+
+#. Default: "Parteciperanno (Persone)"
+#: design/plone/contenttypes/behaviors/evento.py:114
+msgid "parteciperanno_label"
+msgstr ""
+
 #. Default: "Indicare l'ente che supporta l'evento, se presente."
-#: design/plone/contenttypes/behaviors/evento.py:160
+#: design/plone/contenttypes/behaviors/evento.py:107
 msgid "patrocinato_da_help"
 msgstr ""
 
 #. Default: "Patrocinato da"
-#: design/plone/contenttypes/behaviors/evento.py:158
+#: design/plone/contenttypes/behaviors/evento.py:105
 msgid "patrocinato_da_label"
 msgstr ""
 
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:44
-msgid "pec_help"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:27
+msgid "pdc_desc_help"
 msgstr ""
 
-#. Default: "Pec"
-#: design/plone/contenttypes/behaviors/contatti.py:43
-msgid "pec_label"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:26
+msgid "pdc_desc_label"
 msgstr ""
 
-#. Default: "Elenco delle persone dell'amministrazione che parteciperanno all'evento."
-#: design/plone/contenttypes/behaviors/evento.py:53
-msgid "persone_amministrazione_help"
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:16
+msgid "pdc_type_label"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:37
+msgid "pdc_value_help"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:36
+msgid "pdc_value_label"
+msgstr ""
+
+#. Default: "Seleziona la persona che ha questo incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:47
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:66
+msgid "persona_incarico_help"
+msgstr ""
+
+#. Default: "La persona che ha la carica e l'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:43
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:62
+msgid "persona_incarico_label"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:221
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:215
 msgid "persone_label"
 msgstr ""
 
 #. Default: "Seleziona la lista delle persone che compongono la struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
 msgid "persone_struttura_help"
 msgstr ""
 
 #. Default: "Persone che compongono la struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:79
 msgid "persone_struttura_label"
 msgstr ""
 
 #. Default: "Pratica associata"
 #: design/plone/contenttypes/interfaces/documento_personale.py:26
 #: design/plone/contenttypes/interfaces/messaggio.py:35
 msgid "pratica_associata"
@@ -2017,255 +2108,230 @@
 
 #. Default: "Pratica associata al pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:43
 msgid "pratica_associata_ricevuta"
 msgstr ""
 
 #. Default: "Prenota un appuntamento"
-#: design/plone/contenttypes/interfaces/servizio.py:156
+#: design/plone/contenttypes/interfaces/servizio.py:225
 msgid "prenota_appuntamento"
 msgstr ""
 
 #. Default: "Se è possibile prenotare un'appuntamento, indicare le informazioni necessarie e il collegamento al servizio di prenotazione appuntamenti del Comune."
-#: design/plone/contenttypes/interfaces/servizio.py:157
+#: design/plone/contenttypes/interfaces/servizio.py:226
 msgid "prenota_appuntamento_help"
 msgstr ""
 
-#. Default: "Prezzo"
-#: design/plone/contenttypes/behaviors/evento.py:71
+#. Default: "Costo"
+#: design/plone/contenttypes/behaviors/evento.py:59
 msgid "prezzo"
 msgstr ""
 
-#. Default: "Indicare il prezzo dell'evento, se presente, specificando se esistono formati diversi."
-#: design/plone/contenttypes/behaviors/evento.py:73
+#. Default: "Eventuale costo dell'evento (se ci sono uno o più biglietti), con link all'acquisto se disponibile"
+#: design/plone/contenttypes/behaviors/evento.py:61
 msgid "prezzo_help"
 msgstr ""
 
 #. Default: "Indicare, se la procedura è informatizzata online, il riferimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:178
+#: design/plone/contenttypes/behaviors/trasparenza.py:179
 msgid "procedura_online_help"
 msgstr ""
 
 #. Default: "Procedura informatizzata online"
-#: design/plone/contenttypes/behaviors/trasparenza.py:174
+#: design/plone/contenttypes/behaviors/trasparenza.py:175
 msgid "procedura_online_label"
 msgstr ""
 
 #. Default: "Procedure collegate all'esito"
-#: design/plone/contenttypes/interfaces/servizio.py:100
+#: design/plone/contenttypes/interfaces/servizio.py:145
 msgid "procedure_collegate"
 msgstr ""
 
 #. Default: "Indicare cosa deve fare l'utente del servizio per conoscere l'esito della procedura, e dove eventualmente poter ritirare l'esito."
-#: design/plone/contenttypes/interfaces/servizio.py:102
+#: design/plone/contenttypes/interfaces/servizio.py:147
 msgid "procedure_collegate_help"
 msgstr ""
 
 #. Default: "Protocollo"
 #: design/plone/contenttypes/interfaces/documento_personale.py:15
 msgid "protocollo"
 msgstr ""
 
+#. Default: "Il numero di protocollo del documento."
+#: design/plone/contenttypes/interfaces/documento.py:33
+msgid "protocollo_documento_help"
+msgstr ""
+
+#. Default: "Numero di protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:29
+msgid "protocollo_documento_label"
+msgstr ""
+
 #. Default: "Eventuale provvedimento finale del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:114
+#: design/plone/contenttypes/behaviors/trasparenza.py:115
 msgid "provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Provvedimento del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:109
+#: design/plone/contenttypes/behaviors/trasparenza.py:110
 msgid "provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Quartiere"
 #: design/plone/contenttypes/behaviors/address.py:31
 msgid "quartiere"
 msgstr ""
 
-#. Default: "Reperibilità organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:118
-msgid "reperibilita"
-msgstr ""
-
-#. Default: "Indicare gli orari in cui l'organizzatore è telefonicamente reperibile."
-#: design/plone/contenttypes/behaviors/evento.py:120
-msgid "reperibilita_help"
-msgstr ""
-
 #. Default: "Indicare dove è possibile reperre la modulistica per il procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:211
+#: design/plone/contenttypes/behaviors/trasparenza.py:212
 msgid "reperimento_modulistica_help"
 msgstr ""
 
 #. Default: "Dove reperire la modulistica"
-#: design/plone/contenttypes/behaviors/trasparenza.py:207
+#: design/plone/contenttypes/behaviors/trasparenza.py:208
 msgid "reperimento_modulistica_label"
 msgstr ""
 
 #. Default: "Selezionare il/i responsabile/i della struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:48
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:52
 msgid "responsabile_help"
 msgstr ""
 
 #. Default: "Responsabile"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:43
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:47
 msgid "responsabile_label"
 msgstr ""
 
 #. Default: "Responsabile del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:120
+#: design/plone/contenttypes/behaviors/trasparenza.py:121
 msgid "responsabile_procedimento"
 msgstr ""
 
 #. Default: "Indicare il responsabile del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:124
+#: design/plone/contenttypes/behaviors/trasparenza.py:125
 msgid "responsabile_procedimento_help"
 msgstr ""
 
+#. Default: "Se è un incarico di responsabilità, specificare l'organizzazione della quale è responsabile in base all'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:81
+msgid "responsabile_struttura_incarico_help"
+msgstr ""
+
+#. Default: "Responsabile della struttura"
+#: design/plone/contenttypes/interfaces/incarico.py:77
+msgid "responsabile_struttura_incarico_label"
+msgstr ""
+
 #. Default: "Seleziona se mostrare o meno il campo di ricerca in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:32
 msgid "ricerca_in_testata_help"
 msgstr ""
 
 #. Default: "Ricerca in testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:29
 msgid "ricerca_in_testata_label"
 msgstr ""
 
 #. Default: "Ulteriori informazioni non previste negli altri campi; si può trattare di contatti o note informative la cui conoscenza è indispensabile per la partecipazione al bando"
-#: design/plone/contenttypes/interfaces/bando.py:96
+#: design/plone/contenttypes/interfaces/bando.py:97
 msgid "riferimenti_bando_agid_help"
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
-#: design/plone/contenttypes/interfaces/bando.py:95
+#: design/plone/contenttypes/interfaces/bando.py:96
 msgid "riferimenti_bando_agid_label"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
 #: design/plone/contenttypes/interfaces/documento_personale.py:145
 msgid "riferimenti_normativi"
 msgstr ""
 
 #. Default: "Inserisici del testo di dettaglio per eventuali riferimenti normativi utili a questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:100
+#: design/plone/contenttypes/interfaces/documento.py:137
 msgid "riferimenti_normativi_documento_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/interfaces/documento.py:96
+#: design/plone/contenttypes/interfaces/documento.py:133
 msgid "riferimenti_normativi_documento_label"
 msgstr ""
 
 #. Default: "Indicare eventuali riferimenti normativi."
-#: design/plone/contenttypes/behaviors/trasparenza.py:265
+#: design/plone/contenttypes/behaviors/trasparenza.py:266
 msgid "riferimenti_normativi_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/behaviors/trasparenza.py:260
+#: design/plone/contenttypes/behaviors/trasparenza.py:261
 msgid "riferimenti_normativi_label"
 msgstr ""
 
-#. Default: "Fax della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:104
-msgid "riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "E-mail struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:115
-msgid "riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Pec della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:128
-msgid "riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Telefono della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:92
-msgid "riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per il ruolo di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:84
-msgid "ruoli_persona_help"
-msgstr ""
-
-#. Default: "Ruoli Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:83
-msgid "ruoli_persona_label"
-msgstr ""
-
-#. Default: "Seleziona il ruolo della persona tra quelli disponibili."
-#: design/plone/contenttypes/interfaces/persona.py:29
-msgid "ruolo_help"
-msgstr ""
-
 #. Default: "Ruolo"
-#: design/plone/contenttypes/interfaces/persona.py:28
+#: design/plone/contenttypes/interfaces/persona.py:135
 msgid "ruolo_label"
 msgstr ""
 
 #. Default: "Data entro la quale sarà possibile far pervenire domande e richieste di chiarimento a chi eroga il bando"
-#: design/plone/contenttypes/interfaces/bando.py:69
+#: design/plone/contenttypes/interfaces/bando.py:70
 msgid "scadenza_domande_bando_help"
 msgstr ""
 
 #. Default: "Termine per le richieste di chiarimenti"
-#: design/plone/contenttypes/interfaces/bando.py:65
+#: design/plone/contenttypes/interfaces/bando.py:66
 msgid "scadenza_domande_bando_label"
 msgstr ""
 
 #. Default: "Inserire una lista di sezioni per la ricerca."
-#: design/plone/contenttypes/controlpanels/settings.py:129
+#: design/plone/contenttypes/controlpanels/settings.py:71
 msgid "search_sections_help"
 msgstr ""
 
 #. Default: "Sezioni ricerca"
-#: design/plone/contenttypes/controlpanels/settings.py:128
+#: design/plone/contenttypes/controlpanels/settings.py:70
 msgid "search_sections_label"
 msgstr ""
 
-#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente un contenuto di tipo Luogo a cui far riferimento, puoi compilare i campi seguenti. Se selezioni un Luogo, puoi usare comunque i campi seguenti per sovrascrivere alcune informazioni."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:105
+#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente creare il Luogo nella sezione dedicata nell'alberatura del sito."
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:97
 msgid "sede_help"
 msgstr ""
 
 #. Default: "Sede principale"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:103
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
 msgid "sede_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di eventuali contenuti di tipo Luogo che sono sedi secondarie di questa struttura. Per queste sedi non sarà possibile sovrascrivere i dati. Nel caso servano informazioni diverse, è possibile usare il campo sottostante."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:122
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:112
 msgid "sedi_secondarie_help"
 msgstr ""
 
-#. Default: "Sedi secondarie"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:120
+#. Default: "Altre sedi"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:110
 msgid "sedi_secondarie_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei servizi collegati a questo."
-#: design/plone/contenttypes/interfaces/servizio.py:300
+#: design/plone/contenttypes/interfaces/servizio.py:394
 msgid "servizi_collegati_help"
 msgstr ""
 
 #. Default: "Servizi collegati"
-#: design/plone/contenttypes/interfaces/servizio.py:299
+#: design/plone/contenttypes/interfaces/servizio.py:393
 msgid "servizi_collegati_label"
 msgstr ""
 
 #. Default: "Questi servizi non verranno mostrati nel contenuto, ma permetteranno di vedere questo contenuto associato quando si visita il servizio"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:20
 msgid "servizi_correlati_description"
 msgstr ""
 
 #. Default: "Servizi correlati"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:18
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
 msgid "servizi_correlati_label"
 msgstr ""
 
 #. Default: "Servizio che genera il documento"
 #: design/plone/contenttypes/interfaces/documento_personale.py:31
 msgid "servizio_origine"
 msgstr ""
@@ -2277,367 +2343,292 @@
 
 #. Default: "Servizio che origina la pratica"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:35
 msgid "servizio_origine_ricevuta"
 msgstr ""
 
 #. Default: "Settore merceologico"
-#: design/plone/contenttypes/interfaces/servizio.py:280
+#: design/plone/contenttypes/interfaces/servizio.py:369
 msgid "settore_merceologico"
 msgstr ""
 
 #. Default: "Classificazione del servizio basata su catalogo dei servizi (Classificazione NACE)."
-#: design/plone/contenttypes/interfaces/servizio.py:282
+#: design/plone/contenttypes/interfaces/servizio.py:371
 msgid "settore_merceologico_help"
 msgstr ""
 
+#. Default: "Se selezionato, il footer verrà popolato automaticamente con i contenuti di primo livello non esclusi dalla navigazione."
+#: design/plone/contenttypes/controlpanels/settings.py:93
+msgid "show_dynamic_folders_in_footer_help"
+msgstr ""
+
+#. Default: "Footer dinamico"
+#: design/plone/contenttypes/controlpanels/settings.py:92
+msgid "show_dynamic_folders_in_footer_label"
+msgstr ""
+
 #. Default: "Questo è il valore di default per decidere se mostrare o meno la data di modifica nei contenuti che hanno la behavior abilitata. E' poi possibile sovrascrivere il default nei singoli contenuti (nel tab \"Impostazioni\")."
-#: design/plone/contenttypes/controlpanels/settings.py:139
+#: design/plone/contenttypes/controlpanels/settings.py:81
 msgid "show_modified_default_help"
 msgstr ""
 
 #. Default: "Mostra la data di modifica"
-#: design/plone/contenttypes/controlpanels/settings.py:138
+#: design/plone/contenttypes/controlpanels/settings.py:80
 msgid "show_modified_default_label"
 msgstr ""
 
 #. Default: "Se attivo, verrà mostrata la data di ultima modifica in visualizzazione del contenuto."
 #: design/plone/contenttypes/behaviors/show_modified.py:24
 msgid "show_modified_help"
 msgstr ""
 
 #. Default: "Mostra la data di ultima modifica"
 #: design/plone/contenttypes/behaviors/show_modified.py:23
 msgid "show_modified_label"
 msgstr ""
 
 #. Default: "Indicare se il procedimento prevede il silenzio assenso o la dichiarazione dell'interessato sostitutiva del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:103
+#: design/plone/contenttypes/behaviors/trasparenza.py:104
 msgid "silenzio_assenso_help"
 msgstr ""
 
 #. Default: "Silenzio assenso/Dichiarazione dell'interessato sostitutiva del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:97
+#: design/plone/contenttypes/behaviors/trasparenza.py:98
 msgid "silenzio_assenso_label"
 msgstr ""
 
 #. Default: "Inserisci eventuali soggetti esterni, nonché, strutture interne coinvolte nel procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:57
+#: design/plone/contenttypes/behaviors/trasparenza.py:58
 msgid "soggetti_eserni_help"
 msgstr ""
 
 #. Default: "Soggetti esterni, nonché, strutture interne coinvolte nel procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:52
+#: design/plone/contenttypes/behaviors/trasparenza.py:53
 msgid "soggetti_eserni_label"
 msgstr ""
 
 #. Default: "Indica un eventuale sottotitolo/titolo alternativo."
-#: design/plone/contenttypes/behaviors/evento.py:23
-#: design/plone/contenttypes/interfaces/servizio.py:19
+#: design/plone/contenttypes/behaviors/evento.py:24
+#: design/plone/contenttypes/interfaces/servizio.py:64
 msgid "sottotitolo_help"
 msgstr ""
 
 #. Default: "Sottotitolo"
-#: design/plone/contenttypes/behaviors/evento.py:22
-#: design/plone/contenttypes/interfaces/servizio.py:18
+#: design/plone/contenttypes/behaviors/evento.py:23
+#: design/plone/contenttypes/interfaces/servizio.py:63
 msgid "sottotitolo_label"
 msgstr ""
 
 #. Default: "Stampa ricevuta"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:17
 msgid "stampa_ricevuta"
 msgstr ""
 
 #. Default: "Stato della pratica"
 #: design/plone/contenttypes/interfaces/pratica.py:26
 msgid "stato_pratica"
 msgstr ""
 
-#. Default: "Indica se il servizio è effettivamente fruibile."
-#: design/plone/contenttypes/interfaces/servizio.py:32
+#. Default: "Indica se il servizio è effettivamente fruibile; spuntare se non è fruibile."
+#: design/plone/contenttypes/interfaces/servizio.py:77
 msgid "stato_servizio_help"
 msgstr ""
 
-#. Default: "Servizio non attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:30
+#. Default: "Servizio non fruibile"
+#: design/plone/contenttypes/interfaces/servizio.py:75
 msgid "stato_servizio_label"
 msgstr ""
 
 #. Default: "Indicare gli eventuali strumenti di tutela."
-#: design/plone/contenttypes/behaviors/trasparenza.py:230
+#: design/plone/contenttypes/behaviors/trasparenza.py:231
 msgid "strumenti_tutela_help"
 msgstr ""
 
 #. Default: "Strumenti di tutela"
-#: design/plone/contenttypes/behaviors/trasparenza.py:229
+#: design/plone/contenttypes/behaviors/trasparenza.py:230
 msgid "strumenti_tutela_label"
 msgstr ""
 
 #. Default: "Struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:211
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
 msgid "struttura_label"
 msgstr ""
 
 #. Default: "Struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:82
+#: design/plone/contenttypes/behaviors/luogo.py:83
 msgid "struttura_responsabile"
 msgstr ""
 
 #. Default: "Struttura responsabile del luogo."
-#: design/plone/contenttypes/behaviors/luogo.py:63
+#: design/plone/contenttypes/behaviors/luogo.py:64
 msgid "struttura_responsabile_correlati"
 msgstr ""
 
 #. Default: "Indicare la struttura responsabile del luogo qualora sia fra unità organizzative del comune inserite nel sito; altrimenti compilare i campi testuali relativi alla struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:67
+#: design/plone/contenttypes/behaviors/luogo.py:68
 msgid "struttura_responsabile_correlati_help"
 msgstr ""
 
 #. Default: "Nome/link al sito web della struttura che gestisce il luogo, se questa non è comunale."
-#: design/plone/contenttypes/behaviors/luogo.py:84
+#: design/plone/contenttypes/behaviors/luogo.py:85
 msgid "struttura_responsabile_help"
 msgstr ""
 
 #. Default: "Seleziona la lista delle strutture politiche coinvolte."
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:25
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:26
 msgid "strutture_politiche_help"
 msgstr ""
 
 #. Default: "Indicare gli uffici/enti che supportano l'evento."
-#: design/plone/contenttypes/behaviors/evento.py:149
+#: design/plone/contenttypes/behaviors/evento.py:97
 msgid "supportato_da_help"
 msgstr ""
 
 #. Default: "Evento supportato da"
-#: design/plone/contenttypes/behaviors/evento.py:145
+#: design/plone/contenttypes/behaviors/evento.py:93
 msgid "supportato_da_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di argomenti d'interesse per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:22
+#: design/plone/contenttypes/behaviors/argomenti.py:26
 msgid "tassonomia_argomenti_help"
 msgstr ""
 
-#. Default: "Tassonomia argomenti"
-#: design/plone/contenttypes/behaviors/argomenti.py:21
+#. Default: "Argomenti"
+#: design/plone/contenttypes/behaviors/argomenti.py:25
 msgid "tassonomia_argomenti_label"
 msgstr ""
 
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/evento.py:104
-msgid "telefono_event_help"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:105
-msgid "telefono_event_label"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:19
-msgid "telefono_help"
-msgstr ""
-
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/contatti.py:18
-msgid "telefono_label"
-msgstr ""
-
-#. Default: "Contatto telefonico della persona. E' possibile inserire più di un numero. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:117
-msgid "telefono_persona_help"
-msgstr ""
-
-#. Default: "Numero di telefono"
-#: design/plone/contenttypes/interfaces/persona.py:116
-msgid "telefono_persona_label"
-msgstr ""
-
-#. Default: "Temi"
-#: design/plone/contenttypes/interfaces/dataset.py:14
-msgid "temi"
-msgstr ""
-
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:167
+#: design/plone/contenttypes/interfaces/servizio.py:236
 msgid "tempi_e_scadenze"
 msgstr ""
 
 #. Default: "Descrivere le informazioni dettagliate riguardo eventuali tempi e scadenze di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:169
+#: design/plone/contenttypes/interfaces/servizio.py:238
 msgid "tempi_e_scadenze_help"
 msgstr ""
 
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:395
+#: design/plone/contenttypes/interfaces/servizio.py:508
 msgid "tempi_e_scadenze_label"
 msgstr ""
 
 #. Default: "Inserisci il tempo medio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:91
+#: design/plone/contenttypes/behaviors/trasparenza.py:92
 msgid "tempo_medio_help"
 msgstr ""
 
 #. Default: "Tempo medio del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:86
+#: design/plone/contenttypes/behaviors/trasparenza.py:87
 msgid "tempo_medio_label"
 msgstr ""
 
 #. Default: "Testata"
-#: design/plone/contenttypes/behaviors/argomenti.py:104
+#: design/plone/contenttypes/behaviors/argomenti.py:232
 #: design/plone/contenttypes/behaviors/info_testata.py:62
 msgid "testata_fieldset_label"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:28
+#: design/plone/contenttypes/interfaces/bando.py:29
 msgid "text_help"
 msgstr ""
 
 #. Default: "Testo"
-#: design/plone/contenttypes/interfaces/bando.py:27
+#: design/plone/contenttypes/interfaces/bando.py:28
 msgid "text_label"
 msgstr ""
 
-#. Default: "Tipologia documento"
-#: design/plone/contenttypes/interfaces/messaggio.py:49
-msgid "tipologia_documento"
-msgstr ""
-
-#. Default: "Seleziona la tipologia del documento."
-#: design/plone/contenttypes/interfaces/documento.py:30
-msgid "tipologia_documento_help"
-msgstr ""
-
-#. Default: "Tipologia del documento"
-#: design/plone/contenttypes/interfaces/documento.py:29
-msgid "tipologia_documento_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia della notizia."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:29
-msgid "tipologia_notizia_help"
-msgstr ""
-
-#. Default: "Tipologia notizia"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:28
-msgid "tipologia_notizia_label"
-msgstr ""
-
-#. Default: "Specificare la tipologia di organizzazione: politica, amminsitrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:60
-msgid "tipologia_organizzazione_help"
-msgstr ""
-
-#. Default: "Tipologia organizzazione"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:57
-msgid "tipologia_organizzazione_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia di persona: politica, amministrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/persona.py:86
-msgid "tipologia_persona_help"
-msgstr ""
-
-#. Default: "Tipologia persona"
-#: design/plone/contenttypes/interfaces/persona.py:85
-msgid "tipologia_persona_label"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per le tipologie di un Documento. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:46
-msgid "tipologie_documento_help"
+#. Default: "Timeline tempi e scadenze"
+#: design/plone/contenttypes/interfaces/servizio.py:246
+msgid "timeline_tempi_scadenze"
 msgstr ""
 
-#. Default: "Tipologie Documento"
-#: design/plone/contenttypes/controlpanels/settings.py:45
-msgid "tipologie_documento_label"
+#. Default: "Timeline tempi e scadenze del servizio: indicare per ogni scadenza un titolo descrittivo ed un eventuale sottotitolo. Per ogni scadenza, selezionare opzionalmente o l'intervallo (Campi \"Intervallo\" e \"Tipo Intervallo\", es. \"1\" e \"settimana\"), oppure direttamente una data di scadenza (campo: \"Data Scadenza\", esempio 31/12/2023). Se vengono compilati entrambi, ha priorità il campo \"Data Scadenza\"."
+#: design/plone/contenttypes/interfaces/servizio.py:249
+msgid "timeline_tempi_scadenze_help"
 msgstr ""
 
 #. Default: "Inserisci i valori utilizzabili per le tipologie di una Notizia. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:19
+#: design/plone/contenttypes/controlpanels/settings.py:22
 msgid "tipologie_notizia_help"
 msgstr ""
 
 #. Default: "Tipologie Notizia"
-#: design/plone/contenttypes/controlpanels/settings.py:18
+#: design/plone/contenttypes/controlpanels/settings.py:21
 msgid "tipologie_notizia_label"
 msgstr ""
 
-#. Default: "Inserisci i valori utilizzabili per le tipologie di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:72
-msgid "tipologie_persona_help"
-msgstr ""
-
-#. Default: "Tipologie Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:71
-msgid "tipologie_persona_label"
-msgstr ""
-
 #. Default: "Inserisci i valori utilizzabili per le tipologie di un' Unità Organizzativa. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:34
+#: design/plone/contenttypes/controlpanels/settings.py:37
 msgid "tipologie_unita_organizzativa_help"
 msgstr ""
 
 #. Default: "Tipologie Unità Organizzativa"
-#: design/plone/contenttypes/controlpanels/settings.py:30
+#: design/plone/contenttypes/controlpanels/settings.py:33
 msgid "tipologie_unita_organizzativa_label"
 msgstr ""
 
 #. Default: "Titolare"
-#: design/plone/contenttypes/interfaces/dataset.py:29
+#: design/plone/contenttypes/interfaces/dataset.py:22
 msgid "titolare"
 msgstr ""
 
 #. Default: "Eventuale titolare del potere sostitutivo."
-#: design/plone/contenttypes/behaviors/trasparenza.py:243
+#: design/plone/contenttypes/behaviors/trasparenza.py:244
 msgid "titolare_potere_sostitutivo_help"
 msgstr ""
 
 #. Default: "Titolare del potere sostitutivo"
-#: design/plone/contenttypes/behaviors/trasparenza.py:238
+#: design/plone/contenttypes/behaviors/trasparenza.py:239
 msgid "titolare_potere_sostitutivo_label"
 msgstr ""
 
 #. Default: "Trasparenza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:292
+#: design/plone/contenttypes/behaviors/trasparenza.py:291
 msgid "trasparenza_fieldset_label"
 msgstr ""
 
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:17
+msgid "type_help"
+msgstr ""
+
 #. Default: "Seleziona l'ufficio responsabile di questo bando."
-#: design/plone/contenttypes/interfaces/bando.py:110
+#: design/plone/contenttypes/interfaces/bando.py:111
 msgid "ufficio_responsabile_bando_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del bando"
-#: design/plone/contenttypes/interfaces/bando.py:106
+#: design/plone/contenttypes/interfaces/bando.py:107
 msgid "ufficio_responsabile_bando_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio responsabile di questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:43
+#: design/plone/contenttypes/interfaces/documento.py:73
 msgid "ufficio_responsabile_documento_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del documento"
-#: design/plone/contenttypes/interfaces/documento.py:39
+#: design/plone/contenttypes/interfaces/documento.py:69
 msgid "ufficio_responsabile_documento_label"
 msgstr ""
 
 #. Default: "Ufficio responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:62
 msgid "ufficio_responsabile_documento_personale"
 msgstr ""
 
-#. Default: "Uffici responsabili"
-#: design/plone/contenttypes/interfaces/servizio.py:216
+#. Default: "Unità organizzativa responsabile"
+#: design/plone/contenttypes/interfaces/servizio.py:302
 msgid "ufficio_responsabile_erogazione"
 msgstr ""
 
 #. Default: "Seleziona gli uffici responsabili dell'erogazione di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:217
+#: design/plone/contenttypes/interfaces/servizio.py:306
 msgid "ufficio_responsabile_help"
 msgstr ""
 
 #. Default: "Ufficio di riferimento"
 #: design/plone/contenttypes/interfaces/pratica.py:17
 msgid "ufficio_riferimento"
 msgstr ""
@@ -2660,56 +2651,56 @@
 msgstr ""
 
 #. Default: "Seleziona la lista delle unità amministrative responsabili di questo argomento."
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:48
 msgid "unita_amministrative_responsabili_help"
 msgstr ""
 
+#. Default: "Seleziona l'organizzazione presso la quale svolge l'incarico."
+#: design/plone/contenttypes/interfaces/incarico.py:64
+msgid "unita_organizzativa_incarico_help"
+msgstr ""
+
+#. Default: "Unità organizzativa"
+#: design/plone/contenttypes/interfaces/incarico.py:60
+msgid "unita_organizzativa_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione dei compiti assegnati alla struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:19
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:23
 msgid "uo_competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:18
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:22
 msgid "uo_competenze_label"
 msgstr ""
 
-#. Default: "Inserisci eventuali informazioni di contatto aggiuntive non contemplate nei campi precedenti. Utilizza questo campo se ci sono dei contatti aggiuntivi rispetto ai contatti della sede principale. Se inserisci un collegamento con un indirizzo email, aggiungi \"mailto:\" prima dell'indirizzo, per farlo aprire direttamente nel client di posta."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:139
-msgid "uo_contact_info_description"
-msgstr ""
-
 #. Default: "Note di aggiornamento"
-#: design/plone/contenttypes/behaviors/update_note.py:16
+#: design/plone/contenttypes/behaviors/update_note.py:17
 msgid "update_note_label"
 msgstr ""
 
+#. Default: "Il valore del punto di contatto: il numero compreso di prefisso internazionale (se telefono), l'account (se social network), l'URL (se sito o pagina web), l'indirizzo email (se email)."
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:54
+msgid "value_punto_contatto_help"
+msgstr ""
+
 #. Default: "Vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:196
+#: design/plone/contenttypes/interfaces/servizio.py:282
 msgid "vincoli"
 msgstr ""
 
 #. Default: "Descrizione degli eventuali vincoli presenti."
-#: design/plone/contenttypes/interfaces/servizio.py:198
+#: design/plone/contenttypes/interfaces/servizio.py:284
 msgid "vincoli_help"
 msgstr ""
 
-#. Default: "Indicare un indirizzo web di riferimento a questo evento."
-#: design/plone/contenttypes/behaviors/evento.py:138
-msgid "web_event_help"
-msgstr ""
-
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/evento.py:137
-msgid "web_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo web di riferimento."
-#: design/plone/contenttypes/behaviors/contatti.py:53
-msgid "web_help"
+#. Default: "Mostra i PDF in anteprima"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:12
+msgid "visualize_files_title"
 msgstr ""
 
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/contatti.py:52
-msgid "web_label"
+#. Default: "Permette di aprire l'anteprima di tutti i PDF di questa cartella in una tab separata, altrimenti i PDF vengono scaricati"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:13
+msgid "visulize_files_description"
 msgstr ""
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,506 +1,491 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-01-13 13:15+0000\n"
+"POT-Creation-Date: 2024-03-18 13:30+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
-msgid "Abitazione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:36
-msgid "Accesso al trasporto pubblico"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:59
-msgid "Accesso luoghi della cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:18
+msgid "Accesso all'informazione"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:33
 msgid "Accettare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:34
-msgid "Accordo tra enti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:19
 msgid "Acqua"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
+#: design/plone/contenttypes/behaviors/configure.zcml:223
 msgid "Address Event"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Address UO"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:186
+#: design/plone/contenttypes/behaviors/configure.zcml:215
 msgid "Address Venue"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:19
 msgid "Adds fields."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:28
-msgid "Agricoltura, pesca, silvicoltura e prodotti alimentari"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "After Plone6 migration syndication is broken"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:22
-msgid "All the already existing News Types"
-msgstr "Tipologie Notizie presenti sul sito"
-
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:63
-msgid "All the selected items will be moved to indicated path"
-msgstr "Tutti gli elementi selezionati saranno spostati nella cartella indicata"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:20
+msgid "Agricoltura"
+msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:20
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:30
 msgid "All the already existing News Types"
 msgstr "I tipi delle notizie che esistono sul sito"
 
-#: design/plone/contenttypes/vocabularies/dataset.py:36
-msgid "Ambiente"
-msgstr ""
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:113
+msgid "All the selected items will be moved to indicated path"
+msgstr "Tutti gli elementi selezionati saranno spostati nella cartella indicata"
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:21
 msgid "Animale domestico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
-msgid "Anziano"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/bando.py:134
-#: design/plone/contenttypes/interfaces/documento.py:67
-#: design/plone/contenttypes/interfaces/servizio.py:239
+#: design/plone/contenttypes/interfaces/bando.py:135
+#: design/plone/contenttypes/interfaces/documento.py:97
+#: design/plone/contenttypes/interfaces/servizio.py:328
 msgid "Area"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
-msgid "Area di parcheggio"
-msgstr ""
-
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Argomenti"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:76
+#: design/plone/contenttypes/behaviors/configure.zcml:94
 msgid "Argomenti Bando"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:58
+#: design/plone/contenttypes/behaviors/configure.zcml:76
 msgid "Argomenti Document"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:67
+#: design/plone/contenttypes/behaviors/configure.zcml:85
 msgid "Argomenti Documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:28
+#: design/plone/contenttypes/behaviors/configure.zcml:112
+msgid "Argomenti Link"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/argomenti.py:32
 msgid "Argomenti correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
 msgid "Argomento"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:73
+#: design/plone/contenttypes/behaviors/configure.zcml:103
+msgid "Argomento Servizio"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:22
+msgid "Aria"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:65
 msgid "Assessore di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
-msgid "Associazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:23
+msgid "Assistenza agli invalidi"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:24
+msgid "Assistenza sociale"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:25
+msgid "Associazioni"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:29
 msgid "Attivare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:33
-msgid "Atto normativo"
+#: design/plone/contenttypes/interfaces/incarico.py:121
+msgid "Atto di nomina"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:86
 msgid "Autore"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:30
 msgid "Autorizzare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:65
-msgid "Avvio impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:66
-msgid "Avvio nuova attività professionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:69
-msgid "Avvio/registrazione filiale"
+#: design/plone/contenttypes/behaviors/configure.zcml:223
+msgid "Behavior address per Event."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:78
-msgid "Bancarotta"
+#: design/plone/contenttypes/behaviors/configure.zcml:215
+msgid "Behavior address per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:194
-msgid "Behavior address per Event."
+#: design/plone/contenttypes/behaviors/configure.zcml:263
+msgid "Behavior contatti per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:178
-msgid "Behavior address per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:255
+msgid "Behavior contatti per Persona."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:186
-msgid "Behavior address per Venue."
+#: design/plone/contenttypes/behaviors/configure.zcml:247
+msgid "Behavior contatti per Servizio."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
 msgid "Behavior contatti per UO."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:210
+#: design/plone/contenttypes/behaviors/configure.zcml:239
 msgid "Behavior contatti per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:234
+#: design/plone/contenttypes/behaviors/configure.zcml:279
 msgid "Behavior geolocatable per Event."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
-msgid "Behavior geolocatable per UO."
+#: design/plone/contenttypes/behaviors/configure.zcml:271
+msgid "Behavior geolocatable per Venue."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:226
-msgid "Behavior geolocatable per Venue."
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
+msgid "Bilancio"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:18
 msgid "CAP"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:43
-msgid "Cambio di residenza/domicilio"
+#: design/plone/contenttypes/behaviors/configure.zcml:306
+msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:261
-msgid "Campi aggiuntivi per la sezione amministrazione trasparente."
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Campo per escludere un contenuto dalle ricerche del sito."
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
+#: design/plone/contenttypes/behaviors/configure.zcml:315
 msgid "Campo per le note di aggiornamento."
 msgstr ""
 
+#: design/plone/contenttypes/interfaces/servizio.py:183
+msgid "Canale fisico"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:26
 msgid "Canon 5D IV"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 msgid "Cartella Modulistica"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:11
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:13
 msgid "Change News Type"
 msgstr "Cambia la Tipologia Notizia"
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:75
-msgid "Chiusura filiale"
+#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
+msgid "Città"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:74
-msgid "Chiusura impresa e attività professionale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
+msgid "Commercio al minuto"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/geolocation_defaults.py:23
-msgid "Città"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
+msgid "Commercio all'ingrosso"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:39
-msgid "Compravendita/affitto casa/edifici/terreni, costruzione o ristrutturazione casa/edificio	"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
+msgid "Commercio ambulante"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
-msgid "Comunicazione"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:30
+msgid "Comunicazione istituzionale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
-msgid "Condizioni e organizzazione del lavoro"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+msgid "Comunicazione politica"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:57
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:32
+msgid "Concorsi"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:104
 msgid "Contained by"
 msgstr "Contenuto da"
 
-#: design/plone/contenttypes/behaviors/configure.zcml:202
+#: design/plone/contenttypes/behaviors/configure.zcml:231
+#: design/plone/contenttypes/behaviors/contatti.py:112
 msgid "Contatti"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:33
 msgid "Coordinate"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/argomenti.py:42
+#: design/plone/contenttypes/behaviors/argomenti.py:46
 msgid "Correlato in evidenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
-msgid "Cultura"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:33
+msgid "Covid - 19"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:130
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 msgid "Dataset"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:134
 msgid "Dataset collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:104
+#: design/plone/contenttypes/behaviors/configure.zcml:141
 msgid "Dataset correlati"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:31
 msgid "Delegare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:52
-msgid "Denuncia crimini"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:143
+#: design/plone/contenttypes/behaviors/configure.zcml:180
 msgid "Descrizione estesa"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:160
+#: design/plone/contenttypes/behaviors/configure.zcml:197
 msgid "Descrizione estesa documento"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:152
+#: design/plone/contenttypes/behaviors/configure.zcml:189
 msgid "Descrizione estesa servizio"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Design Plone: Content-types"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Design Plone: Content-types (behaviors)"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Design Plone: Content-types (uninstall)"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Design Plone: Content-types to 3000"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:55
-msgid "Dichiarazione dei redditi, versamento e riscossione tributi/imposte e contributi"
+#: design/plone/contenttypes/configure.zcml:66
+msgid "Design Plone: Fix Syndication after Plone6 Migration"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:145
+#: design/plone/contenttypes/behaviors/trasparenza.py:146
 msgid "Dirigente"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:27
-msgid "Documenti albo pretorio"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:134
+msgid "Documenti pubblici"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/servizio.py:252
+#: design/plone/contenttypes/interfaces/servizio.py:341
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Documento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:41
-msgid "Documento (tecnico) di supporto"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
 msgid "Documento Personale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:37
-msgid "Documento attivita politica"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:31
-msgid "Documento funzionamento interno"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:30
-msgid "Economia e Finanze"
-msgstr ""
-
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "Edit"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
-msgid "Elezione"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:35
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
-msgid "Energia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+msgid "Elezioni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:28
-msgid "Famiglia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
+msgid "Energie rinnovabili"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:26
-msgid "Fanciullo"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:36
+msgid "Estero"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:70
-msgid "Finanziamento impresa"
+#: design/plone/contenttypes/behaviors/configure.zcml:324
+msgid "Exclude from search"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:28
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:51
 msgid "Find news with the indicated Path, put attention than generaly sites have the root name \"/Plone/\""
 msgstr "Trova le notizie in path indicato. Attenzione, in maggior parte dei casi il sito ha il nome \"/Plone/\""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:21
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:29
 msgid "Find news with this News Type"
 msgstr "Trova le notizie con la Tipologia Notizia indicata"
 
-#: design/plone/contenttypes/configure.zcml:52
+#: design/plone/contenttypes/configure.zcml:58
 msgid "Fix control panel of design.plone.contenttypes add-on."
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
+msgid "Foreste"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/tags_vocabulary.py:38
 msgid "Formazione professionale"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:218
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:39
+msgid "Gemellaggi"
+msgstr ""
+
+#: design/plone/contenttypes/behaviors/configure.zcml:271
 msgid "Geolocatable"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:43
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Geolocation default"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
-msgid "Gestione dei rifiuti"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:71
-msgid "Gestione personale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:27
-msgid "Giovane"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:40
+msgid "Gestione rifiuti"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:30
 msgid "Giovanni"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:42
-msgid "Giustizia, sistema giuridico e sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:41
+msgid "Giustizia"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:37
-msgid "Governo e settore pubblico"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:42
+msgid "Igiene pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+#: design/plone/contenttypes/browser/utils/change_news_type.py:32
+#: design/plone/contenttypes/browser/utils/move_news_items.py:74
+msgid "Il vocabolario dei valori non è stato trovato"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
 msgid "Immigrazione"
 msgstr ""
 
-#: design/plone/contenttypes/controlpanels/settings.py:154
+#: design/plone/contenttypes/controlpanels/settings.py:106
 #: design/plone/contenttypes/profiles/default/controlpanel.xml
 msgid "Impostazioni Design Plone"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:33
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+msgid "Imposte"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:45
+msgid "Imprese"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/persona.py:68
+msgid "Incarichi"
+msgstr ""
+
+#: design/plone/contenttypes/profiles/default/types/Incarico.xml
+msgid "Incarico"
+msgstr ""
+
+#: design/plone/contenttypes/browser/utils/move_news_items.py:34
 msgid "Indicated path is not valid"
 msgstr "Path indicato non è valido"
 
-#: design/plone/contenttypes/behaviors/configure.zcml:170
+#: design/plone/contenttypes/behaviors/configure.zcml:207
 msgid "Info per la testata"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:32
 msgid "Informare"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
-msgid "Informatica e trattamento dei dati"
+#: design/plone/contenttypes/behaviors/contatti.py:34
+msgid "Informazioni di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
 msgid "Inquinamento"
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:36
+#: design/plone/contenttypes/configure.zcml:32
 msgid "Installs the design.plone.contenttypes add-on."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:34
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:47
 msgid "Integrazione sociale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:28
-msgid "Invalidità"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:26
 msgid "Iscriversi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:26
-msgid "Iscrizione scuola/università e/o richiesta borsa di studio"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:43
-msgid "Istanza"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:48
+msgid "Isolamento termico"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:31
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:49
 msgid "Istruzione"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:33
-msgid "Istruzione, cultura e sport"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:47
+#: design/plone/contenttypes/browser/utils/move_news_items.py:48
 msgid "Items moved with success"
 msgstr "Gli elementi sono stati spostati con successo"
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:50
+msgid "Lavoro"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:28
 msgid "Leggere"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:85
+#: design/plone/contenttypes/behaviors/configure.zcml:122
 msgid "Luoghi correlati"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:44
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
 msgid "Matrimonio"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:49
-msgid "Matrimonio e/o cambio stato civile"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:52
+msgid "Mercato"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Messaggio.xml
 msgid "Messaggio"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:29
@@ -511,529 +496,536 @@
 msgid "Metadati luogo"
 msgstr ""
 
 #: design/plone/contenttypes/behaviors/configure.zcml:39
 msgid "Metadati news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/document_types_vocabulary.py:28
-msgid "Modulistica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:53
+msgid "Mobilità sostenibile"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Modulo"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:50
-msgid "Morte ed eredità"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
+msgid "Morte"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Mostra la data di modifica."
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:70
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:124
 msgid "Move"
 msgstr "Sposta"
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:11
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:13
 msgid "Move News Items"
 msgstr "Sposta le notizie"
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:62
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:110
 msgid "Move to Path"
 msgstr "Sposta nella cartella"
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Multi File"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:48
-msgid "Nascita di un bambino, richiesta adozioni"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
+msgid "Nascita"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:28
 msgid "Nazione"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:21
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:20
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:26
 msgid "News Type"
 msgstr "Tipologia Notizia"
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:30
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:48
 msgid "News Type to substitute"
 msgstr "Tipologia Notizia da sostituire"
 
 #. Default: "Nome e cognome"
-#: design/plone/contenttypes/restapi/services/types/get.py:152
+#: design/plone/contenttypes/restapi/services/types/get.py:163
 msgid "Nome e Cognome"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:73
-msgid "Notifiche autorità"
-msgstr ""
-
-#: design/plone/contenttypes/interfaces/persona.py:48
+#: design/plone/contenttypes/interfaces/persona.py:51
 msgid "Organizzazione di riferimento"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:72
-msgid "Pagamento tasse, iva e dogane"
-msgstr ""
-
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:25
 msgid "Pagare"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:29
 msgid "Paperino"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:81
-msgid "Partecipazione ad appalti pubblici nazionali e trasfrontalieri"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
+msgid "Parcheggi"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:33
-msgid "Pensionamento"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
+msgid "Patrimonio culturale"
 msgstr ""
 
-#: design/plone/contenttypes/profiles/default/types/Persona.xml
+#: design/plone/contenttypes/interfaces/incarico.py:54
 msgid "Persona"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/evento.py:50
-msgid "Persona dell'amministrazione"
+#: design/plone/contenttypes/profiles/default/types/Persona.xml
+msgid "Persona pubblica"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:92
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:84
 msgid "Persone della struttura"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+msgid "Pesca"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
+msgid "Piano di sviluppo"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:27
 msgid "Pippo"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+msgid "Pista ciclabile"
+msgstr ""
+
 #: design/plone/contenttypes/vocabularies/mockup.py:28
 msgid "Pluto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:45
-msgid "Popolazione e società"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:61
+msgid "Politica commerciale"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:60
-msgid "Possesso, cura, smarrimento animale da compagnia"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:62
+msgid "Polizia"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Pratica.xml
 msgid "Pratica"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:51
-msgid "Prenotazione e disdetta visite/esami"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:63
+msgid "Prodotti alimentari"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:35
-msgid "Protezione sociale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:64
+msgid "Protezione civile"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:13
-msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
+#: design/plone/contenttypes/behaviors/contatti.py:78
+msgid "Punti di contatto"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:13
-msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
+#: design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+msgid "Punto di Contatto"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:44
-msgid "Regioni e città"
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:15
+msgid "Questo tool viene usato per cambiare il valore del campo 'Tipologia Notizia' in tutte le notizie che hanno il valore del campo selezionato. Fa anche il giro su tutti i blocchi elenco"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:68
-msgid "Registrazione impresa transfrontalier"
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:15
+msgid "Questo tool viene usato per trovare e spostare le Notizie con una Tipologia Notizia determinata."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:35
-msgid "Registrazione/possesso veicolo"
+#: design/plone/contenttypes/configure.zcml:41
+msgid "Registers taxonomies."
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:45
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:65
+msgid "Residenza"
+msgstr ""
+
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:49
 msgid "Responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/trasparenza.py:129
-msgid "Responsabile procedimento"
+#: design/plone/contenttypes/interfaces/incarico.py:89
+msgid "Responsabile della struttura"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:31
-msgid "Ricerca di lavoro, avvio nuovo lavoro, disoccupazione"
+#: design/plone/contenttypes/behaviors/trasparenza.py:130
+msgid "Responsabile procedimento"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
 msgid "RicevutaPagamento"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/lista_azioni_pratica.py:27
 msgid "Richiedere"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:67
-msgid "Richiesta licenze/permessi/certificati"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:34
-msgid "Richiesta o rinnovo patente"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:46
-msgid "Richiesta passaporto, visto e assistenza viaggi internazionali"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:76
-msgid "Ristrutturazione impresa"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/dataset.py:38
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:54
-msgid "Salute"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:66
+msgid "Risposta alle emergenze"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:46
-msgid "Scienza e tecnologia"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/templates/move_news_items.pt:27
+#: design/plone/contenttypes/browser/utils/templates/move_news_items.pt:47
 msgid "Search Path"
 msgstr "Cartella della ricerca"
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:114
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:104
 msgid "Sede"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:114
+#: design/plone/contenttypes/behaviors/configure.zcml:151
 msgid "Servizi correlati"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Servizio.xml
 msgid "Servizio"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/documento_personale.py:101
 msgid "Servizio collegato"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:252
+#: design/plone/contenttypes/behaviors/configure.zcml:297
 msgid "Show modified"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:56
-msgid "Sicurezza internazionale"
-msgstr ""
-
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:55
-msgid "Sicurezza pubblica"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:67
+msgid "Sistema giuridico"
 msgstr ""
 
 #: design/plone/contenttypes/vocabularies/mockup.py:25
 msgid "Sony Aplha 7R III"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:57
-msgid "Spazio verde"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:68
+msgid "Spazio Verde"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:58
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:69
 msgid "Sport"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:37
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:41
 msgid "Struttura"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:20
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:21
 msgid "Struttura politica coinvolta"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/luogo.py:74
+#: design/plone/contenttypes/behaviors/luogo.py:75
 msgid "Struttura responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:124
+#: design/plone/contenttypes/behaviors/configure.zcml:161
 msgid "Strutture correlate"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:29
-msgid "Studente"
-msgstr ""
-
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:43
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:74
 msgid "Substitute"
 msgstr "Sostituisci"
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:70
+msgid "Sviluppo sostenibile"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:71
+msgid "Tassa sui servizi"
+msgstr ""
+
 #: design/plone/contenttypes/behaviors/configure.zcml:49
 msgid "Tassonomia argomenti"
 msgstr ""
 
+#: design/plone/contenttypes/behaviors/configure.zcml:67
+msgid "Tassonomia argomenti evento"
+msgstr ""
+
 #: design/plone/contenttypes/behaviors/configure.zcml:58
-msgid "Tassonomia argomenti per i Document"
+msgid "Tassonomia argomenti news"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/dataset.py:39
-msgid "Tematiche internazionali"
+#: design/plone/contenttypes/behaviors/configure.zcml:76
+msgid "Tassonomia argomenti per i Document"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:46
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:72
 msgid "Tempo libero"
 msgstr ""
 
-#: design/plone/contenttypes/browser/manage_content/templates/change_news_type.pt:31
+#: design/plone/contenttypes/browser/utils/templates/change_news_type.pt:52
 msgid "The News Type selected above will be substituted by the selected value"
 msgstr "La Tipologia Notizia indicata sopra sarà sostituita dalla tipologia notizia selezionata"
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:97
+#: design/plone/contenttypes/browser/utils/change_news_type.py:108
 msgid "The News Types was changed with success"
 msgstr "Le Tiplogie Notizie sono state sostituite con successo"
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:55
+#: design/plone/contenttypes/browser/utils/change_news_type.py:64
 msgid "The new News Type was not found between available values"
 msgstr "La Tipologia Notizia nuova non è stata trovata tra i valori possibli"
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:49
+#: design/plone/contenttypes/browser/utils/change_news_type.py:58
 msgid "The new type field was not populated"
 msgstr "Il campo della avitabile Tipologia Notizia non è stato popolato"
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:61
+#: design/plone/contenttypes/browser/utils/change_news_type.py:70
 msgid "The old News Type was not found between available values"
 msgstr "La Tipologia Notizia vecchia non è stata trovata tra i valori possibli"
 
-#: design/plone/contenttypes/browser/manage_content/change_news_type.py:43
+#: design/plone/contenttypes/browser/utils/change_news_type.py:52
 msgid "The old type field was not populated"
 msgstr "l campo della Tipologia Notizia esistente non è stato popolato"
 
-#: design/plone/contenttypes/browser/manage_content/move_news_items.py:51
+#: design/plone/contenttypes/browser/utils/move_news_items.py:52
 msgid "The path was not indicated"
 msgstr "Il path non è stato indicato"
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:51
-msgid "Traffico urbano"
-msgstr ""
-
-#: design/plone/contenttypes/behaviors/configure.zcml:261
+#: design/plone/contenttypes/behaviors/configure.zcml:306
 msgid "Trasparenza"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:43
-msgid "Trasporto"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:73
+msgid "Trasparenza amministrativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:59
-msgid "Trasporto stradale"
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:74
+msgid "Trasporto pubblico"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:243
+#: design/plone/contenttypes/behaviors/configure.zcml:288
 msgid "Tre campi file aggiuntivi."
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:60
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:75
 msgid "Turismo"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:117
-#: design/plone/contenttypes/interfaces/documento.py:50
-#: design/plone/contenttypes/interfaces/servizio.py:225
+#: design/plone/contenttypes/interfaces/bando.py:118
+#: design/plone/contenttypes/interfaces/documento.py:80
 msgid "Ufficio responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:134
+#: design/plone/contenttypes/behaviors/configure.zcml:171
 msgid "Ulteriori campi aiuto testuali"
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/Modulo.xml
 msgid "Un modulo compilabile."
 msgstr ""
 
-#: design/plone/contenttypes/configure.zcml:45
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:15
+msgid "Una raccolta di utility per i contenuti agid"
+msgstr ""
+
+#: design/plone/contenttypes/configure.zcml:50
 msgid "Uninstalls the design.plone.contenttypes add-on."
 msgstr ""
 
 #: design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
 msgid "Unita Organizzativa"
 msgstr ""
 
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:45
 msgid "Unità amministrative responsabili"
 msgstr ""
 
-#: design/plone/contenttypes/behaviors/configure.zcml:270
-msgid "Update note"
+#: design/plone/contenttypes/interfaces/incarico.py:71
+msgid "Unità organizzativa"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:37
-msgid "Urbanistica ed edilizia"
+#: design/plone/contenttypes/interfaces/servizio.py:314
+msgid "Unità organizzativa responsabile"
 msgstr ""
 
-#: design/plone/contenttypes/vocabularies/all_life_events_vocabulary.py:77
-msgid "Vendita impresa"
+#: design/plone/contenttypes/behaviors/configure.zcml:315
+msgid "Update note"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:76
+msgid "Urbanizzazione"
 msgstr ""
 
 #: design/plone/contenttypes/controlpanels/geolocation_defaults.py:13
 msgid "Via"
 msgstr ""
 
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:77
+msgid "Viaggi"
+msgstr ""
+
 #: design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
 #: design/plone/contenttypes/profiles/default/types/Dataset.xml
 #: design/plone/contenttypes/profiles/default/types/Documento.xml
 msgid "View"
 msgstr ""
 
-#. Default: "A chi si rivolge questo servizio e chi può usufruirne."
-#: design/plone/contenttypes/interfaces/servizio.py:53
+#: design/plone/contenttypes/browser/utils/templates/utils.pt:13
+msgid "Viste di utility per Design Plone Contenttypes"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:79
+msgid "ZTL"
+msgstr ""
+
+#: design/plone/contenttypes/vocabularies/tags_vocabulary.py:78
+msgid "Zone pedonali"
+msgstr ""
+
+#. Default: "Descrizione testuale dei principali destinatari dell'Evento"
+#: design/plone/contenttypes/behaviors/evento.py:43
+#: design/plone/contenttypes/interfaces/servizio.py:98
 msgid "a_chi_si_rivolge_help"
 msgstr ""
 
-#. Default: "A chi si rivolge"
-#: design/plone/contenttypes/interfaces/servizio.py:51
+#. Default: "A chi è rivolto"
+#: design/plone/contenttypes/behaviors/evento.py:41
+#: design/plone/contenttypes/interfaces/servizio.py:96
 msgid "a_chi_si_rivolge_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio di comunicazione responsabile di questa notizia/comunicato stampa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:47
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:39
 msgid "a_cura_di_help"
 msgstr ""
 
 #. Default: "A cura di"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:46
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
 msgid "a_cura_di_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di persone dell'amministrazione citate in questa notizia/comunicato stampa. Questa informazione verrà mostrata nella sezione \"A cura di\"."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:59
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:51
 msgid "a_cura_di_persone_help"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:58
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:50
 msgid "a_cura_di_persone_label"
 msgstr ""
 
 #. Default: "Accedere al servizio"
-#: design/plone/contenttypes/interfaces/servizio.py:370
+#: design/plone/contenttypes/interfaces/servizio.py:481
 msgid "accedi_al_servizio_label"
 msgstr ""
 
 #. Default: "Modalità di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:171
+#: design/plone/contenttypes/behaviors/luogo.py:140
 msgid "accesso_label"
 msgstr ""
 
 #. Default: "Allegato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:56
 msgid "allegato"
 msgstr ""
 
 #. Default: "Indicare, se esistono, altre modalità di invio."
-#: design/plone/contenttypes/behaviors/trasparenza.py:189
+#: design/plone/contenttypes/behaviors/trasparenza.py:190
 msgid "altre_modalita_invio_help"
 msgstr ""
 
 #. Default: "Altre modalità di invio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:185
+#: design/plone/contenttypes/behaviors/trasparenza.py:186
 msgid "altre_modalita_invio_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei documenti di supporto collegati a questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:246
+#: design/plone/contenttypes/interfaces/servizio.py:335
 msgid "altri_documenti_help"
 msgstr ""
 
 #. Default: "Date and time of the opening of the announcement. Use this field if you want to set a specific opening date. If not set, the announcement will be open immediately."
-#: design/plone/contenttypes/interfaces/bando.py:56
+#: design/plone/contenttypes/interfaces/bando.py:57
 msgid "apertura_bando_help"
 msgstr ""
 
 #. Default: "Opening date"
-#: design/plone/contenttypes/interfaces/bando.py:55
+#: design/plone/contenttypes/interfaces/bando.py:56
 msgid "apertura_bando_label"
 msgstr ""
 
 #. Default: "Area"
-#: design/plone/contenttypes/interfaces/servizio.py:231
+#: design/plone/contenttypes/interfaces/servizio.py:320
 msgid "area"
 msgstr ""
 
 #. Default: "Seleziona l'area da cui dipende questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:234
+#: design/plone/contenttypes/interfaces/servizio.py:323
 msgid "area_help"
 msgstr ""
 
 #. Default: "Area responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:73
 msgid "area_responsabile_documento_personale"
 msgstr ""
 
 #. Default: "Seleziona l'area amministrativa responsabile del documento."
-#: design/plone/contenttypes/interfaces/bando.py:127
-#: design/plone/contenttypes/interfaces/documento.py:60
+#: design/plone/contenttypes/interfaces/bando.py:128
+#: design/plone/contenttypes/interfaces/documento.py:90
 msgid "area_responsabile_help"
 msgstr ""
 
 #. Default: "Area responsabile del documento"
-#: design/plone/contenttypes/interfaces/bando.py:123
-#: design/plone/contenttypes/interfaces/documento.py:56
+#: design/plone/contenttypes/interfaces/bando.py:124
+#: design/plone/contenttypes/interfaces/documento.py:86
 msgid "area_responsabile_label"
 msgstr ""
 
 #. Default: "Argomenti utenti"
 #: design/plone/contenttypes/interfaces/documento_personale.py:42
 msgid "argomenti_utenti"
 msgstr ""
 
 #. Default: "Inserire l'assessore di riferimento della struttura, se esiste."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:76
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:68
 msgid "assessore_riferimento_help"
 msgstr ""
 
+#. Default: "Assessore di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:61
+msgid "assessore_riferimento_title"
+msgstr ""
+
 #. Default: "Indicare, se la esistono, atti e documenti a corredo dell'istanza."
-#: design/plone/contenttypes/behaviors/trasparenza.py:200
+#: design/plone/contenttypes/behaviors/trasparenza.py:201
 msgid "atti_documenti_corredo_help"
 msgstr ""
 
 #. Default: "Atti e documenti a corredo dell'istanza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:196
+#: design/plone/contenttypes/behaviors/trasparenza.py:197
 msgid "atti_documenti_corredo_label"
 msgstr ""
 
-#. Default: "Inserire un file contenente l'atto di nomina della persona."
-#: design/plone/contenttypes/interfaces/persona.py:160
-msgid "atto_nomina_help"
+#. Default: "Inserire riferimento all'atto di nomina della persona"
+#: design/plone/contenttypes/interfaces/incarico.py:114
+msgid "atto_nomina_incarico_help"
 msgstr ""
 
 #. Default: "Atto di nomina"
-#: design/plone/contenttypes/interfaces/persona.py:158
-msgid "atto_nomina_label"
-msgstr ""
-
-#. Default: "Autenticazione"
-#: design/plone/contenttypes/interfaces/servizio.py:121
-msgid "autenticazione"
-msgstr ""
-
-#. Default: "Indicare, se previste, le modalità di autenticazione necessarie per poter accedere al servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:122
-msgid "autenticazione_help"
+#: design/plone/contenttypes/interfaces/incarico.py:110
+msgid "atto_nomina_incarico_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di autori che hanno pubblicato il documento. Possono essere Persone o Unità Organizzative."
-#: design/plone/contenttypes/interfaces/documento.py:76
+#: design/plone/contenttypes/interfaces/documento.py:106
 msgid "autori_help"
 msgstr ""
 
 #. Default: "Autore/i"
-#: design/plone/contenttypes/interfaces/documento.py:72
+#: design/plone/contenttypes/interfaces/documento.py:102
 msgid "autori_label"
 msgstr ""
 
 #. Default: "Azioni"
 #: design/plone/contenttypes/interfaces/messaggio.py:28
 msgid "azioni_pratica"
 msgstr ""
@@ -1045,662 +1037,688 @@
 
 #. Default: "Azioni utente"
 #: design/plone/contenttypes/interfaces/pratica.py:47
 msgid "azioni_utente"
 msgstr ""
 
 #. Default: "Solo per persona politica: testo descrittivo che riporta la biografia della persona."
-#: design/plone/contenttypes/interfaces/persona.py:107
+#: design/plone/contenttypes/interfaces/persona.py:94
 msgid "biografia_help"
 msgstr ""
 
 #. Default: "Biografia"
-#: design/plone/contenttypes/interfaces/persona.py:106
+#: design/plone/contenttypes/interfaces/persona.py:93
 msgid "biografia_label"
 msgstr ""
 
 #. Default: "Canale digitale"
-#: design/plone/contenttypes/interfaces/servizio.py:111
+#: design/plone/contenttypes/interfaces/servizio.py:156
 msgid "canale_digitale"
 msgstr ""
 
-#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:112
+#. Default: "Testo di introduzione del canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:157
 msgid "canale_digitale_help"
 msgstr ""
 
+#. Default: "Link al canale digitale"
+#: design/plone/contenttypes/interfaces/servizio.py:165
+msgid "canale_digitale_link"
+msgstr ""
+
+#. Default: "Collegamento con l'eventuale canale digitale di attivazione del servizio."
+#: design/plone/contenttypes/interfaces/servizio.py:166
+msgid "canale_digitale_link_help"
+msgstr ""
+
 #. Default: "Canale digitale servizio collegato"
 #: design/plone/contenttypes/interfaces/documento_personale.py:108
 msgid "canale_digitale_servizio"
 msgstr ""
 
+#. Default: "Canale fisico"
+#: design/plone/contenttypes/interfaces/servizio.py:175
+msgid "canale_fisico"
+msgstr ""
+
+#. Default: "Unità organizzative per la fruizione del servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:176
+msgid "canale_fisico_help"
+msgstr ""
+
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:205
+#: design/plone/contenttypes/interfaces/servizio.py:291
 msgid "casi_particolari"
 msgstr ""
 
 #. Default: "Descrizione degli evetuali casi particolari riferiti alla fruibilità di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:207
+#: design/plone/contenttypes/interfaces/servizio.py:293
 msgid "casi_particolari_help"
 msgstr ""
 
 #. Default: "Casi particolari"
-#: design/plone/contenttypes/interfaces/servizio.py:401
+#: design/plone/contenttypes/interfaces/servizio.py:514
 msgid "casi_particolari_label"
 msgstr ""
 
 #. Default: "Descrizione di chi può presentare domanda per usufruire del servizio e delle diverse casistiche."
-#: design/plone/contenttypes/interfaces/servizio.py:62
+#: design/plone/contenttypes/interfaces/servizio.py:107
 msgid "chi_puo_presentare_help"
 msgstr ""
 
 #. Default: "Chi può presentare"
-#: design/plone/contenttypes/interfaces/servizio.py:60
+#: design/plone/contenttypes/interfaces/servizio.py:105
 msgid "chi_puo_presentare_label"
 msgstr ""
 
 #. Default: "Circoscrizione"
 #: design/plone/contenttypes/behaviors/address.py:37
 msgid "circoscrizione"
 msgstr ""
 
 #. Default: "Codice dell'ente erogatore (ipa)"
-#: design/plone/contenttypes/interfaces/servizio.py:268
+#: design/plone/contenttypes/interfaces/servizio.py:357
 msgid "codice_ipa"
 msgstr ""
 
 #. Default: "Specificare il nome dell’organizzazione, come indicato nell’Indice della Pubblica Amministrazione (IPA), che esercita uno specifico ruolo sul Servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:270
+#: design/plone/contenttypes/interfaces/servizio.py:359
 msgid "codice_ipa_help"
 msgstr ""
 
-#. Default: "Come si fa"
-#: design/plone/contenttypes/interfaces/servizio.py:80
+#. Default: "Come fare"
+#: design/plone/contenttypes/interfaces/servizio.py:125
 msgid "come_si_fa"
 msgstr ""
 
 #. Default: "Descrizione della procedura da seguire per poter usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:82
+#: design/plone/contenttypes/interfaces/servizio.py:127
 msgid "come_si_fa_help"
 msgstr ""
 
+#. Default: "Solo per incarico politico: compensi di qualsiasi natura connessi all'assunzione della carica."
+#: design/plone/contenttypes/interfaces/incarico.py:21
+msgid "compensi_incarico_help"
+msgstr ""
+
+#. Default: "Compensi"
+#: design/plone/contenttypes/interfaces/incarico.py:17
+msgid "compensi_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione del ruolo e dei compiti della persona."
-#: design/plone/contenttypes/interfaces/persona.py:69
+#: design/plone/contenttypes/interfaces/persona.py:77
 msgid "competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/persona.py:68
+#: design/plone/contenttypes/interfaces/persona.py:76
 msgid "competenze_label"
 msgstr ""
 
-#. Default: "Informazioni di contatto generiche"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:137
+#. Default: "Condizioni di servizio"
+#: design/plone/contenttypes/interfaces/servizio.py:388
+msgid "condizioni_di_servizio"
+msgstr ""
+
+#. Default: "Contatti dell'unità organizzativa."
+#: design/plone/contenttypes/behaviors/contatti.py:27
+msgid "contact_info_help"
+msgstr ""
+
+#. Default: "Punti di contatto dell'unità organizzativa"
+#: design/plone/contenttypes/behaviors/contatti.py:23
 msgid "contact_info_label"
 msgstr ""
 
 #. Default: "Contatti"
 #: design/plone/contenttypes/interfaces/pratica.py:44
 msgid "contatti"
 msgstr ""
 
 #. Default: "Contatti"
-#: design/plone/contenttypes/behaviors/address.py:52
-#: design/plone/contenttypes/behaviors/contatti.py:76
-#: design/plone/contenttypes/behaviors/evento.py:215
+#: design/plone/contenttypes/behaviors/contatti.py:57
+#: design/plone/contenttypes/behaviors/evento.py:170
+#: design/plone/contenttypes/behaviors/geolocation.py:18
 msgid "contatti_label"
 msgstr ""
 
 #. Default: "Contenuto"
 #: design/plone/contenttypes/interfaces/pratica.py:42
 msgid "contenuto"
 msgstr ""
 
 #. Default: "Indicare se il servizio si riferisce ad una particolare area geografica o all'intero territorio di riferimento."
-#: design/plone/contenttypes/interfaces/servizio.py:72
+#: design/plone/contenttypes/interfaces/servizio.py:117
 msgid "copertura_geografica_help"
 msgstr ""
 
 #. Default: "Copertura geografica"
-#: design/plone/contenttypes/interfaces/servizio.py:70
+#: design/plone/contenttypes/interfaces/servizio.py:115
 msgid "copertura_geografica_label"
 msgstr ""
 
 #. Default: "Contenuti collegati"
-#: design/plone/contenttypes/behaviors/argomenti.py:74
+#: design/plone/contenttypes/behaviors/argomenti.py:108
 #: design/plone/contenttypes/behaviors/dataset_correlati.py:40
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:43
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:120
 msgid "correlati_label"
 msgstr ""
 
 #. Default: "Seleziona un correlato da mettere in evidenza per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:36
+#: design/plone/contenttypes/behaviors/argomenti.py:40
 msgid "correlato_in_evidenza_help"
 msgstr ""
 
 #. Default: "Correlato in evidenza"
-#: design/plone/contenttypes/behaviors/argomenti.py:35
+#: design/plone/contenttypes/behaviors/argomenti.py:39
 msgid "correlato_in_evidenza_label"
 msgstr ""
 
-#. Default: "Cosa fa"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
+#. Default: "Competenze"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:201
 msgid "cosa_fa_label"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:177
+#: design/plone/contenttypes/interfaces/servizio.py:263
 msgid "cosa_serve"
 msgstr ""
 
 #. Default: "Descrizione delle istruzioni per usufruire del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:179
+#: design/plone/contenttypes/interfaces/servizio.py:265
 msgid "cosa_serve_help"
 msgstr ""
 
 #. Default: "Cosa serve"
-#: design/plone/contenttypes/interfaces/servizio.py:384
+#: design/plone/contenttypes/interfaces/servizio.py:497
 msgid "cosa_serve_label"
 msgstr ""
 
 #. Default: "Cosa si ottiene"
-#: design/plone/contenttypes/interfaces/servizio.py:90
+#: design/plone/contenttypes/interfaces/servizio.py:135
 msgid "cosa_si_ottiene"
 msgstr ""
 
 #. Default: "Indicare cosa si può ottenere dal servizio, ad esempio 'carta di identità elettronica', 'certificato di residenza'."
-#: design/plone/contenttypes/interfaces/servizio.py:91
+#: design/plone/contenttypes/interfaces/servizio.py:136
 msgid "cosa_si_ottiene_help"
 msgstr ""
 
 #. Default: "Cos'è"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:40
-#: design/plone/contenttypes/behaviors/evento.py:200
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:52
+#: design/plone/contenttypes/behaviors/evento.py:155
 msgid "cose_label"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/interfaces/servizio.py:186
+#: design/plone/contenttypes/interfaces/servizio.py:272
 msgid "costi"
 msgstr ""
 
 #. Default: "Costi e vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:389
+#: design/plone/contenttypes/interfaces/servizio.py:502
 msgid "costi_e_vincoli_label"
 msgstr ""
 
 #. Default: "Descrizione delle condizioni e dei termini economici per completare la procedura di richiesta del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:188
+#: design/plone/contenttypes/interfaces/servizio.py:274
 msgid "costi_help"
 msgstr ""
 
 #. Default: "Costi"
-#: design/plone/contenttypes/behaviors/evento.py:212
+#: design/plone/contenttypes/behaviors/evento.py:167
 msgid "costi_label"
 msgstr ""
 
 #. Default: "Allega un file contenente il curriculum vitae della persona. Se ha più file da allegare, utilizza questo campo per quello principale e gli altri mettili dentro alla cartella \"Curriculum vitae\" che troverai dentro alla Persona."
-#: design/plone/contenttypes/interfaces/persona.py:149
+#: design/plone/contenttypes/interfaces/persona.py:105
 msgid "curriculum_vitae_help"
 msgstr ""
 
 #. Default: "Curriculum vitae"
-#: design/plone/contenttypes/interfaces/persona.py:147
+#: design/plone/contenttypes/interfaces/persona.py:103
 msgid "curriculum_vitae_label"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction."
-#: design/plone/contenttypes/behaviors/trasparenza.py:254
+#: design/plone/contenttypes/behaviors/trasparenza.py:255
 msgid "customer_satisfaction_help"
 msgstr ""
 
 #. Default: "Risultati indagini di customer satisfaction"
-#: design/plone/contenttypes/behaviors/trasparenza.py:249
+#: design/plone/contenttypes/behaviors/trasparenza.py:250
 msgid "customer_satisfaction_label"
 msgstr ""
 
-#. Default: "Data di conclusione dell'incarico."
-#: design/plone/contenttypes/interfaces/persona.py:60
-msgid "data_conclusione_incarico_help"
-msgstr ""
-
 #. Default: "Data conclusione incarico"
-#: design/plone/contenttypes/interfaces/persona.py:56
-msgid "data_conclusione_incarico_label"
+#: design/plone/contenttypes/interfaces/incarico.py:100
+msgid "data_conclusione_incarico"
 msgstr ""
 
 #. Default: "Data e fasi intermedie"
 #: design/plone/contenttypes/interfaces/documento_personale.py:120
 msgid "data_e_fasi_intermedie"
 msgstr ""
 
 #. Default: "Data di inizio"
 #: design/plone/contenttypes/interfaces/documento_personale.py:116
 msgid "data_inizio"
 msgstr ""
 
-#. Default: "Solo per persona politica: specificare la data di insediamento."
-#: design/plone/contenttypes/interfaces/persona.py:97
-msgid "data_insediamento_help"
+#. Default: "Data inizio incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:95
+msgid "data_inizio_incarico"
 msgstr ""
 
 #. Default: "Data insediamento"
-#: design/plone/contenttypes/interfaces/persona.py:96
-msgid "data_insediamento_label"
+#: design/plone/contenttypes/interfaces/incarico.py:105
+msgid "data_insediamento"
 msgstr ""
 
 #. Default: "Data del messaggio"
 #: design/plone/contenttypes/interfaces/messaggio.py:12
 msgid "data_messaggio"
 msgstr ""
 
 #. Default: "Data pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:21
 msgid "data_pagamento"
 msgstr ""
 
 #. Default: "Data del protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:41
 #: design/plone/contenttypes/interfaces/documento_personale.py:19
 msgid "data_protocollo"
 msgstr ""
 
+#. Default: "Data scadenza"
+#: design/plone/contenttypes/interfaces/servizio.py:49
+msgid "data_scadenza_label"
+msgstr ""
+
 #. Default: "Data di scadenza della procedura"
 #: design/plone/contenttypes/interfaces/messaggio.py:40
 msgid "data_scadenza_procedura"
 msgstr ""
 
 #. Default: "Dataset"
-#: design/plone/contenttypes/interfaces/dataset.py:27
+#: design/plone/contenttypes/interfaces/dataset.py:20
 msgid "dataset"
 msgstr ""
 
+#. Default: "Schede dataset collegate al documento"
+#: design/plone/contenttypes/interfaces/documento.py:150
+msgid "dataset_collegati_help"
+msgstr ""
+
 #. Default: "Seleziona una lista di schede dataset collegate a questo contenuto."
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:20
 msgid "dataset_correlati_help"
 msgstr ""
 
 #. Default: "Dataset correlati"
-#: design/plone/contenttypes/behaviors/dataset_correlati.py:18
+#: design/plone/contenttypes/behaviors/dataset_correlati.py:19
 msgid "dataset_correlati_label"
 msgstr ""
 
+#. Default: "Dataset collegati"
+#: design/plone/contenttypes/interfaces/documento.py:146
+msgid "dataset_label"
+msgstr ""
+
+#. Default: "Date e informazioni"
+#: design/plone/contenttypes/interfaces/incarico.py:175
+msgid "date_e_informazioni_label"
+msgstr ""
+
 #. Default: "Date e orari"
-#: design/plone/contenttypes/behaviors/evento.py:209
-#: design/plone/contenttypes/schema_overrides.py:34
+#: design/plone/contenttypes/behaviors/evento.py:164
+#: design/plone/contenttypes/schema_overrides.py:33
 msgid "date_e_orari_label"
 msgstr ""
 
 #. Default: "Inserisci la decorrenza termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:69
+#: design/plone/contenttypes/behaviors/trasparenza.py:70
 msgid "decorrenza_termini_help"
 msgstr ""
 
 #. Default: "Decorrenza termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:64
+#: design/plone/contenttypes/behaviors/trasparenza.py:65
 msgid "decorrenza_termini_label"
 msgstr ""
 
 #. Default: "Elenco delle deleghe a capo della persona."
-#: design/plone/contenttypes/interfaces/persona.py:77
+#: design/plone/contenttypes/interfaces/persona.py:85
 msgid "deleghe_help"
 msgstr ""
 
 #. Default: "Deleghe"
-#: design/plone/contenttypes/interfaces/persona.py:76
+#: design/plone/contenttypes/interfaces/persona.py:84
 msgid "deleghe_label"
 msgstr ""
 
 #. Default: "Descrizione completa"
-#: design/plone/contenttypes/behaviors/luogo.py:23
+#: design/plone/contenttypes/behaviors/luogo.py:24
 msgid "descrizione_completa"
 msgstr ""
 
-#. Default: "Descrizione destinatari"
-#: design/plone/contenttypes/behaviors/evento.py:38
-msgid "descrizione_destinatari"
-msgstr ""
-
-#. Default: "Descrizione dei principali interlocutori dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:40
-msgid "descrizione_destinatari_help"
-msgstr ""
-
 #. Default: "Descrizione estesa"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:16
-#: design/plone/contenttypes/behaviors/evento.py:30
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:19
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:17
+#: design/plone/contenttypes/behaviors/evento.py:32
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
 msgid "descrizione_estesa"
 msgstr ""
 
 #. Default: "Descrizione dettagliata e completa."
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:18
-#: design/plone/contenttypes/behaviors/evento.py:32
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:21
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:19
+#: design/plone/contenttypes/behaviors/evento.py:34
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:23
 msgid "descrizione_estesa_help"
 msgstr ""
 
 #. Default: "Descrizione"
-#: design/plone/contenttypes/behaviors/descrizione_estesa.py:51
-#: design/plone/contenttypes/behaviors/luogo.py:166
-#: design/plone/contenttypes/interfaces/documento.py:162
+#: design/plone/contenttypes/behaviors/descrizione_estesa.py:72
+#: design/plone/contenttypes/behaviors/luogo.py:135
+#: design/plone/contenttypes/interfaces/documento.py:242
 msgid "descrizione_label"
 msgstr ""
 
 #. Default: "Inserisci eventuale testo descrittivo del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:37
+#: design/plone/contenttypes/behaviors/trasparenza.py:38
 msgid "descrizione_procedimento_help"
 msgstr ""
 
 #. Default: "Descrizione del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:32
+#: design/plone/contenttypes/behaviors/trasparenza.py:33
 msgid "descrizione_procedimento_label"
 msgstr ""
 
 #. Default: "Dirigente"
-#: design/plone/contenttypes/behaviors/trasparenza.py:136
+#: design/plone/contenttypes/behaviors/trasparenza.py:137
 msgid "dirigente"
 msgstr ""
 
 #. Default: "Indicare il dirigente."
-#: design/plone/contenttypes/behaviors/trasparenza.py:140
+#: design/plone/contenttypes/behaviors/trasparenza.py:141
 msgid "dirigente_help"
 msgstr ""
 
 #. Default: "Distribuzione"
-#: design/plone/contenttypes/interfaces/dataset.py:22
+#: design/plone/contenttypes/interfaces/dataset.py:15
 msgid "distribuzione"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/messaggio.py:56
+#: design/plone/contenttypes/interfaces/messaggio.py:48
 msgid "documenti_allegati"
 msgstr ""
 
 #. Default: "Seleziona una serie di altri contenuti di tipo Documento che vanno allegati a questo."
-#: design/plone/contenttypes/interfaces/documento.py:113
+#: design/plone/contenttypes/interfaces/documento.py:194
 msgid "documenti_allegati_help"
 msgstr ""
 
 #. Default: "Documenti allegati"
-#: design/plone/contenttypes/interfaces/documento.py:109
+#: design/plone/contenttypes/interfaces/documento.py:190
 msgid "documenti_allegati_label"
 msgstr ""
 
 #. Default: "Documenti"
-#: design/plone/contenttypes/interfaces/persona.py:199
-#: design/plone/contenttypes/interfaces/servizio.py:412
+#: design/plone/contenttypes/interfaces/persona.py:146
+#: design/plone/contenttypes/interfaces/servizio.py:525
 msgid "documenti_label"
 msgstr ""
 
+#. Default: "Documenti pubblici importanti, collegati a questa Unità Organizzativa"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:129
+msgid "documenti_pubblici_help"
+msgstr ""
+
+#. Default: "Documenti pubblici"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:127
+msgid "documenti_pubblici_label"
+msgstr ""
+
 #. Default: "Dove"
-#: design/plone/contenttypes/behaviors/address.py:71
-#: design/plone/contenttypes/behaviors/geolocation.py:29
+#: design/plone/contenttypes/behaviors/address.py:53
+#: design/plone/contenttypes/behaviors/geolocation.py:26
 msgid "dove_label"
 msgstr ""
 
 #. Default: "Dove rivolgersi: informazioni aggiuntive"
-#: design/plone/contenttypes/interfaces/servizio.py:143
+#: design/plone/contenttypes/interfaces/servizio.py:212
 msgid "dove_rivolgersi_extra"
 msgstr ""
 
 #. Default: "Indicare eventuali informazioni aggiuntive riguardo al dove rivolgersi per questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:147
+#: design/plone/contenttypes/interfaces/servizio.py:216
 msgid "dove_rivolgersi_extra_help"
 msgstr ""
 
 #. Default: "Seleziona una lista delle sedi e dei luoghi in cui è presente questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:135
+#: design/plone/contenttypes/interfaces/servizio.py:204
 msgid "dove_rivolgersi_help"
 msgstr ""
 
 #. Default: "Elementi di interesse"
-#: design/plone/contenttypes/behaviors/luogo.py:44
+#: design/plone/contenttypes/behaviors/luogo.py:45
 msgid "elementi_di_interesse"
 msgstr ""
 
-#. Default: "Indicare un indirizzo mail per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:128
-msgid "email_event_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/evento.py:127
-msgid "email_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:35
-msgid "email_help"
-msgstr ""
-
-#. Default: "E-mail"
-#: design/plone/contenttypes/behaviors/contatti.py:34
-msgid "email_label"
-msgstr ""
-
-#. Default: "Contatto mail della persona. E' possibile inserire più di un indirizzo. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:135
-msgid "email_persona_help"
-msgstr ""
-
-#. Default: "Indirizzo email"
-#: design/plone/contenttypes/interfaces/persona.py:134
-msgid "email_persona_label"
-msgstr ""
-
 #. Default: "Esito"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:51
 msgid "esito"
 msgstr ""
 
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/evento.py:113
-msgid "fax_event_help"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/evento.py:114
-msgid "fax_event_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/behaviors/contatti.py:29
-msgid "fax_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/behaviors/contatti.py:28
-msgid "fax_label"
-msgstr ""
-
-#. Default: "Indicare un numero di fax."
-#: design/plone/contenttypes/interfaces/persona.py:130
-msgid "fax_persona_help"
-msgstr ""
-
-#. Default: "Fax"
-#: design/plone/contenttypes/interfaces/persona.py:129
-msgid "fax_persona_label"
+#. Default: "Escludi dalla ricerca"
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:17
+msgid "exclude_from_search_label"
 msgstr ""
 
 #. Default: "Inserisci il file correlato di questo pocedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:44
+#: design/plone/contenttypes/behaviors/trasparenza.py:45
 msgid "file_correlato_help"
 msgstr ""
 
 #. Default: "File correlato"
-#: design/plone/contenttypes/behaviors/trasparenza.py:43
+#: design/plone/contenttypes/behaviors/trasparenza.py:44
 msgid "file_correlato_label"
 msgstr ""
 
 #. Default: "Inserisci il file principale di questo contenuto."
-#: design/plone/contenttypes/behaviors/multi_file.py:16
+#: design/plone/contenttypes/behaviors/multi_file.py:17
 msgid "file_principale_help"
 msgstr ""
 
 #. Default: "File principale"
-#: design/plone/contenttypes/behaviors/multi_file.py:15
+#: design/plone/contenttypes/behaviors/multi_file.py:16
 msgid "file_principale_label"
 msgstr ""
 
 #. Default: "Inserisci la fine termine del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:80
+#: design/plone/contenttypes/behaviors/trasparenza.py:81
 msgid "fine_termine_help"
 msgstr ""
 
 #. Default: "Fine termine del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:75
+#: design/plone/contenttypes/behaviors/trasparenza.py:76
 msgid "fine_termine_label"
 msgstr ""
 
+#. Default: "Lista dei formati in cui è disponibile il documento"
+#: design/plone/contenttypes/interfaces/documento.py:117
+msgid "formati_disponibili_help"
+msgstr ""
+
+#. Default: "Formati disponibili"
+#: design/plone/contenttypes/interfaces/documento.py:116
+msgid "formati_disponibili_label"
+msgstr ""
+
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:25
+#: design/plone/contenttypes/behaviors/multi_file.py:26
 msgid "formato_alternativo_1_help"
 msgstr ""
 
 #. Default: "Formato alternativo 1"
-#: design/plone/contenttypes/behaviors/multi_file.py:24
+#: design/plone/contenttypes/behaviors/multi_file.py:25
 msgid "formato_alternativo_1_label"
 msgstr ""
 
 #. Default: "Inserisci un eventuale formato alternativo del file principale."
-#: design/plone/contenttypes/behaviors/multi_file.py:35
+#: design/plone/contenttypes/behaviors/multi_file.py:36
 msgid "formato_alternativo_2_help"
 msgstr ""
 
 #. Default: "Formato alternativo 2"
-#: design/plone/contenttypes/behaviors/multi_file.py:34
+#: design/plone/contenttypes/behaviors/multi_file.py:35
 msgid "formato_alternativo_2_label"
 msgstr ""
 
-#. Default: "Foto da mostrare della persona. La dimensione suggerita è 180x100 px."
-#: design/plone/contenttypes/interfaces/persona.py:21
+#. Default: "Foto da mostrare della persona. La dimensione suggerita è 100x180px."
+#: design/plone/contenttypes/interfaces/persona.py:30
 msgid "foto_persona_help"
 msgstr ""
 
 #. Default: "Foto della persona"
-#: design/plone/contenttypes/interfaces/persona.py:19
+#: design/plone/contenttypes/interfaces/persona.py:28
 msgid "foto_persona_label"
 msgstr ""
 
 #. Default: "Frequenza di aggiornamento"
-#: design/plone/contenttypes/interfaces/dataset.py:32
+#: design/plone/contenttypes/interfaces/dataset.py:25
 msgid "frequenza_aggiornamento"
 msgstr ""
 
 #. Default: "Invalid geolocation data: ${value}. Provide latitude and longitude coordinates."
-#: design/plone/contenttypes/restapi/deserializers/dxfields.py:28
+#: design/plone/contenttypes/restapi/deserializers/dxfields.py:39
 msgid "geolocation_field_validator_label"
 msgstr ""
 
 #. Default: "Indicare l'eventuale circoscrizione in cui si trova questo luogo"
 #: design/plone/contenttypes/behaviors/address.py:38
 msgid "help_circoscrizione"
 msgstr ""
 
 #. Default: "Indicare una descrizione completa, inserendo tutte le informazioni rilevanti relative al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:24
+#: design/plone/contenttypes/behaviors/luogo.py:25
 msgid "help_descrizione_completa"
 msgstr ""
 
 #. Default: "Indicare eventuali elementi di interesse per il cittadino."
-#: design/plone/contenttypes/behaviors/luogo.py:45
+#: design/plone/contenttypes/behaviors/luogo.py:46
 msgid "help_elementi_di_interesse"
 msgstr ""
 
+#. Default: "Se selezionato, questo contenuto non verrà mostrato nelle ricerche del sito per gli utenti anonimi."
+#: design/plone/contenttypes/behaviors/exclude_from_search.py:18
+msgid "help_exclude_from_search"
+msgstr ""
+
 #. Default: "Indicare tutte le informazioni relative alla modalità di accesso al luogo"
-#: design/plone/contenttypes/behaviors/luogo.py:54
+#: design/plone/contenttypes/behaviors/luogo.py:55
 msgid "help_modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare, se esiste, un nome alternativo per il luogo; questo sarà mostrato affianco al titolo della scheda"
-#: design/plone/contenttypes/behaviors/luogo.py:34
+#: design/plone/contenttypes/behaviors/luogo.py:35
 msgid "help_nome_alternativo"
 msgstr ""
 
 #. Default: "Inserisci il nome della sede, se non è presente tra i Luoghi del sito."
 #: design/plone/contenttypes/behaviors/address.py:17
 msgid "help_nome_sede"
 msgstr ""
 
 #. Default: "Indicare l'eventuale quartiere in cui si trova questo luogo"
 #: design/plone/contenttypes/behaviors/address.py:32
 msgid "help_quartiere"
 msgstr ""
 
-#. Default: "Indicare un numero di fax della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:108
-msgid "help_riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo mail per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:119
-msgid "help_riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:132
-msgid "help_riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Indicare il riferimento telefonico per poter contattare i referenti della struttura responsabile."
-#: design/plone/contenttypes/behaviors/luogo.py:96
-msgid "help_riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato.Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
-#: design/plone/contenttypes/behaviors/update_note.py:17
+#. Default: "Inserisci una nota per indicare che il contenuto corrente è stato aggiornato. Questo testo può essere visualizzato nei blocchi elenco con determinati layout per informare gli utenti che un determinato contenuto è stato aggiornato. Ad esempio se in un bando sono stati aggiunti dei documenti."
+#: design/plone/contenttypes/behaviors/update_note.py:18
 msgid "help_update_note"
 msgstr ""
 
 #. Default: "Icona"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:27
 msgid "icona"
 msgstr ""
 
 #. Default: "Puoi selezionare un’icona fra quelle proposte nel menu a tendina oppure puoi scrivere/incollare nel campo di testo il nome di un’icona di fontawsome 5"
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:28
 msgid "icona_help"
 msgstr ""
 
 #. Default: "Identificativo"
-#: design/plone/contenttypes/interfaces/servizio.py:290
+#: design/plone/contenttypes/interfaces/servizio.py:379
 msgid "identificativo"
 msgstr ""
 
 #. Default: "Un numero identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:21
 msgid "identificativo_documento_help"
 msgstr ""
 
 #. Default: "Identificativo del documento."
 #: design/plone/contenttypes/interfaces/documento.py:17
 msgid "identificativo_documento_label"
 msgstr ""
 
 #. Default: "Eventuale codice identificativo del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:292
+#: design/plone/contenttypes/interfaces/servizio.py:381
 msgid "identificativo_help"
 msgstr ""
 
+#. Default: "Identificativo"
+#: design/plone/contenttypes/behaviors/luogo.py:119
+msgid "identificativo_mibac"
+msgstr ""
+
+#. Default: "Codice identificativo del luogo. Nel MIBAC c'è il codice del DBUnico per i luoghi della cultura e il codice ISIL per le biblioteche. Non deve comparire nel frontend del sito."
+#: design/plone/contenttypes/behaviors/luogo.py:121
+msgid "identificativo_mibac_help"
+msgstr ""
+
 #. Default: "La dimensione dell'immagine dovrebbe essere di ${size} px"
-#: design/plone/contenttypes/restapi/types/adapters.py:31
+#: design/plone/contenttypes/restapi/types/adapters.py:43
 msgid "image_size_help"
 msgstr ""
 
 #. Default: "Immagine"
 #: design/plone/contenttypes/interfaces/documento_personale.py:23
 msgid "immagine"
 msgstr ""
 
+#. Default: "Solo per incarico politico: importi di viaggi di servizio  e missioni pagati con fondi pubblici."
+#: design/plone/contenttypes/interfaces/incarico.py:34
+msgid "importi_viaggio_servizio_incarico_help"
+msgstr ""
+
+#. Default: "Importi di viaggio e/o servizio"
+#: design/plone/contenttypes/interfaces/incarico.py:30
+msgid "importi_viaggio_servizio_incarico_label"
+msgstr ""
+
 #. Default: "Importo pagato"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:25
 msgid "importo_pagato"
 msgstr ""
 
+#. Default: "Seleziona l'incarico corrente della persona."
+#: design/plone/contenttypes/interfaces/persona.py:63
+msgid "incarichi_help"
+msgstr ""
+
+#. Default: "Incarichi"
+#: design/plone/contenttypes/interfaces/persona.py:59
+msgid "incarichi_label"
+msgstr ""
+
 #. Default: "Inserisci eventuale testo informativo che verrà mostrato in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:23
 msgid "info_testata_help"
 msgstr ""
 
 #. Default: "Informazioni aggiuntive per la testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:18
@@ -1708,127 +1726,162 @@
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/interfaces/documento_personale.py:140
 msgid "informazioni"
 msgstr ""
 
+#. Default: "Compensi e trasparenza"
+#: design/plone/contenttypes/interfaces/incarico.py:170
+msgid "informazioni_compensi_label"
+msgstr ""
+
 #. Default: "Ulteriori informazioni"
 #: design/plone/contenttypes/behaviors/additional_help_infos.py:28
-#: design/plone/contenttypes/behaviors/evento.py:229
 #: design/plone/contenttypes/behaviors/strutture_correlate.py:42
+#: design/plone/contenttypes/interfaces/documento.py:253
 msgid "informazioni_label"
 msgstr ""
 
+#. Default: "Intervallo della fase (es. 1)"
+#: design/plone/contenttypes/interfaces/servizio.py:32
+msgid "interval_qt_help"
+msgstr ""
+
+#. Default: "Intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:31
+msgid "interval_qt_label"
+msgstr ""
+
+#. Default: "Ad esempio: ore, giorni, settimane, mesi."
+#: design/plone/contenttypes/interfaces/servizio.py:41
+msgid "interval_type_help"
+msgstr ""
+
+#. Default: "Tipo intervallo"
+#: design/plone/contenttypes/interfaces/servizio.py:40
+msgid "interval_type_label"
+msgstr ""
+
 #. Default: "Se un content-type deve avere una dimensione della leadimage particolare, indicarle qui. Inserire le dimensioni nella forma di esempio PortalType|900x900"
-#: design/plone/contenttypes/controlpanels/settings.py:110
+#: design/plone/contenttypes/controlpanels/settings.py:52
 msgid "lead_image_dimension_help"
 msgstr ""
 
 #. Default: "Dimensioni lead image"
-#: design/plone/contenttypes/controlpanels/settings.py:106
+#: design/plone/contenttypes/controlpanels/settings.py:48
 msgid "lead_image_dimension_label"
 msgstr ""
 
-#. Default: "Servizi o uffici di riferimento"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:27
+#. Default: "Strutture o uffici di riferimento"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
 msgid "legami_altre_strutture_label"
 msgstr ""
 
 #. Default: "Selezionare la lista di strutture e/o uffici collegati a questa unità organizzativa."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:31
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:35
 msgid "legami_con_altre_strutture_help"
 msgstr ""
 
 #. Default: "Licenza"
-#: design/plone/contenttypes/interfaces/dataset.py:25
+#: design/plone/contenttypes/interfaces/dataset.py:18
 msgid "licenza"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
 #: design/plone/contenttypes/interfaces/documento_personale.py:92
 msgid "licenza_distribuzione"
 msgstr ""
 
 #. Default: "La licenza con il quale viene distribuito questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:88
+#: design/plone/contenttypes/interfaces/documento.py:125
 msgid "licenza_distribuzione_help"
 msgstr ""
 
 #. Default: "Licenza di distribuzione"
-#: design/plone/contenttypes/interfaces/documento.py:87
+#: design/plone/contenttypes/interfaces/documento.py:124
 msgid "licenza_distribuzione_label"
 msgstr ""
 
 #. Default: "Link a siti esterni"
-#: design/plone/contenttypes/interfaces/servizio.py:258
+#: design/plone/contenttypes/interfaces/servizio.py:347
 msgid "link_siti_esterni"
 msgstr ""
 
 #. Default: "Eventuali collegamenti a pagine web, siti, servizi esterni all'ambito Comunale utili all'erogazione del servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:260
+#: design/plone/contenttypes/interfaces/servizio.py:349
 msgid "link_siti_esterni_help"
 msgstr ""
 
 #. Default: "Link utili"
-#: design/plone/contenttypes/interfaces/servizio.py:417
+#: design/plone/contenttypes/interfaces/servizio.py:530
 msgid "link_utili_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati. Se il luogo dell'evento non è presente sul sito, inserisci le sue informazioni nei campi seguenti."
 #: design/plone/contenttypes/behaviors/luoghi_correlati.py:52
 msgid "luoghi_correlati_event_help"
 msgstr ""
 
 #. Default: "Seleziona una lista di luoghi citati."
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:72
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:19
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:64
 msgid "luoghi_correlati_help"
 msgstr ""
 
 #. Default: "Luoghi correlati"
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:17
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:71
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:18
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:63
 msgid "luoghi_correlati_label"
 msgstr ""
 
 #. Default: "Luogo"
-#: design/plone/contenttypes/behaviors/address.py:89
-#: design/plone/contenttypes/behaviors/geolocation.py:38
-#: design/plone/contenttypes/behaviors/luoghi_correlati.py:74
+#: design/plone/contenttypes/behaviors/address.py:71
+#: design/plone/contenttypes/behaviors/geolocation.py:34
+#: design/plone/contenttypes/behaviors/luoghi_correlati.py:76
 msgid "luogo_label"
 msgstr ""
 
+#. Default: "Sottotitolo"
+#: design/plone/contenttypes/interfaces/servizio.py:26
+msgid "milestone_description_label"
+msgstr ""
+
+#. Default: "Titolo"
+#: design/plone/contenttypes/interfaces/servizio.py:21
+msgid "milestone_label"
+msgstr ""
+
 #. Default: "Modalita' di accesso"
-#: design/plone/contenttypes/behaviors/luogo.py:53
+#: design/plone/contenttypes/behaviors/luogo.py:54
 msgid "modalita_accesso"
 msgstr ""
 
 #. Default: "Indicare la modalità di avvio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:25
+#: design/plone/contenttypes/behaviors/trasparenza.py:26
 msgid "modalita_avvio_help"
 msgstr ""
 
 #. Default: "Modalita di avvio"
-#: design/plone/contenttypes/behaviors/trasparenza.py:24
+#: design/plone/contenttypes/behaviors/trasparenza.py:25
 msgid "modalita_avvio_label"
 msgstr ""
 
 #. Default: "Modalità pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:29
 msgid "modalita_pagamento"
 msgstr ""
 
 #. Default: "Indicare le modalità per richiedere informazioni riguardo a questo procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:168
+#: design/plone/contenttypes/behaviors/trasparenza.py:169
 msgid "modalita_richiesta_informazioni_help"
 msgstr ""
 
 #. Default: "Modalità per richiedere informazioni"
-#: design/plone/contenttypes/behaviors/trasparenza.py:163
+#: design/plone/contenttypes/behaviors/trasparenza.py:164
 msgid "modalita_richiesta_informazioni_label"
 msgstr ""
 
 #. Default: "Seleziona se mostrare o meno i bottoni con i link per la condivisione sui vari social, mail e stampa."
 #: design/plone/contenttypes/behaviors/info_testata.py:44
 msgid "mostra_bottoni_condivisione_help"
 msgstr ""
@@ -1844,46 +1897,46 @@
 msgstr ""
 
 #. Default: "Mostra la navigazione"
 #: design/plone/contenttypes/behaviors/info_testata.py:51
 msgid "mostra_navigazione_label"
 msgstr ""
 
-#. Default: "Descrizione del motivo per cui il servizio non è attivo."
-#: design/plone/contenttypes/interfaces/servizio.py:44
+#. Default: "Descrizione del motivo per cui il servizio non è attivo. È obbligatorio se il campo precedente è spuntato."
+#: design/plone/contenttypes/interfaces/servizio.py:89
 msgid "motivo_stato_servizio_help"
 msgstr ""
 
-#. Default: "Motivo dello stato del servizio nel caso non sia attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:39
+#. Default: "Motivo dello stato"
+#: design/plone/contenttypes/interfaces/servizio.py:84
 msgid "motivo_stato_servizio_label"
 msgstr ""
 
 #. Default: "Nome alternativo"
-#: design/plone/contenttypes/behaviors/luogo.py:33
+#: design/plone/contenttypes/behaviors/luogo.py:34
 msgid "nome_alternativo"
 msgstr ""
 
 #. Default: "Nome sede"
 #: design/plone/contenttypes/behaviors/address.py:16
 msgid "nome_sede"
 msgstr ""
 
 #. Default: "Seleziona una lista di notizie correlate a questa."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:83
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:75
 msgid "notizie_correlate_help"
 msgstr ""
 
 #. Default: "Notizie correlate"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:82
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:74
 msgid "notizie_correlate_label"
 msgstr ""
 
 #. Default: "Numero progressivo del comunicato stampa"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:38
+#: design/plone/contenttypes/behaviors/news_additional_fields.py:30
 msgid "numero_progressivo_cs_label"
 msgstr ""
 
 #. Default: "Numero protocollo"
 #: design/plone/contenttypes/interfaces/pratica.py:12
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:12
 msgid "numero_protocollo"
@@ -1891,125 +1944,163 @@
 
 #. Default: "Oggetto"
 #: design/plone/contenttypes/interfaces/documento_personale.py:48
 msgid "oggetto"
 msgstr ""
 
 #. Default: "Informazioni sugli orari"
-#: design/plone/contenttypes/behaviors/evento.py:62
+#: design/plone/contenttypes/behaviors/evento.py:50
 msgid "orari"
 msgstr ""
 
 #. Default: "Informazioni sugli orari di svolgimento dell'evento."
-#: design/plone/contenttypes/behaviors/evento.py:64
+#: design/plone/contenttypes/behaviors/evento.py:52
 msgid "orari_help"
 msgstr ""
 
 #. Default: "Orari di apertura"
-#: design/plone/contenttypes/behaviors/contatti.py:86
+#: design/plone/contenttypes/behaviors/luogo.py:151
 msgid "orari_label"
 msgstr ""
 
+#. Default: "Orario per il pubblico"
+#: design/plone/contenttypes/behaviors/luogo.py:93
+msgid "orario_pubblico"
+msgstr ""
+
 #. Default: "Indicare eventuali orari di accesso al pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:59
+#: design/plone/contenttypes/behaviors/contatti.py:40
+#: design/plone/contenttypes/behaviors/luogo.py:95
 msgid "orario_pubblico_help"
 msgstr ""
 
 #. Default: "Orario per il pubblico"
-#: design/plone/contenttypes/behaviors/contatti.py:58
+#: design/plone/contenttypes/behaviors/contatti.py:39
 msgid "orario_pubblico_label"
 msgstr ""
 
 #. Default: "Se l'evento non è organizzato direttamente dal comune oppure ha anche un organizzatore esterno, indicare il nome del contatto."
-#: design/plone/contenttypes/behaviors/evento.py:97
+#: design/plone/contenttypes/behaviors/evento.py:86
 msgid "organizzato_da_esterno_help"
 msgstr ""
 
 #. Default: "Organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:95
+#: design/plone/contenttypes/behaviors/evento.py:84
 msgid "organizzato_da_esterno_label"
 msgstr ""
 
 #. Default: "Se l'evento è organizzato direttamente dal comune, indicare l'ufficio/ente organizzatore. I dati di contatto verranno presi direttamente dall'ufficio selezionato. Se l'evento non è organizzato direttamente dal comune, o si vogliono sovrascrivere alcuni dati di contatto, utilizzare i seguenti campi."
-#: design/plone/contenttypes/behaviors/evento.py:84
+#: design/plone/contenttypes/behaviors/evento.py:74
 msgid "organizzato_da_interno_help"
 msgstr ""
 
 #. Default: "Organizzato da"
-#: design/plone/contenttypes/behaviors/evento.py:80
+#: design/plone/contenttypes/behaviors/evento.py:70
 msgid "organizzato_da_interno_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di organizzazioni a cui la persona appartiene."
-#: design/plone/contenttypes/interfaces/persona.py:42
+#: design/plone/contenttypes/interfaces/persona.py:45
 msgid "organizzazione_riferimento_help"
 msgstr ""
 
 #. Default: "Organizzazione di riferimento"
-#: design/plone/contenttypes/interfaces/persona.py:38
+#: design/plone/contenttypes/interfaces/persona.py:41
 msgid "organizzazione_riferimento_label"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:157
+#: design/plone/contenttypes/behaviors/trasparenza.py:158
 msgid "organo_competente_provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Organo competente del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:152
+#: design/plone/contenttypes/behaviors/trasparenza.py:153
 msgid "organo_competente_provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Indicare le informazioni riguardanti i pagamenti previsti e modalità di pagamento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:222
+#: design/plone/contenttypes/behaviors/trasparenza.py:223
 msgid "pagamenti_help"
 msgstr ""
 
 #. Default: "Pagamenti previsti e modalità"
-#: design/plone/contenttypes/behaviors/trasparenza.py:218
+#: design/plone/contenttypes/behaviors/trasparenza.py:219
 msgid "pagamenti_label"
 msgstr ""
 
+#. Default: "Link a persone dell'amministrazione che interverranno all'evento"
+#: design/plone/contenttypes/behaviors/evento.py:118
+msgid "parteciperanno_help"
+msgstr ""
+
+#. Default: "Parteciperanno (Persone)"
+#: design/plone/contenttypes/behaviors/evento.py:114
+msgid "parteciperanno_label"
+msgstr ""
+
 #. Default: "Indicare l'ente che supporta l'evento, se presente."
-#: design/plone/contenttypes/behaviors/evento.py:160
+#: design/plone/contenttypes/behaviors/evento.py:107
 msgid "patrocinato_da_help"
 msgstr ""
 
 #. Default: "Patrocinato da"
-#: design/plone/contenttypes/behaviors/evento.py:158
+#: design/plone/contenttypes/behaviors/evento.py:105
 msgid "patrocinato_da_label"
 msgstr ""
 
-#. Default: "Indicare un indirizzo pec per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:44
-msgid "pec_help"
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:27
+msgid "pdc_desc_help"
+msgstr ""
+
+#. Default: "Descrizione"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:26
+msgid "pdc_desc_label"
+msgstr ""
+
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:16
+msgid "pdc_type_label"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:37
+msgid "pdc_value_help"
+msgstr ""
+
+#. Default: "Contatto"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:36
+msgid "pdc_value_label"
 msgstr ""
 
-#. Default: "Pec"
-#: design/plone/contenttypes/behaviors/contatti.py:43
-msgid "pec_label"
+#. Default: "Seleziona la persona che ha questo incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:47
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:66
+msgid "persona_incarico_help"
 msgstr ""
 
-#. Default: "Elenco delle persone dell'amministrazione che parteciperanno all'evento."
-#: design/plone/contenttypes/behaviors/evento.py:53
-msgid "persone_amministrazione_help"
+#. Default: "La persona che ha la carica e l'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:43
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:62
+msgid "persona_incarico_label"
 msgstr ""
 
 #. Default: "Persone"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:221
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:215
 msgid "persone_label"
 msgstr ""
 
 #. Default: "Seleziona la lista delle persone che compongono la struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
 msgid "persone_struttura_help"
 msgstr ""
 
 #. Default: "Persone che compongono la struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:87
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:79
 msgid "persone_struttura_label"
 msgstr ""
 
 #. Default: "Pratica associata"
 #: design/plone/contenttypes/interfaces/documento_personale.py:26
 #: design/plone/contenttypes/interfaces/messaggio.py:35
 msgid "pratica_associata"
@@ -2017,255 +2108,230 @@
 
 #. Default: "Pratica associata al pagamento"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:43
 msgid "pratica_associata_ricevuta"
 msgstr ""
 
 #. Default: "Prenota un appuntamento"
-#: design/plone/contenttypes/interfaces/servizio.py:156
+#: design/plone/contenttypes/interfaces/servizio.py:225
 msgid "prenota_appuntamento"
 msgstr ""
 
 #. Default: "Se è possibile prenotare un'appuntamento, indicare le informazioni necessarie e il collegamento al servizio di prenotazione appuntamenti del Comune."
-#: design/plone/contenttypes/interfaces/servizio.py:157
+#: design/plone/contenttypes/interfaces/servizio.py:226
 msgid "prenota_appuntamento_help"
 msgstr ""
 
-#. Default: "Prezzo"
-#: design/plone/contenttypes/behaviors/evento.py:71
+#. Default: "Costo"
+#: design/plone/contenttypes/behaviors/evento.py:59
 msgid "prezzo"
 msgstr ""
 
-#. Default: "Indicare il prezzo dell'evento, se presente, specificando se esistono formati diversi."
-#: design/plone/contenttypes/behaviors/evento.py:73
+#. Default: "Eventuale costo dell'evento (se ci sono uno o più biglietti), con link all'acquisto se disponibile"
+#: design/plone/contenttypes/behaviors/evento.py:61
 msgid "prezzo_help"
 msgstr ""
 
 #. Default: "Indicare, se la procedura è informatizzata online, il riferimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:178
+#: design/plone/contenttypes/behaviors/trasparenza.py:179
 msgid "procedura_online_help"
 msgstr ""
 
 #. Default: "Procedura informatizzata online"
-#: design/plone/contenttypes/behaviors/trasparenza.py:174
+#: design/plone/contenttypes/behaviors/trasparenza.py:175
 msgid "procedura_online_label"
 msgstr ""
 
 #. Default: "Procedure collegate all'esito"
-#: design/plone/contenttypes/interfaces/servizio.py:100
+#: design/plone/contenttypes/interfaces/servizio.py:145
 msgid "procedure_collegate"
 msgstr ""
 
 #. Default: "Indicare cosa deve fare l'utente del servizio per conoscere l'esito della procedura, e dove eventualmente poter ritirare l'esito."
-#: design/plone/contenttypes/interfaces/servizio.py:102
+#: design/plone/contenttypes/interfaces/servizio.py:147
 msgid "procedure_collegate_help"
 msgstr ""
 
 #. Default: "Protocollo"
 #: design/plone/contenttypes/interfaces/documento_personale.py:15
 msgid "protocollo"
 msgstr ""
 
+#. Default: "Il numero di protocollo del documento."
+#: design/plone/contenttypes/interfaces/documento.py:33
+msgid "protocollo_documento_help"
+msgstr ""
+
+#. Default: "Numero di protocollo"
+#: design/plone/contenttypes/interfaces/documento.py:29
+msgid "protocollo_documento_label"
+msgstr ""
+
 #. Default: "Eventuale provvedimento finale del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:114
+#: design/plone/contenttypes/behaviors/trasparenza.py:115
 msgid "provvedimento_finale_help"
 msgstr ""
 
 #. Default: "Provvedimento del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:109
+#: design/plone/contenttypes/behaviors/trasparenza.py:110
 msgid "provvedimento_finale_label"
 msgstr ""
 
 #. Default: "Quartiere"
 #: design/plone/contenttypes/behaviors/address.py:31
 msgid "quartiere"
 msgstr ""
 
-#. Default: "Reperibilità organizzatore"
-#: design/plone/contenttypes/behaviors/evento.py:118
-msgid "reperibilita"
-msgstr ""
-
-#. Default: "Indicare gli orari in cui l'organizzatore è telefonicamente reperibile."
-#: design/plone/contenttypes/behaviors/evento.py:120
-msgid "reperibilita_help"
-msgstr ""
-
 #. Default: "Indicare dove è possibile reperre la modulistica per il procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:211
+#: design/plone/contenttypes/behaviors/trasparenza.py:212
 msgid "reperimento_modulistica_help"
 msgstr ""
 
 #. Default: "Dove reperire la modulistica"
-#: design/plone/contenttypes/behaviors/trasparenza.py:207
+#: design/plone/contenttypes/behaviors/trasparenza.py:208
 msgid "reperimento_modulistica_label"
 msgstr ""
 
 #. Default: "Selezionare il/i responsabile/i della struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:48
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:52
 msgid "responsabile_help"
 msgstr ""
 
 #. Default: "Responsabile"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:43
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:47
 msgid "responsabile_label"
 msgstr ""
 
 #. Default: "Responsabile del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:120
+#: design/plone/contenttypes/behaviors/trasparenza.py:121
 msgid "responsabile_procedimento"
 msgstr ""
 
 #. Default: "Indicare il responsabile del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:124
+#: design/plone/contenttypes/behaviors/trasparenza.py:125
 msgid "responsabile_procedimento_help"
 msgstr ""
 
+#. Default: "Se è un incarico di responsabilità, specificare l'organizzazione della quale è responsabile in base all'incarico"
+#: design/plone/contenttypes/interfaces/incarico.py:81
+msgid "responsabile_struttura_incarico_help"
+msgstr ""
+
+#. Default: "Responsabile della struttura"
+#: design/plone/contenttypes/interfaces/incarico.py:77
+msgid "responsabile_struttura_incarico_label"
+msgstr ""
+
 #. Default: "Seleziona se mostrare o meno il campo di ricerca in testata."
 #: design/plone/contenttypes/behaviors/info_testata.py:32
 msgid "ricerca_in_testata_help"
 msgstr ""
 
 #. Default: "Ricerca in testata"
 #: design/plone/contenttypes/behaviors/info_testata.py:29
 msgid "ricerca_in_testata_label"
 msgstr ""
 
 #. Default: "Ulteriori informazioni non previste negli altri campi; si può trattare di contatti o note informative la cui conoscenza è indispensabile per la partecipazione al bando"
-#: design/plone/contenttypes/interfaces/bando.py:96
+#: design/plone/contenttypes/interfaces/bando.py:97
 msgid "riferimenti_bando_agid_help"
 msgstr ""
 
 #. Default: "Ulteriori informazioni"
-#: design/plone/contenttypes/interfaces/bando.py:95
+#: design/plone/contenttypes/interfaces/bando.py:96
 msgid "riferimenti_bando_agid_label"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
 #: design/plone/contenttypes/interfaces/documento_personale.py:145
 msgid "riferimenti_normativi"
 msgstr ""
 
 #. Default: "Inserisici del testo di dettaglio per eventuali riferimenti normativi utili a questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:100
+#: design/plone/contenttypes/interfaces/documento.py:137
 msgid "riferimenti_normativi_documento_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/interfaces/documento.py:96
+#: design/plone/contenttypes/interfaces/documento.py:133
 msgid "riferimenti_normativi_documento_label"
 msgstr ""
 
 #. Default: "Indicare eventuali riferimenti normativi."
-#: design/plone/contenttypes/behaviors/trasparenza.py:265
+#: design/plone/contenttypes/behaviors/trasparenza.py:266
 msgid "riferimenti_normativi_help"
 msgstr ""
 
 #. Default: "Riferimenti normativi"
-#: design/plone/contenttypes/behaviors/trasparenza.py:260
+#: design/plone/contenttypes/behaviors/trasparenza.py:261
 msgid "riferimenti_normativi_label"
 msgstr ""
 
-#. Default: "Fax della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:104
-msgid "riferimento_fax_struttura"
-msgstr ""
-
-#. Default: "E-mail struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:115
-msgid "riferimento_mail_struttura"
-msgstr ""
-
-#. Default: "Pec della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:128
-msgid "riferimento_pec_struttura"
-msgstr ""
-
-#. Default: "Telefono della struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:92
-msgid "riferimento_telefonico_struttura"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per il ruolo di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:84
-msgid "ruoli_persona_help"
-msgstr ""
-
-#. Default: "Ruoli Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:83
-msgid "ruoli_persona_label"
-msgstr ""
-
-#. Default: "Seleziona il ruolo della persona tra quelli disponibili."
-#: design/plone/contenttypes/interfaces/persona.py:29
-msgid "ruolo_help"
-msgstr ""
-
 #. Default: "Ruolo"
-#: design/plone/contenttypes/interfaces/persona.py:28
+#: design/plone/contenttypes/interfaces/persona.py:135
 msgid "ruolo_label"
 msgstr ""
 
 #. Default: "Data entro la quale sarà possibile far pervenire domande e richieste di chiarimento a chi eroga il bando"
-#: design/plone/contenttypes/interfaces/bando.py:69
+#: design/plone/contenttypes/interfaces/bando.py:70
 msgid "scadenza_domande_bando_help"
 msgstr ""
 
 #. Default: "Termine per le richieste di chiarimenti"
-#: design/plone/contenttypes/interfaces/bando.py:65
+#: design/plone/contenttypes/interfaces/bando.py:66
 msgid "scadenza_domande_bando_label"
 msgstr ""
 
 #. Default: "Inserire una lista di sezioni per la ricerca."
-#: design/plone/contenttypes/controlpanels/settings.py:129
+#: design/plone/contenttypes/controlpanels/settings.py:71
 msgid "search_sections_help"
 msgstr ""
 
 #. Default: "Sezioni ricerca"
-#: design/plone/contenttypes/controlpanels/settings.py:128
+#: design/plone/contenttypes/controlpanels/settings.py:70
 msgid "search_sections_label"
 msgstr ""
 
-#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente un contenuto di tipo Luogo a cui far riferimento, puoi compilare i campi seguenti. Se selezioni un Luogo, puoi usare comunque i campi seguenti per sovrascrivere alcune informazioni."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:105
+#. Default: "Seleziona il Luogo in cui questa struttura ha sede. Se non è presente creare il Luogo nella sezione dedicata nell'alberatura del sito."
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:97
 msgid "sede_help"
 msgstr ""
 
 #. Default: "Sede principale"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:103
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:95
 msgid "sede_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di eventuali contenuti di tipo Luogo che sono sedi secondarie di questa struttura. Per queste sedi non sarà possibile sovrascrivere i dati. Nel caso servano informazioni diverse, è possibile usare il campo sottostante."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:122
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:112
 msgid "sedi_secondarie_help"
 msgstr ""
 
-#. Default: "Sedi secondarie"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:120
+#. Default: "Altre sedi"
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:110
 msgid "sedi_secondarie_label"
 msgstr ""
 
 #. Default: "Seleziona la lista dei servizi collegati a questo."
-#: design/plone/contenttypes/interfaces/servizio.py:300
+#: design/plone/contenttypes/interfaces/servizio.py:394
 msgid "servizi_collegati_help"
 msgstr ""
 
 #. Default: "Servizi collegati"
-#: design/plone/contenttypes/interfaces/servizio.py:299
+#: design/plone/contenttypes/interfaces/servizio.py:393
 msgid "servizi_collegati_label"
 msgstr ""
 
 #. Default: "Questi servizi non verranno mostrati nel contenuto, ma permetteranno di vedere questo contenuto associato quando si visita il servizio"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:20
 msgid "servizi_correlati_description"
 msgstr ""
 
 #. Default: "Servizi correlati"
-#: design/plone/contenttypes/behaviors/servizi_correlati.py:18
+#: design/plone/contenttypes/behaviors/servizi_correlati.py:19
 msgid "servizi_correlati_label"
 msgstr ""
 
 #. Default: "Servizio che genera il documento"
 #: design/plone/contenttypes/interfaces/documento_personale.py:31
 msgid "servizio_origine"
 msgstr ""
@@ -2277,367 +2343,292 @@
 
 #. Default: "Servizio che origina la pratica"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:35
 msgid "servizio_origine_ricevuta"
 msgstr ""
 
 #. Default: "Settore merceologico"
-#: design/plone/contenttypes/interfaces/servizio.py:280
+#: design/plone/contenttypes/interfaces/servizio.py:369
 msgid "settore_merceologico"
 msgstr ""
 
 #. Default: "Classificazione del servizio basata su catalogo dei servizi (Classificazione NACE)."
-#: design/plone/contenttypes/interfaces/servizio.py:282
+#: design/plone/contenttypes/interfaces/servizio.py:371
 msgid "settore_merceologico_help"
 msgstr ""
 
+#. Default: "Se selezionato, il footer verrà popolato automaticamente con i contenuti di primo livello non esclusi dalla navigazione."
+#: design/plone/contenttypes/controlpanels/settings.py:93
+msgid "show_dynamic_folders_in_footer_help"
+msgstr ""
+
+#. Default: "Footer dinamico"
+#: design/plone/contenttypes/controlpanels/settings.py:92
+msgid "show_dynamic_folders_in_footer_label"
+msgstr ""
+
 #. Default: "Questo è il valore di default per decidere se mostrare o meno la data di modifica nei contenuti che hanno la behavior abilitata. E' poi possibile sovrascrivere il default nei singoli contenuti (nel tab \"Impostazioni\")."
-#: design/plone/contenttypes/controlpanels/settings.py:139
+#: design/plone/contenttypes/controlpanels/settings.py:81
 msgid "show_modified_default_help"
 msgstr ""
 
 #. Default: "Mostra la data di modifica"
-#: design/plone/contenttypes/controlpanels/settings.py:138
+#: design/plone/contenttypes/controlpanels/settings.py:80
 msgid "show_modified_default_label"
 msgstr ""
 
 #. Default: "Se attivo, verrà mostrata la data di ultima modifica in visualizzazione del contenuto."
 #: design/plone/contenttypes/behaviors/show_modified.py:24
 msgid "show_modified_help"
 msgstr ""
 
 #. Default: "Mostra la data di ultima modifica"
 #: design/plone/contenttypes/behaviors/show_modified.py:23
 msgid "show_modified_label"
 msgstr ""
 
 #. Default: "Indicare se il procedimento prevede il silenzio assenso o la dichiarazione dell'interessato sostitutiva del provvedimento finale."
-#: design/plone/contenttypes/behaviors/trasparenza.py:103
+#: design/plone/contenttypes/behaviors/trasparenza.py:104
 msgid "silenzio_assenso_help"
 msgstr ""
 
 #. Default: "Silenzio assenso/Dichiarazione dell'interessato sostitutiva del provvedimento finale"
-#: design/plone/contenttypes/behaviors/trasparenza.py:97
+#: design/plone/contenttypes/behaviors/trasparenza.py:98
 msgid "silenzio_assenso_label"
 msgstr ""
 
 #. Default: "Inserisci eventuali soggetti esterni, nonché, strutture interne coinvolte nel procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:57
+#: design/plone/contenttypes/behaviors/trasparenza.py:58
 msgid "soggetti_eserni_help"
 msgstr ""
 
 #. Default: "Soggetti esterni, nonché, strutture interne coinvolte nel procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:52
+#: design/plone/contenttypes/behaviors/trasparenza.py:53
 msgid "soggetti_eserni_label"
 msgstr ""
 
 #. Default: "Indica un eventuale sottotitolo/titolo alternativo."
-#: design/plone/contenttypes/behaviors/evento.py:23
-#: design/plone/contenttypes/interfaces/servizio.py:19
+#: design/plone/contenttypes/behaviors/evento.py:24
+#: design/plone/contenttypes/interfaces/servizio.py:64
 msgid "sottotitolo_help"
 msgstr ""
 
 #. Default: "Sottotitolo"
-#: design/plone/contenttypes/behaviors/evento.py:22
-#: design/plone/contenttypes/interfaces/servizio.py:18
+#: design/plone/contenttypes/behaviors/evento.py:23
+#: design/plone/contenttypes/interfaces/servizio.py:63
 msgid "sottotitolo_label"
 msgstr ""
 
 #. Default: "Stampa ricevuta"
 #: design/plone/contenttypes/interfaces/ricevuta_pagamento.py:17
 msgid "stampa_ricevuta"
 msgstr ""
 
 #. Default: "Stato della pratica"
 #: design/plone/contenttypes/interfaces/pratica.py:26
 msgid "stato_pratica"
 msgstr ""
 
-#. Default: "Indica se il servizio è effettivamente fruibile."
-#: design/plone/contenttypes/interfaces/servizio.py:32
+#. Default: "Indica se il servizio è effettivamente fruibile; spuntare se non è fruibile."
+#: design/plone/contenttypes/interfaces/servizio.py:77
 msgid "stato_servizio_help"
 msgstr ""
 
-#. Default: "Servizio non attivo"
-#: design/plone/contenttypes/interfaces/servizio.py:30
+#. Default: "Servizio non fruibile"
+#: design/plone/contenttypes/interfaces/servizio.py:75
 msgid "stato_servizio_label"
 msgstr ""
 
 #. Default: "Indicare gli eventuali strumenti di tutela."
-#: design/plone/contenttypes/behaviors/trasparenza.py:230
+#: design/plone/contenttypes/behaviors/trasparenza.py:231
 msgid "strumenti_tutela_help"
 msgstr ""
 
 #. Default: "Strumenti di tutela"
-#: design/plone/contenttypes/behaviors/trasparenza.py:229
+#: design/plone/contenttypes/behaviors/trasparenza.py:230
 msgid "strumenti_tutela_label"
 msgstr ""
 
 #. Default: "Struttura"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:211
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:206
 msgid "struttura_label"
 msgstr ""
 
 #. Default: "Struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:82
+#: design/plone/contenttypes/behaviors/luogo.py:83
 msgid "struttura_responsabile"
 msgstr ""
 
 #. Default: "Struttura responsabile del luogo."
-#: design/plone/contenttypes/behaviors/luogo.py:63
+#: design/plone/contenttypes/behaviors/luogo.py:64
 msgid "struttura_responsabile_correlati"
 msgstr ""
 
 #. Default: "Indicare la struttura responsabile del luogo qualora sia fra unità organizzative del comune inserite nel sito; altrimenti compilare i campi testuali relativi alla struttura responsabile"
-#: design/plone/contenttypes/behaviors/luogo.py:67
+#: design/plone/contenttypes/behaviors/luogo.py:68
 msgid "struttura_responsabile_correlati_help"
 msgstr ""
 
 #. Default: "Nome/link al sito web della struttura che gestisce il luogo, se questa non è comunale."
-#: design/plone/contenttypes/behaviors/luogo.py:84
+#: design/plone/contenttypes/behaviors/luogo.py:85
 msgid "struttura_responsabile_help"
 msgstr ""
 
 #. Default: "Seleziona la lista delle strutture politiche coinvolte."
-#: design/plone/contenttypes/behaviors/strutture_correlate.py:25
+#: design/plone/contenttypes/behaviors/strutture_correlate.py:26
 msgid "strutture_politiche_help"
 msgstr ""
 
 #. Default: "Indicare gli uffici/enti che supportano l'evento."
-#: design/plone/contenttypes/behaviors/evento.py:149
+#: design/plone/contenttypes/behaviors/evento.py:97
 msgid "supportato_da_help"
 msgstr ""
 
 #. Default: "Evento supportato da"
-#: design/plone/contenttypes/behaviors/evento.py:145
+#: design/plone/contenttypes/behaviors/evento.py:93
 msgid "supportato_da_label"
 msgstr ""
 
 #. Default: "Seleziona una lista di argomenti d'interesse per questo contenuto."
-#: design/plone/contenttypes/behaviors/argomenti.py:22
+#: design/plone/contenttypes/behaviors/argomenti.py:26
 msgid "tassonomia_argomenti_help"
 msgstr ""
 
-#. Default: "Tassonomia argomenti"
-#: design/plone/contenttypes/behaviors/argomenti.py:21
+#. Default: "Argomenti"
+#: design/plone/contenttypes/behaviors/argomenti.py:25
 msgid "tassonomia_argomenti_label"
 msgstr ""
 
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/evento.py:104
-msgid "telefono_event_help"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare gli organizzatori."
-#: design/plone/contenttypes/behaviors/evento.py:105
-msgid "telefono_event_label"
-msgstr ""
-
-#. Default: "Indicare un riferimento telefonico per poter contattare i referenti."
-#: design/plone/contenttypes/behaviors/contatti.py:19
-msgid "telefono_help"
-msgstr ""
-
-#. Default: "Telefono"
-#: design/plone/contenttypes/behaviors/contatti.py:18
-msgid "telefono_label"
-msgstr ""
-
-#. Default: "Contatto telefonico della persona. E' possibile inserire più di un numero. Premendo \"Invio\" o \"tab\" si può passare al successivo da inserire."
-#: design/plone/contenttypes/interfaces/persona.py:117
-msgid "telefono_persona_help"
-msgstr ""
-
-#. Default: "Numero di telefono"
-#: design/plone/contenttypes/interfaces/persona.py:116
-msgid "telefono_persona_label"
-msgstr ""
-
-#. Default: "Temi"
-#: design/plone/contenttypes/interfaces/dataset.py:14
-msgid "temi"
-msgstr ""
-
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:167
+#: design/plone/contenttypes/interfaces/servizio.py:236
 msgid "tempi_e_scadenze"
 msgstr ""
 
 #. Default: "Descrivere le informazioni dettagliate riguardo eventuali tempi e scadenze di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:169
+#: design/plone/contenttypes/interfaces/servizio.py:238
 msgid "tempi_e_scadenze_help"
 msgstr ""
 
 #. Default: "Tempi e scadenze"
-#: design/plone/contenttypes/interfaces/servizio.py:395
+#: design/plone/contenttypes/interfaces/servizio.py:508
 msgid "tempi_e_scadenze_label"
 msgstr ""
 
 #. Default: "Inserisci il tempo medio del procedimento."
-#: design/plone/contenttypes/behaviors/trasparenza.py:91
+#: design/plone/contenttypes/behaviors/trasparenza.py:92
 msgid "tempo_medio_help"
 msgstr ""
 
 #. Default: "Tempo medio del procedimento"
-#: design/plone/contenttypes/behaviors/trasparenza.py:86
+#: design/plone/contenttypes/behaviors/trasparenza.py:87
 msgid "tempo_medio_label"
 msgstr ""
 
 #. Default: "Testata"
-#: design/plone/contenttypes/behaviors/argomenti.py:104
+#: design/plone/contenttypes/behaviors/argomenti.py:232
 #: design/plone/contenttypes/behaviors/info_testata.py:62
 msgid "testata_fieldset_label"
 msgstr ""
 
-#: design/plone/contenttypes/interfaces/bando.py:28
+#: design/plone/contenttypes/interfaces/bando.py:29
 msgid "text_help"
 msgstr ""
 
 #. Default: "Testo"
-#: design/plone/contenttypes/interfaces/bando.py:27
+#: design/plone/contenttypes/interfaces/bando.py:28
 msgid "text_label"
 msgstr ""
 
-#. Default: "Tipologia documento"
-#: design/plone/contenttypes/interfaces/messaggio.py:49
-msgid "tipologia_documento"
-msgstr ""
-
-#. Default: "Seleziona la tipologia del documento."
-#: design/plone/contenttypes/interfaces/documento.py:30
-msgid "tipologia_documento_help"
-msgstr ""
-
-#. Default: "Tipologia del documento"
-#: design/plone/contenttypes/interfaces/documento.py:29
-msgid "tipologia_documento_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia della notizia."
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:29
-msgid "tipologia_notizia_help"
-msgstr ""
-
-#. Default: "Tipologia notizia"
-#: design/plone/contenttypes/behaviors/news_additional_fields.py:28
-msgid "tipologia_notizia_label"
-msgstr ""
-
-#. Default: "Specificare la tipologia di organizzazione: politica, amminsitrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:60
-msgid "tipologia_organizzazione_help"
-msgstr ""
-
-#. Default: "Tipologia organizzazione"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:57
-msgid "tipologia_organizzazione_label"
-msgstr ""
-
-#. Default: "Seleziona la tipologia di persona: politica, amministrativa o di altro tipo."
-#: design/plone/contenttypes/interfaces/persona.py:86
-msgid "tipologia_persona_help"
-msgstr ""
-
-#. Default: "Tipologia persona"
-#: design/plone/contenttypes/interfaces/persona.py:85
-msgid "tipologia_persona_label"
-msgstr ""
-
-#. Default: "Inserisci i valori utilizzabili per le tipologie di un Documento. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:46
-msgid "tipologie_documento_help"
+#. Default: "Timeline tempi e scadenze"
+#: design/plone/contenttypes/interfaces/servizio.py:246
+msgid "timeline_tempi_scadenze"
 msgstr ""
 
-#. Default: "Tipologie Documento"
-#: design/plone/contenttypes/controlpanels/settings.py:45
-msgid "tipologie_documento_label"
+#. Default: "Timeline tempi e scadenze del servizio: indicare per ogni scadenza un titolo descrittivo ed un eventuale sottotitolo. Per ogni scadenza, selezionare opzionalmente o l'intervallo (Campi \"Intervallo\" e \"Tipo Intervallo\", es. \"1\" e \"settimana\"), oppure direttamente una data di scadenza (campo: \"Data Scadenza\", esempio 31/12/2023). Se vengono compilati entrambi, ha priorità il campo \"Data Scadenza\"."
+#: design/plone/contenttypes/interfaces/servizio.py:249
+msgid "timeline_tempi_scadenze_help"
 msgstr ""
 
 #. Default: "Inserisci i valori utilizzabili per le tipologie di una Notizia. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:19
+#: design/plone/contenttypes/controlpanels/settings.py:22
 msgid "tipologie_notizia_help"
 msgstr ""
 
 #. Default: "Tipologie Notizia"
-#: design/plone/contenttypes/controlpanels/settings.py:18
+#: design/plone/contenttypes/controlpanels/settings.py:21
 msgid "tipologie_notizia_label"
 msgstr ""
 
-#. Default: "Inserisci i valori utilizzabili per le tipologie di una Persona. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:72
-msgid "tipologie_persona_help"
-msgstr ""
-
-#. Default: "Tipologie Persona"
-#: design/plone/contenttypes/controlpanels/settings.py:71
-msgid "tipologie_persona_label"
-msgstr ""
-
 #. Default: "Inserisci i valori utilizzabili per le tipologie di un' Unità Organizzativa. Se il sito è multilingua, puoi inserire valori diversi a seconda delle lingue del sito."
-#: design/plone/contenttypes/controlpanels/settings.py:34
+#: design/plone/contenttypes/controlpanels/settings.py:37
 msgid "tipologie_unita_organizzativa_help"
 msgstr ""
 
 #. Default: "Tipologie Unità Organizzativa"
-#: design/plone/contenttypes/controlpanels/settings.py:30
+#: design/plone/contenttypes/controlpanels/settings.py:33
 msgid "tipologie_unita_organizzativa_label"
 msgstr ""
 
 #. Default: "Titolare"
-#: design/plone/contenttypes/interfaces/dataset.py:29
+#: design/plone/contenttypes/interfaces/dataset.py:22
 msgid "titolare"
 msgstr ""
 
 #. Default: "Eventuale titolare del potere sostitutivo."
-#: design/plone/contenttypes/behaviors/trasparenza.py:243
+#: design/plone/contenttypes/behaviors/trasparenza.py:244
 msgid "titolare_potere_sostitutivo_help"
 msgstr ""
 
 #. Default: "Titolare del potere sostitutivo"
-#: design/plone/contenttypes/behaviors/trasparenza.py:238
+#: design/plone/contenttypes/behaviors/trasparenza.py:239
 msgid "titolare_potere_sostitutivo_label"
 msgstr ""
 
 #. Default: "Trasparenza"
-#: design/plone/contenttypes/behaviors/trasparenza.py:292
+#: design/plone/contenttypes/behaviors/trasparenza.py:291
 msgid "trasparenza_fieldset_label"
 msgstr ""
 
+#. Default: "Tipo"
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:17
+msgid "type_help"
+msgstr ""
+
 #. Default: "Seleziona l'ufficio responsabile di questo bando."
-#: design/plone/contenttypes/interfaces/bando.py:110
+#: design/plone/contenttypes/interfaces/bando.py:111
 msgid "ufficio_responsabile_bando_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del bando"
-#: design/plone/contenttypes/interfaces/bando.py:106
+#: design/plone/contenttypes/interfaces/bando.py:107
 msgid "ufficio_responsabile_bando_label"
 msgstr ""
 
 #. Default: "Seleziona l'ufficio responsabile di questo documento."
-#: design/plone/contenttypes/interfaces/documento.py:43
+#: design/plone/contenttypes/interfaces/documento.py:73
 msgid "ufficio_responsabile_documento_help"
 msgstr ""
 
 #. Default: "Ufficio responsabile del documento"
-#: design/plone/contenttypes/interfaces/documento.py:39
+#: design/plone/contenttypes/interfaces/documento.py:69
 msgid "ufficio_responsabile_documento_label"
 msgstr ""
 
 #. Default: "Ufficio responsabile"
 #: design/plone/contenttypes/interfaces/documento_personale.py:62
 msgid "ufficio_responsabile_documento_personale"
 msgstr ""
 
-#. Default: "Uffici responsabili"
-#: design/plone/contenttypes/interfaces/servizio.py:216
+#. Default: "Unità organizzativa responsabile"
+#: design/plone/contenttypes/interfaces/servizio.py:302
 msgid "ufficio_responsabile_erogazione"
 msgstr ""
 
 #. Default: "Seleziona gli uffici responsabili dell'erogazione di questo servizio."
-#: design/plone/contenttypes/interfaces/servizio.py:217
+#: design/plone/contenttypes/interfaces/servizio.py:306
 msgid "ufficio_responsabile_help"
 msgstr ""
 
 #. Default: "Ufficio di riferimento"
 #: design/plone/contenttypes/interfaces/pratica.py:17
 msgid "ufficio_riferimento"
 msgstr ""
@@ -2660,56 +2651,56 @@
 msgstr ""
 
 #. Default: "Seleziona la lista delle unità amministrative responsabili di questo argomento."
 #: design/plone/contenttypes/interfaces/pagina_argomento.py:48
 msgid "unita_amministrative_responsabili_help"
 msgstr ""
 
+#. Default: "Seleziona l'organizzazione presso la quale svolge l'incarico."
+#: design/plone/contenttypes/interfaces/incarico.py:64
+msgid "unita_organizzativa_incarico_help"
+msgstr ""
+
+#. Default: "Unità organizzativa"
+#: design/plone/contenttypes/interfaces/incarico.py:60
+msgid "unita_organizzativa_incarico_label"
+msgstr ""
+
 #. Default: "Descrizione dei compiti assegnati alla struttura."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:19
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:23
 msgid "uo_competenze_help"
 msgstr ""
 
 #. Default: "Competenze"
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:18
+#: design/plone/contenttypes/interfaces/unita_organizzativa.py:22
 msgid "uo_competenze_label"
 msgstr ""
 
-#. Default: "Inserisci eventuali informazioni di contatto aggiuntive non contemplate nei campi precedenti. Utilizza questo campo se ci sono dei contatti aggiuntivi rispetto ai contatti della sede principale. Se inserisci un collegamento con un indirizzo email, aggiungi \"mailto:\" prima dell'indirizzo, per farlo aprire direttamente nel client di posta."
-#: design/plone/contenttypes/interfaces/unita_organizzativa.py:139
-msgid "uo_contact_info_description"
-msgstr ""
-
 #. Default: "Note di aggiornamento"
-#: design/plone/contenttypes/behaviors/update_note.py:16
+#: design/plone/contenttypes/behaviors/update_note.py:17
 msgid "update_note_label"
 msgstr ""
 
+#. Default: "Il valore del punto di contatto: il numero compreso di prefisso internazionale (se telefono), l'account (se social network), l'URL (se sito o pagina web), l'indirizzo email (se email)."
+#: design/plone/contenttypes/interfaces/punto_di_contatto.py:54
+msgid "value_punto_contatto_help"
+msgstr ""
+
 #. Default: "Vincoli"
-#: design/plone/contenttypes/interfaces/servizio.py:196
+#: design/plone/contenttypes/interfaces/servizio.py:282
 msgid "vincoli"
 msgstr ""
 
 #. Default: "Descrizione degli eventuali vincoli presenti."
-#: design/plone/contenttypes/interfaces/servizio.py:198
+#: design/plone/contenttypes/interfaces/servizio.py:284
 msgid "vincoli_help"
 msgstr ""
 
-#. Default: "Indicare un indirizzo web di riferimento a questo evento."
-#: design/plone/contenttypes/behaviors/evento.py:138
-msgid "web_event_help"
-msgstr ""
-
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/evento.py:137
-msgid "web_event_label"
-msgstr ""
-
-#. Default: "Indicare un indirizzo web di riferimento."
-#: design/plone/contenttypes/behaviors/contatti.py:53
-msgid "web_help"
+#. Default: "Mostra i PDF in anteprima"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:12
+msgid "visualize_files_title"
 msgstr ""
 
-#. Default: "Sito web"
-#: design/plone/contenttypes/behaviors/contatti.py:52
-msgid "web_label"
+#. Default: "Permette di aprire l'anteprima di tutti i PDF di questa cartella in una tab separata, altrimenti i PDF vengono scaricati"
+#: design/plone/contenttypes/interfaces/cartella_modulistica.py:13
+msgid "visulize_files_description"
 msgstr ""
```

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/update.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/locales/update.sh` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/locales/update.sh`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/overrides.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/overrides.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/__init__.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/patches/baseserializer.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/patches/baseserializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/permissions.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/actions.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/catalog.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/controlpanel.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/diff_tool.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/registry/criteria.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/registry/settings.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/repositorytool.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/rolemap.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Bando.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Dataset.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Document.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Documento.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Event.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Incarico.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Modulo.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Modulo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/News_Item.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Persona.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Persona.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Pratica.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Servizio.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Servizio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types/Venue.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types/Venue.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/default/types.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/correlati.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/documento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/dxfields.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/news.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/persona.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/servizio.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/deserializers/venue.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/deserializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/bando.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/documento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/dxcontent.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/dxcontent.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/dxfields.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/modulo.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/persona.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/relationfield.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/relationfield.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/servizio.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/summary.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/summary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/serializers/venue.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/serializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/content/add.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/content/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/controlpanel.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/navigation/get.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/navigation/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/scadenziario/post.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/scadenziario/post.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/trasparenza/get.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/trasparenza/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/services/types/get.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/restapi/types/adapters.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/restapi/types/adapters.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/schema_overrides.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/schema_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/setuphandlers.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/testing.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/example.pdf` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/example.pdf`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/example.png` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/example.png`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_argomenti.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_base_serializer.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_luogo.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_show_modified.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_behavior_update_note.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_behavior_update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_change_news_type.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_bando.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_document.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_documento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_event.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_event.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_folder.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_luogo.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_modulo.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_news.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_persona.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_servizio.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_custom_service_navigation.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_custom_service_navigation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_move_news_items_view.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_move_news_items_view.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_service_scadenziario.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_service_scadenziario.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_setup.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_substructure_creation.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_substructure_creation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_summary_serializer.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/tests/test_vocabularies.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/draftjs_converter.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/draftjs_converter.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/to_7001.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/to_7001.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/to_7002.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/to_7002.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/upgrades/upgrades.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/utils.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/configure.zcml` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/mockup.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/mockup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/people_vocabulary.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/people_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py` & `design.plone.contenttypes-6.2.2/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/PKG-INFO` & `design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.2.1
+Version: 6.2.2
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,37 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
-Requires-Dist: setuptools
-Requires-Dist: z3c.jbot
-Requires-Dist: plone.api>=1.8.4
-Requires-Dist: plone.app.dexterity>2.6.9
-Requires-Dist: collective.venue[geolocation]
-Requires-Dist: collective.volto.blocksfield
-Requires-Dist: collective.z3cform.datagridfield
-Requires-Dist: plone.formwidget.geolocation
-Requires-Dist: redturtle.volto>=5.0.0
-Requires-Dist: redturtle.bandi
-Requires-Dist: z3c.unconfigure
-Requires-Dist: eea.api.taxonomy
-Requires-Dist: openpyxl
-Requires-Dist: collective.volto.enhancedlinks
-Provides-Extra: test
-Requires-Dist: plone.app.testing; extra == "test"
-Requires-Dist: collective.volto.blocksfield; extra == "test"
-Requires-Dist: plone.testing>=5.0.0; extra == "test"
-Requires-Dist: plone.app.contenttypes; extra == "test"
-Requires-Dist: plone.app.robotframework[debug]; extra == "test"
-Requires-Dist: collective.MockMailHost; extra == "test"
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Tests](https://github.com/RedTurtle/design.plone.contenttypes/actions/workflows/tests.yml/badge.svg)](https://github.com/RedTurtle/design.plone.contenttypes/actions)
 [![Coverage](https://coveralls.io/repos/github/RedTurtle/design.plone.contenttypes/badge.svg?branch=main)](https://coveralls.io/github/RedTurtle/design.plone.contenttypes?branch=main)
@@ -518,14 +498,22 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.2.2 (2024-03-19)
+------------------
+
+- @@check-servizi: provides also the full list of servizi.
+  [daniele]
+- UnitaOrganizzativa.assessore_riferimento title internationalize.
+  [folix-01]
+
 6.2.1 (2024-03-07)
 ------------------
 
 - Added check for blocks field in check_luoghi view.
   [eikichi18]
```

### Comparing `design.plone.contenttypes-6.2.1/src/design.plone.contenttypes.egg-info/SOURCES.txt` & `design.plone.contenttypes-6.2.2/src/design.plone.contenttypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

