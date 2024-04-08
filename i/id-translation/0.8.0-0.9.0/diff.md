# Comparing `tmp/id_translation-0.8.0.tar.gz` & `tmp/id_translation-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_translation-0.8.0.tar", max compression
+gzip compressed data, was "id_translation-0.9.0.tar", max compression
```

## Comparing `id_translation-0.8.0.tar` & `id_translation-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     1077 2024-03-23 15:35:42.593447 id_translation-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     5120 2024-03-23 15:35:42.597447 id_translation-0.8.0/README.md
--rw-r--r--   0        0        0     4774 2024-03-23 15:35:42.605447 id_translation-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      566 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/__init__.py
--rw-r--r--   0        0        0      192 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_tasks/__init__.py
--rw-r--r--   0        0        0     1477 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_tasks/_base_task.py
--rw-r--r--   0        0        0     6177 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_tasks/_map.py
--rw-r--r--   0        0        0     5768 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_tasks/_names.py
--rw-r--r--   0        0        0    11220 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_tasks/_translate.py
--rw-r--r--   0        0        0    50715 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_translator.py
--rw-r--r--   0        0        0     1091 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/_uuid_utils.py
--rw-r--r--   0        0        0      263 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/__init__.py
--rw-r--r--   0        0        0     2036 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_data_structure_io.py
--rw-r--r--   0        0        0     1644 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_dict.py
--rw-r--r--   0        0        0     6201 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_pandas.py
--rw-r--r--   0        0        0     2027 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_resolve.py
--rw-r--r--   0        0        0     2558 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_sequence.py
--rw-r--r--   0        0        0     1088 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_set.py
--rw-r--r--   0        0        0     1037 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/_single_value.py
--rw-r--r--   0        0        0      761 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/dio/exceptions.py
--rw-r--r--   0        0        0      902 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/exceptions.py
--rw-r--r--   0        0        0    13150 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/factory.py
--rw-r--r--   0        0        0     1265 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/__init__.py
--rw-r--r--   0        0        0    27240 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_abstract_fetcher.py
--rw-r--r--   0        0        0     7441 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_cache.py
--rw-r--r--   0        0        0     4039 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_fetcher.py
--rw-r--r--   0        0        0     2427 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_memory_fetcher.py
--rw-r--r--   0        0        0    18000 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_multi_fetcher.py
--rw-r--r--   0        0        0     6386 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_pandas_fetcher.py
--rw-r--r--   0        0        0    19864 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/_sql_fetcher.py
--rw-r--r--   0        0        0     2203 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/exceptions.py
--rw-r--r--   0        0        0     1338 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/fetching/types.py
--rw-r--r--   0        0        0      602 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/__init__.py
--rw-r--r--   0        0        0     5687 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/_cardinality.py
--rw-r--r--   0        0        0     8008 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/_directional_mapping.py
--rw-r--r--   0        0        0     8015 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/_heuristic_score.py
--rw-r--r--   0        0        0    22292 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/_mapper.py
--rw-r--r--   0        0        0     2736 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/exceptions.py
--rw-r--r--   0        0        0     6244 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/filter_functions.py
--rw-r--r--   0        0        0    15230 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/heuristic_functions.py
--rw-r--r--   0        0        0     3372 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/score_functions.py
--rw-r--r--   0        0        0    13655 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/support.py
--rw-r--r--   0        0        0     2920 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/mapping/types.py
--rw-r--r--   0        0        0      288 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/__init__.py
--rw-r--r--   0        0        0     5480 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/_format.py
--rw-r--r--   0        0        0     5302 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/_format_applier.py
--rw-r--r--   0        0        0     5343 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/_magic_dict.py
--rw-r--r--   0        0        0    10454 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/_translation_map.py
--rw-r--r--   0        0        0     8133 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/parse_format_string.py
--rw-r--r--   0        0        0     3980 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/offline/types.py
--rw-r--r--   0        0        0        0 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/py.typed
--rw-r--r--   0        0        0     2417 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/settings.py
--rw-r--r--   0        0        0     3946 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/testing.py
--rw-r--r--   0        0        0      148 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/transform/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 15:35:42.605447 id_translation-0.8.0/src/id_translation/transform/_impl/__init__.py
--rw-r--r--   0        0        0     5875 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/transform/_impl/bitmask.py
--rw-r--r--   0        0        0     2136 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/transform/types.py
--rw-r--r--   0        0        0     2586 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/translator_typing.py
--rw-r--r--   0        0        0     5105 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/types.py
--rw-r--r--   0        0        0      250 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/utils/__init__.py
--rw-r--r--   0        0        0     4096 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/utils/_base_metadata.py
--rw-r--r--   0        0        0     3977 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/utils/_config_utils.py
--rw-r--r--   0        0        0     1389 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/utils/_load_toml.py
--rw-r--r--   0        0        0      594 2024-03-23 15:35:42.609447 id_translation-0.8.0/src/id_translation/utils/logging.py
--rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 id_translation-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-28 01:40:01.655576 id_translation-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     5435 2024-03-28 01:40:01.655576 id_translation-0.9.0/README.md
+-rw-r--r--   0        0        0     4774 2024-03-28 01:40:01.663576 id_translation-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      566 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/__init__.py
+-rw-r--r--   0        0        0      192 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_tasks/__init__.py
+-rw-r--r--   0        0        0     1477 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_tasks/_base_task.py
+-rw-r--r--   0        0        0     6177 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_tasks/_map.py
+-rw-r--r--   0        0        0     5768 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_tasks/_names.py
+-rw-r--r--   0        0        0    10767 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_tasks/_translate.py
+-rw-r--r--   0        0        0    54406 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_translator.py
+-rw-r--r--   0        0        0     1044 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/_uuid_utils.py
+-rw-r--r--   0        0        0      263 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/__init__.py
+-rw-r--r--   0        0        0     2036 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_data_structure_io.py
+-rw-r--r--   0        0        0     1644 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_dict.py
+-rw-r--r--   0        0        0     6193 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_pandas.py
+-rw-r--r--   0        0        0     2027 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_resolve.py
+-rw-r--r--   0        0        0     2571 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_sequence.py
+-rw-r--r--   0        0        0     1077 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_set.py
+-rw-r--r--   0        0        0     1037 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/_single_value.py
+-rw-r--r--   0        0        0      761 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/dio/exceptions.py
+-rw-r--r--   0        0        0      902 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/exceptions.py
+-rw-r--r--   0        0        0    13150 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/factory.py
+-rw-r--r--   0        0        0     1265 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/__init__.py
+-rw-r--r--   0        0        0    27240 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_abstract_fetcher.py
+-rw-r--r--   0        0        0     7441 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_cache.py
+-rw-r--r--   0        0        0     4039 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_fetcher.py
+-rw-r--r--   0        0        0     2427 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_memory_fetcher.py
+-rw-r--r--   0        0        0    18000 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_multi_fetcher.py
+-rw-r--r--   0        0        0     6386 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_pandas_fetcher.py
+-rw-r--r--   0        0        0    19864 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/_sql_fetcher.py
+-rw-r--r--   0        0        0     2203 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/exceptions.py
+-rw-r--r--   0        0        0     1338 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/fetching/types.py
+-rw-r--r--   0        0        0      602 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/__init__.py
+-rw-r--r--   0        0        0     5687 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/_cardinality.py
+-rw-r--r--   0        0        0     8008 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/_directional_mapping.py
+-rw-r--r--   0        0        0     8015 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/_heuristic_score.py
+-rw-r--r--   0        0        0    22292 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/_mapper.py
+-rw-r--r--   0        0        0     2736 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/exceptions.py
+-rw-r--r--   0        0        0     6244 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/filter_functions.py
+-rw-r--r--   0        0        0    15230 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/heuristic_functions.py
+-rw-r--r--   0        0        0     3372 2024-03-28 01:40:01.663576 id_translation-0.9.0/src/id_translation/mapping/score_functions.py
+-rw-r--r--   0        0        0    13655 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/mapping/support.py
+-rw-r--r--   0        0        0     2920 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/mapping/types.py
+-rw-r--r--   0        0        0      288 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/__init__.py
+-rw-r--r--   0        0        0     6948 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/_format.py
+-rw-r--r--   0        0        0     5078 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/_format_applier.py
+-rw-r--r--   0        0        0     7303 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/_magic_dict.py
+-rw-r--r--   0        0        0    10600 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/_translation_map.py
+-rw-r--r--   0        0        0    10418 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/parse_format_string.py
+-rw-r--r--   0        0        0     3980 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/offline/types.py
+-rw-r--r--   0        0        0        0 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/py.typed
+-rw-r--r--   0        0        0     2417 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/settings.py
+-rw-r--r--   0        0        0     3946 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/testing.py
+-rw-r--r--   0        0        0      148 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/transform/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/transform/_impl/__init__.py
+-rw-r--r--   0        0        0     5875 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/transform/_impl/bitmask.py
+-rw-r--r--   0        0        0     2136 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/transform/types.py
+-rw-r--r--   0        0        0     4967 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/translator_typing.py
+-rw-r--r--   0        0        0     4835 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/types.py
+-rw-r--r--   0        0        0      250 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/utils/__init__.py
+-rw-r--r--   0        0        0     4096 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/utils/_base_metadata.py
+-rw-r--r--   0        0        0     3977 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/utils/_config_utils.py
+-rw-r--r--   0        0        0     1389 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/utils/_load_toml.py
+-rw-r--r--   0        0        0      594 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/utils/logging.py
+-rw-r--r--   0        0        0    18356 2024-03-28 01:40:01.667576 id_translation-0.9.0/src/id_translation/utils/translation_helper.py
+-rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 id_translation-0.9.0/PKG-INFO
```

### Comparing `id_translation-0.8.0/LICENSE.md` & `id_translation-0.9.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2022, Richard Sundqvist
+Copyright (c) 2024, Richard Sundqvist
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `id_translation-0.8.0/README.md` & `id_translation-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ## What is it?
 A package suite for translating integer IDs typically found in databases. Translation is highly configurable and tested
 for multiple different SQL dialects and schema naming paradigms. The included TOML configuration format as well as the
 support functions make it easy to create and share working configurations with anyone who needs them.
 
 # Cookiecutter template project
-The fastest way to get started with `id-translation` is the 🍪[id-translation-project] cookiecutter template. It is
+The fastest way to get started with `id-translation` is the 🍪[id-translation-project] Cookiecutter template. It is
 designed to allow power users to quickly specify shared configurations that "just work" for other users; see the example
 below.
 
 ```python
 from big_corporation_inc.id_translation import translate
 print(
   "The first employee at Big Corporation Inc. was:", 
@@ -42,31 +42,37 @@
 Check out this [demo project](https://github.com/rsundqvist/id-translation-project/tree/master/demo/bci-id-translation)
 (and its 📚[generated documentation](https://rsundqvist.github.io/id-translation-project/)) to get a preview of what 
 Your generated project might look like, or continue to the next section for a brief feature overview.
 
 [id-translation-project]: https://github.com/rsundqvist/id-translation-project/
 
 # Highlighted Features
-- Support for ``int`` and ``string`` IDs, including ``UUID``-like types.
-- Translation of [pandas types][pandas-translation], including `pandas.Index` types.
-- Intuitive [Format strings][format], with support for optional elements.
-- Powerful automated [Name-to-source][n2s-mapping] and [Format placeholder][pm-mapping] mapping.
-- Prebuilt fetchers for [SQL][sql-fetcher] and [file-system][pandas-fetcher] sources.
-- Configure using [TOML][translator-config], support for [persistent] instances stored on disk.
+- Intuitive [Format strings] (modern `'{id}:{name}'` syntax), including support for
+  [Format Specification Mini-Language] features and extensions for optional keys.
+- Fetchers for [SQL] and local or remote [file-system] sources.
+- Powerful [Name-to-source] and [Placeholder-to-column] mapping and name extraction.
+- Configurable using [TOML] - see the 🍪[id-translation-project] Cookiecutter template.
+- Highly configurable interface: [Translator.translate()].
+
+[Format strings]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.offline.html#id_translation.offline.Format
+[Format Specification Mini-Language]: https://docs.python.org/3/library/string.html#formatspec
+[SQL]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.SqlFetcher
+[file-system]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.PandasFetcher
+[Name-to-source]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#name-to-source-mapping
+[Placeholder-to-column]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#placeholder-mapping
+[TOML]: https://id-translation.readthedocs.io/en/stable/documentation/translator-config.html
+[cached instances]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.load_persistent_instance.html
+[Translator.translate()]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.translate.html
+
+## Supported types
+- Supported ID types: `int`, `string`, and `UUID`.
+- Supports translation of build-in collections: `list`, `dict`, `set`, `tuple`.
+- Supports translation of [pandas types][pandas-translation], including `pandas.MultiIndex` types.
 
 [pandas-translation]: https://id-translation.readthedocs.io/en/stable/documentation/examples/notebooks/cookbook/pandas-index.html
-[translate]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.translate.html
-[format]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.offline.html#id_translation.offline.Format
-[n2s-mapping]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#name-to-source-mapping
-[pm-mapping]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#placeholder-mapping
-[persistent]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.load_persistent_instance.html
-[sql-fetcher]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.SqlFetcher
-[pandas-fetcher]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.PandasFetcher
-[translator-config]: https://id-translation.readthedocs.io/en/stable/documentation/translator-config.html
-
 
 # Installation
 The package is published through the [Python Package Index (PyPI)]. Source code
 is available on GitHub: https://github.com/rsundqvist/id-translation
 
 ```sh
 pip install -U id-translation
```

### Comparing `id_translation-0.8.0/pyproject.toml` & `id_translation-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "id-translation"
-version = "0.8.0"
+version = "0.9.0"
 description = "Convert IDs into human-readable labels."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/id-translation"
 repository = "https://github.com/rsundqvist/id-translation"
 documentation = "https://id-translation.readthedocs.io"
```

### Comparing `id_translation-0.8.0/src/id_translation/__init__.py` & `id_translation-0.9.0/src/id_translation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 from ._translator import Translator
 
 __all__ = [
     "Translator",
     "__version__",  # Make MyPy happy
 ]
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 _logging.getLogger(__name__).addHandler(_logging.NullHandler())
```

### Comparing `id_translation-0.8.0/src/id_translation/_tasks/_base_task.py` & `id_translation-0.9.0/src/id_translation/_tasks/_base_task.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/_tasks/_map.py` & `id_translation-0.9.0/src/id_translation/_tasks/_map.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/_tasks/_names.py` & `id_translation-0.9.0/src/id_translation/_tasks/_names.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/_tasks/_translate.py` & `id_translation-0.9.0/src/id_translation/_tasks/_translate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import logging
 import warnings
 from collections import defaultdict
 from collections.abc import Sequence
-from copy import deepcopy
 from time import perf_counter
 from typing import TYPE_CHECKING, Any, get_args
 
 from numpy import isnan, unique
 from rics.misc import tname
 from rics.performance import format_seconds
 
 from .. import _uuid_utils
-from ..dio._dict import DictIO
 from ..exceptions import TooManyFailedTranslationsError
 from ..mapping.types import UserOverrideFunction
 from ..offline import Format, TranslationMap
 from ..settings import logging as settings
 from ..types import IdType, IdTypes, Names, NameToSource, NameType, NameTypes, SourceType, Translatable
 from ..utils.logging import cast_unsafe
 from ._map import MappingTask
@@ -192,59 +190,45 @@
                 copy=not inplace,
             )
         finally:
             translation_map.reverse_mode = False
 
         return None if inplace else result
 
-    def _should_verify(self) -> bool:
-        return LOGGER.isEnabledFor(logging.DEBUG) or self.maximal_untranslated_fraction < 1.0
-
-    def verify(self, translation_map: TranslationMap[NameType, SourceType, IdType]) -> None:
+    def verify(self, tmap: TranslationMap[NameType, SourceType, IdType]) -> None:
         """Verify translations.
 
         Performs translation with pre-defined formats, counting the number of IDs which are (and aren't) known to the
         translation map.
         """
-        if not self._should_verify():
+        if not (self.maximal_untranslated_fraction < 1.0 or LOGGER.isEnabledFor(logging.DEBUG)):
             return
 
         name_to_ids = self._name_to_ids_in_order()
-        name_to_mask = deepcopy(name_to_ids)
+        translations = tmap.to_translations()
 
-        fmt, default_fmt = translation_map.fmt, translation_map.default_fmt
-        try:
-            translation_map.fmt = Format("")
-            translation_map.default_fmt = None
-            DictIO.insert(
-                name_to_mask,
-                names=self.io_names,
-                tmap=translation_map,
-                copy=False,
-            )
-        finally:
-            translation_map.fmt, translation_map.default_fmt = fmt, default_fmt
+        for name, ids in name_to_ids.items():
+            source = tmap.name_to_source[name]
+            known = translations[source].real
+            if self.reverse != tmap.reverse_mode:
+                known = set(known.values())  # type: ignore[assignment]
 
-        for name, mask in name_to_mask.items():
-            n_untranslated, n_total = sum(t is None for t in mask), len(mask)
+            is_missing = [idx not in known for idx in ids]
+            n_untranslated = sum(is_missing)
             if n_untranslated == 0:
                 continue
+            n_total = len(ids)
             f_untranslated = n_untranslated / n_total
 
-            sample_ids = self._get_untranslated_ids(name_to_ids[name], mask=mask)
-
-            extra = {
-                "name_of_ids": name,
-                "source": translation_map.name_to_source[name],
-                "sample_ids": cast_unsafe(sample_ids),
-            }
+            sample_ids = self._get_untranslated_ids(name_to_ids[name], is_missing_mask=is_missing)
 
+            extra = {"name_of_ids": name, "source": source, "sample_ids": cast_unsafe(sample_ids)}
             message = (
                 f"Failed to translate {n_untranslated}/{n_total} ({f_untranslated:.1%}{{reason}}) of IDs "
-                f"for {name=} using source={translation_map.name_to_source[name]!r}. Sample IDs: {sample_ids}."
+                f"for {name=} using source={source!r}. Sample IDs: {sample_ids}."
             )
 
             if f_untranslated > self.maximal_untranslated_fraction:
                 message = message.format(
                     reason=f" > maximal_untranslated_fraction={self.maximal_untranslated_fraction:.1%}"
                 )
                 LOGGER.error(message, extra=extra)
@@ -264,26 +248,21 @@
 
         name_to_ids = {name: ids for name, ids in name_to_ids.items() if len(ids) > 0}
         if not self._names_without_ids:
             self._names_without_ids = set(self.io_names).difference(name_to_ids)
         return name_to_ids
 
     @staticmethod
-    def _get_untranslated_ids(
-        ids: Sequence[IdType],
-        *,
-        mask: Sequence[str | None],
-    ) -> list[IdType]:
+    def _get_untranslated_ids(ids: Sequence[IdType], *, is_missing_mask: Sequence[bool]) -> list[IdType]:
         seen = set()
         retval = []
 
-        for i, idx in enumerate(ids):
-            if idx in seen:
+        for idx, is_missing in zip(ids, is_missing_mask, strict=True):
+            if not is_missing or idx in seen:
                 continue
 
-            if mask[i] is None:
-                seen.add(idx)
-                retval.append(idx)
-                if len(retval) == NUM_SAMPLE_IDS:
-                    break
+            seen.add(idx)
+            retval.append(idx)
+            if len(retval) == NUM_SAMPLE_IDS:
+                break
 
         return retval
```

### Comparing `id_translation-0.8.0/src/id_translation/_translator.py` & `id_translation-0.9.0/src/id_translation/_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,21 @@
 ID_TRANSLATION_DISABLED: Literal["ID_TRANSLATION_DISABLED"] = "ID_TRANSLATION_DISABLED"
 
 if TYPE_CHECKING:
     from uuid import UUID
 
     ID_TRANSLATION_PANDAS_IS_TYPED: bool = False
 
-DEFAULT_FORMAT = Format("<Failed: id={id!r}>")
-
 
 class Translator(Generic[NameType, SourceType, IdType], HasSources[SourceType]):
     """End-user interface for all translation tasks.
 
+    See :meth:`.Translator.translate` for runtime configuration options. Any argument chosen when the ``Translator`` is
+    created can be overridden with :meth:`.Translator.copy`. Use :meth:`.go_offline` to store translations in memory.
+
     Args:
         fetcher: A :class:`.Fetcher` or ready-to-use translations.
         fmt: String :class:`.Format` specification for translations.
         mapper: A :class:`~.mapping.Mapper` instance for binding names to sources.
         default_fmt: Alternative :class:`.Format` to use fallback translation of unknown IDs.
         default_fmt_placeholders: Shared and/or source-specific default placeholder values for unknown IDs. See
             :meth:`rics.collections.dicts.InheritedKeysDict.make` for details. Sources that are translated using default
@@ -138,28 +139,26 @@
 
         Check out the :ref:`translation-primer` to learn how this is done "under the hood".
     """
 
     def __init__(
         self,
         fetcher: FetcherTypes[NameType, SourceType, IdType] | None = None,
-        fmt: FormatType = "{id}:{name}",
+        fmt: FormatType = Format.DEFAULT,
         mapper: Mapper[NameType, SourceType, None] = None,
-        default_fmt: FormatType = DEFAULT_FORMAT,
-        default_fmt_placeholders: MakeType[SourceType, str, Any] = None,
+        default_fmt: FormatType = Format.DEFAULT_FAILED,
+        default_fmt_placeholders: MakeType[SourceType, str, Any] | None = None,
         enable_uuid_heuristics: bool = False,
         transformers: dict[SourceType, Transformer[IdType]] | None = None,
     ) -> None:
         self._transformers = {} if transformers is None else transformers
 
         self._fmt = fmt if isinstance(fmt, Format) else Format(fmt)
         self._default_fmt_placeholders: InheritedKeysDict[SourceType, str, Any] | None
-        self._default_fmt_placeholders, self._default_fmt = _handle_default(
-            self._fmt, default_fmt, default_fmt_placeholders
-        )
+        self._default_fmt_placeholders, self._default_fmt = _handle_default(default_fmt, default_fmt_placeholders)
         self._enable_uuid_heuristics = enable_uuid_heuristics
 
         self._cached_tmap: TranslationMap[NameType, SourceType, IdType] = TranslationMap({})
         self._fetcher: Fetcher[SourceType, IdType]
         if fetcher is None:
             from .testing import TestFetcher, TestMapper
 
@@ -183,15 +182,15 @@
             self._cached_tmap = self._to_translation_map(
                 {source: PlaceholderTranslations.make(source, pht) for source, pht in fetcher.items()}
             )
         elif isinstance(fetcher, TranslationMap):
             tmap = fetcher.copy()
             tmap.fmt = self._fmt
             tmap.default_fmt = self._default_fmt
-            tmap.default_fmt_placeholders = self._default_fmt_placeholders  # type: ignore
+            tmap.default_fmt_placeholders = self._default_fmt_placeholders
             self._cached_tmap = tmap
         else:
             raise TypeError(type(fetcher))  # pragma: no cover
 
         self._mapper: Mapper[NameType, SourceType, None] = mapper or Mapper()
         self._mapper.logger = logging.getLogger(__package__).getChild("mapping").getChild("name-to-source")
 
@@ -602,14 +601,42 @@
                 override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
                 maximal_untranslated_fraction: float = 1.0,
                 # Translation specification
                 reverse: bool = False,
                 fmt: FormatType | None = None,
             ) -> NoReturn: ...
 
+        @overload
+        def translate(
+            self,
+            translatable: Translatable[NameType, IdType],
+            names: NameTypes[NameType] | NameToSource[NameType, SourceType] | None = None,
+            *,
+            ignore_names: Names[NameType] | None = None,
+            inplace: Literal[False] = False,
+            override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
+            maximal_untranslated_fraction: float = 1.0,
+            reverse: Literal[False] = False,
+            fmt: FormatType | None = None,
+        ) -> Translatable[NameType, str]: ...
+
+        @overload
+        def translate(
+            self,
+            translatable: Translatable[NameType, str],
+            names: NameTypes[NameType] | NameToSource[NameType, SourceType] | None = None,
+            *,
+            ignore_names: Names[NameType] | None = None,
+            inplace: Literal[False] = False,
+            override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
+            maximal_untranslated_fraction: float = 1.0,
+            reverse: Literal[True] = True,
+            fmt: FormatType | None = None,
+        ) -> Translatable[NameType, IdType]: ...
+
     def translate(
         self,
         translatable: Translatable[NameType, IdType],
         names: NameTypes[NameType] | NameToSource[NameType, SourceType] | None = None,
         *,
         ignore_names: Names[NameType] | None = None,
         inplace: bool = False,
@@ -635,18 +662,17 @@
             translatable: A data structure to translate.
             names: Explicit names to translate. Derive from `translatable` if ``None``. Alternatively, you may pass a
                 ``dict`` on the form ``{name_in_translatable: source_to_use}``.
             ignore_names: Names **not** to translate, or a predicate ``(NameType) -> bool``.
             inplace: If ``True``, translate in-place and return ``None``.
             override_function: A callable ``(name, sources, ids) -> Source | None``. See :meth:`.Mapper.apply`
                 for details.
-            maximal_untranslated_fraction: The maximum fraction of IDs for which translation may fail before an error is
-                raised. 1=disabled. Ignored in `reverse` mode.
+            maximal_untranslated_fraction: The maximum fraction of IDs for which translation may fail. 1=disabled.
             reverse: If ``True``, perform translations back to IDs. Offline mode only.
-            fmt: Format to use. If ``None``, fall back to init format.
+            fmt: A :class:`format string <.Format>` such as **'{id}:{name}'** use. Default is :attr:`.Translator.fmt`.
 
         Returns:
             A translated copy of `translatable` if ``inplace=False``, otherwise ``None``.
 
         Examples:
             Manual `name-to-source <../documentation/translation-primer.html#name-to-source-mapping>`__ mapping with a
             temporary name-only :class:`.Format`.
@@ -735,15 +761,15 @@
         if self._translated_names is None:
             raise ValueError("No names have been translated using this Translator.")
         return dict(self._translated_names) if with_source else list(self._translated_names)
 
     def map(
         self,
         translatable: Translatable[NameType, IdType],
-        names: NameTypes[NameType] = None,
+        names: NameTypes[NameType] | None = None,
         *,
         ignore_names: Names[NameType] | None = None,
         override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
     ) -> NameToSource[NameType, SourceType]:
         """Map names to translation sources.
 
         Args:
@@ -773,15 +799,15 @@
             ignore_names=ignore_names,
             override_function=override_function,
         ).name_to_source
 
     def map_scores(
         self,
         translatable: Translatable[NameType, IdType],
-        names: NameTypes[NameType] = None,
+        names: NameTypes[NameType] | None = None,
         *,
         ignore_names: Names[NameType] | None = None,
         override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
     ) -> "pandas.DataFrame":
         """Returns raw match scores for name-to-source mapping. See :meth:`map` for details."""
         return MappingTask(
             self,
@@ -805,15 +831,15 @@
 
         Placeholders shown here are the names as they appear **in the source**.
         """
         return self._fetcher.placeholders if self.online else self._cached_tmap.placeholders
 
     @property
     def fmt(self) -> Format:
-        """Main translation :class:`.Format`."""
+        """Main translation :class:`.Format` for this ``Translator`` instance."""
         return self._fmt
 
     @property
     def default_fmt(self) -> Format | None:
         """Alternative translation :class:`.Format`, used for unknown IDs."""
         return self._default_fmt
 
@@ -936,30 +962,37 @@
             extra = "" if ans._config_metadata is None else f" with {ans.config_metadata}"
             LOGGER.debug(f"Deserialized {ans}{extra}.")
 
         return ans
 
     def go_offline(
         self,
-        translatable: Translatable[NameType, IdType] = None,
-        names: NameTypes[NameType] = None,
+        translatable: Translatable[NameType, IdType] | None = None,
+        names: NameTypes[NameType] | NameToSource[NameType, SourceType] | None = None,
         *,
         ignore_names: Names[NameType] | None = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
+        maximal_untranslated_fraction: float = 1.0,
+        fmt: FormatType | None = None,
         path: PathLikeType = None,
     ) -> Self:
         """Retrieve and store translations in memory.
 
         .. warning::
 
            The translator will be disconnected. No new translations may be fetched after this method returns.
 
         Args:
             translatable: Data from which IDs to fetch will be extracted. Fetch all IDs if ``None``.
             names: Explicit names to translate. Derive from `translatable` if ``None``.
             ignore_names: Names **not** to translate, or a predicate ``(NameType) -> bool``.
+            override_function: A callable ``(name, sources, ids) -> Source | None``. See :meth:`.Mapper.apply`
+                for details.
+            maximal_untranslated_fraction: The maximum fraction of IDs for which translation may fail. 1=disabled.
+            fmt: A :class:`format string <.Format>` such as **'{id}:{name}'** use. Default is :attr:`.Translator.fmt`.
             path: If given, serialize the :class:`.Translator` to disk after retrieving data.
 
         Returns:
             Self, for chained assignment.
 
         Raises:
             ForbiddenOperationError: If :meth:`.Fetcher.fetch_all` is disabled and ``translatable=None``.
@@ -969,15 +1002,22 @@
             The :class:`.Translator` is guaranteed to be :func:`~rics.misc.serializable` once offline. Fetchers often
             aren't as they require things like database connections to function.
 
         See Also:
             The :meth:`restore` method.
         """
         start = perf_counter()
-        translation_map = self._user_fetch(translatable, names, ignore_names=ignore_names)
+        translation_map = self._user_fetch(
+            translatable,
+            names,
+            ignore_names=ignore_names,
+            override_function=override_function,
+            maximal_untranslated_fraction=maximal_untranslated_fraction,
+            fmt=fmt,
+        )
         self.fetcher.close()
         del self._fetcher
         self._cached_tmap = translation_map
 
         LOGGER.info(f"Created {translation_map} in {format_perf_counter(start)}.")
         if path:
             import pickle
@@ -991,29 +1031,37 @@
             pretty = get_public_module(cls, resolve_reexport=True) + "." + tname(self, prefix_classname=True)
             LOGGER.info(f"Serialized {pretty!r} of size {path.stat().st_size / 2**20:.2g} MiB at path='{path}'.")
 
         return self
 
     def fetch(
         self,
-        translatable: Translatable[NameType, IdType] = None,
-        names: NameTypes[NameType] = None,
+        translatable: Translatable[NameType, IdType] | None = None,
+        names: NameTypes[NameType] | NameToSource[NameType, SourceType] | None = None,
         *,
         ignore_names: Names[NameType] | None = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
+        maximal_untranslated_fraction: float = 1.0,
+        fmt: FormatType | None = None,
     ) -> TranslationMap[NameType, SourceType, IdType]:
         """Fetch translations.
 
         Calling ``fetch`` without arguments will perform a :meth:`.Fetcher.fetch_all` -operation, without going offline.
-        The returned :class:`.TranslationMap` may be converted to native types.
+
+        The returned :class:`.TranslationMap` may be converted to native types with :meth:`.TranslationMap.to_dicts`.
 
         Args:
-            translatable: A data structure to translate. Fetch all available data if ``None``.
+            translatable: A data structure to translate.
             names: Explicit names to translate. Derive from `translatable` if ``None``. Alternatively, you may pass a
                 ``dict`` on the form ``{name_in_translatable: source_to_use}``.
             ignore_names: Names **not** to translate, or a predicate ``(NameType) -> bool``.
+            override_function: A callable ``(name, sources, ids) -> Source | None``. See :meth:`.Mapper.apply`
+                for details.
+            maximal_untranslated_fraction: The maximum fraction of IDs for which translation may fail. 1=disabled.
+            fmt: A :class:`format string <.Format>` such as **'{id}:{name}'** use. Default is :attr:`.Translator.fmt`.
 
         Returns:
             A :class:`.TranslationMap`.
 
         Raises:
             ConnectionStatusError: If disconnected from the fetcher, i.e. not :attr:`online`.
 
@@ -1056,40 +1104,69 @@
 
             * :meth:`.TranslationMap.to_pandas` → ``{source: DataFrame}``
             * :meth:`.TranslationMap.to_dicts` → ``{source: {placeholder: [values...]}}``
 
             >>> translation_map.to_dicts()["people"]
             {'id': [1999, 1991], 'name': ['Sofia', 'Richard']}
         """
-        return self._user_fetch(translatable, names, ignore_names=ignore_names)
+        return self._user_fetch(
+            translatable,
+            names,
+            ignore_names=ignore_names,
+            override_function=override_function,
+            maximal_untranslated_fraction=maximal_untranslated_fraction,
+            fmt=fmt,
+        )
 
     def _user_fetch(
         self,
-        translatable: Translatable[NameType, IdType] = None,
-        names: NameTypes[NameType] = None,
+        translatable: Translatable[NameType, IdType] | None = None,
+        names: NameTypes[NameType] | NameToSource[NameType, SourceType] | None = None,
         *,
         ignore_names: Names[NameType] | None = None,
+        override_function: UserOverrideFunction[NameType, SourceType, None] | None = None,
+        maximal_untranslated_fraction: float = 1.0,
+        fmt: FormatType | None = None,
     ) -> TranslationMap[NameType, SourceType, IdType]:
+        fmt = self._fmt if fmt is None else Format.parse(fmt)
+
         if translatable is None:
-            translation_map = self._to_translation_map(self._fetch(None))
-            if names is not None:
-                names = as_list(names)
-                translation_map.name_to_source = self.mapper.apply(names, translation_map.sources).flatten()
+            translation_map = self._to_translation_map(self._fetch(None), fmt=fmt)
+
+            if names is None:
+                pass  # Callers must perform mapping unless name=source.
+            elif isinstance(names, dict):
+                translation_map.name_to_source = names
+            else:
+                translation_map.name_to_source = self.mapper.apply(
+                    as_list(names),
+                    translation_map.sources,
+                    override_function=override_function,
+                ).flatten()
         else:
-            name_to_source = self.map(translatable, names, ignore_names=ignore_names)
-            if not name_to_source:
-                pretty = repr(tname(translatable, prefix_classname=True))
-                raise MappingError(f"No names in the {pretty}-type data were mapped.")
+            task = TranslationTask(
+                self,
+                translatable,
+                self._fmt,
+                names,
+                ignore_names=ignore_names,
+                maximal_untranslated_fraction=maximal_untranslated_fraction,
+                enable_uuid_heuristics=self._enable_uuid_heuristics,
+            )
+            if not task.name_to_source:
+                msg = f"No names in the {tname(translatable, prefix_classname=True)!r}-type data were mapped."
+                raise MappingError(msg)
 
-            task = TranslationTask(self, translatable, self._fmt, name_to_source)
             translation_map = self._get_updated_tmap(task, force_fetch=True)
             if LOGGER.isEnabledFor(logging.DEBUG):
                 not_fetched = set(self.fetcher.sources).difference(translation_map.sources)
                 LOGGER.debug(f"Available sources {not_fetched} were not fetched.")
 
+            task.verify(translation_map)
+
         return translation_map
 
     def _get_updated_tmap(
         self,
         task: TranslationTask[NameType, SourceType, IdType],
         force_fetch: bool = False,
     ) -> TranslationMap[NameType, SourceType, IdType]:
@@ -1175,22 +1252,21 @@
         more = f"fetcher={self.fetcher}" if self.online else f"cache={self.cache}"
 
         online = self.online
         return f"{tname(self)}({online=}: {more})"
 
 
 def _handle_default(
-    fmt: Format,
     default_fmt: FormatType,
     default_fmt_placeholders: MakeType[SourceType, str, Any] | None,
-) -> tuple[InheritedKeysDict[SourceType, str, Any] | None, Format | None]:  # pragma: no cover
+) -> tuple[InheritedKeysDict[SourceType, str, Any], Format]:
     default_fmt = Format.parse(default_fmt)
 
     if not default_fmt_placeholders:
         return InheritedKeysDict(), default_fmt
 
     if isinstance(default_fmt_placeholders, InheritedKeysDict):
         default_placeholders = default_fmt_placeholders
     else:
         default_placeholders = InheritedKeysDict.make(default_fmt_placeholders)
 
-    return default_placeholders, fmt if default_fmt is DEFAULT_FORMAT else default_fmt
+    return default_placeholders, default_fmt
```

### Comparing `id_translation-0.8.0/src/id_translation/_uuid_utils.py` & `id_translation-0.9.0/src/id_translation/_uuid_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 import numpy as np
 
 IdCollectionT = TypeVar("IdCollectionT", bound=Sequence)  # type: ignore[type-arg] # TODO: Need Higher-Kinded TypeVars
 
 
 def cast_many(ids: IdCollectionT) -> IdCollectionT:
     """Cast `ids` to UUIDs."""
-    if isinstance(ids[0], UUID):
-        return ids
-
     uuids = map(UUID, ids)
     if isinstance(ids, np.ndarray):
         return np.fromiter(uuids, dtype=UUID)
     else:
         return type(ids)(uuids)  # type: ignore[call-arg]
 
 
 def try_cast_many(ids: IdCollectionT) -> IdCollectionT:
     """Try casting `ids` to UUIDs, falling back to the original input."""
-    if not ids:
+    if len(ids) == 0:
         return ids
 
     try:
         return cast_many(ids)
     except (ValueError, AttributeError, TypeError):
         return ids
```

### Comparing `id_translation-0.8.0/src/id_translation/dio/_data_structure_io.py` & `id_translation-0.9.0/src/id_translation/dio/_data_structure_io.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/dio/_dict.py` & `id_translation-0.9.0/src/id_translation/dio/_dict.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/dio/_pandas.py` & `id_translation-0.9.0/src/id_translation/dio/_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,24 +90,24 @@
         # Optimization for single-name vectors. Faster than SequenceIO for pretty much every size.
         magic_dict = tmap[names[0]]
 
         mapping: dict[IdType, str | None]
         if is_numeric_dtype(pvt):
             # We don't need to cast float to int here, since hash(1.0) == hash(1). The cast in extract() is required
             # because some database drivers may complain, especially if they receive floats (especially NaN).
-            mapping = {idx: magic_dict.get(idx) for idx in pvt.unique()}
+            mapping = {idx: magic_dict[idx] for idx in pvt.unique()}
             return pvt.map(mapping)
         else:
             mapping = {}
             data: list[Any] = pvt.to_list()
             for i, idx in enumerate(data):
                 if idx in mapping:
                     value = mapping[idx]
                 else:
-                    value = magic_dict.get(idx)
+                    value = magic_dict[idx]
                     mapping[idx] = value
                 data[i] = value
 
         return data
     else:
         return translate_sequence(pvt, names, tmap)
```

### Comparing `id_translation-0.8.0/src/id_translation/dio/_resolve.py` & `id_translation-0.9.0/src/id_translation/dio/_resolve.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/dio/_sequence.py` & `id_translation-0.9.0/src/id_translation/dio/_sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,25 +46,24 @@
         try:
             translatable[:] = t[:]  # type: ignore
             return None
         except TypeError as e:
             raise NotInplaceTranslatableError(translatable) from e
 
 
-def translate_sequence(
-    s: T, names: list[NameType], tmap: TranslationMap[NameType, SourceType, IdType]
-) -> list[str | None]:
+def translate_sequence(s: T, names: list[NameType], tmap: TranslationMap[NameType, SourceType, IdType]) -> list[str]:
     """Return a translated copy of the sequence `s`."""
     if len(names) == 1:
-        return list(map(tmap[names[0]].get, s))
+        magic_dict = tmap[names[0]]
+        return [magic_dict[i] for i in s]
 
     return [
         translate_sequence(element, [name], tmap)  # type: ignore
         if SequenceIO.handles_type(element)
-        else tmap[name].get(element)
+        else tmap[name][element]
         for name, element in zip(names, s)
     ]
 
 
 def verify_names(data_len: int, names: list[NameType]) -> None:  # pragma: no cover
     """Verify that the length of names is either 1 or equal to the length of the data."""
     num_names = len(names)
```

### Comparing `id_translation-0.8.0/src/id_translation/dio/_set.py` & `id_translation-0.9.0/src/id_translation/dio/_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
             raise ValueError("Length of names must be one.")
 
         return {names[0]: list(translatable)}
 
     @staticmethod
     def insert(
         translatable: set[IdType], names: list[NameType], tmap: TranslationMap[NameType, SourceType, IdType], copy: bool
-    ) -> set[str | None] | None:
+    ) -> set[str] | None:
         magic_dict = tmap[names[0]]
-        translated = {magic_dict.get(e) for e in translatable}
+        translated = {magic_dict[e] for e in translatable}
 
         if copy:
             return translated
 
         translatable.clear()
         translatable.update(translated)  # type: ignore[arg-type]
         return None
```

### Comparing `id_translation-0.8.0/src/id_translation/dio/_single_value.py` & `id_translation-0.9.0/src/id_translation/dio/_single_value.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/dio/exceptions.py` & `id_translation-0.9.0/src/id_translation/dio/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/exceptions.py` & `id_translation-0.9.0/src/id_translation/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/factory.py` & `id_translation-0.9.0/src/id_translation/factory.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/__init__.py` & `id_translation-0.9.0/src/id_translation/fetching/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_abstract_fetcher.py` & `id_translation-0.9.0/src/id_translation/fetching/_abstract_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_cache.py` & `id_translation-0.9.0/src/id_translation/fetching/_cache.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_fetcher.py` & `id_translation-0.9.0/src/id_translation/fetching/_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_memory_fetcher.py` & `id_translation-0.9.0/src/id_translation/fetching/_memory_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_multi_fetcher.py` & `id_translation-0.9.0/src/id_translation/fetching/_multi_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_pandas_fetcher.py` & `id_translation-0.9.0/src/id_translation/fetching/_pandas_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/_sql_fetcher.py` & `id_translation-0.9.0/src/id_translation/fetching/_sql_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/exceptions.py` & `id_translation-0.9.0/src/id_translation/fetching/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/fetching/types.py` & `id_translation-0.9.0/src/id_translation/fetching/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/__init__.py` & `id_translation-0.9.0/src/id_translation/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/_cardinality.py` & `id_translation-0.9.0/src/id_translation/mapping/_cardinality.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/_directional_mapping.py` & `id_translation-0.9.0/src/id_translation/mapping/_directional_mapping.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/_heuristic_score.py` & `id_translation-0.9.0/src/id_translation/mapping/_heuristic_score.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/_mapper.py` & `id_translation-0.9.0/src/id_translation/mapping/_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
         self,
         score_function: str | ScoreFunction[ValueType, CandidateType, ContextType] = "disabled",
         score_function_kwargs: dict[str, Any] | None = None,
         filter_functions: Iterable[
             tuple[str | FilterFunction[ValueType, CandidateType, ContextType], dict[str, Any]]
         ] = (),
         min_score: float = 0.90,
-        overrides: InheritedKeysDict[ContextType, ValueType, CandidateType]
-        | dict[ValueType, CandidateType]
+        overrides: dict[ValueType, CandidateType]
+        | InheritedKeysDict[ContextType, ValueType, CandidateType]
         | None = None,
         unmapped_values_action: ActionLevel.ParseType = ActionLevel.IGNORE,
         unknown_user_override_action: ActionLevel.ParseType = ActionLevel.RAISE,
         cardinality: Cardinality.ParseType | None = Cardinality.ManyToOne,
         verbose_logging: bool = False,
     ) -> None:
         if min_score <= 0 or np.isinf(min_score):
```

### Comparing `id_translation-0.8.0/src/id_translation/mapping/exceptions.py` & `id_translation-0.9.0/src/id_translation/mapping/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/filter_functions.py` & `id_translation-0.9.0/src/id_translation/mapping/filter_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/heuristic_functions.py` & `id_translation-0.9.0/src/id_translation/mapping/heuristic_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/score_functions.py` & `id_translation-0.9.0/src/id_translation/mapping/score_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/support.py` & `id_translation-0.9.0/src/id_translation/mapping/support.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/mapping/types.py` & `id_translation-0.9.0/src/id_translation/mapping/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/offline/_format.py` & `id_translation-0.9.0/src/id_translation/offline/_format.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rics.misc import tname
 
 from . import parse_format_string
 from .types import FormatType, PlaceholdersTuple
 
 
 class Format:
-    r"""Format specification for translations strings.
+    """Format specification for translations strings.
 
     Translation formats are similar to regular f-strings, with two important exceptions:
 
     1. Positional placeholders (``'{}'``) may not be used; correct form is ``'{placeholder-name}'``.
     2. Placeholders surrounded by ``'[]'`` denote an optional element. Optional elements are rendered...
 
        * Only if `all` of its placeholders are defined.
@@ -24,55 +24,108 @@
        Double the wanted bracket character to render as a literal, analogous to ``'{{'`` and ``'}}'``
        in plain Python f-strings. See the example below for a demonstration.
 
     Args:
         fmt: A translation fstring.
 
     Examples:
+        **Basic usage**
+
+        Formats are created by passing a single ``str`` arguments, as described above.
+
+        >>> Format(Format.DEFAULT)
+        "Format('{id}:{name}')"
+        >>> Format(Format.DEFAULT).fstring().format(id=1, name="First")
+        '1:First'
+
+        Using :meth:`Format.fstring` and :py:meth:`str.format` is flexible but verbose. Formats can be applier either
+        through :meth:`Format.format`...
+
+        >>> fmt = Format(Format.DEFAULT_FAILED)
+        >>> fmt.format(id=1, name="First")
+
+        ...or just ``Format.__call__()``.
+
+        >>> fmt(id=1, name="First")
+        '<Failed: id=1>'
+
+        Using either convenience method will use as many placeholders as possible.
+
+        >>> fmt = Format(Format.DEFAULT)
+        >>> fmt.placeholders
+        "('id', 'name')"
+        >>> fmt(id=1, name="First")
+        '1:First'
+        >>> fmt(id=1, name="First", unknown=20.19)
+        '1:First'
+
+        Unknown placeholders are simply ignored.
+
+        **Optional placeholders**
+
         A format string using literal angle brackets and an optional element.
 
         >>> from id_translation.offline import Format
         >>> fmt = Format("{id}:[[{name}]][, nice={is_nice}]")
 
         The ``Format`` class when used directly only returns required placeholders by default...
 
         >>> fmt.fstring()
         '{id}:[{name}]'
-        >>> fmt.fstring().format(id=0, name="Tarzan")
+        >>> fmt(id=0, name="Tarzan")
         '0:[Tarzan]'
 
         ...but the :attr:`placeholders` attribute can be used to retrieve all placeholders, required and optional:
 
         >>> fmt.placeholders
         ('id', 'name', 'is_nice')
-        >>> fmt.fstring(fmt.placeholders).format(id=1, name="Morris", is_nice=True)
+        >>> fmt(id=1, name="Morris", is_nice=True)
         '1:[Morris], nice=True'
 
     The :class:`.Translator` will automatically add optional placeholders, if they are present in the source.
 
     .. note::
        Python format specifications and conversions are preserved.
 
     This is especially useful for long values such as UUIDs.
 
     >>> from uuid import UUID
     >>> uuid = UUID("550e8400-e29b-41d4-a716-446655440000")
 
     Convert to string and truncate to eight characters.
 
-    >>> Format("{id!s:.8}:{name!r}").fstring().format(id=uuid, name="Sofia")
+    >>> Format("{id!s:.8}:{name!r}").format(id=uuid, name="Sofia")
     "550e8400:'Sofia'"
 
     See the official :py:ref:`formatspec` documentation for details.
     """
 
+    DEFAULT: str = "{id}:{name}"
+    """Default translation format."""
+
+    DEFAULT_FAILED: str = "<Failed: id={id!r}>"
+    """Default format for missing IDs."""
+
     def __init__(self, fmt: str) -> None:
         self._fmt = fmt
         self._elements: list[parse_format_string.Element] = parse_format_string.get_elements(fmt)
 
+    def format(self, **placeholders: Any) -> str:
+        """Apply the format.
+
+        Args:
+            **placeholders: Formats to use in the finals string.
+
+        Returns:
+            Formatting using `placeholders`.
+        """
+        return self.fstring(placeholders, positional=False).format_map(placeholders)
+
+    __call__ = format
+
     def fstring(self, placeholders: Iterable[str] | None = None, *, positional: bool = False) -> str:
         """Create a format string for the given placeholders.
 
         Args:
             placeholders: Keys to keep. Passing ``None`` is equivalent to passing :attr:`required_placeholders`.
             positional: If ``True``, remove names to return a positional fstring.
 
@@ -101,16 +154,16 @@
         Args:
             defaults: Keys which should be replaced with real values. Keys which are **not** part of `defaults` will
                 be left as-is.
 
         Returns:
             A partially formatted fstring.
         """
-        parts, _ = parse_format_string.Element.parse_block(self._fmt, defaults=defaults)
-        return Format("".join(parts))
+        new_fmt, _placeholders = parse_format_string.Element.parse_block(self._fmt, defaults=defaults)
+        return Format(new_fmt)
 
     @staticmethod
     def parse(fmt: FormatType) -> "Format":
         """Parse a format.
 
         Args:
             fmt: Input to parse.
```

### Comparing `id_translation-0.8.0/src/id_translation/offline/_format_applier.py` & `id_translation-0.9.0/src/id_translation/offline/_format_applier.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,17 @@
         self._placeholder_names = translations.placeholders
         self._n_ids = len(translations.records)
         self._transformer = transformer
 
     def __call__(
         self,
         fmt: Format,
-        placeholders: PlaceholdersTuple = None,
-        default_fmt: Format = None,
+        *,
+        default_fmt: Format,
+        placeholders: PlaceholdersTuple | None = None,
         default_fmt_placeholders: dict[str, Any] | None = None,
         enable_uuid_heuristics: bool = True,
     ) -> MagicDict[IdType]:
         """Translate IDs.
 
         Args:
             fmt: Translation format to use.
@@ -56,30 +57,25 @@
         if placeholders is None:
             # Use as many placeholders as possible.
             placeholders = tuple(filter(self._placeholder_names.__contains__, fmt.placeholders))
 
         fstring = fmt.fstring(placeholders, positional=True)
         real_translations = self._apply(fstring, placeholders)
 
-        if default_fmt is not None or default_fmt_placeholders is not None:
-            if default_fmt is None:
-                default_fmt = fmt
-            if default_fmt_placeholders is None:
-                default_fmt_placeholders = {}
-
-            partial = default_fmt.partial(default_fmt_placeholders)
-            try:
-                default_fstring = partial.fstring(positional=True)
-            except KeyError as e:
-                raise ValueError(
-                    f"All required placeholders except {{{ID}}} must be provided for {default_fmt=}:"
-                    f" {default_fmt.required_placeholders}."
-                ) from e
-        else:
-            default_fstring = None
+        if default_fmt_placeholders is None:
+            default_fmt_placeholders = {}
+
+        partial = default_fmt.partial(default_fmt_placeholders)
+        try:
+            default_fstring = partial.fstring(positional=True)
+        except KeyError as e:
+            raise ValueError(
+                f"All required placeholders except {{{ID}}} must be provided for {default_fmt=}:"
+                f" {default_fmt.required_placeholders}."
+            ) from e
 
         return MagicDict(real_translations, default_fstring, enable_uuid_heuristics, self._transformer)
 
     def to_dict(self) -> dict[str, Sequence[Any]]:
         """Get the underlying data used for translations as a dict.
 
         Returns:
```

### Comparing `id_translation-0.8.0/src/id_translation/offline/_magic_dict.py` & `id_translation-0.9.0/src/id_translation/offline/_magic_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,149 @@
 import logging
 from collections.abc import Iterator, MutableMapping
 from typing import Any
+from uuid import UUID
 
 from rics.misc import tname
 
 from .. import _uuid_utils
 from ..transform.types import Transformer, TransformerStop
 from ..types import IdType
+from ._format import Format
 from .types import TranslatedIds
 
 
 class MagicDict(MutableMapping[IdType, str]):
     """Dictionary type for translated IDs.
 
-    If `default_value` is given, it is used as the default answer for any calls to ``__getitem__`` where the key is
-    not in `translated_ids`.
+    A ``dict``-like mapping which returns "real" values if present in a backing dict. Values for unknown keys are
+    generated using the :attr:`default_value`.
 
     Args:
-        real_translations: A dict holding real translations.
+        real_translations: A dict holding :attr:`real` translations.
         default_value: A string with exactly one or zero placeholders.
         enable_uuid_heuristics: Enabling may improve matching when :py:class:`~uuid.UUID`-like IDs are in use.
         transformer: Initialized :class:`.Transformer` instance.
 
+            .. note:
+
+               If any of the `real_translations` are not ``UUID``-like,
+               ``enable_uuid_heuristics`` is forcibly set to ``False``.
+
     Examples:
-        Behaviour with :attr:`default_value`.
+        **Similarities with the built-in dict**
 
-        >>> magic = MagicDict(
-        ...     {1999: "1999:Sofia", 1991: "1991:Richard"},
-        ...     default_value="<Failed: id={!r}>",
-        ... )
-        >>> magic
-        {1999: '1999:Sofia', 1991: '1991:Richard'}
+        >>> magic = MagicDict({1999: "Sofia", 1991: "Richard"})
 
-        Calls to ``__getitem__`` and ``__contains__`` will never return ``False``.
+        Iteration, equality, and length are based on the :attr:`real`  values.
 
-        >>> magic[1999], 1999 in magic
-        ('1999:Sofia', True)
-        >>> magic["1999"], "1999" in magic
-        ("<Failed: id='1999'>", True)
+        >>> magic
+        {1999: 'Sofia', 1991: 'Richard'}
+        >>> len(magic)
+        2
+        >>> list(magic)
+        [1999, 1991]
+        >>> magic.real == magic
+        True
+        >>> magic == {1999: "Sofia"}  # Element missing
+        False
+
+        As you'd expect, casting to a regular ``dict`` removes all special handling.
+
+        **Differences from the built-in dict**
+
+        Methods ``__getitem__`` and ``__contains__`` never fail or return False. Using a default with ``get`` will
+        generate a value rather than using the provided default.
+
+        >>> magic[1999]
+        'Sofia'
+        >>> magic[2019]
+        '<Failed: id=2019>'
+        >>> magic.get(2019, "foo")  # doctest: +SKIP
+        '<Failed: id=2019>'
+
+        **ID translation heuristics**
 
         Special handling for :py:class:`uuid.UUID` and ``UUID``-like strings improve matching.
 
-        >>> from uuid import UUID
         >>> string_uuid = "550e8400-e29b-41d4-a716-446655440000"
         >>> magic = MagicDict(
         ...     {string_uuid: "Found!"},
         ...     enable_uuid_heuristics=True,
         ... )
         >>> magic
         {UUID('550e8400-e29b-41d4-a716-446655440000'): 'Found!'}
 
+        When ``enable_uuid_heuristics=True`` is set, the ``MagicDict`` will attempt to cast "promising" keys to
+        :class:`uuid.UUID`.
+
+        >>> from uuid import UUID
         >>> magic[string_uuid], magic[UUID(string_uuid)]
         ('Found!', 'Found!')
 
-        Converting to a regular ``dict``.
+        Keys that cannot be converted are left as-is.
 
-        >>> dict(magic)
-        {UUID('550e8400-e29b-41d4-a716-446655440000'): 'Found!'}
+        >>> magic["Hello"] = "World!"
+        >>> magic["unknown"], magic["Hello"]
+        ("<Failed: id='unknown'>", 'World!')
 
-        Casting to ``dict`` removes all special handling.
+        To further customize ID matching behaviour, refer to the :class:`.Transformer` interface.
     """
 
     LOGGER = logging.getLogger(__package__).getChild("MagicDict")
 
     def __init__(
         self,
         real_translations: TranslatedIds[IdType],
-        default_value: str | None = None,
+        default_value: str = Format(Format.DEFAULT_FAILED).fstring(positional=True),
         enable_uuid_heuristics: bool = True,
-        transformer: Transformer[IdType] = None,
+        transformer: Transformer[IdType] | None = None,
     ) -> None:
         if enable_uuid_heuristics and real_translations:
             real_translations, enable_uuid_heuristics = _try_stringify_many(real_translations)
 
         self._real: TranslatedIds[IdType] = real_translations
-        self._default = default_value
+        self._default = self._verify_default_value(default_value)
         self._cast_key = enable_uuid_heuristics
 
         self._try_add_missing_key = None
         if transformer is not None:
             transformer.update_translations(real_translations)
             self._try_add_missing_key = transformer.try_add_missing_key
 
+    def get(self, __key: IdType, /, _: Any = None) -> str:
+        """Same as ``__getitem__``.
+
+        Values for missing keys are generated from :attr:`default_value`.
+        """
+        return self[__key]
+
+    @property
+    def real(self) -> dict[IdType, str]:
+        """Returns the backing dict."""
+        return self._real
+
     @property
-    def default_value(self) -> str | None:
+    def default_value(self) -> str:
         """Return the default string value to return for unknown keys, if any."""
         return self._default
 
     def _try_stringify(self, key: IdType) -> Any:
         return _uuid_utils.try_cast_one(key) if self._cast_key else key
 
     def __getitem__(self, key: IdType) -> str:
-        key = self._on_read(key)
-        if key in self._real or self.default_value is None:
+        if key in self._real:
             return self._real[key]
 
-        return self.default_value.format(key)
+        key = self._on_read(key)
+        return self._real[key] if key in self._real else self.default_value.format(key)
 
     def __contains__(self, key: Any) -> bool:
-        key = self._on_read(key)
-        return self.default_value is not None or key in self._real
+        """Always returns ``True``."""
+        return True  # We can always render something with default_value.
 
     def _on_read(self, key: IdType) -> IdType:
         key = self._try_stringify(key)
         if self._try_add_missing_key and key not in self._real:
             try:
                 self._try_add_missing_key(key, translations=self)
             except TransformerStop as e:
@@ -130,20 +170,35 @@
 
     def __iter__(self) -> Iterator[IdType]:
         return iter(self._real)
 
     def __repr__(self) -> str:
         return repr(self._real)
 
+    @classmethod
+    def _verify_default_value(cls, default_value: str) -> str:
+        for sample in "id", 0, UUID(int=0):
+            try:
+                default_value.format(sample)
+                return default_value  # Formatting OK
+            except KeyError as e:  # noqa: PERF203
+                raise ValueError(f"Bad {default_value=}") from e
+            except Exception:  # noqa: S110
+                pass  # Attribute error, value error, etc. Happens naturally when the sample type is wrong.
+
+        return default_value
+
 
 def _try_stringify_many(real_translations: TranslatedIds[IdType]) -> tuple[TranslatedIds[IdType], bool]:
     original_ids = list(real_translations)
-    try:
-        new_keys = _uuid_utils.cast_many(original_ids)
-    except (ValueError, AttributeError, TypeError):
+    if len(original_ids) == 0:
+        return real_translations, True
+
+    new_keys = _uuid_utils.try_cast_many(original_ids)
+    if not isinstance(new_keys[0], UUID):
         return real_translations, False  # Keys are not UUID-like.
 
     uuid_translations = {uuid: real_translations[idx] for uuid, idx in zip(new_keys, original_ids)}
     if len(real_translations) != len(uuid_translations):
         raise TypeError("Duplicate UUIDs found. Verify translation sources or set enable_uuid_heuristics=False.")
 
     return uuid_translations, True
```

### Comparing `id_translation-0.8.0/src/id_translation/offline/_translation_map.py` & `id_translation-0.9.0/src/id_translation/offline/_translation_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Iterator, Mapping, Sequence
 from copy import copy
-from typing import TYPE_CHECKING, Any, Generic, Union
+from typing import TYPE_CHECKING, Any, Generic, Self, Union
 
 from rics.collections.dicts import InheritedKeysDict, reverse_dict
 from rics.misc import tname
 
 from ..transform.types import Transformer
 from ..types import HasSources, IdType, NameToSource, NameType, SourceType
 from ._format import Format
@@ -28,32 +28,30 @@
         name_to_source: Mappings ``{name: source}``, but may be overridden by the user.
         fmt: A translation format. Must be given to use as a mapping.
         default_fmt: Alternative format specification to use instead of `fmt` for fallback translation.
         default_fmt_placeholders: Per-source default placeholder values.
         enable_uuid_heuristics: Enabling may improve matching when :py:class:`~uuid.UUID`-like IDs are in use.
         transformers: A dict ``{source: transformer}`` of initialized :class:`.Transformer` instances.
 
-    Notes:
-        Type checking of `fmt` and `default_fmt_placeholders` attributes may fail due to
-        `mypy#3004 <https://github.com/python/mypy/issues/3004>`_
     """
 
     def __init__(
         self,
         source_translations: SourcePlaceholderTranslations[SourceType],
-        name_to_source: NameToSource[NameType, SourceType] = None,
-        fmt: FormatType = None,
-        default_fmt: FormatType = None,
-        default_fmt_placeholders: InheritedKeysDict[SourceType, str, Any] = None,
+        *,
+        fmt: FormatType = Format.DEFAULT,
+        default_fmt: FormatType = Format.DEFAULT_FAILED,
+        name_to_source: NameToSource[NameType, SourceType] | None = None,
+        default_fmt_placeholders: InheritedKeysDict[SourceType, str, Any] | None = None,
         enable_uuid_heuristics: bool = True,
         transformers: dict[SourceType, Transformer[IdType]] | None = None,
     ) -> None:
-        self.default_fmt = default_fmt  # type: ignore
-        self.default_fmt_placeholders = default_fmt_placeholders  # type: ignore
-        self.fmt = fmt  # type: ignore
+        self.fmt = Format.parse(fmt)
+        self.default_fmt = Format.parse(default_fmt)
+        self.default_fmt_placeholders = default_fmt_placeholders or InheritedKeysDict.make({})
 
         transformers = transformers or {}
         self._format_appliers: dict[SourceType, FormatApplier[NameType, SourceType, IdType]] = {
             source: FormatApplier(translations, transformer=transformers.get(source))
             for source, translations in source_translations.items()
         }
         self._names_and_sources: set[NameType | SourceType] = set()
@@ -101,31 +99,41 @@
         Returns:
             A dict of translations ``{source: MagicDict}``.
         """
         return {source: self.apply(source, fmt=fmt) for source in self.sources}
 
     @classmethod
     def from_pandas(
-        cls, frames: dict[SourceType, "pandas.DataFrame"]
-    ) -> "TranslationMap[NameType, SourceType, IdType]":
+        cls,
+        frames: dict[SourceType, "pandas.DataFrame"],
+        fmt: FormatType = Format.DEFAULT,
+        *,
+        default_fmt: FormatType = Format.DEFAULT_FAILED,
+    ) -> Self:
         """Create a new instance from a :class:`pandas.DataFrame` dict.
 
         Args:
             frames: A dict ``{source: DataFrame}``.
+            fmt: A translation format. Must be given to use as a mapping.
+            default_fmt: Alternative format specification to use instead of `fmt` for fallback translation.
 
         Returns:
             A new ``TranslationMap``.
         """
         source_translations = {
             source: PlaceholderTranslations.from_dataframe(source, frame) for source, frame in frames.items()
         }
-        return cls(source_translations)
+        return cls(source_translations, fmt=fmt, default_fmt=default_fmt)
 
     def apply(
-        self, name_or_source: NameType | SourceType, fmt: FormatType = None, default_fmt: FormatType = None
+        self,
+        name_or_source: NameType | SourceType,
+        fmt: FormatType | None = None,
+        *,
+        default_fmt: FormatType | None = None,
     ) -> MagicDict[IdType]:
         """Create translations for a given name or source.
 
         Args:
             name_or_source: A name or source to translate.
             fmt: :class:`.Format` to use. If ``None``, fall back to init format.
             default_fmt: Alternative format for default translation. Resolution: Arg -> init arg, fmt arg, init fmt arg
@@ -152,16 +160,16 @@
             default_fmt=default_fmt,
             default_fmt_placeholders=self.default_fmt_placeholders.get(source),
             enable_uuid_heuristics=self.enable_uuid_heuristics,
         )
 
         return (
             MagicDict(
-                reverse_dict(translations),  # type: ignore
-                default_value=None,  # force failure for unknown keys
+                reverse_dict(translations, duplicate_key_action="raise"),  # type: ignore
+                default_value=default_fmt.fstring(positional=True),
                 enable_uuid_heuristics=False,
             )
             if self.reverse_mode
             else translations
         )
 
     @property
@@ -176,47 +184,47 @@
     @property
     def placeholders(self) -> dict[SourceType, list[str]]:
         return {applier.source: applier.placeholders for applier in self._format_appliers.values()}
 
     @property
     def name_to_source(self) -> NameToSource[NameType, SourceType]:
         """Return name-to-source mapping."""
-        return self._name_to_source
+        return dict(self._name_to_source)
 
     @name_to_source.setter
     def name_to_source(self, value: NameToSource[NameType, SourceType]) -> None:
         self._name_to_source: NameToSource[NameType, SourceType] = value
         self._names_and_sources = set(value).union(self._format_appliers)
 
     @property
-    def fmt(self) -> Format | None:
+    def fmt(self) -> Format:
         """Return the translation format."""
         return self._fmt
 
     @fmt.setter
-    def fmt(self, value: FormatType | None) -> None:
-        self._fmt = None if value is None else Format.parse(value)
+    def fmt(self, value: FormatType) -> None:
+        self._fmt = Format.parse(value)
 
     @property
-    def default_fmt(self) -> Format | None:
-        """Return the format specification to use instead of `fmt` for fallback translation."""
+    def default_fmt(self) -> Format:
+        """Return the format specification to use instead of :attr:`fmt` for fallback translation."""
         return self._default_fmt
 
     @default_fmt.setter
-    def default_fmt(self, value: FormatType | None) -> None:
-        self._default_fmt = None if value is None else Format.parse(value)
+    def default_fmt(self, value: FormatType) -> None:
+        self._default_fmt = Format.parse(value)
 
     @property
     def default_fmt_placeholders(self) -> InheritedKeysDict[SourceType, str, Any]:
         """Return the default translations used for `default_fmt_placeholders` placeholders."""
         return self._default_fmt_placeholders
 
     @default_fmt_placeholders.setter
-    def default_fmt_placeholders(self, value: InheritedKeysDict[SourceType, str, Any] | None) -> None:
-        self._default_fmt_placeholders = InheritedKeysDict() if value is None else InheritedKeysDict.make(value)
+    def default_fmt_placeholders(self, value: InheritedKeysDict[SourceType, str, Any]) -> None:
+        self._default_fmt_placeholders = InheritedKeysDict.make(value) if value else InheritedKeysDict()
 
     @property
     def reverse_mode(self) -> bool:
         """Return reversed mode status flag.
 
          If set, the mappings returned by :meth:`apply` (and therefore also ``__getitem__``) are reversed.
 
@@ -243,15 +251,15 @@
         """Get a dict ``{source: transformer}`` of :class:`.Transformer` instances used by this ``TranslationMap``."""
         return {
             source: applier.transformer
             for source, applier in self._format_appliers.items()
             if applier.transformer is not None
         }
 
-    def copy(self) -> "TranslationMap[NameType, SourceType, IdType]":
+    def copy(self) -> Self:
         """Make a copy of this ``TranslationMap``."""
         return copy(self)
 
     def __getitem__(self, name_or_source: NameType | SourceType) -> MagicDict[IdType]:
         return self.apply(name_or_source)
 
     def __len__(self) -> int:
```

### Comparing `id_translation-0.8.0/src/id_translation/offline/parse_format_string.py` & `id_translation-0.9.0/src/id_translation/offline/parse_format_string.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 """Utility module for parsing raw ``Format`` input strings."""
 
 import collections.abc as _abc
 from dataclasses import dataclass as _dataclass
 from string import Formatter as _Formatter
 from typing import Any as _Any
+from typing import NamedTuple as _NamedTuple
 
 OPTIONAL_BLOCK_START_DELIMITER = "["
 _START = OPTIONAL_BLOCK_START_DELIMITER
 OPTIONAL_BLOCK_END_DELIMITER = "]"
 _END = OPTIONAL_BLOCK_END_DELIMITER
 
 
+class ParseBlockResult(_NamedTuple):
+    """Output type of :meth:`.Element.parse_block`."""
+
+    parsed_block: str
+    """Processed parts of the block."""
+    placeholders: list[str]
+    """Names of the :attr:`.Format.placeholders` in `parsed_block`, in the order in which they appear."""
+
+
 class MalformedOptionalBlockError(ValueError):
     """Error raised for improper optional blocks."""
 
     @staticmethod
     def get_marker_row(format_string: str, open_idx: int = -1, idx: int = -1) -> str:
         """Get a string of length equal to `format_string` which marks problem locations."""
         markers = [" "] * len(format_string)
@@ -79,54 +89,100 @@
             in_optional_block: Flag indicating whether `s` was found inside an optional block.
 
         Returns:
             A new ``Element``.
         """
         block = fmt
         fmt = block.replace("[[", "[").replace("]]", "]")
-        # block = block.replace("{{", "{").replace("}}", "}")
-        parts, placeholders = cls.parse_block(fmt)
 
-        return Element(fmt, placeholders, not (placeholders and in_optional_block), "".join(parts))
+        positional_part, placeholders = cls.parse_block(fmt)
+        is_optional = placeholders and in_optional_block
+
+        return Element(fmt, placeholders, required=not is_optional, positional_part=positional_part)
 
     @classmethod
-    def parse_block(cls, block: str, defaults: _abc.Mapping[str, _Any] | None = None) -> tuple[list[str], list[str]]:
+    def parse_block(cls, block: str, defaults: _abc.Mapping[str, _Any] | None = None) -> ParseBlockResult:
         """Parse an entire block with optional defaults for placeholders found.
 
-        Using `defaults`:
-            Keys in `defaults` will replace placeholders in the block. That is, the returned placeholders are guaranteed
-            not to contain any keys in the `defaults`. Passing defaults will retain placeholder names in the returned
-            `parts`.
+        .. hint::
+
+           With `defaults`, the value of the :attr:`ParseBlockResult.parsed_block` is more or less what you'd expect if
+           the built-in :py:meth:`str.format_map`-method allowed missing keys.
+
+        Anonymous fields are not permitted.
+
+        ..
+           >>> from uuid import UUID
+
+        Output with ``defaults == None``:
+            When `defaults` are ``None``, placeholder names are stripped from the
+            :attr:`~.ParseBlockResult.parsed_block`.
 
-        If `defaults` are not given, placeholder values are strip from returned `parts`.
+            >>> block, placeholders = Element.parse_block("{id!s:.8}:{name!r}")
+            >>> print(f"{block=} has {placeholders=}")
+            block='{!s:.8}:{!r}' has placeholders=['id', 'name']
+
+            Field names in `block` are returned as :attr:`.ParseBlockResult.placeholders`, in the order in which they
+            appeared in the input `block`. The field names of :attr:`~.ParseBlockResult.parsed_block` will be
+            anonymous.
+
+            >>> block.format(UUID(int=10**38), "Morran Borran")
+            "4b3b4ca8:'Morran Borran'"
+
+        Output with ``defaults != None``:
+            When `defaults` are given, all placeholders in the `block` which are present in the `defaults` are replaced
+            with ``defaults[field_name]`` in the :attr:`~.ParseBlockResult.parsed_block`.
+
+            >>> block, placeholders = Element.parse_block(
+            ...     "{id!s:.8}:{name!r}",
+            ...     defaults={"name": "Morran Borran"},
+            ... )
+            >>> print(f"{block=} has {placeholders=}")
+            block="{id!s:.8}:'Morran Borran'" has placeholders=['id']
+
+            Field names without defaults will be present both in :attr:`~.ParseBlockResult.placeholders`, and as named
+            fields in the :attr:`~.ParseBlockResult.parsed_block`.
+
+            >>> block.format(id=UUID(int=10**38))
+            "4b3b4ca8:'Morran Borran'"
 
         Args:
             block: A block to parse.
             defaults: A dict ``{placeholder: value}``.
 
         Returns:
-            A tuple of two lists ``([positional_parts...], [placeholders...])``.
+            A :class:`.ParseBlockResult` tuple.
+
+        Raises:
+            ValueError: If `block` contains anonymous fields.
         """
         if defaults is None:
             defaults = {}
-            positional = True
+            keep_placeholder_names = False
         else:
-            positional = False
+            keep_placeholder_names = True
 
         parts = []
         placeholders = []
 
         # Optional block backtracking
         replaced_parts_index = []
         placeholders_index = []
 
         formatter = _Formatter()
 
         for literal_text, field_name, format_spec, conversion in formatter.parse(block):
             parts.append(literal_text.replace("{", "{{").replace("}", "}}"))
+
+            if field_name == "":
+                msg = f"Bad {block=}; anonymous fields are not permitted."
+                msg += "\n- Hint: Replace '{}' with '{field_name}' to give this field a name"
+                msg += "\n- Hint: Replace '{}' with '{{}}' to render literal curly braces"
+                raise ValueError(msg)
+
             if field_name:
                 placeholder, _, attribute = field_name.partition(".")
                 formatting_parts = _get_formatting_parts(
                     attribute=attribute, conversion=conversion, format_spec=format_spec
                 )
 
                 if placeholder in defaults:
@@ -134,22 +190,22 @@
                     formatting = "".join(["{", *formatting_parts, "}"])
                     value = defaults[placeholder]
                     parts.append(formatting.format(value))
                 else:
                     parts.append("{")
 
                     placeholders.append(placeholder)
-                    if not positional:
+                    if keep_placeholder_names:
                         placeholders_index.append(len(parts))
                         parts.append(placeholder)
 
                     parts.extend(formatting_parts)
                     parts.append("}")
 
-        return parts, placeholders
+        return ParseBlockResult("".join(parts), placeholders=placeholders)
 
 
 def _get_delimiter_index(part: str, *, start: bool) -> int | None:
     def _exec(func: _abc.Callable[[str], int], sign: str) -> int | None:
         try:
             return func(sign)
         except ValueError:
```

### Comparing `id_translation-0.8.0/src/id_translation/offline/types.py` & `id_translation-0.9.0/src/id_translation/offline/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/settings.py` & `id_translation-0.9.0/src/id_translation/settings.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/testing.py` & `id_translation-0.9.0/src/id_translation/testing.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/transform/_impl/bitmask.py` & `id_translation-0.9.0/src/id_translation/transform/_impl/bitmask.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/transform/types.py` & `id_translation-0.9.0/src/id_translation/transform/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/types.py` & `id_translation-0.9.0/src/id_translation/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,23 @@
 
 Rules of thumb
 --------------
 * The :attr:`IdTypes` are the only `"truly"` translatable types. Collections thereof are also supported.
 * Non-inplace (copy-translation, default) always `tries` to return a collection of the same type, with all
   :attr:`IdTypes` converted to :py:class:`str`.
 * In-place translation always returns ``None``, or raises :class:`~.dio.exceptions.NotInplaceTranslatableError`.
-* When ``default_fmt=None``, IDs may be replaced by ``None`` as well (contrary to type hints).
-* Translating with ``maximal_untranslated_fraction=0`` guarantees that IDs are never replaced with ``None``.
 
 Overloads err on the overly-permissive side. Static type checkers (only MyPy is tested) may incorrectly allow things
 like ``translator.translate("a-string-id")`` for ``int``-only ``Translator`` instances.
 
 Limitations
 -----------
 Python does not support generics-of-generics, which is the primary domain in which the ``Translator.translate``-method
 operates. See https://github.com/python/typing/issues/548 for details on this subject.
 
-* Reverse-mode translation (``reverse=True``) is not type-hinted.
 * Numpy is supported, but not typed.
 * Pandas typing must be enabled using the ``ID_TRANSLATION_PANDAS_IS_TYPED``-flag.
 
 .. code-block:: console
 
    pip install pandas-stubs
    mypy --always-true=ID_TRANSLATION_PANDAS_IS_TYPED /path/to/file.py
```

### Comparing `id_translation-0.8.0/src/id_translation/utils/_base_metadata.py` & `id_translation-0.9.0/src/id_translation/utils/_base_metadata.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/utils/_config_utils.py` & `id_translation-0.9.0/src/id_translation/utils/_config_utils.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/utils/_load_toml.py` & `id_translation-0.9.0/src/id_translation/utils/_load_toml.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/src/id_translation/utils/logging.py` & `id_translation-0.9.0/src/id_translation/utils/logging.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.8.0/PKG-INFO` & `id_translation-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id-translation
-Version: 0.8.0
+Version: 0.9.0
 Summary: Convert IDs into human-readable labels.
 Home-page: https://github.com/rsundqvist/id-translation
 Keywords: id-translation
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.11,<4
 Classifier: Development Status :: 4 - Beta
@@ -52,15 +52,15 @@
 
 ## What is it?
 A package suite for translating integer IDs typically found in databases. Translation is highly configurable and tested
 for multiple different SQL dialects and schema naming paradigms. The included TOML configuration format as well as the
 support functions make it easy to create and share working configurations with anyone who needs them.
 
 # Cookiecutter template project
-The fastest way to get started with `id-translation` is the 🍪[id-translation-project] cookiecutter template. It is
+The fastest way to get started with `id-translation` is the 🍪[id-translation-project] Cookiecutter template. It is
 designed to allow power users to quickly specify shared configurations that "just work" for other users; see the example
 below.
 
 ```python
 from big_corporation_inc.id_translation import translate
 print(
   "The first employee at Big Corporation Inc. was:", 
@@ -71,31 +71,37 @@
 Check out this [demo project](https://github.com/rsundqvist/id-translation-project/tree/master/demo/bci-id-translation)
 (and its 📚[generated documentation](https://rsundqvist.github.io/id-translation-project/)) to get a preview of what 
 Your generated project might look like, or continue to the next section for a brief feature overview.
 
 [id-translation-project]: https://github.com/rsundqvist/id-translation-project/
 
 # Highlighted Features
-- Support for ``int`` and ``string`` IDs, including ``UUID``-like types.
-- Translation of [pandas types][pandas-translation], including `pandas.Index` types.
-- Intuitive [Format strings][format], with support for optional elements.
-- Powerful automated [Name-to-source][n2s-mapping] and [Format placeholder][pm-mapping] mapping.
-- Prebuilt fetchers for [SQL][sql-fetcher] and [file-system][pandas-fetcher] sources.
-- Configure using [TOML][translator-config], support for [persistent] instances stored on disk.
+- Intuitive [Format strings] (modern `'{id}:{name}'` syntax), including support for
+  [Format Specification Mini-Language] features and extensions for optional keys.
+- Fetchers for [SQL] and local or remote [file-system] sources.
+- Powerful [Name-to-source] and [Placeholder-to-column] mapping and name extraction.
+- Configurable using [TOML] - see the 🍪[id-translation-project] Cookiecutter template.
+- Highly configurable interface: [Translator.translate()].
+
+[Format strings]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.offline.html#id_translation.offline.Format
+[Format Specification Mini-Language]: https://docs.python.org/3/library/string.html#formatspec
+[SQL]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.SqlFetcher
+[file-system]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.PandasFetcher
+[Name-to-source]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#name-to-source-mapping
+[Placeholder-to-column]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#placeholder-mapping
+[TOML]: https://id-translation.readthedocs.io/en/stable/documentation/translator-config.html
+[cached instances]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.load_persistent_instance.html
+[Translator.translate()]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.translate.html
+
+## Supported types
+- Supported ID types: `int`, `string`, and `UUID`.
+- Supports translation of build-in collections: `list`, `dict`, `set`, `tuple`.
+- Supports translation of [pandas types][pandas-translation], including `pandas.MultiIndex` types.
 
 [pandas-translation]: https://id-translation.readthedocs.io/en/stable/documentation/examples/notebooks/cookbook/pandas-index.html
-[translate]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.translate.html
-[format]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.offline.html#id_translation.offline.Format
-[n2s-mapping]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#name-to-source-mapping
-[pm-mapping]: https://id-translation.readthedocs.io/en/stable/documentation/translation-primer.html#placeholder-mapping
-[persistent]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.Translator.load_persistent_instance.html
-[sql-fetcher]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.SqlFetcher
-[pandas-fetcher]: https://id-translation.readthedocs.io/en/stable/_autosummary/id_translation.fetching.html#id_translation.fetching.PandasFetcher
-[translator-config]: https://id-translation.readthedocs.io/en/stable/documentation/translator-config.html
-
 
 # Installation
 The package is published through the [Python Package Index (PyPI)]. Source code
 is available on GitHub: https://github.com/rsundqvist/id-translation
 
 ```sh
 pip install -U id-translation
```

