# Comparing `tmp/unitxt-1.7.4.tar.gz` & `tmp/unitxt-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.7.4.tar", last modified: Thu Mar 28 15:18:29 2024, max compression
+gzip compressed data, was "unitxt-1.7.6.tar", last modified: Mon Apr  8 17:50:17 2024, max compression
```

## Comparing `unitxt-1.7.4.tar` & `unitxt-1.7.6.tar`

### file list

```diff
@@ -1,1044 +1,1083 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.579349 unitxt-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 15:18:22.000000 unitxt-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-28 15:18:22.000000 unitxt-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-03-28 15:18:29.575349 unitxt-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-28 15:18:22.000000 unitxt-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-28 15:18:22.000000 unitxt-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:18:29.579349 unitxt-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-28 15:18:22.000000 unitxt-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.383347 unitxt-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.403347 unitxt-1.7.4/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.411347 unitxt-1.7.4/src/unitxt/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/card.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.395347 unitxt-1.7.4/src/unitxt/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.415347 unitxt-1.7.4/src/unitxt/catalog/augmentors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/augmentors/no_augmentation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.423347 unitxt-1.7.4/src/unitxt/catalog/cards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.423347 unitxt-1.7.4/src/unitxt/catalog/cards/20_newsgroups/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/20_newsgroups.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.383347 unitxt-1.7.4/src/unitxt/catalog/cards/CFPB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.423347 unitxt-1.7.4/src/unitxt/catalog/cards/CFPB/product/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/CFPB/product/2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/CFPB/product/watsonx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ag_news.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.423347 unitxt-1.7.4/src/unitxt/catalog/cards/ai2_arc/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.427347 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/it.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.435347 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.435347 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/all_1/
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/am_ET.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/da_DK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/de_DE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/el_GR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/en_US.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/es_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/he_IL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/id_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/is_IS.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/it_IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/km_KH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/my_MM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/te_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/th_TH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/argument_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/atis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/atta_q.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.435347 unitxt-1.7.4/src/unitxt/catalog/cards/babi/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/babi/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/banking77.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.459348 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/acm_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/afr_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/als_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/amh_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/apc_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/arb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/arb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ars_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ary_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/arz_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/asm_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/azj_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/bam_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ben_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ben_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/bod_tibt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/bul_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/cat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ceb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ces_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ckb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/dan_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/deu_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ell_grek.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/eng_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/est_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/eus_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/fin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/fra_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/fuv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/gaz_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/grn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/guj_gujr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hau_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/heb_hebr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hin_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hrv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hye_armn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ibo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ilo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ind_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/isl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ita_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/jav_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/jpn_jpan.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kac_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kan_knda.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kat_geor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kea_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/khk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/khm_khmr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kir_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kor_hang.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lao_laoo.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lit_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lug_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/luo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lvs_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mal_mlym.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mar_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mlt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mri_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mya_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nld_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nob_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/npi_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/npi_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nya_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ory_orya.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pan_guru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pbt_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pes_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/plt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/por_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ron_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/rus_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/shn_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sin_sinh.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/slk_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/slv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sna_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/snd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/som_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sot_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/spa_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/srp_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ssw_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/swe_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/swh_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tam_taml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tel_telu.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tgl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tha_thai.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tir_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tsn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tur_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/urd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/urd_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/uzn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/vie_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/war_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/wol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/xho_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/yor_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zho_hans.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zho_hant.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zsm_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zul_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/bold.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.459348 unitxt-1.7.4/src/unitxt/catalog/cards/boolq/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/boolq/classification.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/boolq/multiple_choice.json
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/claim_stance_topic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.459348 unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/plus.json
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/small.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cnn_dailymail.json
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/coedit_gec.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.387347 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.459348 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.463348 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.463348 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/cola.json
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/copa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.463348 unitxt-1.7.4/src/unitxt/catalog/cards/coqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/coqa/completion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/coqa/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/dart.json
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/dbpedia_14.json
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ethos_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.463348 unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/16k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/2k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/4k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/8k.json
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/financial_tweets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.463348 unitxt-1.7.4/src/unitxt/catalog/cards/head_qa/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/head_qa/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/head_qa/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/hellaswag.json
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/human_eval.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/law_stack_exchange.json
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/ledgar.json
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mbpp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/medical_abstracts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.463348 unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/de.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/tu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/anatomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/astronomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/business_ethics.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/computer_security.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/econometrics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/formal_logic.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/global_facts.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_geography.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/human_aging.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/human_sexuality.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/international_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/jurisprudence.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/machine_learning.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/management.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/marketing.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/medical_genetics.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/miscellaneous.json
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/moral_disputes.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/nutrition.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/philosophy.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/prehistory.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_accounting.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/public_relations.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/security_studies.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/sociology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/virology.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/world_religions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/mrpc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/multidoc2dial/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/multidoc2dial/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/news_category_classification_headline.json
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/openbook_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/piqa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/pop_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/qnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/qqp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/race_all.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/race_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/race_middle.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/ModApte.json
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/ModHayes.json
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/ModLewis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/rte.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/sciq.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/sst2.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/stsb.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/tab_fact.json
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/tablerow_classify.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/toxigen.json
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/trec.json
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/unfair_tos.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.387347 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/ceb/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/da/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/da/ddt.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/de/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.475348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/en/ewt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/en/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/hr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/pt/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/ru/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sk/snk.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sv/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sv/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/tl/trg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/zh/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/zh/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wiki_bio.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wikitq.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/debiased.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/l.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/m.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/s.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/xl.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/xs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.479348 unitxt-1.7.4/src/unitxt/catalog/cards/wmt/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wmt/en_de.json
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wmt/en_fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wmt/en_ro.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.483348 unitxt-1.7.4/src/unitxt/catalog/cards/wnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wnli/truthfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/wsc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.491348 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/amharic.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/arabic.json
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/azerbaijani.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/bengali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/burmese.json
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/english.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/french.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/gujarati.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/hausa.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/hindi.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/igbo.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/indonesian.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/japanese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/kirundi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/korean.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/kyrgyz.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/marathi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/nepali.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/oromo.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/pashto.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/persian.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/pidgin.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/portuguese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/punjabi.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/russian.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/serbian_latin.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/sinhala.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/somali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/spanish.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/swahili.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/tamil.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/telugu.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/thai.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/tigrinya.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/turkish.json
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/ukrainian.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/urdu.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/uzbek.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/vietnamese.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/welsh.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/yoruba.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.491348 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/bg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/hi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/sw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/th.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/ur.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/vi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xnli/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xsum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.491348 unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/jp.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/cards/yahoo_answers_topics.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.495348 unitxt-1.7.4/src/unitxt/catalog/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/empty_input_output_separator.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/human_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.495348 unitxt-1.7.4/src/unitxt/catalog/formats/models/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/alpaca_instruct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.495348 unitxt-1.7.4/src/unitxt/catalog/formats/models/flan/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/flan/exq_exa.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/flan/few_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.495348 unitxt-1.7.4/src/unitxt/catalog/formats/models/labrador/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/labrador/few_shot.json
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/labrador/zero_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.495348 unitxt-1.7.4/src/unitxt/catalog/formats/models/mistral/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.495348 unitxt-1.7.4/src/unitxt/catalog/formats/models/mistral/instruction/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/models/mistral/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/textual_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/user_agent.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/formats/user_assistant.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.503348 unitxt-1.7.4/src/unitxt/catalog/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/accuracy_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.503348 unitxt-1.7.4/src/unitxt/catalog/metrics/bert_score/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/bleu.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/f1_macro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/f1_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/f1_micro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/f1_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/f1_weighted.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/kendalltau_b.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/kpa.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/map.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/matthews_correlation.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/max_accuracy_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/max_f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/ndcg.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/ner.json
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/normalized_sacrebleu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.503348 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.503348 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity_a/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.503348 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity_chat/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.503348 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity_q/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/precision_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/precision_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/precision_micro_multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.507348 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/answer_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/answer_reward.json
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/bert_k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/bert_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/context_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/context_perplexity.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/context_relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.507348 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/correctness/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/faithfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/map.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rag/recall.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/recall_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/recall_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/recall_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/regard.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/retrieval_at_k.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.507348 unitxt-1.7.4/src/unitxt/catalog/metrics/reward/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.511349 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/roc_auc.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rouge.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/sacrebleu.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/safety.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.511349 unitxt-1.7.4/src/unitxt/catalog/metrics/sentence_bert/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/spearman.json
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/token_overlap_with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/metrics/wer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.391347 unitxt-1.7.4/src/unitxt/catalog/operators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.391347 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.511349 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/classification/by_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.511349 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.511349 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.511349 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/operators/balancers/qa/by_answer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.515349 unitxt-1.7.4/src/unitxt/catalog/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/capitalize.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/convert_to_boolean.json
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/first_character.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/get_string_after_colon.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/load_json.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/load_json_from_predictions.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/lower_case.json
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/lower_case_till_punc.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/match_closest_option.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/remove_none_from_list.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/stance_to_pro_con.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/str_to_float_format.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/take_first_non_empty_line.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/take_first_word.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/to_list_by_comma.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/to_span_label_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/to_string.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/to_string_stripped.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/to_yes_or_none.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/toxic_or_not_toxic.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/processors/yes_no_to_int.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.515349 unitxt-1.7.4/src/unitxt/catalog/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/default.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/diverse_labels_sampler.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/large_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/large_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/small_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/small_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/splitters/test_only.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.391347 unitxt-1.7.4/src/unitxt/catalog/system_prompt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.515349 unitxt-1.7.4/src/unitxt/catalog/system_prompt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/system_prompt/models/japanese_llama.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/system_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/system_prompts/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/alpaca.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/labrador.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/classification/binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/classification/multi_class/relation.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/classification/multi_class.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/classification/multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/completion/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/completion/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/completion/multiple_choice.json
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/generation.json
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/grammatical_error_correction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/ner/all_entity_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/ner/single_entity_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.519349 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/qa/with_context/extractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/tasks/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/regression/single_text.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/regression/two_texts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/tasks/span_labeling/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/span_labeling/extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/tasks/summarization/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/summarization/abstractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/tasks/translation/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/tasks/translation/directed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.395347 unitxt-1.7.4/src/unitxt/catalog/templates/classification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/instruction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.523349 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.527349 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.527349 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.395347 unitxt-1.7.4/src/unitxt/catalog/templates/completion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.527349 unitxt-1.7.4/src/unitxt/catalog/templates/completion/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/abstractive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/abstractive/standard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.527349 unitxt-1.7.4/src/unitxt/catalog/templates/completion/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/multiple_choice/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/completion/multiple_choice/title.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.527349 unitxt-1.7.4/src/unitxt/catalog/templates/generation/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/generation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/generation/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.527349 unitxt-1.7.4/src/unitxt/catalog/templates/grammatical_error_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/key_val.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/key_val_with_new_lines.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.399347 unitxt-1.7.4/src/unitxt/catalog/templates/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.531349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.531349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.531349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.531349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.531349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.531349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.535349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.535349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.535349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.535349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.535349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.539349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.539349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.539349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.539349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.539349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.543349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.543349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.543349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.543349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.547349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.547349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.547349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.547349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.547349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.547349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.551349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/open/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/open/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/open/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/open/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/open/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/open/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.551349 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/ffqa.json
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/question_first.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/qa/with_context/with_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.399347 unitxt-1.7.4/src/unitxt/catalog/templates/regression/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.551349 unitxt-1.7.4/src/unitxt/catalog/templates/regression/single_text/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/single_text/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/single_text/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/single_text/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.551349 unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.551349 unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.399347 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.555349 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/having.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/span_labeling/extraction/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.399347 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.555349 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/full.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/passive.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/professional.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.555349 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.559349 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.559349 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.559349 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.559349 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.399347 unitxt-1.7.4/src/unitxt/catalog/templates/translation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.559349 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/instructional.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/playful.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog/templates/translation/directed/title.json
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/collections_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    16611 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/dialog_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    22321 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   128646 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21231 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    76385 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/parsing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.559349 unitxt-1.7.4/src/unitxt/prepare_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/prepare_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/prepare_utils/card_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/prepare_utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.563349 unitxt-1.7.4/src/unitxt/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.563349 unitxt-1.7.4/src/unitxt/service/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/service/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/service/metrics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/service/metrics/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/settings_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/span_lableing_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/string_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/struct_data_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/system_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    20522 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.563349 unitxt-1.7.4/src/unitxt/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/card.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.563349 unitxt-1.7.4/src/unitxt/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/gradio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/load_catalog_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/ui_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/ui/ui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:18:22.000000 unitxt-1.7.4/src/unitxt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:18:29.563349 unitxt-1.7.4/src/unitxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-03-28 15:18:29.000000 unitxt-1.7.4/src/unitxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47647 2024-03-28 15:18:29.000000 unitxt-1.7.4/src/unitxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:18:29.000000 unitxt-1.7.4/src/unitxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 15:18:29.000000 unitxt-1.7.4/src/unitxt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-28 15:18:29.000000 unitxt-1.7.4/src/unitxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 15:18:29.000000 unitxt-1.7.4/src/unitxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.445190 unitxt-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 17:50:13.000000 unitxt-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:50:13.000000 unitxt-1.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-08 17:50:17.445190 unitxt-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-08 17:50:13.000000 unitxt-1.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-08 17:50:14.000000 unitxt-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:17.445190 unitxt-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-08 17:50:14.000000 unitxt-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.253187 unitxt-1.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.273187 unitxt-1.7.6/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.281187 unitxt-1.7.6/src/unitxt/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/card.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.285187 unitxt-1.7.6/src/unitxt/catalog/augmentors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/no_augmentation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.293187 unitxt-1.7.6/src/unitxt/catalog/cards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.293187 unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.253187 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.297187 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/watsonx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ag_news.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.297187 unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.297187 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/it.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.305187 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.305187 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/am_ET.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/da_DK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/de_DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/el_GR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/en_US.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/es_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/he_IL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/id_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/is_IS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/it_IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/km_KH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/my_MM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/te_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/th_TH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/argument_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/atis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/atta_q.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.305187 unitxt-1.7.6/src/unitxt/catalog/cards/babi/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/babi/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/banking77.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.325188 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/acm_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/afr_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/als_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/amh_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/apc_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ars_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ary_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arz_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/asm_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/azj_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bam_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bod_tibt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bul_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/cat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ceb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ces_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ckb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/dan_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/deu_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ell_grek.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eng_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/est_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eus_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fra_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fuv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/gaz_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/grn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/guj_gujr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hau_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/heb_hebr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hrv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hye_armn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ibo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ilo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ind_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/isl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ita_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jav_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jpn_jpan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kac_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kan_knda.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kat_geor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kea_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khm_khmr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kir_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kor_hang.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lao_laoo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lit_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lug_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/luo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lvs_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mal_mlym.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mar_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mlt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mri_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mya_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nld_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nob_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nya_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ory_orya.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pan_guru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pbt_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pes_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/plt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/por_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ron_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/rus_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/shn_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_sinh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slk_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sna_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/snd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/som_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sot_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/spa_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/srp_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ssw_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swe_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swh_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tam_taml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tel_telu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tha_thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tir_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tsn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tur_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/uzn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/vie_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/war_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/wol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/xho_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/yor_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hans.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zsm_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zul_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/bold.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.325188 unitxt-1.7.6/src/unitxt/catalog/cards/boolq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/boolq/classification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/boolq/multiple_choice.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/claim_stance_topic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.325188 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/plus.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/small.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cnn_dailymail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/paraphrase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/rewriting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/selection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit_error_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit_gec.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.253187 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cola.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/copa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/coqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coqa/completion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coqa/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/dart.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/dbpedia_14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ethos_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/16k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/2k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/4k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/8k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/financial_tweets.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/hellaswag.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/hh_rlhf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/human_eval.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/law_stack_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ledgar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mbpp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/medical_abstracts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.333188 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/tu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/anatomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/astronomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/business_ethics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/computer_security.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/econometrics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/formal_logic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/global_facts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_geography.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_aging.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_sexuality.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/international_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/jurisprudence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/machine_learning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/management.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/marketing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/medical_genetics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/miscellaneous.json
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_disputes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/nutrition.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/philosophy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/prehistory.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_accounting.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/public_relations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/security_studies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/sociology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/virology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/world_religions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mrpc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/news_category_classification_headline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/openbook_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/piqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/pop_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/qnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/qqp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/race_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/race_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/race_middle.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModApte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModHayes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModLewis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/rte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/sciq.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/sst2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/stsb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/summarize_from_human_feedback.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/tab_fact.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/tablerow_classify.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/toxigen.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/trec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/unfair_tos.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.257187 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ceb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/da/ddt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/de/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/ewt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/hr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ru/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sk/snk.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/trg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wiki_bio.json
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wikitq.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/debiased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/l.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/m.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/s.json
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_ro.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/wnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wnli/truthfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wsc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.353188 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/amharic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/arabic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/azerbaijani.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/bengali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/burmese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/english.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/french.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/gujarati.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hausa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hindi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/igbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/indonesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/japanese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kirundi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/korean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kyrgyz.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/marathi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/nepali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/oromo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pashto.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/persian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pidgin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/portuguese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/punjabi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/russian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_latin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/sinhala.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/somali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/spanish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/swahili.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tamil.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/telugu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tigrinya.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/turkish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/ukrainian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/urdu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/uzbek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/vietnamese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/welsh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/yoruba.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/bg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/hi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/sw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/th.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ur.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/vi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xsum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/jp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/yahoo_answers_topics.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/empty_input_output_separator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/human_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/formats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/alpaca_instruct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/formats/models/flan/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/flan/exq_exa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/flan/few_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.361188 unitxt-1.7.6/src/unitxt/catalog/formats/models/labradorite/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/labradorite/few_shot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.361188 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.361188 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/instruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/textual_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/user_agent.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/user_assistant.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.365188 unitxt-1.7.6/src/unitxt/catalog/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/accuracy_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/char_edit_distance.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_macro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_micro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_weighted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/kendalltau_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/kpa.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/matthews_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/max_accuracy_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/max_f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/ndcg.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/ner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/normalized_sacrebleu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_q/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/precision_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/precision_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/precision_micro_multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_reward.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_perplexity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/correctness/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/faithfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/recall_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/recall_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/recall_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/regard.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rerank_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/retrieval_at_k.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/reward/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/roc_auc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rouge.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/sacrebleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/safety.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/sentence_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/spearman.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/token_overlap_with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/wer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/operators/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/classification/by_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/qa/by_answer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/capitalize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/convert_to_boolean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/first_character.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/get_string_after_colon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/load_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/load_json_from_predictions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/lower_case.json
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/lower_case_till_punc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/match_closest_option.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/remove_none_from_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/stance_to_pro_con.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/str_to_float_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/take_first_non_empty_line.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/take_first_word.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_list_by_comma.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_string_stripped.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_yes_or_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/toxic_or_not_toxic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/yes_no_to_int.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/diverse_labels_sampler.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/large_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/large_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/small_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/small_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/test_only.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/system_prompt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/system_prompt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompt/models/japanese_llama.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/system_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/alpaca.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/labradorite.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_class/relation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_class.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/multiple_choice.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/evaluation/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/generation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/grammatical_error_correction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/ner/all_entity_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/ner/single_entity_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/with_context/extractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/regression/single_text.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/regression/two_texts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/rewriting/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/rewriting/by_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/rewriting/paraphrase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/selection/by_attribute.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/span_labeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/span_labeling/extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/summarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/summarization/abstractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/translation/directed.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.265187 unitxt-1.7.6/src/unitxt/catalog/templates/classification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/instruction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.265187 unitxt-1.7.6/src/unitxt/catalog/templates/completion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.265187 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/generation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/generation/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_correction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_detection/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/key_val.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/key_val_with_new_lines.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/ffqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/question_first.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/with_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/regression/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/paraphrase/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/selection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/having.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/full.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/passive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/professional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/translation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/instructional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/playful.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/collections_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dialog_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133392 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21234 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76915 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/parsing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/prepare_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/prepare_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/prepare_utils/card_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/prepare_utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/service/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/metrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/metrics/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/settings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/span_lableing_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/string_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/struct_data_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/system_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.433189 unitxt-1.7.6/src/unitxt/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.433189 unitxt-1.7.6/src/unitxt/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/gradio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/load_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/ui_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/ui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.433189 unitxt-1.7.6/src/unitxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    49194 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.7.4/LICENSE` & `unitxt-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/PKG-INFO` & `unitxt-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,52 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.7.4
+Version: 1.7.6
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasets>=2.16.0
 Requires-Dist: evaluate
 Requires-Dist: absl-py
 Requires-Dist: ipadic
 Requires-Dist: scipy
+Provides-Extra: service
+Requires-Dist: torch==1.12.1; extra == "service"
+Requires-Dist: fastapi==0.109.0; extra == "service"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
+Requires-Dist: transformers; extra == "service"
 Provides-Extra: base
 Requires-Dist: datasets>=2.16.0; extra == "base"
 Requires-Dist: evaluate; extra == "base"
 Requires-Dist: absl-py; extra == "base"
 Requires-Dist: ipadic; extra == "base"
 Requires-Dist: scipy; extra == "base"
+Provides-Extra: docs
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: piccolo_theme; extra == "docs"
+Requires-Dist: sphinxext-opengraph; extra == "docs"
+Requires-Dist: datasets; extra == "docs"
+Requires-Dist: evaluate; extra == "docs"
+Requires-Dist: nltk; extra == "docs"
+Requires-Dist: sacrebleu; extra == "docs"
+Requires-Dist: absl-py; extra == "docs"
+Requires-Dist: rouge_score; extra == "docs"
+Requires-Dist: scikit-learn; extra == "docs"
+Requires-Dist: jiwer; extra == "docs"
+Requires-Dist: editdistance; extra == "docs"
+Provides-Extra: ui
+Requires-Dist: gradio; extra == "ui"
+Requires-Dist: transformers; extra == "ui"
 Provides-Extra: tests
 Requires-Dist: bert_score; extra == "tests"
 Requires-Dist: transformers; extra == "tests"
 Requires-Dist: sentence_transformers; extra == "tests"
 Requires-Dist: ibm-cos-sdk; extra == "tests"
 Requires-Dist: opendatasets; extra == "tests"
 Requires-Dist: httpretty~=1.1.4; extra == "tests"
@@ -34,90 +56,70 @@
 Requires-Dist: mecab-python3; extra == "tests"
 Requires-Dist: sacrebleu[ko]; extra == "tests"
 Requires-Dist: scikit-learn; extra == "tests"
 Requires-Dist: jiwer; extra == "tests"
 Requires-Dist: conllu; extra == "tests"
 Requires-Dist: llama-index-core; extra == "tests"
 Requires-Dist: llama-index-llms-openai; extra == "tests"
-Provides-Extra: docs
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: piccolo_theme; extra == "docs"
-Requires-Dist: sphinxext-opengraph; extra == "docs"
-Requires-Dist: datasets; extra == "docs"
-Requires-Dist: evaluate; extra == "docs"
-Requires-Dist: nltk; extra == "docs"
-Requires-Dist: sacrebleu; extra == "docs"
-Requires-Dist: absl-py; extra == "docs"
-Requires-Dist: rouge_score; extra == "docs"
-Requires-Dist: scikit-learn; extra == "docs"
-Requires-Dist: jiwer; extra == "docs"
-Requires-Dist: editdistance; extra == "docs"
+Requires-Dist: pytrec-eval; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
-Provides-Extra: service
-Requires-Dist: torch==1.12.1; extra == "service"
-Requires-Dist: fastapi==0.109.0; extra == "service"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
-Requires-Dist: transformers; extra == "service"
-Provides-Extra: ui
-Requires-Dist: gradio; extra == "ui"
-Requires-Dist: transformers; extra == "ui"
 Provides-Extra: all
-Requires-Dist: absl-py; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
-Requires-Dist: jiwer; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: datasets; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: gradio; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: bert_score; extra == "all"
-Requires-Dist: ibm-cos-sdk; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
 Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: transformers; extra == "all"
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: evaluate; extra == "all"
-Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: nltk; extra == "all"
+Requires-Dist: codespell; extra == "all"
 Requires-Dist: llama-index-core; extra == "all"
-Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
 Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: rouge-score; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: evaluate; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
+Requires-Dist: ibm-cos-sdk; extra == "all"
 Requires-Dist: mecab-python3; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: nltk; extra == "all"
-Requires-Dist: datasets>=2.16.0; extra == "all"
 Requires-Dist: ipadic; extra == "all"
-Requires-Dist: datasets; extra == "all"
-Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: fastapi==0.109.0; extra == "all"
-Requires-Dist: rouge-score; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: gradio; extra == "all"
+Requires-Dist: jiwer; extra == "all"
 Requires-Dist: conllu; extra == "all"
-Requires-Dist: editdistance; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: scipy; extra == "all"
 Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
 Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: codespell; extra == "all"
+Requires-Dist: sacrebleu; extra == "all"
+Requires-Dist: editdistance; extra == "all"
+Requires-Dist: httpretty~=1.1.4; extra == "all"
+Requires-Dist: transformers; extra == "all"
+Requires-Dist: datasets>=2.16.0; extra == "all"
+Requires-Dist: tomli; extra == "all"
 Requires-Dist: torch==1.12.1; extra == "all"
+Requires-Dist: absl-py; extra == "all"
+Requires-Dist: bert_score; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
 [![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/adding_dataset.html)
 [![Button](https://img.shields.io/badge/Paper-pink?style=for-the-badge)](https://arxiv.org/abs/2401.14019)
 [![Button](https://img.shields.io/badge/Documentation-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/modules.html)
 [![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog.html)
-[![Button](https://img.shields.io/badge/Contributers-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
+[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
 [![Button](https://img.shields.io/badge/PyPi-pink?style=for-the-badge)](https://pypi.org/project/unitxt/)
 
 
 In the dynamic landscape of generative NLP, traditional text processing pipelines limit research flexibility and reproducibility, as they are tailored to specific dataset, task, and model combinations. The escalating complexity, involving system prompts, model-specific formats, instructions, and more, calls for a shift to a structured, modular, and customizable solution.
 
  Addressing this need, we present Unitxt, an innovative library for customizable textual data preparation and evaluation tailored to generative language models. Unitxt natively integrates with common libraries like HuggingFace and LM-eval-harness and deconstructs processing flows into modular components, enabling easy customization and sharing between practitioners. These components encompass model-specific formats, task prompts, and many other comprehensive dataset processing definitions. The Unitxt-Catalog centralizes these components, fostering collaboration and exploration in modern textual data workflows. Beyond being a tool, Unitxt is a community-driven platform, empowering users to build, share, and advance their pipelines collaboratively.
 
@@ -132,19 +134,19 @@
 
 #
 
 https://github.com/IBM/unitxt/assets/23455264/baef9131-39d4-4164-90b2-05da52919fdf
 
 ### 🦄 Currently on Unitxt Catalog
 
-![NLP Tasks](https://img.shields.io/badge/NLP_tasks-22-blue)
-![Dataset Cards](https://img.shields.io/badge/Dataset_Cards-423-blue)
-![Templates](https://img.shields.io/badge/Templates-204-blue)
-![Formats](https://img.shields.io/badge/Formats-13-blue)
-![Metrics](https://img.shields.io/badge/Metrics-79-blue)
+![NLP Tasks](https://img.shields.io/badge/NLP_tasks-29-blue)
+![Dataset Cards](https://img.shields.io/badge/Dataset_Cards-435-blue)
+![Templates](https://img.shields.io/badge/Templates-218-blue)
+![Formats](https://img.shields.io/badge/Formats-15-blue)
+![Metrics](https://img.shields.io/badge/Metrics-84-blue)
 
 ### 🦄 Run Unitxt Exploration Dashboard
 
 To launch unitxt graphical user interface first install unitxt with ui requirements:
 ```
 pip install unitxt[ui]
 ```
```

### Comparing `unitxt-1.7.4/README.md` & `unitxt-1.7.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
 [![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/adding_dataset.html)
 [![Button](https://img.shields.io/badge/Paper-pink?style=for-the-badge)](https://arxiv.org/abs/2401.14019)
 [![Button](https://img.shields.io/badge/Documentation-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/modules.html)
 [![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog.html)
-[![Button](https://img.shields.io/badge/Contributers-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
+[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
 [![Button](https://img.shields.io/badge/PyPi-pink?style=for-the-badge)](https://pypi.org/project/unitxt/)
 
 
 In the dynamic landscape of generative NLP, traditional text processing pipelines limit research flexibility and reproducibility, as they are tailored to specific dataset, task, and model combinations. The escalating complexity, involving system prompts, model-specific formats, instructions, and more, calls for a shift to a structured, modular, and customizable solution.
 
  Addressing this need, we present Unitxt, an innovative library for customizable textual data preparation and evaluation tailored to generative language models. Unitxt natively integrates with common libraries like HuggingFace and LM-eval-harness and deconstructs processing flows into modular components, enabling easy customization and sharing between practitioners. These components encompass model-specific formats, task prompts, and many other comprehensive dataset processing definitions. The Unitxt-Catalog centralizes these components, fostering collaboration and exploration in modern textual data workflows. Beyond being a tool, Unitxt is a community-driven platform, empowering users to build, share, and advance their pipelines collaboratively.
 
@@ -27,19 +27,19 @@
 
 #
 
 https://github.com/IBM/unitxt/assets/23455264/baef9131-39d4-4164-90b2-05da52919fdf
 
 ### 🦄 Currently on Unitxt Catalog
 
-![NLP Tasks](https://img.shields.io/badge/NLP_tasks-22-blue)
-![Dataset Cards](https://img.shields.io/badge/Dataset_Cards-423-blue)
-![Templates](https://img.shields.io/badge/Templates-204-blue)
-![Formats](https://img.shields.io/badge/Formats-13-blue)
-![Metrics](https://img.shields.io/badge/Metrics-79-blue)
+![NLP Tasks](https://img.shields.io/badge/NLP_tasks-29-blue)
+![Dataset Cards](https://img.shields.io/badge/Dataset_Cards-435-blue)
+![Templates](https://img.shields.io/badge/Templates-218-blue)
+![Formats](https://img.shields.io/badge/Formats-15-blue)
+![Metrics](https://img.shields.io/badge/Metrics-84-blue)
 
 ### 🦄 Run Unitxt Exploration Dashboard
 
 To launch unitxt graphical user interface first install unitxt with ui requirements:
 ```
 pip install unitxt[ui]
 ```
```

### Comparing `unitxt-1.7.4/pyproject.toml` & `unitxt-1.7.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 line-length = 88
 indent-width = 4
 
 # Assume Python 3.8
 target-version = "py38"
 
 [tool.ruff.lint.per-file-ignores]
+"src/*" = ["TID252"]
+".github/*" = ["TID251"]
+".vscode/*" = ["TID251"]
+"tests/*" = ["TID251"]
+"utils/*" = ["TID251"]
 "src/unitxt/__init__.py" = ["F811", "F401"]
 "src/unitxt/metric.py" = ["F811", "F401"]
 "src/unitxt/dataset.py" = ["F811", "F401"]
 "src/unitxt/blocks.py" = ["F811", "F401"]
 "tests/library/test_loaders.py" = ["N802", "N803"]
 "tests/library/test_dataclass.py" = ["F811"]
 "src/unitxt/validate.py" = ["B024"]
@@ -55,21 +60,22 @@
   "D",   # pydocstyle
   "F", # pyflakes
   "E", # pycodestyle
   "B", # bugbear
   "C", # mccabe
   "R", # flake8-rst-docstrings
   "T", # flake8-typing-imports
+  "TID25", #
   "W", # pycodestyle-wordlist
-  "M", # flake8-mypy
+  "RUF100", # flake8-mypy
   "I", # isort
   "G", # flake8-bugbear
   "N", # PEP8 Naming
   "Q", # flake8-quotes
-  "RUF" # ruff
+  "RUF", # ruff
 ]
 ignore = ["E501", "E203", "E722", "D101", "D102", "D103", "D100", "D104", "D105", "D106", "D107", "RUF012", "G004"]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
@@ -93,12 +99,17 @@
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = ["fastapi.Depends", "fastapi.params.Depends", "fastapi.Query", "fastapi.params.Query"]
 
+
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
+"src".msg = "Use unitxt outside src/ and relative imports inside src/ and install unitxt from source with `pip install -e '.[dev]'`."
+
 [tool.codespell]
-ignore-words-list = 'rouge,ot,ans'
+ignore-words-list = 'rouge,ot,ans,nd'
 check-filenames = true
 check-hidden = false
-skip = 'prepare/cards/trec.py'
+regex = "(?<![a-z])[a-z'`]+|[A-Z][a-z'`]*|[a-z]+'[a-z]*|[a-z]+(?=[_-])|[a-z]+(?=[A-Z])|\\d+"
+skip = '*cards/trec*,*cards/belebele*,*cards/amazon_mass*,*cards/reuters21578*,*egg-info*,*/logs/*'
```

### Comparing `unitxt-1.7.4/setup.py` & `unitxt-1.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/__init__.py` & `unitxt-1.7.6/src/unitxt/__init__.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/api.py` & `unitxt-1.7.6/src/unitxt/api.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/artifact.py` & `unitxt-1.7.6/src/unitxt/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/blocks.py` & `unitxt-1.7.6/src/unitxt/blocks.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/card.py` & `unitxt-1.7.6/src/unitxt/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/20_newsgroups/sklearn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups/sklearn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/20_newsgroups.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/CFPB/product/2023.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/2023.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/CFPB/product/watsonx.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/watsonx.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ag_news.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ag_news.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/m.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6845238095238095%*

 * *Differences: {"'loader'": "{'path': 'winogrande', 'name': 'winogrande_m'}",*

 * * "'preprocess_steps'": "{2: {'type': 'cast_fields', 'fields': {replace: OrderedDict([('answer', "*

 * *                       "'int')])}}, 4: {'field_to_field': {replace: OrderedDict([('sentence', "*

 * *                       "'question')])}}, insert: [(0, 'splitters.small_no_test'), (1, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('to_field', 'choices')])), (3, Order […]*

```diff
@@ -1,39 +1,38 @@
 {
     "loader": {
-        "name": "ARC-Challenge",
-        "path": "ai2_arc",
+        "name": "winogrande_m",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
+        {
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
         {
             "fields": {
-                "topic": "science"
+                "answer": "int"
             },
-            "type": "add_fields"
+            "type": "cast_fields"
         },
         {
-            "field_to_field": {
-                "answerKey": "label",
-                "choices": "_choices"
-            },
-            "type": "rename_fields"
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "_choices/label": "labels",
-                "_choices/text": "choices"
+                "sentence": "question"
             },
-            "type": "copy_fields",
-            "use_query": true
-        },
-        {
-            "index_of": "label",
-            "search_in": "labels",
-            "to_field": "answer",
-            "type": "index_of"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ai2_arc/arc_easy.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/s.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6845238095238095%*

 * *Differences: {"'loader'": "{'path': 'winogrande', 'name': 'winogrande_s'}",*

 * * "'preprocess_steps'": "{2: {'type': 'cast_fields', 'fields': {replace: OrderedDict([('answer', "*

 * *                       "'int')])}}, 4: {'field_to_field': {replace: OrderedDict([('sentence', "*

 * *                       "'question')])}}, insert: [(0, 'splitters.small_no_test'), (1, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('to_field', 'choices')])), (3, Order […]*

```diff
@@ -1,39 +1,38 @@
 {
     "loader": {
-        "name": "ARC-Easy",
-        "path": "ai2_arc",
+        "name": "winogrande_s",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
+        {
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
         {
             "fields": {
-                "topic": "science"
+                "answer": "int"
             },
-            "type": "add_fields"
+            "type": "cast_fields"
         },
         {
-            "field_to_field": {
-                "answerKey": "label",
-                "choices": "_choices"
-            },
-            "type": "rename_fields"
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "_choices/label": "labels",
-                "_choices/text": "choices"
+                "sentence": "question"
             },
-            "type": "copy_fields",
-            "use_query": true
-        },
-        {
-            "index_of": "label",
-            "search_in": "labels",
-            "to_field": "answer",
-            "type": "index_of"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/de.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/de.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952380952380953%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}}"}*

```diff
@@ -15,16 +15,15 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
                 "extracted_language": "de"
             }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/en.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/pt.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'pt'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "en"
+                "extracted_language": "pt"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/es.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/ru.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'ru'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "es"
+                "extracted_language": "ru"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/fr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/it.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'it'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "fr"
+                "extracted_language": "it"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/it.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/nl.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'nl'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "it"
+                "extracted_language": "nl"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/nl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/fr.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'fr'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "nl"
+                "extracted_language": "fr"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/pt.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/en.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'en'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "pt"
+                "extracted_language": "en"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil/ru.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/es.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}, 2: {'values': {'extracted_language': 'es'}}}"}*

```diff
@@ -15,22 +15,21 @@
         {
             "field_to_field": [
                 [
                     "metadata/language",
                     "extracted_language"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "ru"
+                "extracted_language": "es"
             }
         },
         {
             "fields": [
                 "extracted_language",
                 "metadata"
             ],
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/almost_evil.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/af_ZA.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/af_ZA.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/all.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/all_1/1.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all_1/1.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/am_ET.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/am_ET.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ar_SA.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ar_SA.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/az_AZ.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/az_AZ.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/bn_BD.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/bn_BD.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ca_ES.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ca_ES.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/cy_GB.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/cy_GB.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/da_DK.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/da_DK.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/de_DE.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/de_DE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/el_GR.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/el_GR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/en_US.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/en_US.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/es_ES.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/es_ES.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/fa_IR.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fa_IR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/fi_FI.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fi_FI.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/fr_FR.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fr_FR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/he_IL.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/he_IL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/hi_IN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hi_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/hu_HU.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hu_HU.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/hy_AM.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hy_AM.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/id_ID.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/id_ID.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/is_IS.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/is_IS.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/it_IT.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/it_IT.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ja_JP.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ja_JP.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/jv_ID.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/jv_ID.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ka_GE.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ka_GE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/km_KH.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/km_KH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/kn_IN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/kn_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ko_KR.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ko_KR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/lv_LV.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/lv_LV.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ml_IN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ml_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/mn_MN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/mn_MN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ms_MY.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ms_MY.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/my_MM.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/my_MM.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/nb_NO.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nb_NO.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/nl_NL.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nl_NL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/pl_PL.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pl_PL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/pt_PT.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pt_PT.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ro_RO.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ro_RO.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ru_RU.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ru_RU.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sl_SL.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sl_SL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sq_AL.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sq_AL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sv_SE.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sv_SE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/sw_KE.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sw_KE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ta_IN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ta_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/te_IN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/te_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/th_TH.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/th_TH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/tl_PH.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tl_PH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/tr_TR.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tr_TR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/ur_PK.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ur_PK.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/vi_VN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/vi_VN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/zh_CN.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_CN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/amazon_mass/zh_TW.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_TW.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/argument_topic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/argument_topic.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'preprocess_steps'": '{delete: [0]}'}*

```diff
@@ -2,21 +2,14 @@
     "loader": {
         "name": "argument_topic",
         "path": "ibm/argument_quality_ranking_30k",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": [
-                "label"
-            ],
-            "to_field": "label",
-            "type": "list_field_values"
-        },
-        {
             "fields": {
                 "classes": [
                     "affirmative action",
                     "algorithmic trading",
                     "assisted suicide",
                     "atheism",
                     "austerity regime",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/atis.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/atis.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949999999999999%*

 * *Differences: {"'preprocess_steps'": "{2: {delete: ['use_query']}}"}*

```diff
@@ -263,16 +263,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "aircraft_code",
                     "airline_code",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/atta_q.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/atta_q.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933333333333334%*

 * *Differences: {"'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -21,16 +21,15 @@
             "type": "add_fields"
         },
         {
             "field_to_field": {
                 "input": "input_label/input",
                 "label": "input_label/label"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "_argv": [
                 "input_label"
             ],
             "function": "json.dumps",
             "to_field": "input_label",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/babi/qa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/babi/qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/banking77.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/banking77.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/acm_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/acm_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/afr_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/afr_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/als_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/als_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/amh_ethi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/amh_ethi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/apc_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/apc_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/arb_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/arb_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ars_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ars_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ary_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ary_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/arz_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arz_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/asm_beng.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/asm_beng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/azj_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/azj_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/bam_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bam_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ben_beng.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_beng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ben_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/bod_tibt.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bod_tibt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/bul_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bul_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/cat_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/cat_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ceb_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ceb_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ces_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ces_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ckb_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ckb_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/dan_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/dan_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/deu_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/deu_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ell_grek.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ell_grek.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/eng_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eng_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/est_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/est_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/eus_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eus_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/fin_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/fra_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fra_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/fuv_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fuv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/gaz_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/gaz_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/grn_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/grn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/guj_gujr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/guj_gujr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hat_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hat_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hau_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hau_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/heb_hebr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/heb_hebr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hin_deva.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hin_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hrv_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hrv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hun_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hun_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/hye_armn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hye_armn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ibo_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ibo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ilo_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ilo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ind_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ind_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/isl_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/isl_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ita_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ita_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/jav_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jav_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/jpn_jpan.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jpn_jpan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kac_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kac_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kan_knda.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kan_knda.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kat_geor.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kat_geor.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kaz_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kaz_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kea_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kea_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/khk_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khk_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/khm_khmr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khm_khmr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kin_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kir_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kir_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/kor_hang.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kor_hang.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lao_laoo.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lao_laoo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lin_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lit_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lit_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lug_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lug_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/luo_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/luo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/lvs_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lvs_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mal_mlym.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mal_mlym.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mar_deva.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mar_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mkd_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mkd_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mlt_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mlt_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mri_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mri_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/mya_mymr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mya_mymr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nld_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nld_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nob_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nob_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/npi_deva.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/npi_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nso_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nso_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/nya_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nya_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ory_orya.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ory_orya.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pan_guru.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pan_guru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pbt_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pbt_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pes_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pes_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/plt_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/plt_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/pol_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pol_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/por_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/por_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ron_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ron_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/rus_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/rus_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/shn_mymr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/shn_mymr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sin_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sin_sinh.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_sinh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/slk_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slk_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/slv_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sna_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sna_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/snd_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/snd_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/som_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/som_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sot_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sot_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/spa_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/spa_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/srp_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/srp_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ssw_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ssw_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/sun_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sun_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/swe_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swe_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/swh_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swh_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tam_taml.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tam_taml.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tel_telu.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tel_telu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tgk_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgk_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tgl_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgl_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tha_thai.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tha_thai.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tir_ethi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tir_ethi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tsn_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tsn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tso_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tso_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/tur_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tur_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/ukr_cyrl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ukr_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/urd_arab.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/urd_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/uzn_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/uzn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/vie_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/vie_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/war_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/war_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/wol_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/wol_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/xho_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/xho_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/yor_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/yor_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zho_hans.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hans.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zho_hant.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hant.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zsm_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zsm_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/belebele/zul_latn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zul_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/bold.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/qqp.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8143518518518519%*

 * *Differences: {"'loader'": "{'path': 'glue', 'name': 'qqp'}",*

 * * "'preprocess_steps'": "{1: {'type': 'map_instance_values', 'mappers': OrderedDict([('label', "*

 * *                       "OrderedDict([('0', 'not duplicated'), ('1', 'duplicated')]))]), delete: "*

 * *                       "['mapper']}, 2: {'fields': {replace: OrderedDict([('choices', ['not "*

 * *                       "duplicated', 'duplicated'])])}}, insert: [(0, 'splitters.large_no_test')], "*

 * *                       'delete: [7, 6, 5, 4, 3, 2]}',*

 * * "'task'": "{'inputs' […]*

```diff
@@ -1,94 +1,53 @@
 {
     "loader": {
-        "path": "AlexaAI/bold",
+        "name": "qqp",
+        "path": "glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.large_no_test",
         {
-            "mapper": {
-                "train": "test"
+            "mappers": {
+                "label": {
+                    "0": "not duplicated",
+                    "1": "duplicated"
+                }
             },
-            "type": "rename_splits"
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "input_label": {}
-            },
-            "type": "add_fields"
-        },
-        {
-            "field_to_field": [
-                [
-                    "prompts/0",
-                    "first_prompt"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
-        },
-        {
-            "field_to_field": [
-                [
-                    "wikipedia/0",
-                    "first_wiki"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
-        },
-        {
-            "condition": "in",
-            "type": "filter_by_condition",
-            "values": {
-                "domain": [
-                    "race",
-                    "gender"
+                "choices": [
+                    "not duplicated",
+                    "duplicated"
                 ]
-            }
-        },
-        {
-            "page_size": 10000,
-            "type": "shuffle"
-        },
-        {
-            "field_to_field": {
-                "category": "input_label/category",
-                "first_prompt": "input_label/input",
-                "first_wiki": "input_label/wiki"
             },
-            "type": "copy_fields",
-            "use_query": true
-        },
-        {
-            "_argv": [
-                "input_label"
-            ],
-            "function": "json.dumps",
-            "to_field": "input_label",
-            "type": "apply"
+            "type": "add_fields"
         }
     ],
     "task": {
         "inputs": [
-            "first_prompt"
+            "choices",
+            "question1",
+            "question2"
         ],
         "metrics": [
-            "metrics.regard"
+            "metrics.accuracy"
         ],
         "outputs": [
-            "input_label"
+            "label"
         ],
         "type": "form_task"
     },
     "templates": {
         "items": [
             {
-                "input_format": "{first_prompt}\n",
-                "output_format": "{input_label}",
+                "input_format": "Given this question: {question1}, classify if this question: {question2} is {choices}.",
+                "output_format": "{label}",
                 "type": "input_output_template"
             }
         ],
         "type": "templates_list"
     },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/boolq/classification.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/boolq/classification.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/boolq/multiple_choice.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/boolq/multiple_choice.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/claim_stance_topic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/claim_stance_topic.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'preprocess_steps'": '{delete: [0]}'}*

```diff
@@ -2,21 +2,14 @@
     "loader": {
         "name": "claim_stance_topic",
         "path": "ibm/claim_stance",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": [
-                "label"
-            ],
-            "to_field": "label",
-            "type": "list_field_values"
-        },
-        {
             "fields": {
                 "classes": [
                     "advertising",
                     "all nations a right to nuclear weapons",
                     "a mandatory retirement age",
                     "american jobs act",
                     "asean",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/imbalanced.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/imbalanced.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/plus.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/plus.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/clinc_oos/small.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/small.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cnn_dailymail.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cnn_dailymail.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/coedit_gec.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xl.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6660714285714285%*

 * *Differences: {"'loader'": "{'path': 'winogrande', 'name': 'winogrande_xl', delete: ['streaming']}",*

 * * "'preprocess_steps'": "{1: {'type': 'list_field_values', 'to_field': 'choices', 'fields': "*

 * *                       "['option1', 'option2'], delete: ['expression']}, 4: {'field_to_field': "*

 * *                       "{replace: OrderedDict([('sentence', 'question')])}}, insert: [(2, "*

 * *                       "OrderedDict([('type', 'cast_fields'), ('fields', OrderedDict([('answer', "*

 * *                       "'int')]))])), (3, Or […]*

```diff
@@ -1,40 +1,38 @@
 {
     "loader": {
-        "path": "grammarly/coedit",
-        "streaming": true,
+        "name": "winogrande_xl",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "task": "gec"
-            }
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
+        {
+            "fields": {
+                "answer": "int"
+            },
+            "type": "cast_fields"
         },
-        "splitters.small_no_test",
         {
-            "expression": "': '.join(src.split(': ')[1:])",
-            "to_field": "src",
-            "type": "execute_expression"
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "src": "original_text"
+                "sentence": "question"
             },
             "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "tgt"
-            ],
-            "to_field": "corrected_texts",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.grammatical_error_correction",
-    "templates": [
-        "templates.grammatical_error_correction.simple"
-    ],
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/openbook_qa.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6672222222222223%*

 * *Differences: {"'loader'": "{'path': 'openbookqa', delete: ['name', 'streaming', 'filtering_lambda']}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_fields', 'field_to_field': "*

 * *                       "OrderedDict([('choices/text', 'choices_text'), ('choices/label', "*

 * *                       "'labels')]), delete: ['mix']}, 1: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('choices_text', 'choices'), ('question_stem', "*

 * *                       "'question')])}}, 2: {'type': 'index_of', 'to_field': 'answ […]*

```diff
@@ -1,36 +1,31 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"arb\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "path": "openbookqa",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "field_to_field": {
+                "choices/label": "labels",
+                "choices/text": "choices_text"
             },
-            "type": "split_random_mix"
+            "type": "rename_fields"
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "choices_text": "choices",
+                "question_stem": "question"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "index_of": "answerKey",
+            "search_in": "labels",
+            "to_field": "answer",
+            "type": "index_of"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/extractive.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6616666666666666%*

 * *Differences: {"'loader'": "{'path': 'multidoc2dial', delete: ['name', 'streaming', 'filtering_lambda']}",*

 * * "'preprocess_steps'": "{0: {'field_to_field': {replace: OrderedDict([('answers/text/0', "*

 * *                       "'relevant_context')])}}, 1: {'fields': ['relevant_context']}, insert: [(2, "*

 * *                       "OrderedDict([('type', 'execute_expression'), ('expression', "*

 * *                       '"question.split(\'[SEP]\')[0]"), (\'to_field\', \'question\')])), (3, '*

 * *                       "OrderedDict([('type', […]*

```diff
@@ -1,36 +1,35 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"eng\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "path": "multidoc2dial",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
-            },
-            "type": "split_random_mix"
-        },
-        {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "answers/text/0": "relevant_context"
             },
             "type": "rename_fields"
         },
         {
             "fields": [
-                "answers"
+                "relevant_context"
             ],
             "to_field": "answers",
             "type": "list_field_values"
+        },
+        {
+            "expression": "question.split('[SEP]')[0]",
+            "to_field": "question",
+            "type": "execute_expression"
+        },
+        {
+            "fields": {
+                "context_type": "document"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/jp.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6583333333333333%*

 * *Differences: {"'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'jp', delete: ['streaming', "*

 * *             "'filtering_lambda']}",*

 * * "'preprocess_steps'": "{1: {'type': 'cast_fields', 'fields': OrderedDict([('answer', 'int')]), "*

 * *                       "delete: ['mix']}, 3: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('sentence', 'question')])}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('t […]*

```diff
@@ -1,36 +1,37 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"por\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "name": "jp",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
+        {
+            "fields": {
+                "answer": "int"
             },
-            "type": "split_random_mix"
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "sentence": "question"
             },
             "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/en.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6583333333333333%*

 * *Differences: {"'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'en', delete: ['streaming', "*

 * *             "'filtering_lambda']}",*

 * * "'preprocess_steps'": "{1: {'type': 'cast_fields', 'fields': OrderedDict([('answer', 'int')]), "*

 * *                       "delete: ['mix']}, 3: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('sentence', 'question')])}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('t […]*

```diff
@@ -1,36 +1,37 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"tel\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "name": "en",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
+        {
+            "fields": {
+                "answer": "int"
             },
-            "type": "split_random_mix"
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "sentence": "question"
             },
             "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/pt.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6583333333333333%*

 * *Differences: {"'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'pt', delete: ['streaming', "*

 * *             "'filtering_lambda']}",*

 * * "'preprocess_steps'": "{1: {'type': 'cast_fields', 'fields': OrderedDict([('answer', 'int')]), "*

 * *                       "delete: ['mix']}, 3: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('sentence', 'question')])}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('t […]*

```diff
@@ -1,36 +1,37 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"tur\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "name": "pt",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
+        {
+            "fields": {
+                "answer": "int"
             },
-            "type": "split_random_mix"
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "sentence": "question"
             },
             "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/ru.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6583333333333333%*

 * *Differences: {"'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'ru', delete: ['streaming', "*

 * *             "'filtering_lambda']}",*

 * * "'preprocess_steps'": "{1: {'type': 'cast_fields', 'fields': OrderedDict([('answer', 'int')]), "*

 * *                       "delete: ['mix']}, 3: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('sentence', 'question')])}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('t […]*

```diff
@@ -1,36 +1,37 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"yor\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "name": "ru",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
+        {
+            "fields": {
+                "answer": "int"
             },
-            "type": "split_random_mix"
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "sentence": "question"
             },
             "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/zh.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6583333333333333%*

 * *Differences: {"'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'zh', delete: ['streaming', "*

 * *             "'filtering_lambda']}",*

 * * "'preprocess_steps'": "{1: {'type': 'cast_fields', 'fields': OrderedDict([('answer', 'int')]), "*

 * *                       "delete: ['mix']}, 3: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('sentence', 'question')])}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['option1', "*

 * *                       "'option2']), ('t […]*

```diff
@@ -1,36 +1,37 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"zho\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "name": "zh",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
+        },
+        {
+            "fields": {
+                "answer": "int"
             },
-            "type": "split_random_mix"
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "sentence": "question"
             },
             "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8800000000000001%*

 * *Differences: {"'loader'": "{'name': 'aya_human_annotated', 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="arb"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"fra\"",
-        "name": "dolly_human_edited",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"arb\"",
+        "name": "aya_human_annotated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8800000000000001%*

 * *Differences: {"'loader'": "{'name': 'aya_human_annotated', 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="zho"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"spa\"",
-        "name": "dolly_human_edited",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"zho\"",
+        "name": "aya_human_annotated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8800000000000001%*

 * *Differences: {"'loader'": "{'name': 'aya_human_annotated', 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="tur"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"deu\"",
-        "name": "dolly_machine_translated",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"tur\"",
+        "name": "aya_human_annotated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8800000000000001%*

 * *Differences: {"'loader'": "{'name': 'aya_human_annotated', 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="tel"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"eng\"",
-        "name": "dolly_machine_translated",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"tel\"",
+        "name": "aya_human_annotated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.89%*

 * *Differences: {"'loader'": '{\'filtering_lambda\': \'lambda instance: instance["language"]=="deu"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"jpn\"",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"deu\"",
         "name": "dolly_machine_translated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.89%*

 * *Differences: {"'loader'": '{\'filtering_lambda\': \'lambda instance: instance["language"]=="eng"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"por\"",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"eng\"",
         "name": "dolly_machine_translated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8800000000000001%*

 * *Differences: {"'loader'": "{'name': 'aya_human_annotated', 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="eng"\'}',*

 * * "'task'": "'tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"spa\"",
-        "name": "dolly_machine_translated",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"eng\"",
+        "name": "aya_human_annotated",
         "path": "CohereForAI/aya_evaluation_suite",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
@@ -26,11 +26,11 @@
             "fields": [
                 "answers"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
     "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/cola.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cola.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/copa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/copa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/coqa/completion.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/coqa/completion.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'preprocess_steps'": "{2: {delete: ['use_query']}}"}*

```diff
@@ -14,16 +14,15 @@
         },
         {
             "fields": [
                 "questions",
                 "answers/input_text"
             ],
             "to_field": "dialog",
-            "type": "zip_field_values",
-            "use_query": true
+            "type": "zip_field_values"
         },
         {
             "field": "dialog",
             "process_every_value": true,
             "type": "dictify",
             "with_keys": [
                 "user",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/coqa/qa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/coqa/qa.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935185185185185%*

 * *Differences: {"'preprocess_steps'": "{2: {delete: ['use_query']}, 6: {delete: ['use_query']}}"}*

```diff
@@ -13,16 +13,15 @@
         },
         {
             "fields": [
                 "questions",
                 "answers/input_text"
             ],
             "to_field": "dialog",
-            "type": "zip_field_values",
-            "use_query": true
+            "type": "zip_field_values"
         },
         {
             "field": "dialog",
             "process_every_value": true,
             "type": "dictify",
             "with_keys": [
                 "user",
@@ -40,16 +39,15 @@
             "type": "get"
         },
         {
             "field_to_field": {
                 "last_turn/system": "answer",
                 "last_turn/user": "question"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field": "answer",
             "inside": "list",
             "to_field": "answers",
             "type": "wrap"
         },
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/dart.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/dart.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933333333333334%*

 * *Differences: {"'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -20,16 +20,15 @@
             },
             "type": "rename_fields"
         },
         {
             "field_to_field": {
                 "annotations/text/0": "output"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "type_of_input": "Triples",
                 "type_of_output": "Text"
             },
             "type": "add_fields"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/dbpedia_14.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/dbpedia_14.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ethos_binary.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ethos_binary.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/16k.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/4k.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922619047619048%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}, 2: {'values': {'inputs_len': 4096}}, 6: "*

 * *                       "{'mix': {'train': '4k[80%]', 'validation': '4k[10%]', 'test': '4k[10%]'}}}"}*

```diff
@@ -6,29 +6,28 @@
     "preprocess_steps": [
         {
             "field_to_field": {
                 "conversations/0/tok_len": "inputs_len",
                 "conversations/0/value": "inputs",
                 "conversations/1/value": "answer"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": [
                 "answer"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         },
         {
             "condition": "lt",
             "type": "filter_by_condition",
             "values": {
-                "inputs_len": 16384
+                "inputs_len": 4096
             }
         },
         {
             "expression": "re.search(r\"Document:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
             "imports_list": [
                 "re"
             ],
@@ -47,17 +46,17 @@
             "fields": {
                 "context_type": "document"
             },
             "type": "add_fields"
         },
         {
             "mix": {
-                "test": "16k[10%]",
-                "train": "16k[80%]",
-                "validation": "16k[10%]"
+                "test": "4k[10%]",
+                "train": "4k[80%]",
+                "validation": "4k[10%]"
             },
             "type": "split_random_mix"
         }
     ],
     "task": "tasks.qa.with_context.extractive",
     "templates": "templates.qa.with_context.all",
     "type": "task_card"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/2k.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/2k.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952380952380953%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}}"}*

```diff
@@ -6,16 +6,15 @@
     "preprocess_steps": [
         {
             "field_to_field": {
                 "conversations/0/tok_len": "inputs_len",
                 "conversations/0/value": "inputs",
                 "conversations/1/value": "answer"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": [
                 "answer"
             ],
             "to_field": "answers",
             "type": "list_field_values"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/4k.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/8k.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922619047619048%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}, 2: {'values': {'inputs_len': 8800}}, 6: "*

 * *                       "{'mix': {'train': '8k[80%]', 'validation': '8k[10%]', 'test': '8k[10%]'}}}"}*

```diff
@@ -6,29 +6,28 @@
     "preprocess_steps": [
         {
             "field_to_field": {
                 "conversations/0/tok_len": "inputs_len",
                 "conversations/0/value": "inputs",
                 "conversations/1/value": "answer"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": [
                 "answer"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         },
         {
             "condition": "lt",
             "type": "filter_by_condition",
             "values": {
-                "inputs_len": 4096
+                "inputs_len": 8800
             }
         },
         {
             "expression": "re.search(r\"Document:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
             "imports_list": [
                 "re"
             ],
@@ -47,17 +46,17 @@
             "fields": {
                 "context_type": "document"
             },
             "type": "add_fields"
         },
         {
             "mix": {
-                "test": "4k[10%]",
-                "train": "4k[80%]",
-                "validation": "4k[10%]"
+                "test": "8k[10%]",
+                "train": "8k[80%]",
+                "validation": "8k[10%]"
             },
             "type": "split_random_mix"
         }
     ],
     "task": "tasks.qa.with_context.extractive",
     "templates": "templates.qa.with_context.all",
     "type": "task_card"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ffqa_filtered/8k.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/16k.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922619047619048%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}, 2: {'values': {'inputs_len': 16384}}, 6: "*

 * *                       "{'mix': {'train': '16k[80%]', 'validation': '16k[10%]', 'test': "*

 * *                       "'16k[10%]'}}}"}*

```diff
@@ -6,29 +6,28 @@
     "preprocess_steps": [
         {
             "field_to_field": {
                 "conversations/0/tok_len": "inputs_len",
                 "conversations/0/value": "inputs",
                 "conversations/1/value": "answer"
             },
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": [
                 "answer"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         },
         {
             "condition": "lt",
             "type": "filter_by_condition",
             "values": {
-                "inputs_len": 8800
+                "inputs_len": 16384
             }
         },
         {
             "expression": "re.search(r\"Document:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
             "imports_list": [
                 "re"
             ],
@@ -47,17 +46,17 @@
             "fields": {
                 "context_type": "document"
             },
             "type": "add_fields"
         },
         {
             "mix": {
-                "test": "8k[10%]",
-                "train": "8k[80%]",
-                "validation": "8k[10%]"
+                "test": "16k[10%]",
+                "train": "16k[80%]",
+                "validation": "16k[10%]"
             },
             "type": "split_random_mix"
         }
     ],
     "task": "tasks.qa.with_context.extractive",
     "templates": "templates.qa.with_context.all",
     "type": "task_card"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/financial_tweets.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/financial_tweets.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/head_qa/en.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/coedit_gec.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6502380952380953%*

 * *Differences: {"'loader'": '{\'path\': \'grammarly/coedit\', \'streaming\': True, \'filtering_lambda\': "lambda '*

 * *             'x: x[\'task\'] == \'gec\'", delete: [\'name\']}',*

 * * "'preprocess_steps'": "{4: {'field_to_field': {replace: OrderedDict([('src', "*

 * *                       "'original_text')])}}, 5: {'fields': ['tgt'], 'to_field': "*

 * *                       "'corrected_texts'}, insert: [(0, 'splitters.small_no_test'), (1, "*

 * *                       "OrderedDict([('type', 'split'), ('field', 'src'), ('by', ': ')])), (2, […]*

```diff
@@ -1,41 +1,42 @@
 {
     "loader": {
-        "name": "en",
-        "path": "head_qa",
+        "filtering_lambda": "lambda x: x['task'] == 'gec'",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "split"
+        },
+        {
+            "field": "src",
+            "start": 1,
+            "type": "slice"
+        },
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "join"
+        },
         {
             "field_to_field": {
-                "category": "label",
-                "qtext": "text"
+                "src": "original_text"
             },
             "type": "rename_fields"
         },
         {
             "fields": [
-                "label"
+                "tgt"
             ],
-            "to_field": "label",
+            "to_field": "corrected_texts",
             "type": "list_field_values"
-        },
-        {
-            "fields": {
-                "classes": [
-                    "biology",
-                    "chemistry",
-                    "medicine",
-                    "nursery",
-                    "pharmacology",
-                    "psychology"
-                ],
-                "text_type": "question",
-                "type_of_class": "topic"
-            },
-            "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.grammatical_error_correction",
+    "templates": "templates.grammatical_error_correction.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/head_qa/es.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xs.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6861111111111111%*

 * *Differences: {"'loader'": "{'path': 'winogrande', 'name': 'winogrande_xs'}",*

 * * "'preprocess_steps'": "{1: {'fields': ['option1', 'option2'], 'to_field': 'choices'}, 2: {'type': "*

 * *                       "'cast_fields', 'fields': {replace: OrderedDict([('answer', 'int')])}}, "*

 * *                       "insert: [(0, 'splitters.small_no_test'), (3, OrderedDict([('type', "*

 * *                       "'add_constant'), ('field', 'answer'), ('add', -1)])), (4, "*

 * *                       "OrderedDict([('type', 'rename_fields'), ('field_t […]*

```diff
@@ -1,41 +1,38 @@
 {
     "loader": {
-        "name": "es",
-        "path": "head_qa",
+        "name": "winogrande_xs",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "field_to_field": {
-                "category": "label",
-                "qtext": "text"
-            },
-            "type": "rename_fields"
-        },
+        "splitters.small_no_test",
         {
             "fields": [
-                "label"
+                "option1",
+                "option2"
             ],
-            "to_field": "label",
+            "to_field": "choices",
             "type": "list_field_values"
         },
         {
             "fields": {
-                "classes": [
-                    "biology",
-                    "chemistry",
-                    "medicine",
-                    "nursery",
-                    "pharmacology",
-                    "psychology"
-                ],
-                "text_type": "question",
-                "type_of_class": "topic"
+                "answer": "int"
+            },
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
+        },
+        {
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/hellaswag.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/hellaswag.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/human_eval.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/human_eval.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/law_stack_exchange.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/law_stack_exchange.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/ledgar.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/ledgar.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mbpp.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mbpp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/medical_abstracts.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/medical_abstracts.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/de.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/es.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/fr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/ru.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mlsum/tu.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/tu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/abstract_algebra.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/abstract_algebra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/anatomy.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/anatomy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/astronomy.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/astronomy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/business_ethics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/business_ethics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_biology.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_biology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_chemistry.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_chemistry.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_computer_science.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_computer_science.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_mathematics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_medicine.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_medicine.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/college_physics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/computer_security.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/computer_security.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/conceptual_physics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/conceptual_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/econometrics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/econometrics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/electrical_engineering.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/electrical_engineering.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/formal_logic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/formal_logic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/global_facts.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/global_facts.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_biology.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_biology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_european_history.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_european_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_geography.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_geography.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_physics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_psychology.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_psychology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_statistics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_statistics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_us_history.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_us_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/high_school_world_history.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_world_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/human_aging.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_aging.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/human_sexuality.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_sexuality.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/international_law.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/international_law.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/jurisprudence.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/jurisprudence.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/logical_fallacies.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/logical_fallacies.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/machine_learning.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/machine_learning.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/management.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/management.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/marketing.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/marketing.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/medical_genetics.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/medical_genetics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/miscellaneous.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/miscellaneous.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/moral_disputes.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_disputes.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/moral_scenarios.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_scenarios.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/nutrition.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/nutrition.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/philosophy.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/philosophy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/prehistory.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/prehistory.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_accounting.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_accounting.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_law.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_law.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_medicine.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_medicine.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/professional_psychology.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_psychology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/public_relations.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/public_relations.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/security_studies.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/security_studies.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/sociology.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/sociology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/virology.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/virology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mmlu/world_religions.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/world_religions.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mnli.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/mrpc.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/mrpc.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/multidoc2dial/abstractive.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wikitq.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7859375%*

 * *Differences: {"'loader'": "{'path': 'wikitablequestions'}",*

 * * "'preprocess_steps'": "{1: {'fields': {'context_type': 'table'}}, insert: [(0, "*

 * *                       "'splitters.small_no_test'), (2, OrderedDict([('type', "*

 * *                       "'truncate_table_cells'), ('max_length', 15), ('table', 'table'), "*

 * *                       "('text_output', 'answers')])), (3, OrderedDict([('type', "*

 * *                       "'truncate_table_rows'), ('field', 'table'), ('rows_to_keep', 50)])), (4, "*

 * *                       "Ordere […]*

```diff
@@ -1,36 +1,38 @@
 {
     "loader": {
-        "path": "multidoc2dial",
+        "path": "wikitablequestions",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "field_to_field": {
-                "answers/text/0": "relevant_context"
+            "fields": {
+                "context_type": "table"
             },
-            "type": "rename_fields",
-            "use_query": true
+            "type": "add_fields"
         },
         {
-            "fields": [
-                "utterance"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "max_length": 15,
+            "table": "table",
+            "text_output": "answers",
+            "type": "truncate_table_cells"
         },
         {
-            "expression": "question.split('[SEP]')[0]",
-            "to_field": "question",
-            "type": "execute_expression"
+            "field": "table",
+            "rows_to_keep": 50,
+            "type": "truncate_table_rows"
         },
         {
-            "fields": {
-                "context_type": "document"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "table",
+                    "context"
+                ]
+            ],
+            "type": "serialize_table_as_indexed_row_major"
         }
     ],
-    "task": "tasks.qa.with_context.abstractive",
+    "task": "tasks.qa.with_context.extractive",
     "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/multidoc2dial/extractive.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/abstractive.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8875%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}, 1: {'fields': ['utterance']}}",*

 * * "'task'": "'tasks.qa.with_context.abstractive'"}*

```diff
@@ -4,20 +4,19 @@
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
                 "answers/text/0": "relevant_context"
             },
-            "type": "rename_fields",
-            "use_query": true
+            "type": "rename_fields"
         },
         {
             "fields": [
-                "relevant_context"
+                "utterance"
             ],
             "to_field": "answers",
             "type": "list_field_values"
         },
         {
             "expression": "question.split('[SEP]')[0]",
             "to_field": "question",
@@ -26,11 +25,11 @@
         {
             "fields": {
                 "context_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
+    "task": "tasks.qa.with_context.abstractive",
     "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/news_category_classification_headline.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/news_category_classification_headline.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/openbook_qa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wnli/truthfulness.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.667%*

 * *Differences: {"'loader'": "{'path': 'glue', 'name': 'wnli'}",*

 * * "'preprocess_steps'": "{1: {'field_to_field': {replace: OrderedDict([('sentence1', 'text_a'), "*

 * *                       "('sentence2', 'text_b')])}}, 3: {'type': 'add_fields', 'fields': "*

 * *                       "OrderedDict([('classes', ['yes', 'no']), ('type_of_relation', "*

 * *                       "'truthfulness'), ('text_a_type', 'premise'), ('text_b_type', "*

 * *                       "'hypothesis')]), delete: ['search_in', 'index_of', 'to_field']}, insert: "*

 * *  […]*

```diff
@@ -1,32 +1,41 @@
 {
     "loader": {
-        "path": "openbookqa",
+        "name": "wnli",
+        "path": "glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
             "field_to_field": {
-                "choices/label": "labels",
-                "choices/text": "choices_text"
+                "sentence1": "text_a",
+                "sentence2": "text_b"
             },
-            "type": "rename_fields",
-            "use_query": true
+            "type": "rename_fields"
         },
         {
-            "field_to_field": {
-                "choices_text": "choices",
-                "question_stem": "question"
+            "mappers": {
+                "label": {
+                    "0": "yes",
+                    "1": "no"
+                }
             },
-            "type": "rename_fields"
+            "type": "map_instance_values"
         },
         {
-            "index_of": "answerKey",
-            "search_in": "labels",
-            "to_field": "answer",
-            "type": "index_of"
+            "fields": {
+                "classes": [
+                    "yes",
+                    "no"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "truthfulness"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.truthfulness.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/piqa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/piqa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/pop_qa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/pop_qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/qnli.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/qnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/qqp.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/race_high.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6849999999999999%*

 * *Differences: {"'loader'": "{'path': 'race', 'name': 'high'}",*

 * * "'preprocess_steps'": "{2: {'type': 'rename_fields', 'field_to_field': OrderedDict([('options', "*

 * *                       "'choices'), ('article', 'context')]), delete: ['mappers']}, 3: {'fields': "*

 * *                       "{replace: OrderedDict([('context_type', 'article')])}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'add_fields'), ('fields', OrderedDict([('numbering', "*

 * *                       "['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I' […]*

```diff
@@ -1,53 +1,64 @@
 {
     "loader": {
-        "name": "qqp",
-        "path": "glue",
+        "name": "high",
+        "path": "race",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.large_no_test",
         {
-            "mappers": {
-                "label": {
-                    "0": "not duplicated",
-                    "1": "duplicated"
-                }
+            "fields": {
+                "numbering": [
+                    "A",
+                    "B",
+                    "C",
+                    "D",
+                    "E",
+                    "F",
+                    "G",
+                    "H",
+                    "I",
+                    "J",
+                    "K",
+                    "L",
+                    "M",
+                    "N",
+                    "O",
+                    "P",
+                    "Q",
+                    "R",
+                    "S",
+                    "T",
+                    "U",
+                    "V",
+                    "W",
+                    "X",
+                    "Y",
+                    "Z"
+                ]
             },
-            "type": "map_instance_values"
+            "type": "add_fields"
+        },
+        {
+            "index_of": "answer",
+            "search_in": "numbering",
+            "to_field": "answer",
+            "type": "index_of"
+        },
+        {
+            "field_to_field": {
+                "article": "context",
+                "options": "choices"
+            },
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "choices": [
-                    "not duplicated",
-                    "duplicated"
-                ]
+                "context_type": "article"
             },
             "type": "add_fields"
         }
     ],
-    "task": {
-        "inputs": [
-            "choices",
-            "question1",
-            "question2"
-        ],
-        "metrics": [
-            "metrics.accuracy"
-        ],
-        "outputs": [
-            "label"
-        ],
-        "type": "form_task"
-    },
-    "templates": {
-        "items": [
-            {
-                "input_format": "Given this question: {question1}, classify if this question: {question2} is {choices}.",
-                "output_format": "{label}",
-                "type": "input_output_template"
-            }
-        ],
-        "type": "templates_list"
-    },
+    "task": "tasks.qa.multiple_choice.with_context",
+    "templates": "templates.qa.multiple_choice.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/race_all.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/race_all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/race_high.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/race_middle.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'middle'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "high",
+        "name": "middle",
         "path": "race",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "fields": {
                 "numbering": [
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/race_middle.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ar.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6944444444444444%*

 * *Differences: {"'loader'": "{'path': 'xnli', 'name': 'ar'}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_splits', 'mapper': "*

 * *                       "OrderedDict([('validation_matched', 'validation')]), delete: ['fields']}, "*

 * *                       "2: {'field_to_field': {replace: OrderedDict([('premise', 'text_a'), "*

 * *                       "('hypothesis', 'text_b')])}}, 4: {'fields': {replace: "*

 * *                       "OrderedDict([('type_of_relation', 'entailment'), ('text_a_type', "*

 * *                       "'premise') […]*

```diff
@@ -1,64 +1,49 @@
 {
     "loader": {
-        "name": "middle",
-        "path": "race",
+        "name": "ar",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": {
-                "numbering": [
-                    "A",
-                    "B",
-                    "C",
-                    "D",
-                    "E",
-                    "F",
-                    "G",
-                    "H",
-                    "I",
-                    "J",
-                    "K",
-                    "L",
-                    "M",
-                    "N",
-                    "O",
-                    "P",
-                    "Q",
-                    "R",
-                    "S",
-                    "T",
-                    "U",
-                    "V",
-                    "W",
-                    "X",
-                    "Y",
-                    "Z"
-                ]
+            "mapper": {
+                "validation_matched": "validation"
             },
-            "type": "add_fields"
-        },
-        {
-            "index_of": "answer",
-            "search_in": "numbering",
-            "to_field": "answer",
-            "type": "index_of"
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
             "field_to_field": {
-                "article": "context",
-                "options": "choices"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
             "fields": {
-                "context_type": "article"
+                "classes": [
+                    "entailment",
+                    "neutral",
+                    "contradiction"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/ModApte.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModApte.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/ModHayes.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModHayes.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/reuters21578/ModLewis.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModLewis.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/rte.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/rte.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/sciq.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/sciq.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/squad.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/squad.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888888888888889%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}}"}*

```diff
@@ -8,16 +8,15 @@
         {
             "field_to_field": [
                 [
                     "answers/text",
                     "answers"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "context_type": "passage"
             },
             "type": "add_fields"
         }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/sst2.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/sst2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/stsb.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/stsb.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/tab_fact.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/tab_fact.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/tablerow_classify.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/tablerow_classify.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/toxigen.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/toxigen.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/trec.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/trec.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/unfair_tos.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/unfair_tos.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/ceb/gja.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ceb/gja.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960000000000001%*

 * *Differences: {"'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/da/ddt.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'sv_talbanken'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "da_ddt",
+        "name": "sv_talbanken",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/de/pud.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/pud.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'en_pud'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "de_pud",
+        "name": "en_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/en/ewt.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/pud.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'pt_pud'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "en_ewt",
+        "name": "pt_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/en/pud.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/pud.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'sv_pud'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "en_pud",
+        "name": "sv_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/hr/set.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'tl_ugnayan'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "hr_set",
+        "name": "tl_ugnayan",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/pt/bosque.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sk/snk.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'sk_snk'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "pt_bosque",
+        "name": "sk_snk",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/pt/pud.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ru/pud.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'ru_pud'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "pt_pud",
+        "name": "ru_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/ru/pud.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsd.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'zh_gsd'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "ru_pud",
+        "name": "zh_gsd",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sk/snk.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'zh_gsdsimp'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "sk_snk",
+        "name": "zh_gsdsimp",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sr/set.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/pud.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'zh_pud'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "sr_set",
+        "name": "zh_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sv/pud.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/de/pud.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'de_pud'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "sv_pud",
+        "name": "de_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/trg.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'tl_trg'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "sv_talbanken",
+        "name": "tl_trg",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/tl/trg.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/ewt.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'en_ewt'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "tl_trg",
+        "name": "en_ewt",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/da/ddt.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835%*

 * *Differences: {"'loader'": "{'name': 'da_ddt'}", "'preprocess_steps'": "{3: {delete: ['use_query']}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "tl_ugnayan",
+        "name": "da_ddt",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
@@ -51,16 +51,15 @@
             "field_to_field": {
                 "spans/*/end": "spans_ends",
                 "spans/*/label": "labels",
                 "spans/*/start": "spans_starts"
             },
             "get_default": [],
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "class_type": "entity type",
                 "classes": [
                     "Person",
                     "Organization",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/zh/gsd.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/yahoo_answers_topics.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.663609693877551%*

 * *Differences: {"'loader'": "{'path': 'yahoo_answers_topics', delete: ['name', 'requirements_list']}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('topic', 'label')])}}, 3: "*

 * *                       "{'type': 'map_instance_values', 'mappers': OrderedDict([('label', "*

 * *                       "OrderedDict([('0', 'Society & Culture'), ('1', 'Science & Mathematics'), "*

 * *                       "('2', 'Health'), ('3', 'Education & Reference'), ('4', 'Computers & "*

 * *                       "Internet'), ('5' […]*

```diff
@@ -1,77 +1,80 @@
 {
     "loader": {
-        "name": "zh_gsd",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
-        ],
+        "path": "yahoo_answers_topics",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
+            "page_size": 9223372036854775807,
+            "type": "shuffle"
+        },
+        {
+            "mix": {
+                "test": "test",
+                "train": "train[87.5%]",
+                "validation": "train[12.5%]"
+            },
+            "type": "split_random_mix"
+        },
+        {
             "field_to_field": {
-                "ner_tags": "labels"
+                "topic": "label"
             },
             "type": "rename_fields"
         },
         {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
-            ],
-            "process_every_value": true,
-            "type": "get_item_by_index"
+            "mappers": {
+                "label": {
+                    "0": "Society & Culture",
+                    "1": "Science & Mathematics",
+                    "2": "Health",
+                    "3": "Education & Reference",
+                    "4": "Computers & Internet",
+                    "5": "Sports",
+                    "6": "Business & Finance",
+                    "7": "Entertainment & Music",
+                    "8": "Family & Relationships",
+                    "9": "Politics & Government"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
+            "fields": [
+                "question_title",
+                "question_content",
+                "best_answer"
             ],
-            "outside_label": "O",
-            "type": "iob_extractor"
+            "to_field": "text",
+            "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
-            },
-            "get_default": [],
-            "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "field": "text",
+            "separator": " ",
+            "to_field": "text",
+            "type": "join_str"
         },
         {
             "fields": {
-                "class_type": "entity type",
                 "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
+                    "Society & Culture",
+                    "Science & Mathematics",
+                    "Health",
+                    "Education & Reference",
+                    "Computers & Internet",
+                    "Sports",
+                    "Business & Finance",
+                    "Entertainment & Music",
+                    "Family & Relationships",
+                    "Politics & Government"
                 ],
-                "text_type": "text"
+                "text_type": "text",
+                "type_of_class": "topic"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.classification.multi_class",
+    "templates": "templates.classification.multi_class.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/vi.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.673154761904762%*

 * *Differences: {"'loader'": "{'path': 'xnli', 'name': 'vi', delete: ['requirements_list']}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('premise', 'text_a'), "*

 * *                       "('hypothesis', 'text_b')])}}, 3: {'type': 'map_instance_values', "*

 * *                       "'mappers': OrderedDict([('label', OrderedDict([('0', 'entailment'), ('1', "*

 * *                       "'neutral'), ('2', 'contradiction')]))]), delete: ['field', 'items_list', "*

 * *                       "'process_every_value']},  […]*

```diff
@@ -1,77 +1,49 @@
 {
     "loader": {
-        "name": "zh_gsdsimp",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
-        ],
+        "name": "vi",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "ner_tags": "labels"
+            "mapper": {
+                "validation_matched": "validation"
             },
-            "type": "rename_fields"
-        },
-        {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
-            ],
-            "process_every_value": true,
-            "type": "get_item_by_index"
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
-            ],
-            "outside_label": "O",
-            "type": "iob_extractor"
+            "field_to_field": {
+                "hypothesis": "text_b",
+                "premise": "text_a"
+            },
+            "type": "rename_fields"
         },
         {
-            "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
             },
-            "get_default": [],
-            "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "class_type": "entity type",
                 "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
+                    "entailment",
+                    "neutral",
+                    "contradiction"
                 ],
-                "text_type": "text"
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wiki_bio.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wiki_bio.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949999999999999%*

 * *Differences: {"'preprocess_steps'": "{1: {delete: ['use_query']}}"}*

```diff
@@ -14,16 +14,15 @@
         },
         {
             "fields": [
                 "input_text/table/column_header",
                 "input_text/table/content"
             ],
             "to_field": "kvpairs",
-            "type": "list_to_key_val_pairs",
-            "use_query": true
+            "type": "list_to_key_val_pairs"
         },
         {
             "field_to_field": [
                 [
                     "kvpairs",
                     "input"
                 ]
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wikitq.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6411111111111112%*

 * *Differences: {"'loader'": "{'path': 'CohereForAI/aya_evaluation_suite', 'name': 'dolly_human_edited', "*

 * *             "'streaming': True, 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="spa"\'}',*

 * * "'preprocess_steps'": "{0: {'type': 'split_random_mix', 'mix': OrderedDict([('train', "*

 * *                       "'test[90%]'), ('validation', 'test[5%]'), ('test', 'test[5%]')]), delete: "*

 * *                       "['fields']}, 1: {'type': 'rename_fields', 'field_to_field': {replace: "*

 * *                 […]*

```diff
@@ -1,38 +1,36 @@
 {
     "loader": {
-        "path": "wikitablequestions",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"spa\"",
+        "name": "dolly_human_edited",
+        "path": "CohereForAI/aya_evaluation_suite",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": {
-                "context_type": "table"
+            "mix": {
+                "test": "test[5%]",
+                "train": "test[90%]",
+                "validation": "test[5%]"
             },
-            "type": "add_fields"
+            "type": "split_random_mix"
         },
         {
-            "max_length": 15,
-            "table": "table",
-            "text_output": "answers",
-            "type": "truncate_table_cells"
-        },
-        {
-            "field": "table",
-            "rows_to_keep": 50,
-            "type": "truncate_table_rows"
+            "field_to_field": {
+                "inputs": "question",
+                "targets": "answers"
+            },
+            "type": "rename_fields"
         },
         {
-            "field_to_field": [
-                [
-                    "table",
-                    "context"
-                ]
+            "fields": [
+                "answers"
             ],
-            "type": "serialize_table_as_indexed_row_major"
+            "to_field": "answers",
+            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
-    "templates": "templates.qa.with_context.all",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
+    "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/debiased.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/debiased.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/l.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/l.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/m.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/summarize_from_human_feedback.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6986111111111111%*

 * *Differences: {"'loader'": "{'path': 'openai/summarize_from_feedback', 'name': 'comparisons'}",*

 * * "'preprocess_steps'": "{1: {'type': 'copy_fields', 'field_to_field': OrderedDict([('info/post', "*

 * *                       "'input'), ('summaries/*/text', 'choices')]), delete: ['fields']}, 2: "*

 * *                       "{'field_to_field': {replace: OrderedDict([('choice', 'output_choice')])}}, "*

 * *                       "insert: [(3, OrderedDict([('type', 'add_fields'), ('fields', "*

 * *                       "OrderedDict([('input_typ […]*

```diff
@@ -1,38 +1,34 @@
 {
     "loader": {
-        "name": "winogrande_m",
-        "path": "winogrande",
+        "name": "comparisons",
+        "path": "openai/summarize_from_feedback",
         "type": "load_hf"
     },
     "preprocess_steps": [
         "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "info/post": "input",
+                "summaries/*/text": "choices"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "copy_fields"
         },
         {
             "field_to_field": {
-                "sentence": "question"
+                "choice": "output_choice"
             },
             "type": "rename_fields"
+        },
+        {
+            "fields": {
+                "input_type": "post",
+                "instruction": "Summarize the following post",
+                "output_type": "summary"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
+    "task": "tasks.evaluation.preference",
+    "templates": "templates.evaluation.preference.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/s.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wnli.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6916666666666667%*

 * *Differences: {"'loader'": "{'path': 'glue', 'name': 'wnli'}",*

 * * "'preprocess_steps'": "{1: {'field_to_field': {replace: OrderedDict([('sentence1', 'text_a'), "*

 * *                       "('sentence2', 'text_b')])}}, insert: [(2, OrderedDict([('type', "*

 * *                       "'map_instance_values'), ('mappers', OrderedDict([('label', "*

 * *                       "OrderedDict([('0', 'entailment'), ('1', 'not entailment')]))]))])), (3, "*

 * *                       "OrderedDict([('type', 'add_fields'), ('fields', OrderedDict([('classe […]*

```diff
@@ -1,38 +1,41 @@
 {
     "loader": {
-        "name": "winogrande_s",
-        "path": "winogrande",
+        "name": "wnli",
+        "path": "glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
         "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "sentence1": "text_a",
+                "sentence2": "text_b"
             },
-            "type": "cast_fields"
+            "type": "rename_fields"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "not entailment"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
-            "field_to_field": {
-                "sentence": "question"
+            "fields": {
+                "classes": [
+                    "entailment",
+                    "not entailment"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
-            "type": "rename_fields"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/xl.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_de.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6625%*

 * *Differences: {"'loader'": "{'path': 'wmt16', 'name': 'de-en', 'streaming': True}",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['translation/en', 'text'], "*

 * *                       "['translation/de', 'translation']], delete: ['fields', 'to_field']}, 1: "*

 * *                       "{'type': 'add_fields', 'fields': {replace: "*

 * *                       "OrderedDict([('source_language', 'english'), ('target_language', "*

 * *                       "'deutch')])}}, delete: [4, 3, 0]}",*

 * * "'task'": "'tasks.tran […]*

```diff
@@ -1,38 +1,33 @@
 {
     "loader": {
-        "name": "winogrande_xl",
-        "path": "winogrande",
+        "name": "de-en",
+        "path": "wmt16",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "translation/en",
+                    "text"
+                ],
+                [
+                    "translation/de",
+                    "translation"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
             "fields": {
-                "answer": "int"
+                "source_language": "english",
+                "target_language": "deutch"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
+    "task": "tasks.translation.directed",
+    "templates": "templates.translation.directed.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/winogrande/xs.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/en.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6885416666666666%*

 * *Differences: {"'loader'": "{'path': 'xnli', 'name': 'en'}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('premise', 'text_a'), "*

 * *                       "('hypothesis', 'text_b')])}}, insert: [(0, OrderedDict([('type', "*

 * *                       "'rename_splits'), ('mapper', OrderedDict([('validation_matched', "*

 * *                       "'validation')]))])), (3, OrderedDict([('type', 'map_instance_values'), "*

 * *                       "('mappers', OrderedDict([('label', OrderedDict([('0', 'entailment') […]*

```diff
@@ -1,38 +1,49 @@
 {
     "loader": {
-        "name": "winogrande_xs",
-        "path": "winogrande",
+        "name": "en",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "mapper": {
+                "validation_matched": "validation"
+            },
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
-            "type": "cast_fields"
+            "type": "rename_fields"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
-            "field_to_field": {
-                "sentence": "question"
+            "fields": {
+                "classes": [
+                    "entailment",
+                    "neutral",
+                    "contradiction"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
-            "type": "rename_fields"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wmt/en_de.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_latin.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7041666666666666%*

 * *Differences: {"'loader'": "{'path': 'GEM/xlsum', 'name': 'serbian_latin', delete: ['streaming']}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_fields', 'field_to_field': {replace: "*

 * *                       "OrderedDict([('text', 'document'), ('target', 'summary')])}, delete: "*

 * *                       "['use_query']}, 1: {'fields': {replace: OrderedDict([('document_type', "*

 * *                       "'document')])}}}",*

 * * "'task'": "'tasks.summarization.abstractive'",*

 * * "'templates'": "'templates.summarization.abstractive.all'" […]*

```diff
@@ -1,34 +1,25 @@
 {
     "loader": {
-        "name": "de-en",
-        "path": "wmt16",
-        "streaming": true,
+        "name": "serbian_latin",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "field_to_field": [
-                [
-                    "translation/en",
-                    "text"
-                ],
-                [
-                    "translation/de",
-                    "translation"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
+            "field_to_field": {
+                "target": "summary",
+                "text": "document"
+            },
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "source_language": "english",
-                "target_language": "deutch"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.translation.directed",
-    "templates": "templates.translation.directed.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wmt/en_fr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_fr.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333332%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}}"}*

```diff
@@ -13,16 +13,15 @@
                     "text"
                 ],
                 [
                     "translation/fr",
                     "translation"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "source_language": "english",
                 "target_language": "french"
             },
             "type": "add_fields"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wmt/en_ro.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_ro.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333332%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}}"}*

```diff
@@ -13,16 +13,15 @@
                     "text"
                 ],
                 [
                     "translation/ro",
                     "translation"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "source_language": "english",
                 "target_language": "romanian"
             },
             "type": "add_fields"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wnli/truthfulness.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/fr.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8387499999999999%*

 * *Differences: {"'loader'": "{'path': 'xnli', 'name': 'fr'}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('premise', 'text_a'), "*

 * *                       "('hypothesis', 'text_b')])}}, 3: {'mappers': {'label': {'0': 'entailment', "*

 * *                       "'1': 'neutral', '2': 'contradiction'}}}, 4: {'fields': {'classes': "*

 * *                       "['entailment', 'neutral', 'contradiction'], 'type_of_relation': "*

 * *                       "'entailment'}}, insert: [(0, OrderedDict([('type', 'rename_spl […]*

```diff
@@ -1,41 +1,49 @@
 {
     "loader": {
-        "name": "wnli",
-        "path": "glue",
+        "name": "fr",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        {
+            "mapper": {
+                "validation_matched": "validation"
+            },
+            "type": "rename_splits"
+        },
         "splitters.small_no_test",
         {
             "field_to_field": {
-                "sentence1": "text_a",
-                "sentence2": "text_b"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
             "mappers": {
                 "label": {
-                    "0": "yes",
-                    "1": "no"
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
                 }
             },
             "type": "map_instance_values"
         },
         {
             "fields": {
                 "classes": [
-                    "yes",
-                    "no"
+                    "entailment",
+                    "neutral",
+                    "contradiction"
                 ],
                 "text_a_type": "premise",
                 "text_b_type": "hypothesis",
-                "type_of_relation": "truthfulness"
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
     "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.truthfulness.all",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wnli.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/bg.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9399479166666665%*

 * *Differences: {"'loader'": "{'path': 'xnli', 'name': 'bg'}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('premise', 'text_a'), "*

 * *                       "('hypothesis', 'text_b')])}}, 3: {'mappers': {'label': {'1': 'neutral', "*

 * *                       "'2': 'contradiction'}}}, 4: {'fields': {'classes': {insert: [(1, "*

 * *                       "'neutral'), (2, 'contradiction')], delete: [1]}}}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'rename_splits'), ('mapper', "*

 * *               […]*

```diff
@@ -1,36 +1,44 @@
 {
     "loader": {
-        "name": "wnli",
-        "path": "glue",
+        "name": "bg",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        {
+            "mapper": {
+                "validation_matched": "validation"
+            },
+            "type": "rename_splits"
+        },
         "splitters.small_no_test",
         {
             "field_to_field": {
-                "sentence1": "text_a",
-                "sentence2": "text_b"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
             "mappers": {
                 "label": {
                     "0": "entailment",
-                    "1": "not entailment"
+                    "1": "neutral",
+                    "2": "contradiction"
                 }
             },
             "type": "map_instance_values"
         },
         {
             "fields": {
                 "classes": [
                     "entailment",
-                    "not entailment"
+                    "neutral",
+                    "contradiction"
                 ],
                 "text_a_type": "premise",
                 "text_b_type": "hypothesis",
                 "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/wsc.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/wsc.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/amharic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/amharic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/arabic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/arabic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/azerbaijani.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/azerbaijani.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/bengali.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/bengali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/burmese.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/burmese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/chinese_simplified.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_simplified.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/chinese_traditional.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_traditional.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/english.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/english.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/french.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/french.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/gujarati.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/gujarati.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/hausa.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hausa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/hindi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hindi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/igbo.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/igbo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/indonesian.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/indonesian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/japanese.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/japanese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/kirundi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kirundi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/korean.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/korean.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/kyrgyz.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kyrgyz.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/marathi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/marathi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/nepali.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/nepali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/oromo.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/oromo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/pashto.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pashto.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/persian.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/persian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/pidgin.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pidgin.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/portuguese.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/portuguese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/punjabi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/punjabi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/russian.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/russian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/serbian_latin.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/ukrainian.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'ukrainian'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "serbian_latin",
+        "name": "ukrainian",
         "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
                 "target": "summary",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/sinhala.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/sinhala.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/somali.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/somali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/spanish.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/spanish.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/swahili.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/swahili.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/tamil.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tamil.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/telugu.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/telugu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/thai.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/thai.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/tigrinya.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tigrinya.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/turkish.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/turkish.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/ukrainian.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/uzbek.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'uzbek'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "ukrainian",
+        "name": "uzbek",
         "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
                 "target": "summary",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/urdu.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/urdu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/uzbek.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/vietnamese.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'vietnamese'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "uzbek",
+        "name": "vietnamese",
         "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
                 "target": "summary",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/vietnamese.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/welsh.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'welsh'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "vietnamese",
+        "name": "welsh",
         "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
                 "target": "summary",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/welsh.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/yoruba.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'yoruba'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "welsh",
+        "name": "yoruba",
         "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
                 "target": "summary",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xlsum/yoruba.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6761111111111111%*

 * *Differences: {"'loader'": "{'path': 'CohereForAI/aya_evaluation_suite', 'name': 'aya_human_annotated', "*

 * *             "'streaming': True, 'filtering_lambda': 'lambda instance: "*

 * *             'instance["language"]=="por"\'}',*

 * * "'preprocess_steps'": "{1: {'field_to_field': {replace: OrderedDict([('inputs', 'question'), "*

 * *                       "('targets', 'answers')])}}, 2: {'type': 'list_field_values', 'fields': "*

 * *                       "['answers'], 'to_field': 'answers'}, insert: [(0, OrderedDict([('type', "*

 * *          […]*

```diff
@@ -1,25 +1,36 @@
 {
     "loader": {
-        "name": "yoruba",
-        "path": "GEM/xlsum",
+        "filtering_lambda": "lambda instance: instance[\"language\"]==\"por\"",
+        "name": "aya_human_annotated",
+        "path": "CohereForAI/aya_evaluation_suite",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
+            "mix": {
+                "test": "test[5%]",
+                "train": "test[90%]",
+                "validation": "test[5%]"
+            },
+            "type": "split_random_mix"
+        },
+        {
             "field_to_field": {
-                "target": "summary",
-                "text": "document"
+                "inputs": "question",
+                "targets": "answers"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
+            "fields": [
+                "answers"
+            ],
+            "to_field": "answers",
+            "type": "list_field_values"
         }
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
+    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
+    "templates": "templates.qa.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/ar.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/hi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'hi'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "ar",
+        "name": "hi",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/bg.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/zh.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'zh'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "bg",
+        "name": "zh",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/de.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/el.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/el.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/en.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/sw.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'sw'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "en",
+        "name": "sw",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/es.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/fr.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ru.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'ru'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "fr",
+        "name": "ru",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/hi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/tr.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'tr'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "hi",
+        "name": "tr",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/ru.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ur.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'ur'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "ru",
+        "name": "ur",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/sw.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/th.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'th'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "sw",
+        "name": "th",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/th.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/es.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6970833333333333%*

 * *Differences: {"'loader'": "{'path': 'head_qa', 'name': 'es'}",*

 * * "'preprocess_steps'": "{0: {'field_to_field': {replace: OrderedDict([('qtext', 'text'), "*

 * *                       "('category', 'label')])}}, 1: {'fields': {'classes': ['biology', "*

 * *                       "'chemistry', 'medicine', 'nursery', 'pharmacology', 'psychology'], "*

 * *                       "'text_type': 'question', 'type_of_class': 'topic', delete: "*

 * *                       "['type_of_relation', 'text_a_type', 'text_b_type']}}, delete: [3, 1, 0]}",*

 * * "' […]*

```diff
@@ -1,49 +1,34 @@
 {
     "loader": {
-        "name": "th",
-        "path": "xnli",
+        "name": "es",
+        "path": "head_qa",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "validation_matched": "validation"
-            },
-            "type": "rename_splits"
-        },
-        "splitters.small_no_test",
-        {
             "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
+                "category": "label",
+                "qtext": "text"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
             "fields": {
                 "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
+                    "biology",
+                    "chemistry",
+                    "medicine",
+                    "nursery",
+                    "pharmacology",
+                    "psychology"
                 ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "text_type": "question",
+                "type_of_class": "topic"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.classification.multi_class",
+    "templates": "templates.classification.multi_class.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/vi.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/bold.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6675925925925925%*

 * *Differences: {"'loader'": "{'path': 'AlexaAI/bold', delete: ['name']}",*

 * * "'preprocess_steps'": "{0: {'mapper': {replace: OrderedDict([('train', 'test')])}}, 3: {'type': "*

 * *                       "'copy_fields', 'field_to_field': [['wikipedia/0', 'first_wiki']]}, 5: "*

 * *                       "{'type': 'shuffle', 'page_size': 10000, delete: ['mappers']}, 6: {'type': "*

 * *                       "'copy_fields', 'field_to_field': OrderedDict([('first_prompt', "*

 * *                       "'input_label/input'), ('category', 'input_lab […]*

```diff
@@ -1,49 +1,91 @@
 {
     "loader": {
-        "name": "vi",
-        "path": "xnli",
+        "path": "AlexaAI/bold",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "validation_matched": "validation"
+                "train": "test"
             },
             "type": "rename_splits"
         },
-        "splitters.small_no_test",
         {
-            "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
+            "fields": {
+                "input_label": {}
             },
-            "type": "rename_fields"
+            "type": "add_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
+            "field_to_field": [
+                [
+                    "prompts/0",
+                    "first_prompt"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+            "field_to_field": [
+                [
+                    "wikipedia/0",
+                    "first_wiki"
+                ]
+            ],
+            "type": "copy_fields"
+        },
+        {
+            "condition": "in",
+            "type": "filter_by_condition",
+            "values": {
+                "domain": [
+                    "race",
+                    "gender"
+                ]
+            }
+        },
+        {
+            "page_size": 10000,
+            "type": "shuffle"
+        },
+        {
+            "field_to_field": {
+                "category": "input_label/category",
+                "first_prompt": "input_label/input",
+                "first_wiki": "input_label/wiki"
             },
-            "type": "add_fields"
+            "type": "copy_fields"
+        },
+        {
+            "_argv": [
+                "input_label"
+            ],
+            "function": "json.dumps",
+            "to_field": "input_label",
+            "type": "apply"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": {
+        "inputs": [
+            "first_prompt"
+        ],
+        "metrics": [
+            "metrics.regard"
+        ],
+        "outputs": [
+            "input_label"
+        ],
+        "type": "form_task"
+    },
+    "templates": {
+        "items": [
+            {
+                "input_format": "{first_prompt}\n",
+                "output_format": "{input_label}",
+                "type": "input_output_template"
+            }
+        ],
+        "type": "templates_list"
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xnli/zh.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/coedit/paraphrase.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6585714285714286%*

 * *Differences: {"'loader'": '{\'path\': \'grammarly/coedit\', \'streaming\': True, \'filtering_lambda\': "lambda '*

 * *             'x: x[\'task\'] == \'paraphrase\'", delete: [\'name\']}',*

 * * "'preprocess_steps'": "{2: {'type': 'slice', 'field': 'src', 'start': 1, delete: "*

 * *                       "['field_to_field']}, 3: {'type': 'join', 'field': 'src', 'by': ': ', "*

 * *                       "delete: ['mappers']}, 4: {'fields': {replace: OrderedDict([('text_type', "*

 * *                       "'sentence')])}}, insert: [(1, OrderedDi […]*

```diff
@@ -1,49 +1,42 @@
 {
     "loader": {
-        "name": "zh",
-        "path": "xnli",
+        "filtering_lambda": "lambda x: x['task'] == 'paraphrase'",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "mapper": {
-                "validation_matched": "validation"
-            },
-            "type": "rename_splits"
+            "by": ": ",
+            "field": "src",
+            "type": "split"
         },
-        "splitters.small_no_test",
         {
-            "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
-            },
-            "type": "rename_fields"
+            "field": "src",
+            "start": 1,
+            "type": "slice"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "text_type": "sentence"
             },
             "type": "add_fields"
+        },
+        {
+            "field_to_field": {
+                "src": "input_text",
+                "tgt": "output_text"
+            },
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.rewriting.paraphrase",
+    "templates": "templates.rewriting.paraphrase.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/en.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_reward.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15238095238095237%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.reward.deberta_v3_large_v2'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['question', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, insert: [(2, "*

 * *                       "OrderedDict([('type', 'list_field_values'), ('fields', ['references']), "*

 * *                       "('to_field', 'references')]))], delete: [2, 0]} […]*

```diff
@@ -1,37 +1,32 @@
 {
-    "loader": {
-        "name": "en",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "score",
+    "metric": "metrics.reward.deberta_v3_large_v2",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "question",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
+            "type": "copy_fields"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "fields": [
+                "references"
+            ],
+            "to_field": "references",
+            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/jp.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/faithfulness.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [2, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,37 +1,25 @@
 {
-    "loader": {
-        "name": "jp",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "precision",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/pt.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/k_precision.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [2, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,37 +1,25 @@
 {
-    "loader": {
-        "name": "pt",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "precision",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/ru.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_correctness.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'recall'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['ground_truths', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [2, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,37 +1,25 @@
 {
-    "loader": {
-        "name": "ru",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "recall",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "ground_truths",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/cards/xwinogrande/zh.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/recall.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'recall'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['ground_truths', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [2, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,37 +1,25 @@
 {
-    "loader": {
-        "name": "zh",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "recall",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "ground_truths",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/normalized_sacrebleu.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/normalized_sacrebleu.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971875%*

 * *Differences: {"'preprocess_steps'": "{0: {delete: ['use_query']}, 1: {delete: ['use_query']}}"}*

```diff
@@ -9,16 +9,15 @@
                 [
                     "task_data/target_language",
                     "task_data/tokenize"
                 ]
             ],
             "get_default": "en",
             "not_exist_ok": true,
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "mappers": {
                 "task_data/tokenize": {
                     "Arabic": "intl",
                     "French": null,
                     "German": null,
@@ -38,13 +37,12 @@
                     "japanese": "ja-mecab",
                     "ko": "ko-mecab",
                     "pt": null,
                     "romanian": null
                 }
             },
             "strict": true,
-            "type": "map_instance_values",
-            "use_query": true
+            "type": "map_instance_values"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/answer_correctness.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_perplexity.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5555555555555556%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.perplexity_q.flan_t5_small'",*

 * * "'postpreprocess_steps'": "[OrderedDict([('type', 'copy_fields'), ('field_to_field', "*

 * *                           "[['score/instance/reference_scores', 'score/instance/score']])])]",*

 * * "'preprocess_steps'": "{0: {'field_to_field': {0: {insert: [(0, 'contexts')], delete: [0]}}, "*

 * *                       "delete: ['use_query']}, 1: {'field_to_field': {0: {insert: [(0, "*

 * *                       "'question')], delete: [0]}}, delete:  […]*

```diff
@@ -1,27 +1,36 @@
 {
-    "main_score": "recall",
-    "metric": "metrics.token_overlap",
+    "main_score": "score",
+    "metric": "metrics.perplexity_q.flan_t5_small",
+    "postpreprocess_steps": [
+        {
+            "field_to_field": [
+                [
+                    "score/instance/reference_scores",
+                    "score/instance/score"
+                ]
+            ],
+            "type": "copy_fields"
+        }
+    ],
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
-                    "ground_truths",
+                    "contexts",
                     "references"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field_to_field": [
                 [
-                    "answer",
+                    "question",
                     "prediction"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/answer_reward.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_correctness.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {"'metric'": "'metrics.mrr'",*

 * * "'preprocess_steps'": "{0: {'field_to_field': [['context_ids', 'prediction']], delete: "*

 * *                       "['use_query']}, 1: {'field_to_field': [['ground_truths_context_ids', "*

 * *                       "'references']], delete: ['use_query']}, delete: [2]}"}*

```diff
@@ -1,34 +1,25 @@
 {
     "main_score": "score",
-    "metric": "metrics.reward.deberta_v3_large_v2",
+    "metric": "metrics.mrr",
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
-                    "question",
-                    "references"
+                    "context_ids",
+                    "prediction"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field_to_field": [
                 [
-                    "answer",
-                    "prediction"
+                    "ground_truths_context_ids",
+                    "references"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
-        },
-        {
-            "fields": [
-                "references"
-            ],
-            "to_field": "references",
-            "type": "list_field_values"
+            "type": "copy_fields"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/bert_k_precision.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/mrr.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6875%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.mrr'",*

 * * "'preprocess_steps'": "{0: {'field_to_field': [['context_ids', 'prediction']], delete: "*

 * *                       "['use_query']}, 1: {'field_to_field': [['ground_truths_context_ids', "*

 * *                       "'references']], delete: ['use_query']}}"}*

```diff
@@ -1,27 +1,25 @@
 {
-    "main_score": "precision",
-    "metric": "metrics.bert_score.deberta_xlarge_mnli",
+    "main_score": "score",
+    "metric": "metrics.mrr",
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
-                    "contexts",
-                    "references"
+                    "context_ids",
+                    "prediction"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field_to_field": [
                 [
-                    "answer",
-                    "prediction"
+                    "ground_truths_context_ids",
+                    "references"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/bert_recall.json` & `unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1%*

 * *Differences: {"'steps'": "[OrderedDict([('type', 'regex_parser'), ('regex', "*

 * *            "'\\\\s*((?:[^,:\\\\\\\\]|\\\\\\\\.)+?)\\\\s*:\\\\s*((?:[^,:\\\\\\\\]|\\\\\\\\.)+?)\\\\s*(?=,|$)'), "*

 * *            "('field', 'prediction'), ('process_every_value', False)]), OrderedDict([('type', "*

 * *            "'regex_parser'), ('regex', "*

 * *            "'\\\\s*((?:[^,:\\\\\\\\]|\\\\\\\\.)+?)\\\\s*:\\\\s*((?:[^,:\\\\\\\\]|\\\\\\\\.)+?)\\\\s*(?=,|$)'), "*

 * *            "('field', 'references'), ('process_every_value', True)])]",*

 * * "'type' […]*

```diff
@@ -1,27 +1,17 @@
 {
-    "main_score": "recall",
-    "metric": "metrics.bert_score.deberta_xlarge_mnli",
-    "preprocess_steps": [
+    "steps": [
         {
-            "field_to_field": [
-                [
-                    "ground_truths",
-                    "references"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
+            "field": "prediction",
+            "process_every_value": false,
+            "regex": "\\s*((?:[^,:\\\\]|\\\\.)+?)\\s*:\\s*((?:[^,:\\\\]|\\\\.)+?)\\s*(?=,|$)",
+            "type": "regex_parser"
         },
         {
-            "field_to_field": [
-                [
-                    "answer",
-                    "prediction"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
+            "field": "references",
+            "process_every_value": true,
+            "regex": "\\s*((?:[^,:\\\\]|\\\\.)+?)\\s*:\\s*((?:[^,:\\\\]|\\\\.)+?)\\s*(?=,|$)",
+            "type": "regex_parser"
         }
     ],
-    "type": "metric_pipeline"
+    "type": "sequential_operator"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/context_correctness.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/spearman.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6614583333333334%*

 * *Differences: {"'main_score'": "'spearmanr'",*

 * * "'metric'": "{replace: OrderedDict([('type', 'spearmanr')])}",*

 * * "'preprocess_steps'": "{0: {'field_to_field': [['references/0', 'references']], delete: "*

 * *                       "['use_query']}, 1: {'type': 'cast_fields', 'fields': "*

 * *                       "OrderedDict([('prediction', 'float'), ('references', 'float')]), "*

 * *                       "'failure_defaults': OrderedDict([('prediction', 0.0)]), "*

 * *                       "'use_nested_query': True, delete: ['field_to_fiel […]*

```diff
@@ -1,27 +1,29 @@
 {
-    "main_score": "score",
-    "metric": "metrics.mrr",
+    "main_score": "spearmanr",
+    "metric": {
+        "type": "spearmanr"
+    },
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
-                    "context_ids",
-                    "prediction"
+                    "references/0",
+                    "references"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
-            "field_to_field": [
-                [
-                    "ground_truths_context_ids",
-                    "references"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
+            "failure_defaults": {
+                "prediction": 0.0
+            },
+            "fields": {
+                "prediction": "float",
+                "references": "float"
+            },
+            "type": "cast_fields",
+            "use_nested_query": true
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/context_relevance.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_k_precision.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7013888888888888%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.bert_score.deberta_large_mnli'",*

 * * "'preprocess_steps'": "{0: {delete: ['use_query']}, 1: {'field_to_field': {0: {insert: [(0, "*

 * *                       "'answer')], delete: [0]}}, delete: ['use_query']}}"}*

```diff
@@ -1,27 +1,25 @@
 {
-    "main_score": "perplexity",
-    "metric": "metrics.perplexity_q.flan_t5_small",
+    "main_score": "precision",
+    "metric": "metrics.bert_score.deberta_large_mnli",
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
                     "contexts",
                     "references"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field_to_field": [
                 [
-                    "question",
+                    "answer",
                     "prediction"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/rag/map.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_recall.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6875%*

 * *Differences: {"'main_score'": "'recall'",*

 * * "'metric'": "'metrics.bert_score.deberta_large_mnli'",*

 * * "'preprocess_steps'": "{0: {'field_to_field': [['ground_truths', 'references']], delete: "*

 * *                       "['use_query']}, 1: {'field_to_field': [['answer', 'prediction']], delete: "*

 * *                       "['use_query']}}"}*

```diff
@@ -1,27 +1,25 @@
 {
-    "main_score": "score",
-    "metric": "metrics.map",
+    "main_score": "recall",
+    "metric": "metrics.bert_score.deberta_large_mnli",
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
-                    "context_ids",
-                    "prediction"
+                    "ground_truths",
+                    "references"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field_to_field": [
                 [
-                    "ground_truths_context_ids",
-                    "references"
+                    "answer",
+                    "prediction"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/squad.json` & `unitxt-1.7.6/src/unitxt/catalog/metrics/squad.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'preprocess_steps'": "{2: {delete: ['use_query']}, 3: {delete: ['use_query']}}"}*

```diff
@@ -41,27 +41,25 @@
                     "prediction_template/id"
                 ],
                 [
                     "id",
                     "reference_template/id"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         },
         {
             "field_to_field": [
                 [
                     "reference_template",
                     "references"
                 ],
                 [
                     "prediction_template",
                     "prediction"
                 ]
             ],
-            "type": "copy_fields",
-            "use_query": true
+            "type": "copy_fields"
         }
     ],
     "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/metrics/token_overlap_with_context.json` & `unitxt-1.7.6/src/unitxt/catalog/cards/coedit_error_detection.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1303240740740741%*

 * *Differences: {"'loader'": "OrderedDict([('type', 'load_hf'), ('path', 'grammarly/coedit'), ('streaming', True), "*

 * *             '(\'filtering_lambda\', "lambda x: x[\'task\'] == \'gec\'")])',*

 * * "'preprocess_steps'": "{3: {'type': 'join', 'field': 'src', 'by': ': ', delete: "*

 * *                       "['field_to_field', 'use_query']}, 4: {'fields': ['tgt', 'src'], "*

 * *                       "'to_field': 'correct_and_incorrect'}, insert: [(0, "*

 * *                       "'splitters.small_no_test'), (1, OrderedDict([('type', 'split […]*

```diff
@@ -1,46 +1,59 @@
 {
-    "main_score": "score",
-    "metric": {
-        "type": "token_overlap"
+    "loader": {
+        "filtering_lambda": "lambda x: x['task'] == 'gec'",
+        "path": "grammarly/coedit",
+        "streaming": true,
+        "type": "load_hf"
     },
-    "postpreprocess_steps": [
-        {
-            "field_to_field": [
-                [
-                    "score/global/f1",
-                    "score/global/f1_overlap_with_context"
-                ],
-                [
-                    "score/global/recall",
-                    "score/global/recall_overlap_with_context"
-                ],
-                [
-                    "score/global/precision",
-                    "score/global/precision_overlap_with_context"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
-        }
-    ],
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "field_to_field": [
-                [
-                    "task_data/context",
-                    "references"
-                ]
-            ],
-            "type": "copy_fields",
-            "use_query": true
+            "by": ": ",
+            "field": "src",
+            "type": "split"
+        },
+        {
+            "field": "src",
+            "start": 1,
+            "type": "slice"
+        },
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "fields": [
-                "references"
+                "tgt",
+                "src"
             ],
-            "to_field": "references",
+            "to_field": "correct_and_incorrect",
             "type": "list_field_values"
+        },
+        {
+            "field": "correct_and_incorrect",
+            "to_field": "text",
+            "type": "duplicate_by_list"
+        },
+        {
+            "index_of": "text",
+            "search_in": "correct_and_incorrect",
+            "to_field": "label",
+            "type": "index_of"
+        },
+        {
+            "fields": {
+                "class": "Grammatically incorrect",
+                "text_type": "text"
+            },
+            "type": "add_fields"
+        },
+        {
+            "page_size": 9223372036854775807,
+            "type": "shuffle"
         }
     ],
-    "type": "metric_pipeline"
+    "task": "tasks.classification.binary[metrics=[metrics.accuracy,metrics.f1_binary,metrics.precision_binary,metrics.recall_binary]]",
+    "templates": "templates.grammatical_error_detection.all",
+    "type": "task_card"
 }
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json` & `unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/labrador.json` & `unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/labradorite.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/llama.json` & `unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/system_prompts/models/llama2.json` & `unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/default.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/instruction.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/instruction.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/classification/multi_label/title.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'choices_separator'": "'\\n'", 'delete': "['choices_seperator']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "choices_seperator": "\n",
+    "choices_separator": "\n",
     "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
     "instruction": "Answer the multiple choice Question from one of the Choices (choose from {numerals}) based on the {context_type}.",
     "postprocessors": [
         "processors.take_first_non_empty_line",
         "processors.match_closest_option"
     ],
     "target_choice_format": "{choice_numeral}. {choice_text}",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'choices_separator'": "'\\n'", 'delete': "['choices_seperator']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "choices_seperator": "\n",
+    "choices_separator": "\n",
     "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
     "instruction": "Answer the multiple choice Question from one of the Choices (choose from {numerals}) based on the {context_type}.",
     "postprocessors": [
         "processors.to_string_stripped",
         "processors.first_character"
     ],
     "target_field": "answer",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'choices_separator'": "'\\n'", 'delete': "['choices_seperator']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "choices_seperator": "\n",
+    "choices_separator": "\n",
     "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
     "instruction": "Answer the multiple choice Question about {topic} from one of the Choices (choose from {numerals}) based on the {context_type}.",
     "postprocessors": [
         "processors.take_first_non_empty_line",
         "processors.match_closest_option"
     ],
     "target_choice_format": "{choice_numeral}. {choice_text}",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'choices_separator'": "'\\n'", 'delete': "['choices_seperator']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "choices_seperator": "\n",
+    "choices_separator": "\n",
     "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
     "instruction": "Answer the multiple choice Question about {topic} from one of the Choices (choose from {numerals}) based on the {context_type}.",
     "postprocessors": [
         "processors.to_string_stripped",
         "processors.first_character"
     ],
     "target_field": "answer",
```

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/summarization/abstractive/all.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json` & `unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/catalog.py` & `unitxt-1.7.6/src/unitxt/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     location: str = constants.default_catalog_path
     is_local: bool = True
 
     def path(self, artifact_identifier: str):
         assert (
             artifact_identifier.strip()
         ), "artifact_identifier should not be an empty string."
-        parts = artifact_identifier.split(constants.catalog_hirarchy_sep)
+        parts = artifact_identifier.split(constants.catalog_hierarchy_sep)
         parts[-1] = parts[-1] + ".json"
         return os.path.join(self.location, *parts)
 
     def load(self, artifact_identifier: str, overwrite_args=None):
         assert (
             artifact_identifier in self
         ), f"Artifact with name {artifact_identifier} does not exist"
@@ -112,15 +112,15 @@
         url = self.path(artifact_identifier)
         response = requests.head(url)
         return response.status_code == 200
 
 
 def verify_legal_catalog_name(name):
     assert re.match(
-        r"^[\w" + constants.catalog_hirarchy_sep + "]+$", name
+        r"^[\w" + constants.catalog_hierarchy_sep + "]+$", name
     ), f'Artifict name ("{name}") should be alphanumeric. Use "." for nesting (e.g. myfolder.my_artifact)'
 
 
 def add_to_catalog(
     artifact: Artifact,
     name: str,
     catalog: Catalog = None,
```

### Comparing `unitxt-1.7.4/src/unitxt/collections.py` & `unitxt-1.7.6/src/unitxt/collections.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/collections_operators.py` & `unitxt-1.7.6/src/unitxt/collections_operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,23 @@
         if self.inside == "tuple":
             return (value,)
         return {
             value,
         }
 
 
+class Chunk(FieldOperator):
+    size: int
+
+    def process_value(self, collection: Any) -> Any:
+        return [
+            collection[i : i + self.size] for i in range(0, len(collection), self.size)
+        ]
+
+
 class Slice(FieldOperator):
     start: Optional[int] = None
     stop: Optional[int] = None
     step: Optional[int] = None
 
     def process_value(self, collection: Any) -> Any:
         slicer = slice(self.start, self.stop, self.step)
```

### Comparing `unitxt-1.7.4/src/unitxt/dataclass.py` & `unitxt-1.7.6/src/unitxt/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import dataclasses
 import functools
+import warnings
 from abc import ABCMeta
 from inspect import Parameter, Signature
-from typing import Any, final
+from typing import Any, Dict, final
 
 _FIELDS = "__fields__"
 
 
 class Undefined:
     pass
 
@@ -32,30 +33,38 @@
     type: type = None
     init: bool = True
     also_positional: bool = True
     default_factory: Any = None
     final: bool = False
     abstract: bool = False
     required: bool = False
+    deprecated: bool = False
     internal: bool = False
     origin_cls: type = None
+    metadata: Dict[str, str] = dataclasses.field(default_factory=dict)
 
     def get_default(self):
         if self.default_factory is not None:
             return self.default_factory()
         return self.default
 
 
 @dataclasses.dataclass
 class FinalField(Field):
     def __post_init__(self):
         self.final = True
 
 
 @dataclasses.dataclass
+class DeprecatedField(Field):
+    def __post_init__(self):
+        self.deprecated = True
+
+
+@dataclasses.dataclass
 class RequiredField(Field):
     def __post_init__(self):
         self.required = True
 
 
 class MissingDefaultError(TypeError):
     pass
@@ -107,29 +116,29 @@
     pass
 
 
 class UnexpectedArgumentError(TypeError):
     pass
 
 
-standart_variables = dir(object)
+standard_variables = dir(object)
 
 
 def is_possible_field(field_name, field_value):
     """Check if a name-value pair can potentially represent a field.
 
     Args:
         field_name (str): The name of the field.
         field_value: The value of the field.
 
     Returns:
         bool: True if the name-value pair can represent a field, False otherwise.
     """
     return (
-        field_name not in standart_variables
+        field_name not in standard_variables
         and not field_name.startswith("__")
         and not callable(field_value)
     )
 
 
 def get_fields(cls, attrs):
     """Get the fields for a class based on its attributes.
@@ -225,26 +234,34 @@
     return [field for field in fields(cls) if field.final]
 
 
 def required_fields(cls):
     return [field for field in fields(cls) if field.required]
 
 
+def deprecated_fields(cls):
+    return [field for field in fields(cls) if field.deprecated]
+
+
 def abstract_fields(cls):
     return [field for field in fields(cls) if field.abstract]
 
 
 def is_abstract_field(field):
     return field.abstract
 
 
 def is_final_field(field):
     return field.final
 
 
+def is_deprecated_field(field):
+    return field.deprecated
+
+
 def get_field_default(field):
     if field.default_factory is not None:
         return field.default_factory()
 
     return field.default
 
 
@@ -390,21 +407,28 @@
     __allow_unexpected_arguments__ = False
 
     @final
     def __init__(self, *argv, **kwargs):
         """Initialize fields based on kwargs.
 
         Checks for abstract fields when an instance is created.
+        Warn when a deprecated is used
         """
         _init_fields = [field for field in fields(self) if field.init]
         _init_fields_names = [field.name for field in _init_fields]
         _init_positional_fields_names = [
             field.name for field in _init_fields if field.also_positional
         ]
 
+        _init_deprecated_fields = [field for field in _init_fields if field.deprecated]
+        for dep_field in _init_deprecated_fields:
+            warnings.warn(
+                dep_field.metadata["deprecation_msg"], DeprecationWarning, stacklevel=2
+            )
+
         for name in _init_positional_fields_names[: len(argv)]:
             if name in kwargs:
                 raise TypeError(
                     f"{self.__class__.__name__} got multiple values for argument '{name}'"
                 )
 
         expected_unexpected_argv = kwargs.pop("_argv", None)
```

### Comparing `unitxt-1.7.4/src/unitxt/dataset.py` & `unitxt-1.7.6/src/unitxt/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .dialog_operators import __file__ as _
 from .dict_utils import __file__ as _
 from .eval_utils import __file__ as _
 from .file_utils import __file__ as _
 from .formats import __file__ as _
 from .fusion import __file__ as _
 from .generator_utils import __file__ as _
-from .hf_utils import __file__ as _
+from .hf_utils import verify_versions_compatibility
 from .instructions import __file__ as _
 from .loaders import __file__ as _
 from .logging_utils import get_logger
 from .metric import __file__ as _
 from .metric_utils import __file__ as _
 from .metrics import __file__ as _
 from .normalizers import __file__ as _
@@ -61,23 +61,16 @@
 
     VERSION = constants.version
 
     @property
     def generators(self):
         if not hasattr(self, "_generators") or self._generators is None:
             if is_package_installed("unitxt"):
-                from unitxt.settings_utils import (
-                    get_constants as installed_get_constants,
-                )
+                verify_versions_compatibility("dataset", self.VERSION)
 
-                installed_package_constants = installed_get_constants()
-                if installed_package_constants.version != self.VERSION:
-                    raise ValueError(
-                        f"Located installed unitxt version {installed_get_constants.version} that is different then unitxt dataset version {self.VERSION}. Please make sure the installed version is identical to the dataset version."
-                    )
                 from unitxt.dataset_utils import (
                     get_dataset_artifact as get_dataset_artifact_installed,
                 )
 
                 logger.info("Loading with installed unitxt library...")
                 dataset = get_dataset_artifact_installed(self.config.name)
             else:
```

### Comparing `unitxt-1.7.4/src/unitxt/dataset_utils.py` & `unitxt-1.7.6/src/unitxt/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/deprecation_utils.py` & `unitxt-1.7.6/src/unitxt/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/dialog_operators.py` & `unitxt-1.7.6/src/unitxt/dialog_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,57 +32,57 @@
         last_system_turn_to_field (Optional[str]): Field to store the last system turn.
         context_field (Optional[str]): Field that contains additional context to be prepended to the dialog.
     """
 
     format: Optional[SystemFormat] = None
     last_response_to_field: Optional[str] = None
     context_field: Optional[str] = None
-    context_seperator: str = " "
+    context_separator: str = " "
 
-    def standartize_format(self, demo_format):
+    def standardize_format(self, demo_format):
         turn_format = demo_format.replace("{source}", "{user}")
         turn_format = turn_format.replace("{target}", "{system}")
         return turn_format.replace("{target_prefix}", "")
 
     def slice_first_turn(self, turn_format):
         return turn_format[turn_format.index("{user}") :]
 
     def slice_last_turn(self, turn_format):
         return turn_format[: turn_format.index("{system}") + len("{system}")]
 
-    def slice_last_reponse(self, turn_format):
+    def slice_last_response(self, turn_format):
         return turn_format[: turn_format.index("{user}") + len("{user}")]
 
     def get_turn_format(self, turn_format, step, length):
         if step == 0:
             turn_format = self.slice_first_turn(turn_format)
         if step == length - 1:
             turn_format = self.slice_last_turn(turn_format)
             if self.last_response_to_field is not None:
-                turn_format = self.slice_last_reponse(turn_format)
+                turn_format = self.slice_last_response(turn_format)
         return turn_format
 
     def get_general_turn_format(self, instance):
         general_format = (
             instance["recipe_metadata"]["format"]
             if self.format is None
             else self.format
         )
-        return self.standartize_format(general_format.demo_format)
+        return self.standardize_format(general_format.demo_format)
 
     def process_instance_value(
-        self, structred_dialog: List[Dict[str, str]], instance: Dict[str, Any]
+        self, structured_dialog: List[Dict[str, str]], instance: Dict[str, Any]
     ):
         dialog = (
             ""
             if self.context_field is None
-            else instance[self.context_field] + self.context_seperator
+            else instance[self.context_field] + self.context_separator
         )
         general_turn_format = self.get_general_turn_format(instance)
-        for i, turn in enumerate(structred_dialog):
+        for i, turn in enumerate(structured_dialog):
             turn_format = self.get_turn_format(
-                general_turn_format, i, len(structred_dialog)
+                general_turn_format, i, len(structured_dialog)
             )
             dialog += turn_format.format(**turn)
         if self.last_response_to_field is not None:
             instance[self.last_response_to_field] = turn["system"]
         return dialog
```

### Comparing `unitxt-1.7.4/src/unitxt/dict_utils.py` & `unitxt-1.7.6/src/unitxt/dict_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,36 +174,51 @@
 
 
 def dict_delete(
     dic: dict, query: str, not_exist_ok: bool = False, remove_empty_ancestors=False
 ):
     # We remove from dic the value from each and every element lead to by a path matching the query.
     # If remove_empty_ancestors=True, and the removal of any such value leaves its containing element (list or dict)
-    # within dic empty -- remove that element as well, and continue recursively
+    # within dic empty -- remove that element as well, and continue recursively, but stop one step before deleting dic
+    # altogether, even if became {}. If successful, changes dic into its new shape
+
+    if dic is None or not isinstance(dic, (list, dict)):
+        raise ValueError(
+            f"dic {dic} is either None or not a list nor a dict. Can not delete from it."
+        )
+
+    if len(query) == 0:
+        raise ValueError(
+            "Query is an empty string, implying the deletion of dic as a whole. This can not be done via this function call."
+        )
+
+    if isinstance(dic, dict) and query.strip() in dic:
+        dic.pop(query.strip())
+        return
+
     qpath = validate_query_and_break_to_components(query)
-    if len(qpath) == 1:
-        if qpath[0] in dic:
-            dic.pop(qpath[0])
-            return
-        if not not_exist_ok:
-            raise ValueError(
-                f"An attempt to delete from dictionary {dic}, an element {query}, that does not exist in the dictionary"
-            )
 
     try:
         success, new_val = delete_values(
             current_element=dic,
             query=qpath,
             index_into_query=(-1) * len(qpath),
             remove_empty_ancestors=remove_empty_ancestors,
         )
-        if not success and not not_exist_ok:
+
+        if success:
+            if new_val == {}:
+                dic.clear()
+            return
+
+        if not not_exist_ok:
             raise ValueError(
-                f"An attempt to delete from dictionary {dic}, an element {query}, that does not exist in the dictionary"
+                f"An attempt to delete from dictionary {dic}, an element {query}, that does not exist in the dictionary, while not_exist_ok=False"
             )
+
     except Exception as e:
         raise ValueError(f"query {query} matches no path in dictionary {dic}") from e
 
 
 # returns all the values sitting inside dic, in all the paths that match query_path
 # if query includes * then return a list of values reached by all paths that match the query
 # flake8: noqa: C901
@@ -229,15 +244,16 @@
             try:
                 success, val = get_values(sub_element, query, index_into_query + 1)
                 if success:
                     to_ret.append(val)
             except:
                 continue
 
-        return (len(to_ret) > 0, to_ret)
+        return (len(to_ret) > 0 or index_into_query == -1, to_ret)
+        # when * is the last component, it refers to 'all the contents' of an empty list being current_element.
     # next_component is indx or name, current_element must be a list or a dict
     if indx.match(component):
         component = int(component)
     try:
         success, new_val = get_values(
             current_element[component], query, index_into_query + 1
         )
@@ -257,34 +273,41 @@
     fixed_parameters: dict,
     set_multiple: bool = False,
 ) -> Tuple[bool, Any]:
     if index_into_query == 0:
         return (True, value)  # matched query all along!
 
     # current_element should be a list or dict: a containing element
-    if current_element and not isinstance(current_element, (list, dict)):
+    if current_element is not None and not isinstance(current_element, (list, dict)):
         current_element = None  # give it a chance to become what is needed, if allowed
 
-    if not current_element and not fixed_parameters["generate_if_not_exists"]:
+    if current_element is None and not fixed_parameters["generate_if_not_exists"]:
         return (False, None)
-    component = fixed_parameters["query"][index_into_query]
 
+    component = fixed_parameters["query"][index_into_query]
     if component == "*":
-        if current_element and set_multiple:
+        if current_element is not None and set_multiple:
             if isinstance(current_element, dict) and len(current_element) != len(value):
                 return (False, None)
             if isinstance(current_element, list) and len(current_element) > len(value):
                 return (False, None)
             if len(current_element) < len(value):
                 if not fixed_parameters["generate_if_not_exists"]:
                     return (False, None)
                 # current_element must be a list, extend current_element to the length needed
                 current_element.extend([None] * (len(value) - len(current_element)))
-        if not current_element:
-            current_element = [None] * (len(value) if set_multiple else 1)
+        if current_element is None or current_element == []:
+            current_element = [None] * (
+                len(value)
+                if set_multiple
+                else value is None
+                or not isinstance(value, list)
+                or len(value) > 0
+                or index_into_query < -1
+            )
         # now current_element is of size suiting value
         if isinstance(current_element, dict):
             keys = sorted(current_element.keys())
         else:
             keys = list(range(len(current_element)))
 
         any_success = False
@@ -300,40 +323,38 @@
                 if not success:
                     continue
                 any_success = True
                 current_element[keys[i]] = new_val
 
             except:
                 continue
-        return (any_success, current_element)
+        return (
+            any_success or (len(keys) == 0 and index_into_query == -1),
+            current_element,
+        )
 
     # component is an index into a list or a key into a dictionary
     if indx.match(component):
-        if current_element and not isinstance(current_element, list):
+        if current_element is None or not isinstance(current_element, list):
             if not fixed_parameters["generate_if_not_exists"]:
                 return (False, None)
             current_element = []
+        # current_element is a list
         component = int(component)
-        if (
-            current_element and component >= len(current_element)
-        ) or not current_element:
+        if component >= len(current_element):
             if not fixed_parameters["generate_if_not_exists"]:
                 return (False, None)
             # extend current_element to the length needed
-            if not current_element:
-                current_element = []
             current_element.extend([None] * (component + 1 - len(current_element)))
         next_current_element = current_element[component]
     else:  # component is a key into a dictionary
-        if current_element and not isinstance(current_element, dict):
+        if current_element is None or not isinstance(current_element, dict):
             if not fixed_parameters["generate_if_not_exists"]:
                 return (False, None)
             current_element = {}
-        if not current_element:
-            current_element = {}
         if (
             component not in current_element
             and not fixed_parameters["generate_if_not_exists"]
         ):
             return (False, None)
         next_current_element = (
             None if component not in current_element else current_element[component]
@@ -354,53 +375,54 @@
         return (False, None)
 
 
 # the returned values are ordered by the lexicographic order of the paths leading to them
 def dict_get(
     dic: dict,
     query: str,
-    use_dpath: bool = True,
     not_exist_ok: bool = False,
     default: Any = None,
 ):
-    if use_dpath and "/" in query:
-        components = validate_query_and_break_to_components(query)
+    if len(query.strip()) == 0:
+        return dic
+
+    if dic is None:
+        raise ValueError("Can not get any value from a dic that is None")
+
+    if isinstance(dic, dict) and query.strip() in dic:
+        return dic[query.strip()]
+
+    components = validate_query_and_break_to_components(query)
+    if len(components) > 1:
         try:
             success, values = get_values(dic, components, -1 * len(components))
             if not success:
                 if not_exist_ok:
                     return default
                 raise ValueError(
                     f'query "{query}" did not match any item in dict: {dic}'
                 )
-            if isinstance(values, list) and len(values) == 0:
-                if not_exist_ok:
-                    return default
-                raise ValueError(
-                    f'query "{query}" did not match any item in dict: {dic} while not_exist_ok=False'
-                )
 
             return values
 
         except Exception as e:
             if not_exist_ok:
                 return default
             raise ValueError(
-                f'query "{query}" did not match any item in dict: {dic} while not_exist_ok=False'
+                f'query "{query}" did not match any item in dict: {dic}'
             ) from e
 
-    if query.strip() in dic:
-        return dic[query.strip()]
+    # len(components) == 1
+    if components[0] in dic:
+        return dic[components[0]]
 
     if not_exist_ok:
         return default
 
-    raise ValueError(
-        f'query "{query}" did not match any item in dict: {dic} while not_exist_ok=False'
-    )
+    raise ValueError(f'query "{query}" did not match any item in dict: {dic}')
 
 
 # dict_set sets a value, 'value', which by itself, can be a dict or list or scalar, into 'dic', to become the value of
 # the element the path from 'dic' head to which matches 'query'. (aka - 'the element specified by the query')
 # 'the element specified by the query' is thus either a key in a dictionary, or a list member specified by its index in the list.
 # Unless otherwise specified (through 'not_exist_ok=True'), the processing of 'query' by dict_set does not generate
 # any new elements into 'dic'. Rather - it just sets the 'value' arg to each and every element the path to which matches
@@ -444,33 +466,52 @@
 # as the target value for the i-th path that goes through el.
 # Such a breakdown of 'value' for set_multiple=True, is done only once - on the leftmost * in 'query'.
 #
 def dict_set(
     dic: dict,
     query: str,
     value: Any,
-    use_dpath=True,
     not_exist_ok=True,
     set_multiple=False,
-):
-    if set_multiple and (
-        not isinstance(value, list) or len(value) == 0 or "*" not in query
-    ):
+):  # sets dic to its new value
+    if dic is None or not isinstance(dic, (list, dict)):
         raise ValueError(
-            f"set_multiple == True, and yet value, {value}, is not a list or '*' is not in query '{query}'"
+            f"Can not change dic that is either None or not a dict nor a list. Got dic = {dic}"
         )
-    if not use_dpath or "/" not in query:
-        if query.strip() in dic or not_exist_ok:
-            dic[query] = value
+
+    if query.strip() == "":
+        # change the whole input dic, as dic indeed matches ""
+        if isinstance(dic, dict):
+            if value is None or not isinstance(value, dict):
+                raise ValueError(
+                    f"Through an empty query, trying to set a whole new value, {value}, to the whole of dic, {dic}, but value is not a dict"
+                )
+            dic.clear()
+            dic.update(value)
             return
-        raise ValueError(
-            f"not_exist_ok=False and the single component query '{query}' is not a key in dic {dic}"
-        )
 
-    # use_dpath and "/" in query
+        if isinstance(dic, list):
+            if value is None or not isinstance(value, list):
+                raise ValueError(
+                    f"Through an empty query, trying to set a whole new value, {value}, to the whole of dic, {dic}, but value is not a list"
+                )
+            dic.clear()
+            dic.extend(value)
+            return
+
+    if isinstance(dic, dict) and query.strip() in dic:
+        dic[query.strip()] = value
+        return
+
+    if set_multiple:
+        if value is None or not isinstance(value, list) or len(value) == 0:
+            raise ValueError(
+                f"set_multiple=True, but value, {value}, can not be broken up, as either it is not a list or it is an empty list"
+            )
+
     components = validate_query_and_break_to_components(query)
     fixed_parameters = {
         "query": components,
         "generate_if_not_exists": not_exist_ok,
     }
     try:
         success, val = set_values(
```

### Comparing `unitxt-1.7.4/src/unitxt/eval_utils.py` & `unitxt-1.7.6/src/unitxt/eval_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/file_utils.py` & `unitxt-1.7.6/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/fusion.py` & `unitxt-1.7.6/src/unitxt/fusion.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/generator_utils.py` & `unitxt-1.7.6/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/loaders.py` & `unitxt-1.7.6/src/unitxt/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
                         trust_remote_code=settings.allow_unverified_code,
                     )
                 except ValueError as e:
                     if "trust_remote_code" in str(e):
                         raise ValueError(
                             f"{self.__class__.__name__} cannot run remote code from huggingface without setting unitxt.settings.allow_unverified_code=True or by setting environment variable: UNITXT_ALLOW_UNVERIFIED_CODE."
                         ) from e
+                    raise e
 
             if self.filtering_lambda is not None:
                 dataset = self.filtered_load(dataset)
 
             if self.split is not None:
                 dataset = {self.split: dataset}
```

### Comparing `unitxt-1.7.4/src/unitxt/logging_utils.py` & `unitxt-1.7.6/src/unitxt/logging_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/metric.py` & `unitxt-1.7.6/src/unitxt/metric.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .dialog_operators import __file__ as _
 from .dict_utils import __file__ as _
 from .eval_utils import __file__ as _
 from .file_utils import __file__ as _
 from .formats import __file__ as _
 from .fusion import __file__ as _
 from .generator_utils import __file__ as _
-from .hf_utils import __file__ as _
+from .hf_utils import verify_versions_compatibility
 from .instructions import __file__ as _
 from .loaders import __file__ as _
 from .logging_utils import __file__ as _
 from .metric_utils import UNITXT_METRIC_SCHEMA, _compute
 from .metrics import __file__ as _
 from .normalizers import __file__ as _
 from .operator import __file__ as _
@@ -71,21 +71,15 @@
         self,
         predictions: List[str],
         references: Iterable,
         flatten: bool = False,
         split_name: str = "all",
     ):
         if is_package_installed("unitxt"):
-            from unitxt.settings_utils import get_constants as installed_get_constants
-
-            installed_package_constants = installed_get_constants()
-            if installed_package_constants.version != self.VERSION:
-                raise ValueError(
-                    f"Located installed unitxt version {installed_get_constants.version} that is different then unitxt metric version {self.VERSION}. Please make sure the installed version is identical to the dataset version."
-                )
+            verify_versions_compatibility("metric", self.VERSION)
 
             from unitxt.metric_utils import _compute as _compute_installed
 
             return _compute_installed(
                 predictions=predictions,
                 references=references,
                 flatten=flatten,
```

### Comparing `unitxt-1.7.4/src/unitxt/metric_utils.py` & `unitxt-1.7.6/src/unitxt/metric_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Iterable, List, Optional
 
 from datasets import Features, Value
 
 from .dataclass import Dataclass
 from .operator import (
     MultiStreamOperator,
-    SequentialOperatorInitilizer,
+    SequentialOperatorInitializer,
     StreamInitializerOperator,
 )
 from .operators import (
     Apply,
     ApplyMetric,
     ApplyOperatorsField,
     FlattenInstances,
@@ -20,15 +20,15 @@
 from .register import _reset_env_local_catalogs, register_all_artifacts
 from .schema import UNITXT_DATASET_SCHEMA
 from .settings_utils import get_settings
 from .stream import MultiStream, Stream
 
 
 class MultiStreamScoreMean(MultiStreamOperator):
-    def aggegate_results(self, multi_stream: MultiStream):
+    def aggregate_results(self, multi_stream: MultiStream):
         scores = []
         for stream in multi_stream.values():
             instance = stream.peek()
             scores.append(instance["score"]["global"]["score"])
 
         from statistics import mean
 
@@ -54,15 +54,15 @@
         if len(multi_stream) == 1:
             for stream_name, stream in multi_stream.items():
                 result[stream_name] = Stream(
                     self.spread_results_one_stream, gen_kwargs={"stream": stream}
                 )
             return MultiStream(result)
 
-        mean_score = self.aggegate_results(multi_stream)
+        mean_score = self.aggregate_results(multi_stream)
         result = {}
         for stream_name, stream in multi_stream.items():
             result[stream_name] = Stream(
                 self.spread_results, gen_kwargs={"stream": stream, "score": mean_score}
             )
 
         return MultiStream(result)
@@ -88,15 +88,15 @@
 
 # The task_data field in the schema is defined as
 # Sequence({"key": Value(dtype="string"), "value": Value("string")})
 # When receiving instances from this scheme, the keys and values are returned as two separate
 # lists, and are converted to a dictionary.
 
 
-class MetricRecipe(SequentialOperatorInitilizer):
+class MetricRecipe(SequentialOperatorInitializer):
     calc_confidence_intervals: bool = True
 
     def prepare(self):
         register_all_artifacts()
         self.steps = [
             FromPredictionsAndOriginalData(),
             Apply(
```

### Comparing `unitxt-1.7.4/src/unitxt/metrics.py` & `unitxt-1.7.6/src/unitxt/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import evaluate
 import numpy
 import numpy as np
 from scipy.stats import bootstrap
 from scipy.stats._warnings_errors import DegenerateDataWarning
 
 from .artifact import Artifact
-from .dataclass import AbstractField, InternalField, OptionalField
+from .dataclass import AbstractField, InternalField, NonPositionalField, OptionalField
 from .logging_utils import get_logger
 from .metric_utils import InstanceInput, MetricRequest, MetricResponse
 from .operator import (
     MultiStreamOperator,
     SingleStreamOperator,
     StreamingOperator,
     StreamInstanceOperator,
@@ -644,14 +644,17 @@
     subgroup_column = None
     implemented_reductions: List[str] = field(
         default_factory=lambda: ["mean", "group_mean", "max"]
     )
 
     reduction_map: Dict[str, List[str]] = AbstractField()
 
+    reference_field: str = NonPositionalField(default="references")
+    prediction_field: str = NonPositionalField(default="prediction")
+
     def _validate_group_mean_reduction(self, instances: List[dict]):
         """Ensure that group_mean reduction_map is properly formatted.
 
         Example: Apply the variance (np.var) to group Accuracy instance scores.  This class would be specified as follows:
 
         class GroupVarianceAccuracy(Accuracy):
             reduction_map = {'group_mean': {'agg_func': ['variance', np.var, True]}}
@@ -823,18 +826,29 @@
     def compute_instance_scores(
         self, stream: Stream, stream_name: Optional[str] = None
     ):
         global_score = {}
         instances = []
 
         for instance in stream:
-            refs, pred = instance["references"], instance["prediction"]
+            task_data = instance["task_data"] if "task_data" in instance else {}
+
+            if self.reference_field == "references":
+                refs = instance["references"]
+            else:
+                refs = task_data[self.reference_field]
+                if not isinstance(refs, list):
+                    refs = [refs]
+            if self.prediction_field == "prediction":
+                pred = instance["prediction"]
+            else:
+                pred = task_data[self.prediction_field]
+
             self._validate_prediction(pred)
             self._validate_reference(refs)
-            task_data = instance["task_data"] if "task_data" in instance else {}
 
             instance_score = self.compute(
                 references=refs, prediction=pred, task_data=task_data
             )
             instance_score["score"] = instance_score[self.main_score]
             instance_score["score_name"] = self.main_score
             if "score" not in instance:
@@ -1029,15 +1043,14 @@
     def prepare(self):
         super().prepare()
         self.prepare_score = CopyFields(
             field_to_field=[
                 [f"score/instance/{self.main_score}", "score/instance/score"],
                 [f"score/global/{self.main_score}", "score/global/score"],
             ],
-            use_query=True,
         )
 
     def process(self, multi_stream: MultiStream) -> MultiStream:
         for step in self.preprocess_steps:
             multi_stream = step(multi_stream)
         multi_stream = self.metric(multi_stream)
         for step in self.postpreprocess_steps:
@@ -1443,37 +1456,51 @@
                 ["\n".join(self.sent_tokenize(r.strip())) for r in reference]
                 for reference in references
             ]
         return super().compute(references, predictions, task_data)
 
 
 # Computes char edit distance, ignoring whitespace
-class CharEditDistanceAccuracy(InstanceMetric):
-    reduction_map = {"mean": ["char_edit_dist_accuracy"]}
-    main_score = "char_edit_dist_accuracy"
-    ci_scores = ["char_edit_dist_accuracy"]
+class CharEditDistance(InstanceMetric):
+    main_score = "char_edit_distance"
+    reduction_map = {"mean": [main_score]}
+    ci_scores = [main_score]
     prediction_type = "str"
     single_reference_per_prediction = True
 
+    accuracy_metric = False
+
     _requirements_list: List[str] = ["editdistance"]
 
     def prepare(self):
         super().prepare()
         import editdistance
 
         self.eval = editdistance.eval
 
     def compute(self, references, prediction: str, task_data: List[Dict]) -> dict:
         formatted_prediction = "".join(prediction.split())
         formatted_reference = "".join(references[0].split())
         max_length = max(len(formatted_reference), len(formatted_prediction))
         if max_length == 0:
-            return {"char_edit_dist_accuracy": 0.0}
+            return {self.main_score: 0.0}
         edit_dist = self.eval(formatted_reference, formatted_prediction)
-        return {"char_edit_dist_accuracy": (1 - edit_dist / max_length)}
+        if self.accuracy_metric:
+            score = 1 - edit_dist / max_length
+        else:
+            score = edit_dist
+        return {self.main_score: score}
+
+
+class CharEditDistanceAccuracy(CharEditDistance):
+    main_score = "char_edit_dist_accuracy"
+    reduction_map = {"mean": [main_score]}
+    ci_scores = [main_score]
+
+    accuracy_metric = True
 
 
 class Wer(HuggingfaceMetric):
     hf_metric_name = "wer"
     main_score = "wer"
     prediction_type = "str"
     single_reference_per_prediction = True
@@ -1849,14 +1876,16 @@
     hf_metric_name = "bertscore"
     main_score = "f1"
     reduction_map = {"mean": ["f1", "precision", "recall"]}
     hf_metric_fields = ["f1", "precision", "recall"]
     ci_scores = ["f1", "precision", "recall"]
     model_name: str
 
+    prediction_type = "str"
+
     _requirements_list: List[str] = ["bert_score"]
 
     def prepare(self):
         super().prepare()
         self.hf_compute_args = {"model_type": self.model_name, "batch_size": 16}
 
 
@@ -1945,14 +1974,46 @@
         inputs = [{"text": q, "text_pair": a} for q, a in zip(questions, answers)]
 
         # compute the metric
         # add function_to_apply="none" to disable sigmoid
         return self.pipe(inputs, batch_size=self.batch_size)
 
 
+class Detector(BulkInstanceMetric):
+    reduction_map = {"mean": ["score"]}
+    main_score = "score"
+    batch_size: int = 32
+
+    prediction_type = "str"
+
+    model_name: str
+
+    _requirements_list: List[str] = ["transformers", "torch"]
+
+    def prepare(self):
+        super().prepare()
+        import torch
+        from transformers import pipeline
+
+        device = "cuda:0" if torch.cuda.is_available() else "cpu"
+        self.pipe = pipeline(
+            "text-classification", model=self.model_name, device=device
+        )
+
+    def compute(
+        self,
+        references: List[List[Any]],
+        predictions: List[Any],
+        task_data: List[Dict],
+    ) -> List[Dict[str, Any]]:
+        # compute the metric
+        # add function_to_apply="none" to disable sigmoid
+        return self.pipe(predictions, batch_size=self.batch_size)
+
+
 class LlamaIndexCorrectness(InstanceMetric):
     """LlamaIndex based metric class for evaluating correctness."""
 
     model_name: str = ""
     main_score: str = ""
     prediction_type: str = "str"
     reduction_map: Dict[str, List[str]] = None
@@ -3316,14 +3377,107 @@
             if acc > best_acc:
                 best_acc = acc
                 best_thr = thr
 
         return {self.main_score: best_acc, "best_thr_max_acc": best_thr}
 
 
+######################
+# RerankRecallMetric #
+
+
+def pytrec_eval_at_k(results, qrels, at_k, metric_name):
+    import pandas as pd
+    import pytrec_eval
+
+    metric = {}
+
+    for k in at_k:
+        metric[f"{metric_name}@{k}"] = 0.0
+
+    metric_string = f"{metric_name}." + ",".join([str(k) for k in at_k])
+    # print('metric_string = ', metric_string)
+    evaluator = pytrec_eval.RelevanceEvaluator(
+        qrels, {"ndcg", metric_string}
+    )  # {map_string, ndcg_string, recall_string, precision_string})
+    scores = evaluator.evaluate(results)
+    scores = pd.DataFrame(scores).transpose()
+
+    keys = []
+    column_map = {}
+    for k in at_k:
+        keys.append(f"{metric_name}_{k}")
+        column_map[f"{metric_name}_{k}"] = k
+    scores[keys].rename(columns=column_map)
+
+    return scores
+
+
+class RerankRecall(GlobalMetric):
+    """RerankRecall: measures the quality of reranking with respect to ground truth ranking scores.
+
+    This metric measures ranking performance across a dataset.  The
+    references for a query will have a score of 1 for the gold passage
+    and 0 for all other passages.  The model returns scores in [0,1]
+    for each passage,query pair.  This metric measures recall at k by
+    testing that the predicted score for the gold passage,query pair
+    is at least the k'th highest for all passages for that query.  A
+    query receives 1 if so, and 0 if not.  The 1's and 0's are
+    averaged across the dataset.
+
+    query_id_field selects the field containing the query id for an instance.
+    passage_id_field selects the field containing the passage id for an instance.
+    at_k selects the value of k used to compute recall.
+
+    """
+
+    main_score = "recall_at_5"
+    query_id_field: str = "query_id"
+    passage_id_field: str = "passage_id"
+    at_k: List[int] = [1, 2, 5]
+
+    # This doesn't seem to make sense
+    n_resamples = None
+
+    _requirements_list: List[str] = ["pandas", "pytrec_eval"]
+
+    def compute(
+        self,
+        references: List[List[str]],
+        predictions: List[str],
+        task_data: List[Dict],
+    ):
+        # Collect relevance score and ref per query/passage pair
+        results = {}
+        qrels = {}
+        for ref, pred, data in zip(references, predictions, task_data):
+            qid = data[self.query_id_field]
+            pid = data[self.passage_id_field]
+            if qid not in results:
+                results[qid] = {}
+                qrels[qid] = {}
+            # Convert string-wrapped float to regular float
+            try:
+                results[qid][pid] = float(pred)
+            except ValueError:
+                # Card testing feeds nonnumeric values in, so catch that.
+                results[qid][pid] = np.nan
+
+            # There's always a single reference per pid/qid pair
+            qrels[qid][pid] = int(ref[0])
+
+        # Compute recall @ 5
+        scores = pytrec_eval_at_k(results, qrels, self.at_k, "recall")
+        # print(scores.describe())
+        # pytrec returns numpy float32
+        return {
+            f"recall_at_{i}": float(scores[f"recall_{i}"].mean()) for i in self.at_k
+        }
+
+
 KO_ERROR_MESSAGE = """
 
 Additional dependencies required. To install them, run:
 `pip install "sacrebleu[ko]"`.
 
 For MacOS: If error on 'mecab-config' show up during installation ], one should run:
```

### Comparing `unitxt-1.7.4/src/unitxt/normalizers.py` & `unitxt-1.7.6/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/operator.py` & `unitxt-1.7.6/src/unitxt/operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,28 +505,28 @@
         ), "Calling process on a SourceSequentialOperator without any steps"
         multi_stream = self.steps[0]()
         for operator in self.steps[1 : self._get_max_steps()]:
             multi_stream = operator(multi_stream)
         return multi_stream
 
 
-class SequentialOperatorInitilizer(SequentialOperator):
+class SequentialOperatorInitializer(SequentialOperator):
     """A class representing a sequential operator initializer in the streaming system.
 
     A sequential operator initializer is a type of `SequntialOperator` that starts with a stream initializer operator. The first operator in its list of steps is a `StreamInitializerOperator`, which generates the initial `MultiStream` based on the provided arguments and keyword arguments.
     """
 
     def __call__(self, *args, **kwargs) -> MultiStream:
         return self.process(*args, **kwargs)
 
     def process(self, *args, **kwargs) -> MultiStream:
         assert (
             self.num_steps() > 0
-        ), "Calling process on a SequentialOperatorInitilizer without any steps"
+        ), "Calling process on a SequentialOperatorInitializer without any steps"
 
         assert isinstance(
             self.steps[0], StreamInitializerOperator
-        ), "The first step in a SequentialOperatorInitilizer must be a StreamInitializerOperator"
+        ), "The first step in a SequentialOperatorInitializer must be a StreamInitializerOperator"
         multi_stream = self.steps[0](*args, **kwargs)
         for operator in self.steps[1 : self._get_max_steps()]:
             multi_stream = operator(multi_stream)
         return multi_stream
```

### Comparing `unitxt-1.7.4/src/unitxt/operators.py` & `unitxt-1.7.6/src/unitxt/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 - :class:`formats<unitxt.formats>` for preparing data for models.
 
 The rest of this section is dedicated for general operators.
 
 General Operaotrs List:
 ------------------------
 """
-import collections
 import copy
 import operator
 import uuid
 import zipfile
 from abc import abstractmethod
 from collections import Counter
 from copy import deepcopy
@@ -54,15 +53,15 @@
     Tuple,
     Union,
 )
 
 import requests
 
 from .artifact import Artifact, fetch_artifact
-from .dataclass import NonPositionalField, OptionalField
+from .dataclass import DeprecatedField, NonPositionalField, OptionalField
 from .dict_utils import dict_delete, dict_get, dict_set, is_subpath
 from .operator import (
     MultiStream,
     MultiStreamOperator,
     PackageRequirementsMixin,
     PagedStreamOperator,
     SequentialOperator,
@@ -153,15 +152,14 @@
         replaces a list [1,2,3,4] with the string 'All' and an empty list by string 'None'.
         Note that mapped values are defined by their string representation, so mapped values
         must be converted to strings.
     """
 
     mappers: Dict[str, Dict[str, str]]
     strict: bool = True
-    use_query: bool = False
     process_every_value: bool = False
 
     def verify(self):
         # make sure the mappers are valid
         for key, mapper in self.mappers.items():
             assert isinstance(
                 mapper, dict
@@ -171,30 +169,29 @@
                     k, str
                 ), f'Key "{k}" in mapper for field "{key}" should be a string, got {type(k)}'
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         for key, mapper in self.mappers.items():
-            value = dict_get(instance, key, use_dpath=self.use_query)
+            value = dict_get(instance, key)
             if value is not None:
                 if (self.process_every_value is True) and (not isinstance(value, list)):
                     raise ValueError(
                         f"'process_every_field' == True is allowed only when all fields which have mappers, i.e., {list(self.mappers.keys())} are lists. Instance = {instance}"
                     )
                 if isinstance(value, list) and self.process_every_value:
                     for i, val in enumerate(value):
                         value[i] = self.get_mapped_value(instance, key, mapper, val)
                 else:
                     value = self.get_mapped_value(instance, key, mapper, value)
                 dict_set(
                     instance,
                     key,
                     value,
-                    use_dpath=self.use_query,
                 )
 
         return instance
 
     def get_mapped_value(self, instance, key, mapper, val):
         val_as_str = str(val)  # make sure the value is a string
         if self.strict and (val_as_str not in mapper):
@@ -225,15 +222,15 @@
 
 
 class AddFields(StreamInstanceOperator):
     """Adds specified fields to each instance in a given stream or all streams (default) If fields exist, updates them.
 
     Args:
         fields (Dict[str, object]): The fields to add to each instance.
-        use_query (bool) : Use '/' to access inner fields
+             Use '/' to access inner fields
         use_deepcopy (bool) : Deep copy the input value to avoid later modifications
 
     Examples:
         # Add a 'classes' field with a value of a list "positive" and "negative" to all streams
         AddFields(fields={"classes": ["positive","negatives"]})
 
         # Add a 'start' field under the 'span' field with a value of 0 to all streams
@@ -245,29 +242,29 @@
         # Add a 'classes' field on a given list, prevent modification of original list
         # from changing the instance.
         AddFields(fields={"classes": alist}), use_deepcopy=True)
         # if now alist is modified, still the instances remain intact.
     """
 
     fields: Dict[str, object]
-    use_query: bool = False
+    use_query: bool = DeprecatedField(
+        metadata={
+            "deprecation_msg": "Field 'use_query' is deprecated. From now on, default behavior is compatible to use_query=True. "
+            "Please remove this field from your code."
+        }
+    )
     use_deepcopy: bool = False
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
-        if self.use_query:
-            for key, value in self.fields.items():
-                if self.use_deepcopy:
-                    value = deepcopy(value)
-                dict_set(instance, key, value, use_dpath=self.use_query)
-        else:
+        for key, value in self.fields.items():
             if self.use_deepcopy:
-                self.fields = deepcopy(self.fields)
-            instance.update(self.fields)
+                value = deepcopy(value)
+            dict_set(instance, key, value)
         return instance
 
 
 class RemoveFields(StreamInstanceOperator):
     """Remove specified fields from each instance in a stream.
 
     Args:
@@ -298,25 +295,29 @@
           When the type of argument 'field_to_field' is List, the order by which the fields are processed is their order
           in the (outer) List. But when the type of argument 'field_to_field' is Dict, there is no uniquely determined
           order. The end result might depend on that order if either (1) two different fields are mapped to the same
           to_field, or (2) a field shows both as a key and as a value in different mappings.
           The operator throws an AssertionError in either of these cases.
           field_to_field defaults to None
         process_every_value (bool): Processes the values in a list instead of the list as a value, similar to *var. Defaults to False
-        use_query (bool): Whether to use dpath style queries. Defaults to False.
 
         Note: if 'field' and 'to_field' (or both members of a pair in 'field_to_field') are equal (or share a common
-        prefix if 'use_query'=True), then the result of the operation is saved within 'field'
+        prefix if 'field' and 'to_field' contain a /), then the result of the operation is saved within 'field'
     """
 
     field: Optional[str] = None
     to_field: Optional[str] = None
     field_to_field: Optional[Union[List[List[str]], Dict[str, str]]] = None
+    use_query: bool = DeprecatedField(
+        metadata={
+            "deprecation_msg": "Field 'use_query' is deprecated. From now on, default behavior is compatible to use_query=True. "
+            "Please remove this field from your code."
+        }
+    )
     process_every_value: bool = False
-    use_query: bool = False
     get_default: Any = None
     not_exist_ok: bool = False
 
     def verify(self):
         super().verify()
 
         assert (
@@ -393,15 +394,14 @@
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         for from_field, to_field in self._field_to_field:
             try:
                 old_value = dict_get(
                     instance,
                     from_field,
-                    use_dpath=self.use_query,
                     default=self.get_default,
                     not_exist_ok=self.not_exist_ok,
                 )
             except Exception as e:
                 raise ValueError(
                     f"Failed to get '{from_field}' from {instance} due to : {e}"
                 ) from e
@@ -417,15 +417,14 @@
                 raise ValueError(
                     f"Failed to process '{from_field}' from {instance} due to : {e}"
                 ) from e
             dict_set(
                 instance,
                 to_field,
                 new_value,
-                use_dpath=self.use_query,
                 not_exist_ok=True,
             )
         return instance
 
 
 class FieldOperator(InstanceFieldOperator):
     def process_instance_value(self, value: Any, instance: Dict[str, Any]):
@@ -435,28 +434,28 @@
     def process_value(self, value: Any) -> Any:
         pass
 
 
 class RenameFields(FieldOperator):
     """Renames fields.
 
-    Move value from one field to another, potentially, if 'use_query'=True, from one branch into another.
-    Remove the from field, potentially part of it in case of use_query.
+    Move value from one field to another, potentially, if field name contains a /, from one branch into another.
+    Remove the from field, potentially part of it in case of / in from_field.
 
     Examples:
         RenameFields(field_to_field={"b": "c"})
         will change inputs [{"a": 1, "b": 2}, {"a": 2, "b": 3}] to [{"a": 1, "c": 2}, {"a": 2, "c": 3}]
 
-        RenameFields(field_to_field={"b": "c/d"}, use_query=True)
+        RenameFields(field_to_field={"b": "c/d"})
         will change inputs [{"a": 1, "b": 2}, {"a": 2, "b": 3}] to [{"a": 1, "c": {"d": 2}}, {"a": 2, "c": {"d": 3}}]
 
-        RenameFields(field_to_field={"b": "b/d"}, use_query=True)
+        RenameFields(field_to_field={"b": "b/d"})
         will change inputs [{"a": 1, "b": 2}, {"a": 2, "b": 3}] to [{"a": 1, "b": {"d": 2}}, {"a": 2, "b": {"d": 3}}]
 
-        RenameFields(field_to_field={"b/c/e": "b/d"}, use_query=True)
+        RenameFields(field_to_field={"b/c/e": "b/d"})
         will change inputs [{"a": 1, "b": {"c": {"e": 2, "f": 20}}}] to [{"a": 1, "b": {"c": {"f": 20}, "d": 2}}]
 
     """
 
     def process_value(self, value: Any) -> Any:
         return value
 
@@ -535,28 +534,27 @@
             assert not self.augment_task_input
 
         for field_name in fields:
             try:
                 old_value = dict_get(
                     instance,
                     field_name,
-                    use_dpath=True,
                     default="",
                     not_exist_ok=False,
                 )
             except ValueError as e:
                 raise TypeError(f"Failed to get {field_name} from {instance}") from e
 
             try:
                 new_value = self.process_value(old_value)
             except Exception as e:
                 raise RuntimeError(
                     f"Error augmenting value '{old_value}' from '{field_name}' in instance: {instance}"
                 ) from e
-            dict_set(instance, field_name, new_value, use_dpath=True, not_exist_ok=True)
+            dict_set(instance, field_name, new_value, not_exist_ok=True)
         return instance
 
 
 class NullAugmentor(Augmentor):
     """Does not change the input string."""
 
     def verify(self):
@@ -805,22 +803,27 @@
 
 
 class ListFieldValues(StreamInstanceOperator):
     """Concatenates values of multiple fields into a list, and assigns it to a new field."""
 
     fields: List[str]
     to_field: str
-    use_query: bool = False
+    use_query: bool = DeprecatedField(
+        metadata={
+            "deprecation_msg": "Field 'use_query' is deprecated. From now on, default behavior is compatible to use_query=True. "
+            "Please remove this field from your code."
+        }
+    )
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         values = []
         for field_name in self.fields:
-            values.append(dict_get(instance, field_name, use_dpath=self.use_query))
+            values.append(dict_get(instance, field_name))
         instance[self.to_field] = values
         return instance
 
 
 class ZipFieldValues(StreamInstanceOperator):
     """Zips values of multiple fields in a given instance, similar to list(zip(*fields)).
 
@@ -832,64 +835,79 @@
     inputs with None -s.
 
     """
 
     fields: List[str]
     to_field: str
     longest: bool = False
-    use_query: bool = False
+    use_query: bool = DeprecatedField(
+        metadata={
+            "deprecation_msg": "Field 'use_query' is deprecated. From now on, default behavior is compatible to use_query=True. "
+            "Please remove this field from your code."
+        }
+    )
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         values = []
         for field_name in self.fields:
-            values.append(dict_get(instance, field_name, use_dpath=self.use_query))
+            values.append(dict_get(instance, field_name))
         if self.longest:
             zipped = zip_longest(*values)
         else:
             zipped = zip(*values)
         instance[self.to_field] = list(zipped)
         return instance
 
 
 class IndexOf(StreamInstanceOperator):
     """For a given instance, finds the offset of value of field 'index_of', within the value of field 'search_in'."""
 
     search_in: str
     index_of: str
     to_field: str
-    use_query: bool = False
+    use_query: bool = DeprecatedField(
+        metadata={
+            "deprecation_msg": "Field 'use_query' is deprecated. From now on, default behavior is compatible to use_query=True. "
+            "Please remove this field from your code."
+        }
+    )
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
-        lst = dict_get(instance, self.search_in, use_dpath=self.use_query)
-        item = dict_get(instance, self.index_of, use_dpath=self.use_query)
+        lst = dict_get(instance, self.search_in)
+        item = dict_get(instance, self.index_of)
         instance[self.to_field] = lst.index(item)
         return instance
 
 
 class TakeByField(StreamInstanceOperator):
     """From field 'field' of a given instance, select the member indexed by field 'index', and store to field 'to_field'."""
 
     field: str
     index: str
     to_field: str = None
-    use_query: bool = False
+    use_query: bool = DeprecatedField(
+        metadata={
+            "deprecation_msg": "Field 'use_query' is deprecated. From now on, default behavior is compatible to use_query=True. "
+            "Please remove this field from your code."
+        }
+    )
 
     def prepare(self):
         if self.to_field is None:
             self.to_field = self.field
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
-        value = dict_get(instance, self.field, use_dpath=self.use_query)
-        index_value = dict_get(instance, self.index, use_dpath=self.use_query)
+        value = dict_get(instance, self.field)
+        index_value = dict_get(instance, self.index)
         instance[self.to_field] = value[index_value]
         return instance
 
 
 class Perturb(FieldOperator):
     """Slightly perturbs the contents of 'field'. Could be Handy for imitating prediction from given target.
 
@@ -939,25 +957,24 @@
 
 
 class CopyFields(FieldOperator):
     """Copies values from specified fields to specified fields.
 
     Args (of parent class):
         field_to_field (Union[List[List], Dict[str, str]]): A list of lists, where each sublist contains the source field and the destination field, or a dictionary mapping source fields to destination fields.
-        use_query (bool): Whether to use dpath for accessing fields. Defaults to False.
 
     Examples:
         An input instance {"a": 2, "b": 3}, when processed by
         CopyField(field_to_field={"a": "b"}
         would yield {"a": 2, "b": 2}, and when processed by
         CopyField(field_to_field={"a": "c"} would yield
         {"a": 2, "b": 3, "c": 2}
 
-        with use_query=True, we can also copy inside the field:
-        CopyFields(field_to_field={"a/0": "a"}, use_query=True)
+        with field names containing / , we can also copy inside the field:
+        CopyFields(field_to_field={"a/0": "a"})
         would process instance {"a": [1, 3]} into {"a": 1}
 
 
     """
 
     def process_value(self, value: Any) -> Any:
         return copy.deepcopy(value)
@@ -1027,25 +1044,24 @@
     def _cast_multiple(self, values, type, field):
         return [self._cast_single(value, type, field) for value in values]
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         for field_name, type in self.fields.items():
-            value = dict_get(instance, field_name, use_dpath=self.use_nested_query)
+            value = dict_get(instance, field_name)
             if self.process_every_value:
                 assert isinstance(
                     value, list
                 ), f"'process_every_value' can be set to True only for fields that contain lists, whereas in instance {instance}, the contents of field '{field_name}' is of type '{type(value)}'"
                 casted_value = self._cast_multiple(value, type, field_name)
             else:
                 casted_value = self._cast_single(value, type, field_name)
-            dict_set(
-                instance, field_name, casted_value, use_dpath=self.use_nested_query
-            )
+
+            dict_set(instance, field_name, casted_value)
         return instance
 
 
 class DivideAllFieldsBy(StreamInstanceOperator):
     """Recursively reach down to all fields that are float, and divide each by 'divisor'.
 
     The given instance is viewed as a tree whose internal nodes are dictionaries and lists, and
@@ -1705,30 +1721,32 @@
         self.encoder = {}
         return super()._process_multi_stream(multi_stream)
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         for field_name in self.fields:
-            values = dict_get(instance, field_name, use_dpath=True)
+            values = dict_get(instance, field_name)
             values_was_a_list = isinstance(values, list)
             if not isinstance(values, list):
                 values = [values]
             for value in values:
                 if value not in self.encoder:
                     self.encoder[value] = len(self.encoder)
             new_values = [self.encoder[value] for value in values]
             if not values_was_a_list:
                 new_values = new_values[0]
             dict_set(
                 instance,
                 field_name,
                 new_values,
-                use_dpath=True,
-                set_multiple="*" in field_name,
+                not_exist_ok=False,  # the values to encode where just taken from there
+                set_multiple="*" in field_name
+                and isinstance(new_values, list)
+                and len(new_values) > 0,
             )
 
         return instance
 
 
 class StreamRefiner(SingleStreamOperator):
     """Discard from the input stream all instances beyond the leading 'max_instances' instances.
@@ -1777,20 +1795,18 @@
         DeterministicBalancer(fields=["a"])
         the resulting stream will be: [{"a": 1, "b": 1},{"a": 2},{"a": 3},{"a": 4}]
     """
 
     fields: List[str]
 
     def signature(self, instance):
-        return str(
-            tuple(dict_get(instance, field, use_dpath=True) for field in self.fields)
-        )
+        return str(tuple(dict_get(instance, field) for field in self.fields))
 
     def process(self, stream: Stream, stream_name: Optional[str] = None) -> Generator:
-        counter = collections.Counter()
+        counter = Counter()
 
         for instance in stream:
             counter[self.signature(instance)] += 1
 
         if len(counter) == 0:
             return
 
@@ -1798,30 +1814,30 @@
 
         max_total_instances_per_sign = lowest_count
         if self.max_instances is not None:
             max_total_instances_per_sign = min(
                 lowest_count, self.max_instances // len(counter)
             )
 
-        counter = collections.Counter()
+        counter = Counter()
 
         for instance in stream:
             sign = self.signature(instance)
             if counter[sign] < max_total_instances_per_sign:
                 counter[sign] += 1
                 yield instance
 
 
 class LengthBalancer(DeterministicBalancer):
     """Balances by a signature that reflects the total length of the fields' values, quantized into integer segments.
 
     Args:
         segments_boundaries (List[int]): distinct integers sorted in increasing order, that maps a given total length
         into the index of the least of them that exceeds the total length. (If none exceeds -- into one index
-        beyond, namely, the length of segments_boudaries)
+        beyond, namely, the length of segments_boundaries)
 
         fields (Optional, List[str])
 
     Example:
         when input [{"a": [1, 3], "b": 0, "id": 0}, {"a": [1, 3], "b": 0, "id": 1}, {"a": [], "b": "a", "id": 2}] is fed into
 
         .. code-block::
@@ -1833,15 +1849,15 @@
 
     segments_boundaries: List[int]
     fields: Optional[List[str]]
 
     def signature(self, instance):
         total_len = 0
         for field_name in self.fields:
-            total_len += len(dict_get(instance, field_name, use_dpath=True))
+            total_len += len(dict_get(instance, field_name))
         for i, val in enumerate(self.segments_boundaries):
             if total_len < val:
                 return i
         return i + 1
 
 
 class DownloadError(Exception):
```

### Comparing `unitxt-1.7.4/src/unitxt/parsing_utils.py` & `unitxt-1.7.6/src/unitxt/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/prepare_utils/card_types.py` & `unitxt-1.7.6/src/unitxt/prepare_utils/card_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List, Optional, Union
 
-from src.unitxt.card import TaskCard
-from src.unitxt.loaders import Loader
-from src.unitxt.operator import StreamingOperator
-from src.unitxt.operators import AddFields, MapInstanceValues, RenameFields
-from src.unitxt.task import FormTask
-from src.unitxt.templates import TemplatesDict, TemplatesList
+from ..card import TaskCard
+from ..loaders import Loader
+from ..operator import StreamingOperator
+from ..operators import AddFields, MapInstanceValues, RenameFields
+from ..task import FormTask
+from ..templates import TemplatesDict, TemplatesList
 
 
 def add_classification_choices(label_name, label2string):
     return [
         MapInstanceValues(mappers={label_name: label2string}),
         AddFields(
             fields={
```

### Comparing `unitxt-1.7.4/src/unitxt/processors.py` & `unitxt-1.7.6/src/unitxt/processors.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/random_utils.py` & `unitxt-1.7.6/src/unitxt/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/register.py` & `unitxt-1.7.6/src/unitxt/register.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/schema.py` & `unitxt-1.7.6/src/unitxt/schema.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/service/metrics/main.py` & `unitxt-1.7.6/src/unitxt/service/metrics/main.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/service/metrics/tokens.py` & `unitxt-1.7.6/src/unitxt/service/metrics/tokens.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/settings_utils.py` & `unitxt-1.7.6/src/unitxt/settings_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         )
     except ModuleNotFoundError:
         constants.default_catalog_path = constants.local_catalog_path
     constants.catalog_dir = constants.local_catalog_path
     constants.dataset_url = "unitxt/data"
     constants.metric_url = "unitxt/metric"
     constants.version = version
-    constants.catalog_hirarchy_sep = "."
+    constants.catalog_hierarchy_sep = "."
     constants.env_local_catalogs_paths_sep = ":"
     constants.non_registered_files = [
         "__init__.py",
         "artifact.py",
         "utils.py",
         "register.py",
         "metric.py",
```

### Comparing `unitxt-1.7.4/src/unitxt/span_lableing_operators.py` & `unitxt-1.7.6/src/unitxt/span_lableing_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/split_utils.py` & `unitxt-1.7.6/src/unitxt/split_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,21 +227,21 @@
     return {mapping.get(key, key): val for key, val in input_streams.items()}
 
 
 def random_mix_generator(
     new_stream_name, new_stream_sources, stream_routing, input_streams
 ):
     for old_stream_name in new_stream_sources:
-        optinal_streams, weights = stream_routing[old_stream_name]
+        optional_streams, weights = stream_routing[old_stream_name]
         random_generator = new_random_generator(sub_seed=old_stream_name)
         assert (
             old_stream_name in input_streams
         ), f"'{old_stream_name}' split not found.  Possibles options: {input_streams.keys()}"
         for item in input_streams[old_stream_name]:
-            choice = random_generator.choices(optinal_streams, weights=weights, k=1)[0]
+            choice = random_generator.choices(optional_streams, weights=weights, k=1)[0]
             if choice == new_stream_name:
                 yield item
 
 
 def random_mix_streams(input_streams, mapping):
     """Creates new streams based on the provided input streams and mapping.
```

### Comparing `unitxt-1.7.4/src/unitxt/splitters.py` & `unitxt-1.7.6/src/unitxt/splitters.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,9 +286,9 @@
                 source_stream, instance
             )
             sampled_instances = self.sampler.sample(source_stream)
             instance[self.target_field] = sampled_instances
             return instance
         except Exception as e:
             raise Exception(
-                f"Unable to fetch instances from '{self.source_stream}' to '{self.target_field}'"
+                f"Unable to fetch instances from '{self.source_stream}' to '{self.target_field}', due to {e.__class__.__name__}: {e}"
             ) from e
```

### Comparing `unitxt-1.7.4/src/unitxt/standard.py` & `unitxt-1.7.6/src/unitxt/standard.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/stream.py` & `unitxt-1.7.6/src/unitxt/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
 
     generator: callable
     gen_kwargs: Dict[str, any] = OptionalField(default_factory=dict)
     caching: bool = False
     copying: bool = False
 
-    def _get_initator(self):
+    def _get_initiator(self):
         """Private method to get the correct initiator based on the streaming and caching attributes.
 
         Returns:
             function: The correct initiator function.
         """
         if self.caching:
             return Dataset.from_generator
@@ -39,15 +39,15 @@
 
     def _get_stream(self):
         """Private method to get the stream based on the initiator function.
 
         Returns:
             object: The stream object.
         """
-        return self._get_initator()(self.generator, gen_kwargs=self.gen_kwargs)
+        return self._get_initiator()(self.generator, gen_kwargs=self.gen_kwargs)
 
     def __iter__(self):
         return iter(self._get_stream())
 
     def peek(self):
         return next(iter(self))
```

### Comparing `unitxt-1.7.4/src/unitxt/struct_data_operators.py` & `unitxt-1.7.6/src/unitxt/struct_data_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,24 +246,23 @@
         with truncating the corresponding answer as well. This has been addressed in the implementation.
 
     """
 
     max_length: int = 15
     table: str = None
     text_output: Optional[str] = None
-    use_query: bool = False
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
-        table = dict_get(instance, self.table, use_dpath=self.use_query)
+        table = dict_get(instance, self.table)
 
         answers = []
         if self.text_output is not None:
-            answers = dict_get(instance, self.text_output, use_dpath=self.use_query)
+            answers = dict_get(instance, self.text_output)
 
         self.truncate_table(table_content=table, answers=answers)
 
         return instance
 
     # truncate table cells
     def truncate_table(self, table_content: Dict, answers: Optional[List]):
@@ -333,15 +332,15 @@
     max_cell_length: Optional[int] = None
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         linearized_str = ""
         for field in self.fields:
-            value = dict_get(instance, field, use_dpath=False)
+            value = dict_get(instance, field)
             if self.max_cell_length is not None:
                 truncated_value = truncate_cell(value, self.max_cell_length)
                 if truncated_value is not None:
                     value = truncated_value
 
             linearized_str = linearized_str + field + " is " + str(value) + ", "
 
@@ -363,15 +362,15 @@
     max_cell_length: Optional[int] = None
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         linearized_str = ""
         for field in self.fields:
-            value = dict_get(instance, field, use_dpath=False)
+            value = dict_get(instance, field)
             if self.max_cell_length is not None:
                 truncated_value = truncate_cell(value, self.max_cell_length)
                 if truncated_value is not None:
                     value = truncated_value
 
             linearized_str = linearized_str + field + ": " + str(value) + ", "
 
@@ -423,21 +422,20 @@
 
     Sample input in expected format: {"keys": ["name", "age", "sex"], "values": ["Alex", 31, "M"]}
     Sample output: {"name": "Alex", "age": 31, "sex": "M"}
     """
 
     fields: List[str]
     to_field: str
-    use_query: bool = False
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
-        keylist = dict_get(instance, self.fields[0], use_dpath=self.use_query)
-        valuelist = dict_get(instance, self.fields[1], use_dpath=self.use_query)
+        keylist = dict_get(instance, self.fields[0])
+        valuelist = dict_get(instance, self.fields[1])
 
         output_dict = {}
         for key, value in zip(keylist, valuelist):
             output_dict[key] = value
 
         instance[self.to_field] = output_dict
```

### Comparing `unitxt-1.7.4/src/unitxt/system_prompts.py` & `unitxt-1.7.6/src/unitxt/system_prompts.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/task.py` & `unitxt-1.7.6/src/unitxt/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     metrics: List[str]
     augmentable_inputs: List[str] = []
 
     def verify(self):
         for augmentable_input in self.augmentable_inputs:
             assert (
                 augmentable_input in self.inputs
-            ), f"augmentable_input f{augmentable_input} is not part of {self.inputs}"
+            ), f"augmentable_input {augmentable_input} is not part of {self.inputs}"
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         try:
             inputs = {key: instance[key] for key in self.inputs}
         except KeyError as e:
```

### Comparing `unitxt-1.7.4/src/unitxt/templates.py` & `unitxt-1.7.6/src/unitxt/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 class MultipleChoiceTemplate(Template):
     """Formats the input (that specifies the question), the multiple choices to select the answer from, and specifies the field with the correct answer."""
 
     input_format: str
     target_prefix: str = ""
     choices_field: str = "choices"
     target_field: str = "label"
-    choices_seperator: str = ", "
+    choices_separator: str = ", "
     source_choice_format: str = "{choice_numeral}. {choice_text}"
     target_choice_format: str = "{choice_numeral}"
     enumerator: str = "capitals"
     shuffle_choices: bool = False
 
     def prepare(self):
         super().prepare()
@@ -213,15 +213,15 @@
     def prepare_multiple_choice_inputs(
         self, inputs: Dict[str, object]
     ) -> Dict[str, object]:
         choices = self.inputs_to_choices(inputs, self.source_choice_format)
         return {
             "numerals": self.inputs_to_numerals(inputs),
             **inputs,
-            self.choices_field: self.choices_seperator.join(choices),
+            self.choices_field: self.choices_separator.join(choices),
         }
 
     def inputs_to_source(self, inputs: Dict[str, object]) -> Tuple[str, str]:
         inputs = self.prepare_multiple_choice_inputs(inputs)
         return self.apply_formatting(
             inputs, "input", self.input_format, "input_format", serialize=True
         )
@@ -354,18 +354,18 @@
 
 class KeyValTemplate(Template):
     """Generate field 'source' from fields designated as input, and fields 'target' and 'references' from fields designated as output, of the processed instance.
 
     Args specify with what separators to glue together the input and output designated fields of the processed instance into one string ('source' and 'target'), and into a list of strings ('references').
     """
 
-    pairs_seperator: str = ", "
-    key_val_seperator: str = ": "
+    pairs_separator: str = ", "
+    key_val_separator: str = ": "
     use_keys_for_inputs: bool = True
-    outputs_key_val_seperator: str = ": "
+    outputs_key_val_separator: str = ": "
     use_keys_for_outputs: bool = False
 
     def process_dict(
         self, data: Dict[str, object], key_val_sep, pairs_sep, use_keys
     ) -> str:
         data = self.serialize_data(data)
         pairs = []
@@ -373,24 +373,24 @@
             key_val = [key, str(val)] if use_keys else [str(val)]
             pairs.append(key_val_sep.join(key_val))
         return pairs_sep.join(pairs)
 
     def inputs_to_source(self, inputs: Dict[str, object]) -> Tuple[str, str]:
         return self.process_dict(
             inputs,
-            key_val_sep=self.key_val_seperator,
-            pairs_sep=self.pairs_seperator,
+            key_val_sep=self.key_val_separator,
+            pairs_sep=self.pairs_separator,
             use_keys=self.use_keys_for_inputs,
         )
 
     def outputs_to_target_and_references(self, outputs: Dict[str, object]) -> str:
         target = self.process_dict(
             outputs,
-            key_val_sep=self.key_val_seperator,
-            pairs_sep=self.pairs_seperator,
+            key_val_sep=self.key_val_separator,
+            pairs_sep=self.pairs_separator,
             use_keys=self.use_keys_for_outputs,
         )
         return target, [target]
 
 
 class OutputQuantizingTemplate(InputOutputTemplate):
     quantum: Union[float, int] = 0.1  # Now supports both int and float
@@ -410,28 +410,28 @@
                 for key, value in outputs.items()
             }
         return super().outputs_to_target_and_references(quantized_outputs)
 
 
 class MultiLabelTemplate(InputOutputTemplate):
     labels_field: str = "labels"
-    labels_seprator: str = ", "
+    labels_separator: str = ", "
     postprocessors: List[str] = ["processors.to_list_by_comma"]
     output_format: str = "{labels}"
     empty_label: str = "None"
 
     def outputs_to_target_and_references(self, outputs: Dict[str, object]) -> str:
         labels = outputs[self.labels_field]
         if not isinstance(labels, list):
             raise ValueError(
                 f"MultiLabelTemplate requires labels field '{self.labels_field}' to be a list. Got {self.labels_field}<{type(labels).__name__}>: {labels}"
             )
         if len(labels) == 0:
             labels = [self.empty_label]
-        labels_str = self.labels_seprator.join(labels)
+        labels_str = self.labels_separator.join(labels)
         return super().outputs_to_target_and_references({self.labels_field: labels_str})
 
 
 class MultiReferenceTemplate(InputOutputTemplate):
     references_field: str = "references"
     random_reference: bool = False
 
@@ -481,16 +481,16 @@
         for span in sorted(spans):
             if self.labels_support is None or span[3] in self.labels_support:
                 yield span[2], span[3]
 
     def outputs_to_target_and_references(
         self, outputs: Dict[str, object]
     ) -> Dict[str, object]:
-        span_lables_pairs = self.extract_span_label_pairs(outputs)
-        targets = self.span_label_pairs_to_targets(span_lables_pairs)
+        span_labels_pairs = self.extract_span_label_pairs(outputs)
+        targets = self.span_label_pairs_to_targets(span_labels_pairs)
         return super().outputs_to_target_and_references({"labels": targets})
 
     @abstractmethod
     def span_label_pairs_to_targets(self, pairs):
         pass
```

### Comparing `unitxt-1.7.4/src/unitxt/test_utils/artifact.py` & `unitxt-1.7.6/src/unitxt/test_utils/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/test_utils/card.py` & `unitxt-1.7.6/src/unitxt/test_utils/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/test_utils/catalog.py` & `unitxt-1.7.6/src/unitxt/test_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/test_utils/metrics.py` & `unitxt-1.7.6/src/unitxt/test_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/test_utils/operators.py` & `unitxt-1.7.6/src/unitxt/test_utils/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/text_utils.py` & `unitxt-1.7.6/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/type_utils.py` & `unitxt-1.7.6/src/unitxt/type_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/ui/__init__.py` & `unitxt-1.7.6/src/unitxt/ui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     from .run import demo
 
     get_settings().global_loader_limit = 300
     demo.launch(debug=True)
 
 
 def launch_without_header(demo_settings=None):
-    new_settings = {"HEADER_VISBLE": False}
+    new_settings = {"HEADER_VISIBLE": False}
     if demo_settings is not None:
         new_settings = {**new_settings, **demo_settings}
     launch(new_settings)
```

### Comparing `unitxt-1.7.4/src/unitxt/ui/banner.png` & `unitxt-1.7.6/src/unitxt/ui/banner.png`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/ui/gradio_utils.py` & `unitxt-1.7.6/src/unitxt/ui/gradio_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/ui/load_catalog_data.py` & `unitxt-1.7.6/src/unitxt/ui/load_catalog_data.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/ui/run.py` & `unitxt-1.7.6/src/unitxt/ui/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     index = index - 1
     try:
         prompts_list, prompt_args = get_prompts(
             dataset, template, num_demos, system_prompt, format, augmentor
         )
         selected_prompt = prompts_list[index]
         prompt_text = selected_prompt[config.PROMPT_SOURCE_STR]
-        prompt_target = selected_prompt[config.PROPT_TARGET_STR]
+        prompt_target = selected_prompt[config.PROMPT_TARGET_STR]
         command = build_command(prompt_args, with_prediction=run_model)
     except Exception as e:
         logger.info("An exception occurred:\n%s", traceback.format_exc())
         prompt_text = f"""
     Oops... this combination didn't work! Try something else.
 
     Exception: {e!r}
@@ -164,15 +164,15 @@
 
 ######################
 ### UI STARTS HERE ###
 ######################
 demo = gr.Blocks()
 
 with demo:
-    if config.HEADER_VISBLE:
+    if config.HEADER_VISIBLE:
         with gr.Row():
             # LOGO
             logo = gr.Image(
                 config.BANNER_PATH,
                 show_label=False,
                 show_download_button=False,
                 show_share_button=False,
@@ -290,15 +290,15 @@
                     code_intro = gr.Markdown(value=config.CODE_INTRO_TXT)
                     code = gr.Code(language="python", lines=1)
                 with gr.TabItem("View Catalog", id="json"):
                     json_intro = gr.Markdown(value=config.JSON_INTRO_TXT)
                     element_name = gr.Text(label="Selected Item:", visible=False)
                     json_viewer = gr.Json(value=None, visible=False)
 
-    if config.HEADER_VISBLE:
+    if config.HEADER_VISIBLE:
         acknowledgement = gr.Markdown(config.ACK_TEXT)
     # INVISIBLE ELEMENTS FOR VALUE STORAGE
     run_model = gr.Checkbox(value=False, visible=False)
     sample_choice = gr.Number(value=0, visible=False)
 
     # DROPDOWNS AND JSON BUTTONS LOGIC
     tasks.select(
```

### Comparing `unitxt-1.7.4/src/unitxt/ui/settings.py` & `unitxt-1.7.6/src/unitxt/ui/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "catalog",
 )
 BANNER_PATH = os.path.join(os.path.dirname(os.path.abspath(__file__)), "banner.png")
 AUGMENTABLE_STR = "augmentable_inputs"
 LOADER_LIMIT_STR = "loader_limit"
 PROMPT_SOURCE_STR = "source"
 PROMPT_METRICS_STR = "metrics"
-PROPT_TARGET_STR = "target"
+PROMPT_TARGET_STR = "target"
 DEMOS_POOL_SIZE = 10
 PROMPT_SAMPLE_SIZE = 5
 MAX_NEW_TOKENS = 30
 FLAN_T5_BASE = "flan-t5-base"
 GPT2 = "gpt2"
 EMPTY_SCORES_FRAME = list({"": ""}.items())
 SCORE_FRAME_HEADERS = ["Score Name", "Score"]
@@ -26,15 +26,15 @@
 model = pipeline(model="google/{FLAN_T5_BASE}")
 predictions = [output["generated_text"] for output in model(dataset["{PROMPT_SOURCE_STR}"],max_new_tokens={MAX_NEW_TOKENS})]
 metric = evaluate.load("{UNITEXT_METRIC_STR}")
 scores = metric.compute(predictions=predictions,references=dataset)
 
 [print(item) for item in scores[0]['score']['global'].items()]
 """
-HEADER_VISBLE = True
+HEADER_VISIBLE = True
 INTRO_TXT = """
 # Data Preparation and Evaluation for Generative AI
 
 ## Flexible, Shareable and Reusable
 
 [![unitxt](https://badgen.net/badge/icon/GitHub?icon=github&label)](https://github.com/IBM/unitxt)
 """
```

### Comparing `unitxt-1.7.4/src/unitxt/ui/ui_tester.py` & `unitxt-1.7.6/src/unitxt/ui/ui_tester.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/ui/ui_utils.py` & `unitxt-1.7.6/src/unitxt/ui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.4/src/unitxt/utils.py` & `unitxt-1.7.6/src/unitxt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,13 +103,13 @@
         ValueError: If the expression contains tokens not in the allowed list or context keys.
 
     Note:
         This function should be used carefully, as it employs `eval`, which can
         execute arbitrary code. The function attempts to mitigate security risks
         by restricting the available tokens and not exposing built-in functions.
     """
-    allowd_sub_strings = list(context.keys()) + allowed_tokens
-    if is_made_of_sub_strings(expression, allowd_sub_strings):
+    allowed_sub_strings = list(context.keys()) + allowed_tokens
+    if is_made_of_sub_strings(expression, allowed_sub_strings):
         return eval(expression, {"__builtins__": {}}, context)
     raise ValueError(
-        f"The expression '{expression}' can not be evaluated because it contains tokens outside the allowed list of {allowd_sub_strings}."
+        f"The expression '{expression}' can not be evaluated because it contains tokens outside the allowed list of {allowed_sub_strings}."
     )
```

### Comparing `unitxt-1.7.4/src/unitxt/validate.py` & `unitxt-1.7.6/src/unitxt/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def verify(self):
         assert isinstance(
             self.schema, Features
         ), "Schema must be an instance of Features"
         assert self.schema is not None, "Schema must be specified"
 
     def verify_first_instance(self, instance):
-        for std_field in self.standart_fields:
+        for std_field in self.standard_fields:
             assert (
                 std_field in instance
             ), f'Field "{std_field}" is missing in the first instance'
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
@@ -43,9 +43,9 @@
                 "parser": Value("string"),
                 # 'group': Value('string'),
                 # 'guidance': Value('string'),
             }
         )
 
 
-class ValidateStandartSchema:
+class ValidateStandardSchema:
     schema: Features = field(default_factory=StandardSchema)
```

### Comparing `unitxt-1.7.4/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.7.6/src/unitxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,52 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.7.4
+Version: 1.7.6
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasets>=2.16.0
 Requires-Dist: evaluate
 Requires-Dist: absl-py
 Requires-Dist: ipadic
 Requires-Dist: scipy
+Provides-Extra: service
+Requires-Dist: torch==1.12.1; extra == "service"
+Requires-Dist: fastapi==0.109.0; extra == "service"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
+Requires-Dist: transformers; extra == "service"
 Provides-Extra: base
 Requires-Dist: datasets>=2.16.0; extra == "base"
 Requires-Dist: evaluate; extra == "base"
 Requires-Dist: absl-py; extra == "base"
 Requires-Dist: ipadic; extra == "base"
 Requires-Dist: scipy; extra == "base"
+Provides-Extra: docs
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: piccolo_theme; extra == "docs"
+Requires-Dist: sphinxext-opengraph; extra == "docs"
+Requires-Dist: datasets; extra == "docs"
+Requires-Dist: evaluate; extra == "docs"
+Requires-Dist: nltk; extra == "docs"
+Requires-Dist: sacrebleu; extra == "docs"
+Requires-Dist: absl-py; extra == "docs"
+Requires-Dist: rouge_score; extra == "docs"
+Requires-Dist: scikit-learn; extra == "docs"
+Requires-Dist: jiwer; extra == "docs"
+Requires-Dist: editdistance; extra == "docs"
+Provides-Extra: ui
+Requires-Dist: gradio; extra == "ui"
+Requires-Dist: transformers; extra == "ui"
 Provides-Extra: tests
 Requires-Dist: bert_score; extra == "tests"
 Requires-Dist: transformers; extra == "tests"
 Requires-Dist: sentence_transformers; extra == "tests"
 Requires-Dist: ibm-cos-sdk; extra == "tests"
 Requires-Dist: opendatasets; extra == "tests"
 Requires-Dist: httpretty~=1.1.4; extra == "tests"
@@ -34,90 +56,70 @@
 Requires-Dist: mecab-python3; extra == "tests"
 Requires-Dist: sacrebleu[ko]; extra == "tests"
 Requires-Dist: scikit-learn; extra == "tests"
 Requires-Dist: jiwer; extra == "tests"
 Requires-Dist: conllu; extra == "tests"
 Requires-Dist: llama-index-core; extra == "tests"
 Requires-Dist: llama-index-llms-openai; extra == "tests"
-Provides-Extra: docs
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: piccolo_theme; extra == "docs"
-Requires-Dist: sphinxext-opengraph; extra == "docs"
-Requires-Dist: datasets; extra == "docs"
-Requires-Dist: evaluate; extra == "docs"
-Requires-Dist: nltk; extra == "docs"
-Requires-Dist: sacrebleu; extra == "docs"
-Requires-Dist: absl-py; extra == "docs"
-Requires-Dist: rouge_score; extra == "docs"
-Requires-Dist: scikit-learn; extra == "docs"
-Requires-Dist: jiwer; extra == "docs"
-Requires-Dist: editdistance; extra == "docs"
+Requires-Dist: pytrec-eval; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
-Provides-Extra: service
-Requires-Dist: torch==1.12.1; extra == "service"
-Requires-Dist: fastapi==0.109.0; extra == "service"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
-Requires-Dist: transformers; extra == "service"
-Provides-Extra: ui
-Requires-Dist: gradio; extra == "ui"
-Requires-Dist: transformers; extra == "ui"
 Provides-Extra: all
-Requires-Dist: absl-py; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
-Requires-Dist: jiwer; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: datasets; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: gradio; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: bert_score; extra == "all"
-Requires-Dist: ibm-cos-sdk; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
 Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: transformers; extra == "all"
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: evaluate; extra == "all"
-Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: nltk; extra == "all"
+Requires-Dist: codespell; extra == "all"
 Requires-Dist: llama-index-core; extra == "all"
-Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
 Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: rouge-score; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: evaluate; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
+Requires-Dist: ibm-cos-sdk; extra == "all"
 Requires-Dist: mecab-python3; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: nltk; extra == "all"
-Requires-Dist: datasets>=2.16.0; extra == "all"
 Requires-Dist: ipadic; extra == "all"
-Requires-Dist: datasets; extra == "all"
-Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: fastapi==0.109.0; extra == "all"
-Requires-Dist: rouge-score; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: gradio; extra == "all"
+Requires-Dist: jiwer; extra == "all"
 Requires-Dist: conllu; extra == "all"
-Requires-Dist: editdistance; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: scipy; extra == "all"
 Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
 Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: codespell; extra == "all"
+Requires-Dist: sacrebleu; extra == "all"
+Requires-Dist: editdistance; extra == "all"
+Requires-Dist: httpretty~=1.1.4; extra == "all"
+Requires-Dist: transformers; extra == "all"
+Requires-Dist: datasets>=2.16.0; extra == "all"
+Requires-Dist: tomli; extra == "all"
 Requires-Dist: torch==1.12.1; extra == "all"
+Requires-Dist: absl-py; extra == "all"
+Requires-Dist: bert_score; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
 [![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/adding_dataset.html)
 [![Button](https://img.shields.io/badge/Paper-pink?style=for-the-badge)](https://arxiv.org/abs/2401.14019)
 [![Button](https://img.shields.io/badge/Documentation-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/modules.html)
 [![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog.html)
-[![Button](https://img.shields.io/badge/Contributers-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
+[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
 [![Button](https://img.shields.io/badge/PyPi-pink?style=for-the-badge)](https://pypi.org/project/unitxt/)
 
 
 In the dynamic landscape of generative NLP, traditional text processing pipelines limit research flexibility and reproducibility, as they are tailored to specific dataset, task, and model combinations. The escalating complexity, involving system prompts, model-specific formats, instructions, and more, calls for a shift to a structured, modular, and customizable solution.
 
  Addressing this need, we present Unitxt, an innovative library for customizable textual data preparation and evaluation tailored to generative language models. Unitxt natively integrates with common libraries like HuggingFace and LM-eval-harness and deconstructs processing flows into modular components, enabling easy customization and sharing between practitioners. These components encompass model-specific formats, task prompts, and many other comprehensive dataset processing definitions. The Unitxt-Catalog centralizes these components, fostering collaboration and exploration in modern textual data workflows. Beyond being a tool, Unitxt is a community-driven platform, empowering users to build, share, and advance their pipelines collaboratively.
 
@@ -132,19 +134,19 @@
 
 #
 
 https://github.com/IBM/unitxt/assets/23455264/baef9131-39d4-4164-90b2-05da52919fdf
 
 ### 🦄 Currently on Unitxt Catalog
 
-![NLP Tasks](https://img.shields.io/badge/NLP_tasks-22-blue)
-![Dataset Cards](https://img.shields.io/badge/Dataset_Cards-423-blue)
-![Templates](https://img.shields.io/badge/Templates-204-blue)
-![Formats](https://img.shields.io/badge/Formats-13-blue)
-![Metrics](https://img.shields.io/badge/Metrics-79-blue)
+![NLP Tasks](https://img.shields.io/badge/NLP_tasks-29-blue)
+![Dataset Cards](https://img.shields.io/badge/Dataset_Cards-435-blue)
+![Templates](https://img.shields.io/badge/Templates-218-blue)
+![Formats](https://img.shields.io/badge/Formats-15-blue)
+![Metrics](https://img.shields.io/badge/Metrics-84-blue)
 
 ### 🦄 Run Unitxt Exploration Dashboard
 
 To launch unitxt graphical user interface first install unitxt with ui requirements:
 ```
 pip install unitxt[ui]
 ```
```

### Comparing `unitxt-1.7.4/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.7.6/src/unitxt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -71,22 +71,24 @@
 src/unitxt/catalog/cards/argument_topic.json
 src/unitxt/catalog/cards/atis.json
 src/unitxt/catalog/cards/atta_q.json
 src/unitxt/catalog/cards/banking77.json
 src/unitxt/catalog/cards/bold.json
 src/unitxt/catalog/cards/claim_stance_topic.json
 src/unitxt/catalog/cards/cnn_dailymail.json
+src/unitxt/catalog/cards/coedit_error_detection.json
 src/unitxt/catalog/cards/coedit_gec.json
 src/unitxt/catalog/cards/cola.json
 src/unitxt/catalog/cards/copa.json
 src/unitxt/catalog/cards/dart.json
 src/unitxt/catalog/cards/dbpedia_14.json
 src/unitxt/catalog/cards/ethos_binary.json
 src/unitxt/catalog/cards/financial_tweets.json
 src/unitxt/catalog/cards/hellaswag.json
+src/unitxt/catalog/cards/hh_rlhf.json
 src/unitxt/catalog/cards/human_eval.json
 src/unitxt/catalog/cards/law_stack_exchange.json
 src/unitxt/catalog/cards/ledgar.json
 src/unitxt/catalog/cards/mbpp.json
 src/unitxt/catalog/cards/medical_abstracts.json
 src/unitxt/catalog/cards/mnli.json
 src/unitxt/catalog/cards/mrpc.json
@@ -100,14 +102,15 @@
 src/unitxt/catalog/cards/race_high.json
 src/unitxt/catalog/cards/race_middle.json
 src/unitxt/catalog/cards/rte.json
 src/unitxt/catalog/cards/sciq.json
 src/unitxt/catalog/cards/squad.json
 src/unitxt/catalog/cards/sst2.json
 src/unitxt/catalog/cards/stsb.json
+src/unitxt/catalog/cards/summarize_from_human_feedback.json
 src/unitxt/catalog/cards/tab_fact.json
 src/unitxt/catalog/cards/tablerow_classify.json
 src/unitxt/catalog/cards/toxigen.json
 src/unitxt/catalog/cards/trec.json
 src/unitxt/catalog/cards/unfair_tos.json
 src/unitxt/catalog/cards/wiki_bio.json
 src/unitxt/catalog/cards/wikitq.json
@@ -306,14 +309,18 @@
 src/unitxt/catalog/cards/belebele/zsm_latn.json
 src/unitxt/catalog/cards/belebele/zul_latn.json
 src/unitxt/catalog/cards/boolq/classification.json
 src/unitxt/catalog/cards/boolq/multiple_choice.json
 src/unitxt/catalog/cards/clinc_oos/imbalanced.json
 src/unitxt/catalog/cards/clinc_oos/plus.json
 src/unitxt/catalog/cards/clinc_oos/small.json
+src/unitxt/catalog/cards/coedit/paraphrase.json
+src/unitxt/catalog/cards/coedit/preference.json
+src/unitxt/catalog/cards/coedit/rewriting.json
+src/unitxt/catalog/cards/coedit/selection.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
 src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
@@ -500,22 +507,23 @@
 src/unitxt/catalog/formats/llama2.json
 src/unitxt/catalog/formats/textual_assistant.json
 src/unitxt/catalog/formats/user_agent.json
 src/unitxt/catalog/formats/user_assistant.json
 src/unitxt/catalog/formats/models/alpaca_instruct.json
 src/unitxt/catalog/formats/models/flan/exq_exa.json
 src/unitxt/catalog/formats/models/flan/few_shot.json
-src/unitxt/catalog/formats/models/labrador/few_shot.json
-src/unitxt/catalog/formats/models/labrador/zero_shot.json
+src/unitxt/catalog/formats/models/labradorite/few_shot.json
+src/unitxt/catalog/formats/models/labradorite/zero_shot.json
 src/unitxt/catalog/formats/models/mistral/instruction.json
 src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
 src/unitxt/catalog/metrics/accuracy.json
 src/unitxt/catalog/metrics/accuracy_binary.json
 src/unitxt/catalog/metrics/bleu.json
 src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
+src/unitxt/catalog/metrics/char_edit_distance.json
 src/unitxt/catalog/metrics/f1_binary.json
 src/unitxt/catalog/metrics/f1_macro.json
 src/unitxt/catalog/metrics/f1_macro_multi_label.json
 src/unitxt/catalog/metrics/f1_micro.json
 src/unitxt/catalog/metrics/f1_micro_multi_label.json
 src/unitxt/catalog/metrics/f1_weighted.json
 src/unitxt/catalog/metrics/kendalltau_b.json
@@ -531,27 +539,30 @@
 src/unitxt/catalog/metrics/precision_binary.json
 src/unitxt/catalog/metrics/precision_macro_multi_label.json
 src/unitxt/catalog/metrics/precision_micro_multi_label.json
 src/unitxt/catalog/metrics/recall_binary.json
 src/unitxt/catalog/metrics/recall_macro_multi_label.json
 src/unitxt/catalog/metrics/recall_micro_multi_label.json
 src/unitxt/catalog/metrics/regard.json
+src/unitxt/catalog/metrics/rerank_recall.json
 src/unitxt/catalog/metrics/retrieval_at_k.json
 src/unitxt/catalog/metrics/roc_auc.json
 src/unitxt/catalog/metrics/rouge.json
 src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
 src/unitxt/catalog/metrics/sacrebleu.json
 src/unitxt/catalog/metrics/safety.json
 src/unitxt/catalog/metrics/spearman.json
 src/unitxt/catalog/metrics/squad.json
 src/unitxt/catalog/metrics/string_containment.json
 src/unitxt/catalog/metrics/token_overlap.json
 src/unitxt/catalog/metrics/token_overlap_with_context.json
 src/unitxt/catalog/metrics/unsorted_list_exact_match.json
 src/unitxt/catalog/metrics/wer.json
+src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
+src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
 src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
 src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
 src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
 src/unitxt/catalog/metrics/rag/answer_correctness.json
@@ -563,14 +574,15 @@
 src/unitxt/catalog/metrics/rag/context_relevance.json
 src/unitxt/catalog/metrics/rag/faithfulness.json
 src/unitxt/catalog/metrics/rag/k_precision.json
 src/unitxt/catalog/metrics/rag/map.json
 src/unitxt/catalog/metrics/rag/mrr.json
 src/unitxt/catalog/metrics/rag/recall.json
 src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
+src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
 src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
 src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
@@ -625,37 +637,41 @@
 src/unitxt/catalog/splitters/large_no_test.json
 src/unitxt/catalog/splitters/small_no_dev.json
 src/unitxt/catalog/splitters/small_no_test.json
 src/unitxt/catalog/splitters/test_only.json
 src/unitxt/catalog/system_prompt/models/japanese_llama.json
 src/unitxt/catalog/system_prompts/empty.json
 src/unitxt/catalog/system_prompts/models/alpaca.json
-src/unitxt/catalog/system_prompts/models/labrador.json
+src/unitxt/catalog/system_prompts/models/labradorite.json
 src/unitxt/catalog/system_prompts/models/llama.json
 src/unitxt/catalog/system_prompts/models/llama2.json
 src/unitxt/catalog/tasks/generation.json
 src/unitxt/catalog/tasks/grammatical_error_correction.json
 src/unitxt/catalog/tasks/classification/binary.json
 src/unitxt/catalog/tasks/classification/multi_class.json
 src/unitxt/catalog/tasks/classification/multi_label.json
 src/unitxt/catalog/tasks/classification/multi_class/relation.json
 src/unitxt/catalog/tasks/completion/abstractive.json
 src/unitxt/catalog/tasks/completion/extractive.json
 src/unitxt/catalog/tasks/completion/multiple_choice.json
+src/unitxt/catalog/tasks/evaluation/preference.json
 src/unitxt/catalog/tasks/ner/all_entity_types.json
 src/unitxt/catalog/tasks/ner/single_entity_type.json
 src/unitxt/catalog/tasks/qa/open.json
 src/unitxt/catalog/tasks/qa/multiple_choice/open.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
 src/unitxt/catalog/tasks/qa/with_context/abstractive.json
 src/unitxt/catalog/tasks/qa/with_context/extractive.json
 src/unitxt/catalog/tasks/regression/single_text.json
 src/unitxt/catalog/tasks/regression/two_texts.json
+src/unitxt/catalog/tasks/rewriting/by_attribute.json
+src/unitxt/catalog/tasks/rewriting/paraphrase.json
+src/unitxt/catalog/tasks/selection/by_attribute.json
 src/unitxt/catalog/tasks/span_labeling/extraction.json
 src/unitxt/catalog/tasks/summarization/abstractive.json
 src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
 src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
 src/unitxt/catalog/tasks/translation/directed.json
 src/unitxt/catalog/templates/empty.json
 src/unitxt/catalog/templates/key_val.json
@@ -685,17 +701,22 @@
 src/unitxt/catalog/templates/completion/abstractive/empty.json
 src/unitxt/catalog/templates/completion/abstractive/standard.json
 src/unitxt/catalog/templates/completion/multiple_choice/all.json
 src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
 src/unitxt/catalog/templates/completion/multiple_choice/simple.json
 src/unitxt/catalog/templates/completion/multiple_choice/standard.json
 src/unitxt/catalog/templates/completion/multiple_choice/title.json
+src/unitxt/catalog/templates/evaluation/preference/all.json
+src/unitxt/catalog/templates/evaluation/preference/default.json
 src/unitxt/catalog/templates/generation/all.json
 src/unitxt/catalog/templates/generation/default.json
+src/unitxt/catalog/templates/grammatical_error_correction/all.json
 src/unitxt/catalog/templates/grammatical_error_correction/simple.json
+src/unitxt/catalog/templates/grammatical_error_detection/all.json
+src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
 src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
 src/unitxt/catalog/templates/qa/multiple_choice/match.json
 src/unitxt/catalog/templates/qa/multiple_choice/title.json
 src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
 src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
 src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
 src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
@@ -816,14 +837,20 @@
 src/unitxt/catalog/templates/regression/single_text/all.json
 src/unitxt/catalog/templates/regression/single_text/simple.json
 src/unitxt/catalog/templates/regression/single_text/title.json
 src/unitxt/catalog/templates/regression/two_texts/all.json
 src/unitxt/catalog/templates/regression/two_texts/simple.json
 src/unitxt/catalog/templates/regression/two_texts/title.json
 src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
+src/unitxt/catalog/templates/rewriting/by_attribute/all.json
+src/unitxt/catalog/templates/rewriting/by_attribute/default.json
+src/unitxt/catalog/templates/rewriting/paraphrase/all.json
+src/unitxt/catalog/templates/rewriting/paraphrase/default.json
+src/unitxt/catalog/templates/selection/by_attribute/all.json
+src/unitxt/catalog/templates/selection/by_attribute/default.json
 src/unitxt/catalog/templates/span_labeling/extraction/all.json
 src/unitxt/catalog/templates/span_labeling/extraction/carry.json
 src/unitxt/catalog/templates/span_labeling/extraction/empty.json
 src/unitxt/catalog/templates/span_labeling/extraction/extract.json
 src/unitxt/catalog/templates/span_labeling/extraction/having.json
 src/unitxt/catalog/templates/span_labeling/extraction/identify.json
 src/unitxt/catalog/templates/span_labeling/extraction/title.json
```

### Comparing `unitxt-1.7.4/src/unitxt.egg-info/requires.txt` & `unitxt-1.7.6/src/unitxt.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
 
 [all]
-absl-py
-llama-index-llms-openai
-jiwer
+fastapi==0.109.0
+sphinxext-opengraph
+datasets
+ruff
+gradio
 sphinx_rtd_theme
-bert_score
-ibm-cos-sdk
-opendatasets
-pre-commit
 python-jose[cryptography]==3.3.0
-transformers
-tomli
-evaluate
-sphinxext-opengraph
+sentence_transformers
+nltk
+codespell
 llama-index-core
-httpretty~=1.1.4
-sacrebleu[ko]
 rouge_score
+rouge-score
+pytrec-eval
+evaluate
+opendatasets
+ibm-cos-sdk
 mecab-python3
-ruff
-sentence_transformers
-scipy
-nltk
-datasets>=2.16.0
 ipadic
-datasets
-sacrebleu
-fastapi==0.109.0
-rouge-score
-scikit-learn
-gradio
+jiwer
 conllu
-editdistance
+llama-index-llms-openai
+scikit-learn
+pre-commit
+scipy
 uvicorn[standard]==0.27.0.post1
+sacrebleu[ko]
 piccolo_theme
-codespell
+sacrebleu
+editdistance
+httpretty~=1.1.4
+transformers
+datasets>=2.16.0
+tomli
 torch==1.12.1
+absl-py
+bert_score
 
 [base]
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
@@ -89,11 +90,12 @@
 mecab-python3
 sacrebleu[ko]
 scikit-learn
 jiwer
 conllu
 llama-index-core
 llama-index-llms-openai
+pytrec-eval
 
 [ui]
 gradio
 transformers
```

