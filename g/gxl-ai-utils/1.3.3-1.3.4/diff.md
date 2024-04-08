# Comparing `tmp/gxl_ai_utils-1.3.3.tar.gz` & `tmp/gxl_ai_utils-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxl_ai_utils-1.3.3.tar", last modified: Tue Mar 19 12:17:05 2024, max compression
+gzip compressed data, was "gxl_ai_utils-1.3.4.tar", last modified: Mon Apr  8 18:32:05 2024, max compression
```

## Comparing `gxl_ai_utils-1.3.3.tar` & `gxl_ai_utils-1.3.4.tar`

### file list

```diff
@@ -1,388 +1,513 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.557261 gxl_ai_utils-1.3.3/
--rw-rw-rw-   0        0        0      212 2024-03-19 12:17:05.555293 gxl_ai_utils-1.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.607067 gxl_ai_utils-1.3.3/eggs/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.614668 gxl_ai_utils-1.3.3/eggs/aishell/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/aishell/__init__.py
--rw-rw-rw-   0        0        0      238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/aishell/do_infer.py
--rw-rw-rw-   0        0        0     1262 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/aishell/do_train.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.617041 gxl_ai_utils-1.3.3/eggs/asr_handle_to_tts_mode/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_handle_to_tts_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.625033 gxl_ai_utils-1.3.3/eggs/asr_handle_to_tts_mode/punctuation/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_handle_to_tts_mode/punctuation/__init__.py
--rw-rw-rw-   0        0        0     5134 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.661919 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/__init__.py
--rw-rw-rw-   0        0        0     1002 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_gigaspeech.py
--rw-rw-rw-   0        0        0      693 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_haoweilai.py
--rw-rw-rw-   0        0        0     1316 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_librispeech.py
--rw-rw-rw-   0        0        0     1037 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_mls.py
--rw-rw-rw-   0        0        0     1702 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/make_shard.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.672890 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.689845 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.694073 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 07:29:51.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/__init__.py
--rw-rw-rw-   0        0        0    17684 2024-03-17 08:35:12.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py
--rw-rw-rw-   0        0        0    25266 2024-02-29 05:24:42.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py
--rw-rw-rw-   0        0        0    25267 2024-03-09 13:06:04.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py
--rw-rw-rw-   0        0        0    24364 2024-03-05 08:12:26.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py
--rw-rw-rw-   0        0        0    26215 2024-02-29 05:24:42.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.701085 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/__init__.py
--rw-rw-rw-   0        0        0    17693 2024-03-17 09:27:53.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.705805 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/__init__.py
--rw-rw-rw-   0        0        0    17721 2024-03-17 09:57:21.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py
--rw-rw-rw-   0        0        0     3396 2024-03-06 13:40:40.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/make_shard.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.710081 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/__init__.py
--rw-rw-rw-   0        0        0    18376 2024-03-18 06:39:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.720228 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/__init__.py
--rw-rw-rw-   0        0        0    18374 2024-03-17 08:50:53.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.723757 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/__init__.py
--rw-rw-rw-   0        0        0    18529 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.726748 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/__init__.py
--rw-rw-rw-   0        0        0    18757 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.732735 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/__init__.py
--rw-rw-rw-   0        0        0    17630 2024-03-18 06:55:25.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.737720 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/__init__.py
--rw-rw-rw-   0        0        0    20020 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.740709 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_3/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_3/__init__.py
--rw-rw-rw-   0        0        0    16046 2024-03-17 07:56:10.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_3/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.748975 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/__init__.py
--rw-rw-rw-   0        0        0    17748 2024-03-17 10:02:42.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py
--rw-rw-rw-   0        0        0       88 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/main.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.762653 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/__init__.py
--rw-rw-rw-   0        0        0     5838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py
--rw-rw-rw-   0        0        0     9569 2024-02-22 05:44:59.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py
--rw-rw-rw-   0        0        0      962 2024-02-25 03:33:09.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py
--rw-rw-rw-   0        0        0      625 2024-03-18 06:52:14.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.766965 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_fairseq/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_fairseq/__init__.py
--rw-rw-rw-   0        0        0    13907 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.772161 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.778609 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py
--rw-rw-rw-   0        0        0     6851 2024-02-22 07:15:14.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py
--rw-rw-rw-   0        0        0     3385 2024-03-17 16:49:11.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.786147 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_TYPE_CHECKING/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_TYPE_CHECKING/__init__.py
--rw-rw-rw-   0        0        0      256 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_TYPE_CHECKING/fun.py
--rw-rw-rw-   0        0        0      125 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_TYPE_CHECKING/test.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.802744 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/__init__.py
--rw-rw-rw-   0        0        0      232 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/download_test.py
--rw-rw-rw-   0        0        0      793 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py
--rw-rw-rw-   0        0        0      503 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/gxl_test.py
--rw-rw-rw-   0        0        0      746 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/main.py
--rw-rw-rw-   0        0        0      400 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/test.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.805860 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_sentencepiece/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_sentencepiece/__init__.py
--rw-rw-rw-   0        0        0     1781 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_sentencepiece/main.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.812842 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/ximalaya/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/ximalaya/__init__.py
--rw-rw-rw-   0        0        0     2525 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/cats_and_dogs/ximalaya/main.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.815000 gxl_ai_utils-1.3.3/eggs/ch_en_mix/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/ch_en_mix/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.816973 gxl_ai_utils-1.3.3/eggs/ch_en_mix/data_handle/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/ch_en_mix/data_handle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.827924 gxl_ai_utils-1.3.3/eggs/finetune_llm/
--rw-rw-rw-   0        0        0        0 2024-02-29 06:01:16.000000 gxl_ai_utils-1.3.3/eggs/finetune_llm/__init__.py
--rw-rw-rw-   0        0        0      928 2024-03-13 02:52:18.000000 gxl_ai_utils-1.3.3/eggs/finetune_llm/main.py
--rw-rw-rw-   0        0        0     1858 2024-03-13 07:52:36.000000 gxl_ai_utils-1.3.3/eggs/finetune_llm/main_2B.py
--rw-rw-rw-   0        0        0     1367 2024-03-13 07:36:12.000000 gxl_ai_utils-1.3.3/eggs/finetune_llm/transformers_learning.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.870650 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/__init__.py
--rw-rw-rw-   0        0        0     1635 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/gxl_knowledge_distill.py
--rw-rw-rw-   0        0        0     1129 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/gxl_paraformer_infer.py
--rw-rw-rw-   0        0        0     2469 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/gxl_whisper_infer.py
--rw-rw-rw-   0        0        0     1090 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/handle_cmvn_gxl.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.876610 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer/decoder.py
--rw-rw-rw-   0        0        0    27385 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer/encoder.py
--rw-rw-rw-   0        0        0      827 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer_infer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.880804 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/whisper_ctc/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/whisper_ctc/__init__.py
--rw-rw-rw-   0        0        0      741 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/knowledge_distillation/whisper_ctc/main.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.913977 gxl_ai_utils-1.3.3/eggs/spider/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/__init__.py
--rw-rw-rw-   0        0        0      382 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spdier_little_url_get.py
--rw-rw-rw-   0        0        0     9274 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_lizhi_fm.py
--rw-rw-rw-   0        0        0     5810 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_qingting_fm.py
--rw-rw-rw-   0        0        0    16395 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_qingting_fm_new.py
--rw-rw-rw-   0        0        0    14467 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_ximalaya.py
--rw-rw-rw-   0        0        0    10475 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_ximalaya_new.py
--rw-rw-rw-   0        0        0     7041 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_yunting.py
--rw-rw-rw-   0        0        0     4983 2024-02-25 08:28:39.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_zhihu.py
--rw-rw-rw-   0        0        0     4770 2024-02-25 08:26:09.000000 gxl_ai_utils-1.3.3/eggs/spider/spider_zhihu_2.py
--rw-rw-rw-   0        0        0     3479 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/eggs/spider/test.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.923622 gxl_ai_utils-1.3.3/gxl_ai_utils/
--rw-rw-rw-   0        0        0     1651 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/AiConstant.py
--rw-rw-rw-   0        0        0      556 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.965378 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/
--rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/__init__.py
--rw-rw-rw-   0        0        0    14863 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/build_vocab.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.969385 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/classify/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/classify/__init__.py
--rw-rw-rw-   0        0        0     5401 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/classify/data_handler.py
--rw-rw-rw-   0        0        0     6562 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/common_data_handler.py
--rw-rw-rw-   0        0        0     6242 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/gxl_data_handler.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.973396 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/recognition/
--rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/recognition/__init__.py
--rw-rw-rw-   0        0        0    10901 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/recognition/data_handler.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.974353 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_handler/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.978653 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/
--rw-rw-rw-   0        0        0       36 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.986325 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/classify/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/classify/__init__.py
--rw-rw-rw-   0        0        0    17914 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py
--rw-rw-rw-   0        0        0    27764 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/classify/xvector.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.988966 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/
--rw-rw-rw-   0        0        0       50 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.993303 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/deepspeech2/
--rw-rw-rw-   0        0        0       25 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/deepspeech2/__init__.py
--rw-rw-rw-   0        0        0    14593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.003284 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/__init__.py
--rw-rw-rw-   0        0        0     6869 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py
--rw-rw-rw-   0        0        0     5452 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/embedding.py
--rw-rw-rw-   0        0        0     8872 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/subsampling.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.008439 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.018246 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.033196 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/__init__.py
--rw-rw-rw-   0        0        0     1942 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py
--rw-rw-rw-   0        0        0     1662 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py
--rw-rw-rw-   0        0        0      936 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py
--rw-rw-rw-   0        0        0     1193 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py
--rw-rw-rw-   0        0        0     3050 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py
--rw-rw-rw-   0        0        0     2386 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.047159 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/utils/__init__.py
--rw-rw-rw-   0        0        0      569 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py
--rw-rw-rw-   0        0        0      427 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/utils/sequence_mask.py
--rw-rw-rw-   0        0        0     1305 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/transformer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.059142 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/utils/__init__.py
--rw-rw-rw-   0        0        0    14807 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.062120 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/t2s/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/t2s/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.067105 gxl_ai_utils-1.3.3/gxl_ai_utils/config/
--rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/config/__init__.py
--rw-rw-rw-   0        0        0     5179 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/config/gxl_config.py
--rw-rw-rw-   0        0        0      121 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.079190 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_dataset_wenet/
--rw-rw-rw-   0        0        0        2 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_dataset_wenet/__init__.py
--rw-rw-rw-   0        0        0     7429 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py
--rw-rw-rw-   0        0        0    18215 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.132398 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/__init__.py
--rw-rw-rw-   0        0        0    10270 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/alignment.py
--rw-rw-rw-   0        0        0     3616 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/average_model.py
--rw-rw-rw-   0        0        0     5604 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py
--rw-rw-rw-   0        0        0    12155 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/recognize.py
--rw-rw-rw-   0        0        0    12797 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.138497 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_lr_scheduler_wenet/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_lr_scheduler_wenet/__init__.py
--rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.143975 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.153578 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/__init__.py
--rw-rw-rw-   0        0        0     6645 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py
--rw-rw-rw-   0        0        0    16717 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py
--rw-rw-rw-   0        0        0    10038 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.156319 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/cif/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/cif/__init__.py
--rw-rw-rw-   0        0        0    11275 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/cif/predictor.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.165293 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/e_branchformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/e_branchformer/__init__.py
--rw-rw-rw-   0        0        0    16682 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py
--rw-rw-rw-   0        0        0     6840 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.179257 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/__init__.py
--rw-rw-rw-   0        0        0    11117 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py
--rw-rw-rw-   0        0        0     5905 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py
--rw-rw-rw-   0        0        0    26376 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py
--rw-rw-rw-   0        0        0     7093 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py
--rw-rw-rw-   0        0        0     2749 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py
--rw-rw-rw-   0        0        0     7413 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/init_model.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.183246 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/k2/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/k2/__init__.py
--rw-rw-rw-   0        0        0    11851 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/k2/model.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.199863 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/__init__.py
--rw-rw-rw-   0        0        0     8230 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py
--rw-rw-rw-   0        0        0    11269 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py
--rw-rw-rw-   0        0        0     5301 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py
--rw-rw-rw-   0        0        0    17521 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py
--rw-rw-rw-   0        0        0     9883 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py
--rw-rw-rw-   0        0        0     6945 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/search.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.221144 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/__init__.py
--rw-rw-rw-   0        0        0    10509 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py
--rw-rw-rw-   0        0        0     2636 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py
--rw-rw-rw-   0        0        0     6713 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py
--rw-rw-rw-   0        0        0    22398 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py
--rw-rw-rw-   0        0        0     4833 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py
--rw-rw-rw-   0        0        0     3067 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py
--rw-rw-rw-   0        0        0    11264 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.232136 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/__init__.py
--rw-rw-rw-   0        0        0     4110 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/joint.py
--rw-rw-rw-   0        0        0    18089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.243149 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/search/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/search/__init__.py
--rw-rw-rw-   0        0        0     2014 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py
--rw-rw-rw-   0        0        0     6112 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py
--rw-rw-rw-   0        0        0    23241 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.295585 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/__init__.py
--rw-rw-rw-   0        0        0    18961 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py
--rw-rw-rw-   0        0        0    14383 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/attention.py
--rw-rw-rw-   0        0        0     1533 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py
--rw-rw-rw-   0        0        0     5329 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py
--rw-rw-rw-   0        0        0     3084 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py
--rw-rw-rw-   0        0        0    12855 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py
--rw-rw-rw-   0        0        0     4939 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py
--rw-rw-rw-   0        0        0     6339 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py
--rw-rw-rw-   0        0        0    20622 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py
--rw-rw-rw-   0        0        0     9838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py
--rw-rw-rw-   0        0        0     3806 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/paraformer_encoder.py
--rw-rw-rw-   0        0        0     1940 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py
--rw-rw-rw-   0        0        0    18309 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/search.py
--rw-rw-rw-   0        0        0     9512 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py
--rw-rw-rw-   0        0        0     1029 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/swish.py
--rw-rw-rw-   0        0        0     6294 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py
--rw-rw-rw-   0        0        0     8366 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py
--rw-rw-rw-   0        0        0     2582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.340171 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/__init__.py
--rw-rw-rw-   0        0        0     4018 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py
--rw-rw-rw-   0        0        0     3065 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py
--rw-rw-rw-   0        0        0     7954 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/common.py
--rw-rw-rw-   0        0        0     1516 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/config.py
--rw-rw-rw-   0        0        0     9964 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py
--rw-rw-rw-   0        0        0     5411 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py
--rw-rw-rw-   0        0        0     4353 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/executor.py
--rw-rw-rw-   0        0        0     2168 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py
--rw-rw-rw-   0        0        0     1291 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py
--rw-rw-rw-   0        0        0     7440 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/init_model.py
--rw-rw-rw-   0        0        0    13020 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/mask.py
--rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py
--rw-rw-rw-   0        0        0     1568 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py
--rw-rw-rw-   0        0        0    26574 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.355217 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/__init__.py
--rw-rw-rw-   0        0        0    14805 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/attentions.py
--rw-rw-rw-   0        0        0     4860 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/commons.py
--rw-rw-rw-   0        0        0    24767 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/models.py
--rw-rw-rw-   0        0        0    16740 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/modules.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.359298 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_trainer_wenet/
--rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_trainer_wenet/__init__.py
--rw-rw-rw-   0        0        0     9889 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.391693 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/
--rw-rw-rw-   0        0        0     7061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/__init__.py
--rw-rw-rw-   0        0        0       38 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/__main__.py
--rw-rw-rw-   0        0        0     5089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/audio.py
--rw-rw-rw-   0        0        0    33001 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/decoding.py
--rw-rw-rw-   0        0        0    11165 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/model.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.401800 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/normalizers/
--rw-rw-rw-   0        0        0      132 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/normalizers/__init__.py
--rw-rw-rw-   0        0        0     2012 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/normalizers/basic.py
--rw-rw-rw-   0        0        0    21418 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/normalizers/english.py
--rw-rw-rw-   0        0        0    12968 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/timing.py
--rw-rw-rw-   0        0        0    12733 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/tokenizer.py
--rw-rw-rw-   0        0        0    23334 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/transcribe.py
--rw-rw-rw-   0        0        0     3583 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/triton_ops.py
--rw-rw-rw-   0        0        0    11363 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/utils.py
--rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/version.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.404809 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.406686 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.415729 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/encoder/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/encoder/__init__.py
--rw-rw-rw-   0        0        0      414 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/encoder/abs_encoder.py
--rw-rw-rw-   0        0        0     9977 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.420754 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/fastformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/fastformer/__init__.py
--rw-rw-rw-   0        0        0     2297 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/fastformer/fastformer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.437862 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/__init__.py
--rw-rw-rw-   0        0        0    19543 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py
--rw-rw-rw-   0        0        0   102558 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py
--rw-rw-rw-   0        0        0    79092 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py
--rw-rw-rw-   0        0        0    58681 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.452522 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/__init__.py
--rw-rw-rw-   0        0        0     6478 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/component.py
--rw-rw-rw-   0        0        0     2953 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/decoder.py
--rw-rw-rw-   0        0        0     2299 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/encoder.py
--rw-rw-rw-   0        0        0     1405 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/transformer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.467311 gxl_ai_utils-1.3.3/gxl_ai_utils/run/
--rw-rw-rw-   0        0        0       22 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/__init__.py
--rw-rw-rw-   0        0        0     9326 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/base_train_runner.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.477646 gxl_ai_utils-1.3.3/gxl_ai_utils/run/flask_template/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/flask_template/__init__.py
--rw-rw-rw-   0        0        0     1061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/flask_template/flask_predict.py
--rw-rw-rw-   0        0        0     4263 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/flask_template/flask_server.py
--rw-rw-rw-   0        0        0     3023 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/runner.py
--rw-rw-rw-   0        0        0     2602 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/runner_multi_template.py
--rw-rw-rw-   0        0        0      593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/run/runner_single_template.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.491237 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/
--rw-rw-rw-   0        0        0       76 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/__init__.py
--rw-rw-rw-   0        0        0     4311 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_data.py
--rw-rw-rw-   0        0        0      177 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_data_name.py
--rw-rw-rw-   0        0        0      451 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_dataloader.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.496300 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_dataset/
--rw-rw-rw-   0        0        0       29 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_dataset/__init__.py
--rw-rw-rw-   0        0        0     5238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_dataset/store_dataset.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.507383 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/
--rw-rw-rw-   0        0        0       64 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/__init__.py
--rw-rw-rw-   0        0        0     2072 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.525686 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/
--rw-rw-rw-   0        0        0       33 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/__init__.py
--rw-rw-rw-   0        0        0     6223 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/attention_model.py
--rw-rw-rw-   0        0        0     2438 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/cnn_model.py
--rw-rw-rw-   0        0        0      958 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/mlp_model.py
--rw-rw-rw-   0        0        0     2130 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/rnn_model.py
--rw-rw-rw-   0        0        0     2348 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/store_model_class.py
--rw-rw-rw-   0        0        0      578 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_name.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.529823 gxl_ai_utils-1.3.3/gxl_ai_utils/thread/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/thread/__init__.py
--rw-rw-rw-   0        0        0     1522 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/thread/my_thread.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:05.553266 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/
--rw-rw-rw-   0        0        0       80 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_coding.py
--rw-rw-rw-   0        0        0    26659 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_data.py
--rw-rw-rw-   0        0        0      423 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_device.py
--rw-rw-rw-   0        0        0    40545 2024-03-19 12:10:33.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_file.py
--rw-rw-rw-   0        0        0     6520 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_model.py
--rw-rw-rw-   0        0        0     1655 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_showing.py
--rw-rw-rw-   0        0        0     6741 2024-02-25 07:54:16.000000 gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_spider.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:17:04.957418 gxl_ai_utils-1.3.3/gxl_ai_utils.egg-info/
--rw-rw-rw-   0        0        0      212 2024-03-19 12:17:03.000000 gxl_ai_utils-1.3.3/gxl_ai_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14947 2024-03-19 12:17:04.000000 gxl_ai_utils-1.3.3/gxl_ai_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 12:17:03.000000 gxl_ai_utils-1.3.3/gxl_ai_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-19 12:17:03.000000 gxl_ai_utils-1.3.3/gxl_ai_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.3/license.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 12:17:05.557427 gxl_ai_utils-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      519 2024-03-19 12:11:43.000000 gxl_ai_utils-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.131513 gxl_ai_utils-1.3.4/
+-rw-rw-rw-   0        0        0      211 2024-04-08 18:32:05.129115 gxl_ai_utils-1.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.064387 gxl_ai_utils-1.3.4/eggs/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.067226 gxl_ai_utils-1.3.4/eggs/aishell/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/aishell/__init__.py
+-rw-rw-rw-   0        0        0      238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/aishell/do_infer.py
+-rw-rw-rw-   0        0        0     1262 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/aishell/do_train.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.069220 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.077203 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/__init__.py
+-rw-rw-rw-   0        0        0     5134 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.085177 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/__init__.py
+-rw-rw-rw-   0        0        0     1002 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_gigaspeech.py
+-rw-rw-rw-   0        0        0      693 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_haoweilai.py
+-rw-rw-rw-   0        0        0     1316 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_librispeech.py
+-rw-rw-rw-   0        0        0     1037 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_mls.py
+-rw-rw-rw-   0        0        0     1702 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/make_shard.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.091161 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.105525 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.110176 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/__init__.py
+-rw-rw-rw-   0        0        0    19681 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.113176 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/__init__.py
+-rw-rw-rw-   0        0        0    21823 2024-03-29 09:10:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.116160 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/__init__.py
+-rw-rw-rw-   0        0        0    19582 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.122144 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/__init__.py
+-rw-rw-rw-   0        0        0    19589 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.126136 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/__init__.py
+-rw-rw-rw-   0        0        0    22007 2024-03-29 09:10:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.129125 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/__init__.py
+-rw-rw-rw-   0        0        0    15667 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.131120 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/__init__.py
+-rw-rw-rw-   0        0        0    23624 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.138100 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/__init__.py
+-rw-rw-rw-   0        0        0    19465 2024-03-23 15:34:56.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.142091 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/__init__.py
+-rw-rw-rw-   0        0        0    21395 2024-03-26 06:24:07.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/do_handle.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.144085 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 07:29:51.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/__init__.py
+-rw-rw-rw-   0        0        0    17684 2024-03-17 08:35:12.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py
+-rw-rw-rw-   0        0        0    25266 2024-02-29 05:24:42.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py
+-rw-rw-rw-   0        0        0    25267 2024-03-09 13:06:04.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py
+-rw-rw-rw-   0        0        0    24364 2024-03-05 08:12:26.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py
+-rw-rw-rw-   0        0        0    26215 2024-02-29 05:24:42.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py
+-rw-rw-rw-   0        0        0     2878 2024-03-23 18:03:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_remove.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.149071 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/
+-rw-rw-rw-   0        0        0        0 2024-03-26 08:17:34.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/__init__.py
+-rw-rw-rw-   0        0        0    10187 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/common_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.156230 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/__init__.py
+-rw-rw-rw-   0        0        0    17693 2024-03-17 09:27:53.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.160043 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/__init__.py
+-rw-rw-rw-   0        0        0    17721 2024-03-17 09:57:21.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py
+-rw-rw-rw-   0        0        0     1053 2024-04-01 05:20:49.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/make_shard.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.164106 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/__init__.py
+-rw-rw-rw-   0        0        0    18376 2024-03-18 06:39:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.171046 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/__init__.py
+-rw-rw-rw-   0        0        0    18374 2024-03-17 08:50:53.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.174005 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/__init__.py
+-rw-rw-rw-   0        0        0    18529 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.178205 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/__init__.py
+-rw-rw-rw-   0        0        0    18757 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.181984 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/__init__.py
+-rw-rw-rw-   0        0        0    17630 2024-03-18 06:55:25.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.188061 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/__init__.py
+-rw-rw-rw-   0        0        0    20020 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.191013 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/__init__.py
+-rw-rw-rw-   0        0        0    17748 2024-03-17 10:02:42.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.196944 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/
+-rw-rw-rw-   0        0        0        0 2024-03-26 11:48:19.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/__init__.py
+-rw-rw-rw-   0        0        0     5564 2024-04-08 17:21:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/compute_fbank_common.py
+-rw-rw-rw-   0        0        0    11494 2024-04-02 02:44:33.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/icefall_assistant.py
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:22:09.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zip_trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.317709 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:19:27.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/__init__.py
+-rw-rw-rw-   0        0        0    13605 2024-03-27 07:54:26.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/asr_datamodule.py
+-rw-rw-rw-   0        0        0   109372 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/beam_search.py
+-rw-rw-rw-   0        0        0    27050 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode.py
+-rw-rw-rw-   0        0        0    27656 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_bbpe.py
+-rw-rw-rw-   0        0        0     5331 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_stream.py
+-rw-rw-rw-   0        0        0     4755 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decoder.py
+-rw-rw-rw-   0        0        0     1652 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/encoder_interface.py
+-rw-rw-rw-   0        0        0    25164 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx-streaming.py
+-rw-rw-rw-   0        0        0    18723 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx.py
+-rw-rw-rw-   0        0        0    17410 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.376497 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/
+-rw-rw-rw-   0        0        0     1402 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/__init__.py
+-rw-rw-rw-   0        0        0     4780 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ali.py
+-rw-rw-rw-   0        0        0     2991 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/bpe_graph_compiler.py
+-rw-rw-rw-   0        0        0     4044 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/byte_utils.py
+-rw-rw-rw-   0        0        0     3436 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/char_graph_compiler.py
+-rw-rw-rw-   0        0        0    15166 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/checkpoint.py
+-rw-rw-rw-   0        0        0    22548 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/context_graph.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.389310 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/
+-rw-rw-rw-   0        0        0      187 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/prepare_lang.py
+-rw-rw-rw-   0        0        0     3868 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_ctc_topo.py
+-rw-rw-rw-   0        0        0     1100 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_prepare_lang.py
+-rw-rw-rw-   0        0        0     4628 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/topo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.393355 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/
+-rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2002 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/datamodule.py
+-rw-rw-rw-   0        0        0    44213 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/decode.py
+-rw-rw-rw-   0        0        0    27288 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/diagnostics.py
+-rw-rw-rw-   0        0        0     1966 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dist.py
+-rw-rw-rw-   0        0        0     3472 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/env.py
+-rw-rw-rw-   0        0        0     5508 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/graph_compiler.py
+-rw-rw-rw-   0        0        0     3580 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/hooks.py
+-rw-rw-rw-   0        0        0     8723 2024-03-28 08:19:43.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lexicon.py
+-rw-rw-rw-   0        0        0     7821 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lm_wrapper.py
+-rw-rw-rw-   0        0        0     6644 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi.py
+-rw-rw-rw-   0        0        0     7859 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi_graph_compiler.py
+-rw-rw-rw-   0        0        0     5295 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ngram_lm.py
+-rw-rw-rw-   0        0        0     8205 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/otc_graph_compiler.py
+-rw-rw-rw-   0        0        0    30754 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/profiler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.421758 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/
+-rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/__init__.py
+-rw-rw-rw-   0        0        0     3644 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx-streaming.py
+-rw-rw-rw-   0        0        0     3205 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx.py
+-rw-rw-rw-   0        0        0     7275 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/compute_perplexity.py
+-rw-rw-rw-   0        0        0     7647 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/dataset.py
+-rw-rw-rw-   0        0        0    11547 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export-onnx.py
+-rw-rw-rw-   0        0        0     5747 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export.py
+-rw-rw-rw-   0        0        0    10312 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/model.py
+-rw-rw-rw-   0        0        0     2238 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset.py
+-rw-rw-rw-   0        0        0     2977 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset_ddp.py
+-rw-rw-rw-   0        0        0     1842 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_model.py
+-rw-rw-rw-   0        0        0    19664 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/train.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.443469 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/
+-rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/__init__.py
+-rw-rw-rw-   0        0        0    22349 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/attention.py
+-rw-rw-rw-   0        0        0     5497 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/compute_perplexity.py
+-rw-rw-rw-   0        0        0       20 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/dataset.py
+-rw-rw-rw-   0        0        0    11234 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/encoder.py
+-rw-rw-rw-   0        0        0     4925 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/export.py
+-rw-rw-rw-   0        0        0     3396 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/model.py
+-rw-rw-rw-   0        0        0       65 2024-02-26 01:52:00.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/scaling.py
+-rw-rw-rw-   0        0        0    17243 2024-02-26 01:52:00.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/train.py
+-rw-rw-rw-   0        0        0    76655 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/utils.py
+-rw-rw-rw-   0        0        0     7709 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained.py
+-rw-rw-rw-   0        0        0     7751 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_bbpe.py
+-rw-rw-rw-   0        0        0     8146 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_streaming.py
+-rw-rw-rw-   0        0        0     2214 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/joiner.py
+-rw-rw-rw-   0        0        0    12993 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/model.py
+-rw-rw-rw-   0        0        0     7152 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_check.py
+-rw-rw-rw-   0        0        0     8300 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_decode.py
+-rw-rw-rw-   0        0        0    17464 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained-streaming.py
+-rw-rw-rw-   0        0        0    12357 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained.py
+-rw-rw-rw-   0        0        0    50893 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/optim.py
+-rw-rw-rw-   0        0        0    10603 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained.py
+-rw-rw-rw-   0        0        0    11561 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained_bbpe.py
+-rw-rw-rw-   0        0        0    70696 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling.py
+-rw-rw-rw-   0        0        0     3342 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling_converter.py
+-rw-rw-rw-   0        0        0     9817 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_beam_search.py
+-rw-rw-rw-   0        0        0    30030 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_decode.py
+-rw-rw-rw-   0        0        0    13138 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/subsampling.py
+-rw-rw-rw-   0        0        0    43330 2024-03-27 07:55:21.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/train.py
+-rw-rw-rw-   0        0        0    29572 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/train_bbpe.py
+-rw-rw-rw-   0        0        0    92936 2024-03-27 06:19:30.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/zipformer.py
+-rw-rw-rw-   0        0        0       88 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.459484 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/__init__.py
+-rw-rw-rw-   0        0        0     5838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py
+-rw-rw-rw-   0        0        0     9569 2024-02-22 05:44:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.461370 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/
+-rw-rw-rw-   0        0        0        0 2024-04-07 06:18:22.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/__init__.py
+-rw-rw-rw-   0        0        0      962 2024-02-25 03:33:09.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py
+-rw-rw-rw-   0        0        0     1186 2024-03-26 14:51:25.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.467391 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/__init__.py
+-rw-rw-rw-   0        0        0    13907 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.482315 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/__init__.py
+-rw-rw-rw-   0        0        0    20570 2024-03-27 10:48:34.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/compute-wer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.485359 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py
+-rw-rw-rw-   0        0        0     1931 2024-03-27 10:57:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/handle4accent.py
+-rw-rw-rw-   0        0        0     6851 2024-02-22 07:15:14.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py
+-rw-rw-rw-   0        0        0     2000 2024-04-07 05:51:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/prepare_data4prompt_task.py
+-rw-rw-rw-   0        0        0     3385 2024-03-17 16:49:11.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.489295 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/fun.py
+-rw-rw-rw-   0        0        0      125 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.503821 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/download_test.py
+-rw-rw-rw-   0        0        0      793 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py
+-rw-rw-rw-   0        0        0      503 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/gxl_test.py
+-rw-rw-rw-   0        0        0      746 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/main.py
+-rw-rw-rw-   0        0        0      400 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.506815 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/__init__.py
+-rw-rw-rw-   0        0        0     1781 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.511863 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/__init__.py
+-rw-rw-rw-   0        0        0     2525 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.514796 gxl_ai_utils-1.3.4/eggs/ch_en_mix/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/ch_en_mix/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.516786 gxl_ai_utils-1.3.4/eggs/ch_en_mix/data_handle/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/ch_en_mix/data_handle/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.521774 gxl_ai_utils-1.3.4/eggs/finetune_llm/
+-rw-rw-rw-   0        0        0        0 2024-02-29 06:01:16.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/__init__.py
+-rw-rw-rw-   0        0        0      928 2024-03-13 02:52:18.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/main.py
+-rw-rw-rw-   0        0        0     1858 2024-03-13 07:52:36.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/main_2B.py
+-rw-rw-rw-   0        0        0     1367 2024-03-13 07:36:12.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/transformers_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.534794 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/__init__.py
+-rw-rw-rw-   0        0        0     1635 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_knowledge_distill.py
+-rw-rw-rw-   0        0        0     1129 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_paraformer_infer.py
+-rw-rw-rw-   0        0        0     2469 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_whisper_infer.py
+-rw-rw-rw-   0        0        0     1090 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/handle_cmvn_gxl.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.540203 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/decoder.py
+-rw-rw-rw-   0        0        0    27385 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/encoder.py
+-rw-rw-rw-   0        0        0      827 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer_infer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.547122 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/__init__.py
+-rw-rw-rw-   0        0        0      741 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.572638 gxl_ai_utils-1.3.4/eggs/spider/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/__init__.py
+-rw-rw-rw-   0        0        0      382 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spdier_little_url_get.py
+-rw-rw-rw-   0        0        0     9274 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_lizhi_fm.py
+-rw-rw-rw-   0        0        0     5810 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm.py
+-rw-rw-rw-   0        0        0    16395 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm_new.py
+-rw-rw-rw-   0        0        0    24924 2024-04-07 10:46:48.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_voicewiki.py
+-rw-rw-rw-   0        0        0    14467 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya.py
+-rw-rw-rw-   0        0        0    10475 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya_new.py
+-rw-rw-rw-   0        0        0     7041 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_yunting.py
+-rw-rw-rw-   0        0        0     4983 2024-02-25 08:28:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu.py
+-rw-rw-rw-   0        0        0     4770 2024-02-25 08:26:09.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu_2.py
+-rw-rw-rw-   0        0        0     3479 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.582661 gxl_ai_utils-1.3.4/gxl_ai_utils/
+-rw-rw-rw-   0        0        0     1651 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/AiConstant.py
+-rw-rw-rw-   0        0        0      556 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.619558 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/
+-rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/__init__.py
+-rw-rw-rw-   0        0        0    14863 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/build_vocab.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.628010 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/__init__.py
+-rw-rw-rw-   0        0        0     5401 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/data_handler.py
+-rw-rw-rw-   0        0        0     6562 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/common_data_handler.py
+-rw-rw-rw-   0        0        0     6242 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/gxl_data_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.630485 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/
+-rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/__init__.py
+-rw-rw-rw-   0        0        0    10901 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/data_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.632511 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_handler/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.633954 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/
+-rw-rw-rw-   0        0        0       36 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.643326 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/__init__.py
+-rw-rw-rw-   0        0        0    17914 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py
+-rw-rw-rw-   0        0        0    27764 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/xvector.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.646138 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/
+-rw-rw-rw-   0        0        0       50 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.649936 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/
+-rw-rw-rw-   0        0        0       25 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/__init__.py
+-rw-rw-rw-   0        0        0    14593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.663036 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/__init__.py
+-rw-rw-rw-   0        0        0     6869 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py
+-rw-rw-rw-   0        0        0     5452 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/embedding.py
+-rw-rw-rw-   0        0        0     8872 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.667120 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.683889 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.700842 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/__init__.py
+-rw-rw-rw-   0        0        0     1942 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py
+-rw-rw-rw-   0        0        0     1662 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py
+-rw-rw-rw-   0        0        0      936 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py
+-rw-rw-rw-   0        0        0     1193 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py
+-rw-rw-rw-   0        0        0     3050 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py
+-rw-rw-rw-   0        0        0     2386 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.709824 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py
+-rw-rw-rw-   0        0        0      427 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/sequence_mask.py
+-rw-rw-rw-   0        0        0     1305 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.712820 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/__init__.py
+-rw-rw-rw-   0        0        0    14807 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.714830 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/t2s/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/t2s/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.722021 gxl_ai_utils-1.3.4/gxl_ai_utils/config/
+-rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/config/__init__.py
+-rw-rw-rw-   0        0        0     5179 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/config/gxl_config.py
+-rw-rw-rw-   0        0        0      121 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.727866 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/
+-rw-rw-rw-   0        0        0        2 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/__init__.py
+-rw-rw-rw-   0        0        0     7429 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py
+-rw-rw-rw-   0        0        0    18215 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.744901 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/__init__.py
+-rw-rw-rw-   0        0        0    10270 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/alignment.py
+-rw-rw-rw-   0        0        0     3616 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/average_model.py
+-rw-rw-rw-   0        0        0     5604 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py
+-rw-rw-rw-   0        0        0    12155 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize.py
+-rw-rw-rw-   0        0        0    12797 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.751783 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/__init__.py
+-rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.755778 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.761757 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/__init__.py
+-rw-rw-rw-   0        0        0     6645 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py
+-rw-rw-rw-   0        0        0    16717 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py
+-rw-rw-rw-   0        0        0    10038 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.768743 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/__init__.py
+-rw-rw-rw-   0        0        0    11275 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/predictor.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.774724 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/__init__.py
+-rw-rw-rw-   0        0        0    16682 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py
+-rw-rw-rw-   0        0        0     6840 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.791678 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/__init__.py
+-rw-rw-rw-   0        0        0    11117 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py
+-rw-rw-rw-   0        0        0     5905 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py
+-rw-rw-rw-   0        0        0    26376 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py
+-rw-rw-rw-   0        0        0     7093 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     2749 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py
+-rw-rw-rw-   0        0        0     7413 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/init_model.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.794669 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/__init__.py
+-rw-rw-rw-   0        0        0    11851 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/model.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.817608 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/__init__.py
+-rw-rw-rw-   0        0        0     8230 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py
+-rw-rw-rw-   0        0        0    11269 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py
+-rw-rw-rw-   0        0        0     5301 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py
+-rw-rw-rw-   0        0        0    17521 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py
+-rw-rw-rw-   0        0        0     9883 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py
+-rw-rw-rw-   0        0        0     6945 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/search.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.838358 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/__init__.py
+-rw-rw-rw-   0        0        0    10509 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py
+-rw-rw-rw-   0        0        0     2636 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py
+-rw-rw-rw-   0        0        0     6713 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py
+-rw-rw-rw-   0        0        0    22398 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py
+-rw-rw-rw-   0        0        0     4833 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     3067 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py
+-rw-rw-rw-   0        0        0    11264 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.848401 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/__init__.py
+-rw-rw-rw-   0        0        0     4110 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/joint.py
+-rw-rw-rw-   0        0        0    18089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.853271 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/__init__.py
+-rw-rw-rw-   0        0        0     2014 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py
+-rw-rw-rw-   0        0        0     6112 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py
+-rw-rw-rw-   0        0        0    23241 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.915216 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/__init__.py
+-rw-rw-rw-   0        0        0    18961 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py
+-rw-rw-rw-   0        0        0    14383 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/attention.py
+-rw-rw-rw-   0        0        0     1533 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py
+-rw-rw-rw-   0        0        0     5329 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py
+-rw-rw-rw-   0        0        0     3084 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py
+-rw-rw-rw-   0        0        0    12855 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py
+-rw-rw-rw-   0        0        0     4939 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py
+-rw-rw-rw-   0        0        0     6339 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py
+-rw-rw-rw-   0        0        0    20622 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py
+-rw-rw-rw-   0        0        0     9838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     3806 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/paraformer_encoder.py
+-rw-rw-rw-   0        0        0     1940 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py
+-rw-rw-rw-   0        0        0    18309 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/search.py
+-rw-rw-rw-   0        0        0     9512 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py
+-rw-rw-rw-   0        0        0     1029 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/swish.py
+-rw-rw-rw-   0        0        0     6294 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py
+-rw-rw-rw-   0        0        0     8366 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py
+-rw-rw-rw-   0        0        0     2582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.950126 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/__init__.py
+-rw-rw-rw-   0        0        0     4018 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py
+-rw-rw-rw-   0        0        0     3065 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py
+-rw-rw-rw-   0        0        0     7954 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/common.py
+-rw-rw-rw-   0        0        0     1516 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/config.py
+-rw-rw-rw-   0        0        0     9964 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py
+-rw-rw-rw-   0        0        0     5411 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py
+-rw-rw-rw-   0        0        0     4353 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/executor.py
+-rw-rw-rw-   0        0        0     2168 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py
+-rw-rw-rw-   0        0        0     1291 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py
+-rw-rw-rw-   0        0        0     7440 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_model.py
+-rw-rw-rw-   0        0        0    13020 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/mask.py
+-rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py
+-rw-rw-rw-   0        0        0     1568 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py
+-rw-rw-rw-   0        0        0    26574 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.962079 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/__init__.py
+-rw-rw-rw-   0        0        0    14805 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/attentions.py
+-rw-rw-rw-   0        0        0     4860 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/commons.py
+-rw-rw-rw-   0        0        0    24767 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/models.py
+-rw-rw-rw-   0        0        0    16740 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/modules.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.967648 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/
+-rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/__init__.py
+-rw-rw-rw-   0        0        0     9889 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.992089 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/
+-rw-rw-rw-   0        0        0     7061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/__main__.py
+-rw-rw-rw-   0        0        0     5089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/audio.py
+-rw-rw-rw-   0        0        0    33001 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/decoding.py
+-rw-rw-rw-   0        0        0    11165 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/model.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.001099 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/
+-rw-rw-rw-   0        0        0      132 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/__init__.py
+-rw-rw-rw-   0        0        0     2012 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/basic.py
+-rw-rw-rw-   0        0        0    21418 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/english.py
+-rw-rw-rw-   0        0        0    12968 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/timing.py
+-rw-rw-rw-   0        0        0    12733 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/tokenizer.py
+-rw-rw-rw-   0        0        0    23334 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/transcribe.py
+-rw-rw-rw-   0        0        0     3583 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/triton_ops.py
+-rw-rw-rw-   0        0        0    11363 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/utils.py
+-rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/version.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.006040 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.008062 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.012023 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/__init__.py
+-rw-rw-rw-   0        0        0      414 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/abs_encoder.py
+-rw-rw-rw-   0        0        0     9977 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.017584 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/__init__.py
+-rw-rw-rw-   0        0        0     2297 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/fastformer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.027279 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/__init__.py
+-rw-rw-rw-   0        0        0    19543 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py
+-rw-rw-rw-   0        0        0   102558 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py
+-rw-rw-rw-   0        0        0    79092 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py
+-rw-rw-rw-   0        0        0    58681 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.039246 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/__init__.py
+-rw-rw-rw-   0        0        0     6478 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/component.py
+-rw-rw-rw-   0        0        0     2953 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/decoder.py
+-rw-rw-rw-   0        0        0     2299 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/encoder.py
+-rw-rw-rw-   0        0        0     1405 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.052051 gxl_ai_utils-1.3.4/gxl_ai_utils/run/
+-rw-rw-rw-   0        0        0       22 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/__init__.py
+-rw-rw-rw-   0        0        0     9326 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/base_train_runner.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.057051 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_predict.py
+-rw-rw-rw-   0        0        0     4263 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_server.py
+-rw-rw-rw-   0        0        0     3023 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner.py
+-rw-rw-rw-   0        0        0     2602 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_multi_template.py
+-rw-rw-rw-   0        0        0      593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_single_template.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.067429 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/
+-rw-rw-rw-   0        0        0       76 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/__init__.py
+-rw-rw-rw-   0        0        0     4311 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_data.py
+-rw-rw-rw-   0        0        0      177 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_data_name.py
+-rw-rw-rw-   0        0        0      451 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataloader.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.071000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/
+-rw-rw-rw-   0        0        0       29 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/__init__.py
+-rw-rw-rw-   0        0        0     5238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/store_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.076984 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/
+-rw-rw-rw-   0        0        0       64 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/__init__.py
+-rw-rw-rw-   0        0        0     2072 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.096930 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/
+-rw-rw-rw-   0        0        0       33 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/__init__.py
+-rw-rw-rw-   0        0        0     6223 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/attention_model.py
+-rw-rw-rw-   0        0        0     2438 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/cnn_model.py
+-rw-rw-rw-   0        0        0      958 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/mlp_model.py
+-rw-rw-rw-   0        0        0     2130 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/rnn_model.py
+-rw-rw-rw-   0        0        0     2348 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/store_model_class.py
+-rw-rw-rw-   0        0        0      578 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_name.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.100935 gxl_ai_utils-1.3.4/gxl_ai_utils/thread/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/thread/__init__.py
+-rw-rw-rw-   0        0        0     1522 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/thread/my_thread.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.126851 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/
+-rw-rw-rw-   0        0        0       80 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_coding.py
+-rw-rw-rw-   0        0        0    26855 2024-03-27 07:04:56.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_data.py
+-rw-rw-rw-   0        0        0      423 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_device.py
+-rw-rw-rw-   0        0        0    53528 2024-04-08 18:27:59.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_file.py
+-rw-rw-rw-   0        0        0     6520 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_model.py
+-rw-rw-rw-   0        0        0     1655 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_showing.py
+-rw-rw-rw-   0        0        0     6747 2024-03-24 18:40:27.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_spider.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.605550 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    22460 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/license.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:32:05.131967 gxl_ai_utils-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      518 2024-04-08 18:31:17.000000 gxl_ai_utils-1.3.4/setup.py
```

### Comparing `gxl_ai_utils-1.3.3/eggs/aishell/do_train.py` & `gxl_ai_utils-1.3.4/eggs/aishell/do_train.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py` & `gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_gigaspeech.py` & `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_gigaspeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_haoweilai.py` & `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_haoweilai.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_librispeech.py` & `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_librispeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/handle_mls.py` & `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_mls.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/asr_shard_and_format/make_shard.py` & `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/make_shard.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_3/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 sys.path.insert(0,'../../../../')
 import tqdm
 
 from gxl_ai_utils.utils import utils_file
 
 NEW2OLD_TABLE = {}
 VAD_INFO_TABLE = {}
-THREAD_NUM = 40
+THREAD_NUM = 40 # 切割音频的进程
 IF_START_BY_0 = True  # 切割后的音频的名字的序号,是否以0起始,还是以1起始.
-VAD_TYPE = 3
-
-
+VAD_TYPE = 1  # 0:文件,文件内多行,每行都是i:j .. 1:文件, 格式如下:[[i,j],[i,j],[i,j]..] .. 2: str, 格式如下:[[i,j],[i,j],[i,j]..] ... 3:vad str, 格式如下:i:j i:j i:j ...
+TTS_FINAL_TYPE=1  # 0:简短list型.. 1:含txt的scp型
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--tts_final_scp_name", type=str)
     parser.add_argument("--asr_final_scp_name", type=str)
     parser.add_argument("--do_split", type=bool, default=False)
     args = parser.parse_args()
     return args
@@ -33,34 +32,31 @@
     parent_new_name = file_name_item_list[0] + "_" + file_name_item_list[1]
     if file_name_item_list[2].startswith("VAD"):
         index = int(file_name_item_list[2].split("VAD")[1])
     else:
         index = int(file_name_item_list[2])
     millisecond_num = int(file_name_item_list[3])
     return parent_new_name, index, millisecond_num
-
 def get_little_final(input_final_scp_path, output_dir):
     """从非常大的tts_final_scp中取出一小点，组成一个测试用的小的tts_final_scp文件"""
     all_dict = utils_file.load_dict_from_scp(input_final_scp_path)
     little_dict = utils_file.get_random_subdict(all_dict, 25)
     utils_file.write_dict_to_scp(little_dict, os.path.join(output_dir, f"final_scp_little.scp"))
-
 def pre_do(final_tts_scp_path: str, output_dir: str):
     utils_file.logging_print('首先切分tts_final.scp,切分为6个')
     # final_tts_dict = utils_file.load_dict_from_scp(final_tts_scp_path)
     # tts_dict_list = utils_file.do_split_dict(final_tts_dict, 6)
     # for i, tts_dict in enumerate(tts_dict_list):
     #     i = i + 1
     #     utils_file.write_dict_to_scp(tts_dict, os.path.join(output_dir, f"tts_final_{i}.scp"))
     final_tts_list = utils_file.load_list_file_clean(final_tts_scp_path)
     list_list = utils_file.do_split_list(final_tts_list, 6)
     for i, list in enumerate(list_list):
         i = i + 1
         utils_file.write_list_to_file(list, os.path.join(output_dir, f"tts_final_{i}.scp"))
-
 def do_handle_wav(long_wav_new_name, output_dir="./"):
     """
     处理一个长音频. 传入该长音频的new_name, 然后对其进行clean和切割.
     :param long_wav_new_name:
     :param output_dir:
     :return:
     """
@@ -93,16 +89,14 @@
         utils_file.makedir_sil(final_wav_dir)
         slicing_wav(long_clean_path, vad_info4long_new_name, final_wav_dir, long_wav_new_name, THREAD_NUM)
     else:
         utils_file.logging_print(
             f"do_handle_wav(): long_old_clean_path is exist, long_wav_new_name={long_wav_new_name}, 跳过该长音频的处理"
         )
     return True
-
-
 def slicing_wav(input_file_path, vad_info4long_new_name, output_dir, wav_new_name, thread_num=40):
     """
     将一个音频,依据时间戳, 切分成若干小音频. 此处可以多线程并行处理
     """
     global IF_START_BY_0, VAD_TYPE
     sorted_list = get_vad_info_list(vad_info4long_new_name, VAD_TYPE)
     thread_num = thread_num if len(sorted_list) > thread_num else len(sorted_list)
@@ -127,16 +121,14 @@
     start_time = vad_info[0]
     end_time = vad_info[1]
     duration = int(end_time) - int(start_time)
     start_sample = int(start_time) * 16
     end_sample = int(end_time) * 16
     output_path = os.path.join(output_dir, f"{wav_new_name}_{i}_{duration}.wav")
     utils_file.do_extract_audio_segment(input_file_path, output_path, start_sample, end_sample)
-
-
 def get_vad_info_list(vad_info4long_new_name, vad_type=0):
     """
     处理vad_info4long_new_name, 得到排过序的一个双层列表 [[s,e],[s,e],[s,e]...]
     :param vad_info_txt_path:
     :return:
     """
     sorted_list = []
@@ -178,15 +170,14 @@
         vad_info_list = []
         for res in split_list:
             res_i = res.split(":")[0]
             res_j = res.split(":")[1]
             vad_info_list.append([res_i, res_j])
         sorted_list = sorted(vad_info_list, key=lambda x: int(x[0]))
     return sorted_list
-
 def do_get_vad_scp_file(input_dir, output_dir='./'):
     """
     tts处理流程中会对每一个音频生成一个vad_info的txt文件, 我们得到一个key vad_info.txt的字典
     :param input_dir:
     :return:
     """
     if os.path.isdir(input_dir):
@@ -200,15 +191,14 @@
             info = res_line.split('|')[1].strip()
             vad_res_dict[key] = info
     little_res_dict = utils_file.get_subdict(vad_res_dict, 0, 10)
     utils_file.logging_print("do_get_vad_scp_file(): 小字典示例:")
     utils_file.print_dict(little_res_dict)
     utils_file.write_dict_to_scp(vad_res_dict, os.path.join(output_dir, "vad_res.scp"))
 
-
 def do_get_old2new_scp_file(input_dir, output_dir='./'):
     """
     这个input_dir中包含大量的old2new_*.txt文件, 我们得到一个key old2new.txt的字典
     :param input_dir:
     :return:
     """
     if os.path.isfile(input_dir):
@@ -221,15 +211,14 @@
         old2new_dict = utils_file.load_dict_from_scp(old2new_path)
         res_dict.update(old2new_dict)
     little_res_dict = utils_file.get_subdict(res_dict, 0, 10)
     utils_file.logging_print("do_get_old2new_scp_file(): 小字典示例:")
     utils_file.print_dict(little_res_dict)
     utils_file.write_dict_to_scp(res_dict, os.path.join(output_dir, "old2new.scp"))
 
-
 def solution(final_tts_scp_path, output_dir, old2new_dir, input_vad_info_dir):
     utils_file.logging_print('首先从命令行中拿到要处理的tts_final.scp的子集')
     args = get_args()
     if args.do_split:
         utils_file.logging_print('开始do_split')
         pre_do(final_tts_scp_path, output_dir)
         utils_file.logging_print('do_split完成, 直接return')
@@ -243,23 +232,25 @@
     utils_file.makedir_sil(output_dir)
     do_get_vad_scp_file(input_vad_info_dir, output_dir)
     do_get_old2new_scp_file(old2new_dir, output_dir)
     NEW2OLD_TABLE.update(utils_file.load_dict_from_scp(os.path.join(output_dir, "old2new.scp")))
     VAD_INFO_TABLE.update(utils_file.load_dict_from_scp(os.path.join(output_dir, "vad_res.scp")))
 
     utils_file.logging_print('获取tts_scp对应的长音频的新名字列表')
-    tts_dict = utils_file.load_dict_from_scp(tts_scp_path)
-    # wav_path_list = utils_file.load_list_file_clean(tts_scp_path)
     long_wav_new_names_list = []
-    for key in tqdm.tqdm(tts_dict.keys(), total=len(tts_dict)):
-        long_wav_new_name, _, _ = handle_path(key, only_name=True)
-        long_wav_new_names_list.append(long_wav_new_name)
-    # for wav_path in tqdm.tqdm(wav_path_list, total=len(wav_path_list)):
-    #     long_wav_new_name, _, _ = handle_path(wav_path, only_name=False)
-    #     long_wav_new_names_list.append(long_wav_new_name)
+    if TTS_FINAL_TYPE == 0:
+        wav_path_list = utils_file.load_list_file_clean(tts_scp_path)
+        for wav_path in tqdm.tqdm(wav_path_list, total=len(wav_path_list)):
+            long_wav_new_name, _, _ = handle_path(wav_path, only_name=False)
+            long_wav_new_names_list.append(long_wav_new_name)
+    elif TTS_FINAL_TYPE == 1:
+        tts_dict = utils_file.load_dict_from_scp(tts_scp_path)
+        for key in tqdm.tqdm(tts_dict.keys(), total=len(tts_dict)):
+            long_wav_new_name, _, _ = handle_path(key, only_name=True)
+            long_wav_new_names_list.append(long_wav_new_name)
     long_wav_new_names_list = list(set(long_wav_new_names_list))
 
     utils_file.logging_print("开始逐条长音频得处理")
     for long_wav_new_name in tqdm.tqdm(long_wav_new_names_list, total=len(long_wav_new_names_list)):
         do_handle_wav(long_wav_new_name, output_dir)
     utils_file.logging_print('完全切割完毕')
     return
@@ -332,22 +323,42 @@
     utils_file.logging_print(f'text_scp_dict长度为：{len(text_scp_dict)}')
     new_text_scp_dict = {}
     for key, value in text_scp_dict.items():
         if key in wav_scp_dict:
             new_text_scp_dict[key] = value
     utils_file.write_dict_to_scp(new_text_scp_dict, os.path.join(output_dir, 'text'))
     return
+    def little_func(input_text_dict, res_text_dict):
+        for key, path in tqdm.tqdm(input_text_dict.items(), total=len(input_text_dict)):
+            text = utils_file.load_first_row_clean(path)
+            if len(text) > 0:
+                text = text.strip().split()[-1]
+                text = utils_file.do_filter(text)
+                res_text_dict[key] = text
 
 
-
+    text_dict = utils_file.load_dict_from_scp(os.path.join(output_dir, "text_old"))
+    new_text_dict = {}
+    text_dict_list = utils_file.do_split_dict(text_dict, 100)
+    runner = utils_file.GxlDynamicThreadPool()
+    for text_dict_i in text_dict_list:
+        runner.add_task(little_func, [text_dict_i, new_text_dict])
+    runner.start()
+    utils_file.write_dict_to_scp(new_text_dict, os.path.join(output_dir, "text"))
+    utils_file.write_dict_to_scp(text_dict, os.path.join(output_dir, "text_old"))
+    utils_file.do_convert_wav_text_scp_to_jsonl(os.path.join(output_dir, "wav.scp"), os.path.join(output_dir, "text"),
+                                                os.path.join(output_dir, "data.list"))
+    shard_output_dir = "/home/work_nfs14/xlgeng/asr_data_shard/pachong_data/shangye_caijing_4/"
+    utils_file.do_make_shard_file(os.path.join(output_dir, "wav.scp"), os.path.join(output_dir, "text"),
+                                  shard_output_dir, num_threads=50)
 
 
 
 if __name__ == '__main__':
-    output_dir = "/home/node36_data/xlgeng/asr_data_from_pachong/gxl_output/ximalaya_shenghuo_10T_3"
+
+    output_dir = "/home/node36_data/xlgeng/asr_data_from_pachong/gxl_output/yunting_taihaizhisheng_1"
     utils_file.makedir_for_file_or_dir(output_dir)
-    old2new_dir = "/home/node40_data/tlzuo/data_handle/lists/init_lists"
-    vad_info_dir = "/home/work_nfs6/tlzuo/data_handle/lists/vad_result"
-    text_dir="/home/work_nfs6/tlzuo/data_handle/lists/5txts"
-    final_tts_scp_path = "/home/work_nfs13/lhma/life_split4/final1.scp"
-    solution(final_tts_scp_path, output_dir, old2new_dir, vad_info_dir)
-    # post_process(output_dir, final_tts_scp_path)
+    old2new_dir = "/home/work_nfs8/ypjiang/data_process/yunting/台海之声/*_info/init_lists"
+    vad_info_dir = "/home/work_nfs8/ypjiang/data_process/yunting/台海之声/*_info/vad_info"
+    text_dir = "/home/work_nfs6/tlzuo/data_handle/lists/5txts"
+    final_tts_scp_path = "/home/work_nfs14/zhguo/data/lizhi_jiankang/final_cmn.scp"
+    solution(final_tts_scp_path, output_dir, old2new_dir, vad_info_dir)
```

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/do_handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from gxl_ai_utils.utils import utils_file
 
 NEW2OLD_TABLE = {}
 VAD_INFO_TABLE = {}
 THREAD_NUM = 40 # 切割音频的进程
 IF_START_BY_0 = True  # 切割后的音频的名字的序号,是否以0起始,还是以1起始.
-VAD_TYPE = 1  # 0:文件,文件内多行,每行都是i:j .. 1:文件, 格式如下:[[i,j],[i,j],[i,j]..] .. 2: str, 格式如下:[[i,j],[i,j],[i,j]..] ... 3:vad str, 格式如下:i:j i:j i:j ...
+VAD_TYPE = 0  # 0:文件,文件内多行,每行都是i:j .. 1:文件, 格式如下:[[i,j],[i,j],[i,j]..] .. 2: str, 格式如下:[[i,j],[i,j],[i,j]..] ... 3:vad str, 格式如下:i:j i:j i:j ...
 TTS_FINAL_TYPE=1  # 0:简短list型.. 1:含txt的scp型
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--tts_final_scp_name", type=str)
     parser.add_argument("--asr_final_scp_name", type=str)
     parser.add_argument("--do_split", type=bool, default=False)
     args = parser.parse_args()
@@ -37,15 +37,17 @@
     millisecond_num = int(file_name_item_list[3])
     return parent_new_name, index, millisecond_num
 def get_little_final(input_final_scp_path, output_dir):
     """从非常大的tts_final_scp中取出一小点，组成一个测试用的小的tts_final_scp文件"""
     all_dict = utils_file.load_dict_from_scp(input_final_scp_path)
     little_dict = utils_file.get_random_subdict(all_dict, 25)
     utils_file.write_dict_to_scp(little_dict, os.path.join(output_dir, f"final_scp_little.scp"))
-def pre_do(final_tts_scp_path: str, output_dir: str):
+def pre_do(input_vad_info_dir,old2new_dir, final_tts_scp_path: str, output_dir: str):
+    do_get_vad_scp_file(input_vad_info_dir, output_dir)
+    do_get_old2new_scp_file(old2new_dir, output_dir)
     utils_file.logging_print('首先切分tts_final.scp,切分为6个')
     # final_tts_dict = utils_file.load_dict_from_scp(final_tts_scp_path)
     # tts_dict_list = utils_file.do_split_dict(final_tts_dict, 6)
     # for i, tts_dict in enumerate(tts_dict_list):
     #     i = i + 1
     #     utils_file.write_dict_to_scp(tts_dict, os.path.join(output_dir, f"tts_final_{i}.scp"))
     final_tts_list = utils_file.load_list_file_clean(final_tts_scp_path)
@@ -176,15 +178,19 @@
     return sorted_list
 def do_get_vad_scp_file(input_dir, output_dir='./'):
     """
     tts处理流程中会对每一个音频生成一个vad_info的txt文件, 我们得到一个key vad_info.txt的字典
     :param input_dir:
     :return:
     """
-    if os.path.isdir(input_dir):
+    if isinstance(input_dir, list):
+        vad_res_dict = {}
+        for input_dir_i in input_dir:
+            vad_res_dict.update(utils_file.get_scp_for_wav_dir(input_dir_i, suffix="txt"))
+    elif os.path.isdir(input_dir):
         vad_res_dict = utils_file.get_scp_for_wav_dir(input_dir, suffix="txt")
     else:
         res_list = utils_file.load_list_file_clean(input_dir)
         vad_res_dict = {}
         for res_line in res_list:
             wav_path = res_line.split('|')[0]
             key = utils_file.get_file_pure_name_from_path(wav_path)
@@ -193,65 +199,89 @@
     little_res_dict = utils_file.get_subdict(vad_res_dict, 0, 10)
     utils_file.logging_print("do_get_vad_scp_file(): 小字典示例:")
     utils_file.print_dict(little_res_dict)
     utils_file.write_dict_to_scp(vad_res_dict, os.path.join(output_dir, "vad_res.scp"))
 
 def do_get_old2new_scp_file(input_dir, output_dir='./'):
     """
-    这个input_dir中包含大量的old2new_*.txt文件, 我们得到一个key old2new.txt的字典
+    这个input_dir中包含大量的old2new_*.txt文件
     :param input_dir:
     :return:
     """
-    if os.path.isfile(input_dir):
+    if isinstance(input_dir, list):
+        old2new_path_list = input_dir
+    elif os.path.isfile(input_dir):
         utils_file.logging_print("do_get_old2new_scp_file(): input_dir是文件")
         utils_file.copy_file(input_dir, os.path.join(output_dir, "old2new.scp"))
         return
-    old2new_path_list = glob.glob(f"{input_dir}/old2new*.scp")
+    else:
+        old2new_path_list = glob.glob(f"{input_dir}/old2new*.scp")
+
     res_dict = {}
     for old2new_path in old2new_path_list:
         old2new_dict = utils_file.load_dict_from_scp(old2new_path)
         res_dict.update(old2new_dict)
     little_res_dict = utils_file.get_subdict(res_dict, 0, 10)
     utils_file.logging_print("do_get_old2new_scp_file(): 小字典示例:")
     utils_file.print_dict(little_res_dict)
     utils_file.write_dict_to_scp(res_dict, os.path.join(output_dir, "old2new.scp"))
 
 def solution(final_tts_scp_path, output_dir, old2new_dir, input_vad_info_dir):
     utils_file.logging_print('首先从命令行中拿到要处理的tts_final.scp的子集')
     args = get_args()
     if args.do_split:
         utils_file.logging_print('开始do_split')
-        pre_do(final_tts_scp_path, output_dir)
+        pre_do(input_vad_info_dir,old2new_dir,final_tts_scp_path, output_dir)
         utils_file.logging_print('do_split完成, 直接return')
         return
     tts_scp_path = os.path.join(output_dir, args.tts_final_scp_name)
     asr_final_path = os.path.join(output_dir, args.asr_final_scp_name)
     if os.path.exists(asr_final_path):
         utils_file.logging_print('asr_scp_path已经存在，直接删除')
         os.remove(asr_final_path)
-    utils_file.logging_print('加载vad和old2new的信息')
+    utils_file.logging_print('拿到成功\n')
+
+    utils_file.logging_print('加载vad和old2new的信息,从而在output目录下得到vad_res.scp和old2new.scp,这一步基本是不用变动的,然后将dict信息加载到全局变量中')
     utils_file.makedir_sil(output_dir)
-    do_get_vad_scp_file(input_vad_info_dir, output_dir)
-    do_get_old2new_scp_file(old2new_dir, output_dir)
     NEW2OLD_TABLE.update(utils_file.load_dict_from_scp(os.path.join(output_dir, "old2new.scp")))
     VAD_INFO_TABLE.update(utils_file.load_dict_from_scp(os.path.join(output_dir, "vad_res.scp")))
+    utils_file.logging_print('加载vad和old2new的信息完成\n')
 
     utils_file.logging_print('获取tts_scp对应的长音频的新名字列表')
     long_wav_new_names_list = []
     if TTS_FINAL_TYPE == 0:
         wav_path_list = utils_file.load_list_file_clean(tts_scp_path)
         for wav_path in tqdm.tqdm(wav_path_list, total=len(wav_path_list)):
             long_wav_new_name, _, _ = handle_path(wav_path, only_name=False)
             long_wav_new_names_list.append(long_wav_new_name)
     elif TTS_FINAL_TYPE == 1:
         tts_dict = utils_file.load_dict_from_scp(tts_scp_path)
         for key in tqdm.tqdm(tts_dict.keys(), total=len(tts_dict)):
             long_wav_new_name, _, _ = handle_path(key, only_name=True)
             long_wav_new_names_list.append(long_wav_new_name)
     long_wav_new_names_list = list(set(long_wav_new_names_list))
+    utils_file.logging_print('获取tts_scp对应的长音频的新名字列表完成,其一共有:', len(long_wav_new_names_list), '\n')
+
+    utils_file.logging_print('开始验证vad信息和old2new信息是否全面,从而得到最终真正能处理的长音频的新名字列表,以及他的数量')
+    final_long_wav_new_names_list = []
+    for long_wav_new_name in tqdm.tqdm(long_wav_new_names_list, total=len(long_wav_new_names_list)):
+        if long_wav_new_name in VAD_INFO_TABLE and long_wav_new_name in NEW2OLD_TABLE:
+            final_long_wav_new_names_list.append(long_wav_new_name)
+        else:
+            utils_file.logging_print(
+                f"这个长音频 验证vad信息和old2new信息是否全面失败: long_wav_new_name={long_wav_new_name}"
+            )
+            if not (long_wav_new_name in VAD_INFO_TABLE):
+                utils_file.logging_print(f"vad_info表中不包含该音频")
+            if not (long_wav_new_name in NEW2OLD_TABLE):
+                utils_file.logging_print(f"new2old表中不包含该音频")
+    utils_file.logging_print('验证vad信息和old2new信息是否全面完成,其一共有:', len(final_long_wav_new_names_list), '\n')
+    long_wav_new_names_list = final_long_wav_new_names_list
+
+
 
     utils_file.logging_print("开始逐条长音频得处理")
     for long_wav_new_name in tqdm.tqdm(long_wav_new_names_list, total=len(long_wav_new_names_list)):
         do_handle_wav(long_wav_new_name, output_dir)
     utils_file.logging_print('完全切割完毕')
     return
     #  ------------------后处理-----------------------------
@@ -350,15 +380,14 @@
     shard_output_dir = "/home/work_nfs14/xlgeng/asr_data_shard/pachong_data/shangye_caijing_4/"
     utils_file.do_make_shard_file(os.path.join(output_dir, "wav.scp"), os.path.join(output_dir, "text"),
                                   shard_output_dir, num_threads=50)
 
 
 
 if __name__ == '__main__':
-
-    output_dir = "/home/node36_data/xlgeng/asr_data_from_pachong/gxl_output/yunting_taihaizhisheng_1"
+    output_dir = "/home/node36_data/xlgeng/asr_data_from_pachong/gxl_output/liukai_youshengxiaoshuo"
     utils_file.makedir_for_file_or_dir(output_dir)
-    old2new_dir = "/home/work_nfs8/ypjiang/data_process/yunting/台海之声/*_info/init_lists"
-    vad_info_dir = "/home/work_nfs8/ypjiang/data_process/yunting/台海之声/*_info/vad_info"
-    text_dir = "/home/work_nfs6/tlzuo/data_handle/lists/5txts"
-    final_tts_scp_path = "/home/work_nfs14/zhguo/data/lizhi_jiankang/final_cmn.scp"
+    old2new_dir = "/home/work_nfs10/dkguo/data_audiobook/init_lists"
+    vad_info_dir = "/home/work_nfs10/dkguo/data_audiobook/vad_result"
+    final_tts_scp_path = "/home/work_nfs10/dkguo/data_audiobook/final.scp"
+
     solution(final_tts_scp_path, output_dir, old2new_dir, vad_info_dir)
```

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,10 +9,20 @@
     data_names = ['shangye_caijing_3', 'shangye_caijing_2', 'shangye_caijing_4','shenghuo_2']
     all_list = []
     for data_name in data_names:
         temp_path = os.path.join(data_dir, data_name,'shards_list.txt')
         temp_list = utils_file.load_list_file_clean(temp_path)
         all_list.extend(temp_list)
     utils_file.write_list_to_file(all_list, os.path.join(data_dir, 'all_shards_list_2.txt'))
+def do_handle_2():
+    """"""
+    data_dir = "/home/work_nfs14/xlgeng/asr_data_shard/pachong_data"
+    data_names = ['4_lizhi_jiankang', '5_yunting_taihaizhisheng', '6_yunting_zhongguozhisheng','8_liukai_chuantongguoxue','shenghuo_1']
+    all_list = []
+    for data_name in data_names:
+        temp_path = os.path.join(data_dir, data_name,'shards_list.txt')
+        temp_list = utils_file.load_list_file_clean(temp_path)
+        all_list.extend(temp_list)
+    utils_file.write_list_to_file(all_list, os.path.join(data_dir, 'all_shards_list_3.txt'))
 
 if __name__ == '__main__':
-    do_handle()
+    do_handle_2()
```

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_gxl_ai_utils/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/test_sentencepiece/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/cats_and_dogs/ximalaya/main.py` & `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/finetune_llm/main.py` & `gxl_ai_utils-1.3.4/eggs/finetune_llm/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/finetune_llm/main_2B.py` & `gxl_ai_utils-1.3.4/eggs/finetune_llm/main_2B.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/finetune_llm/transformers_learning.py` & `gxl_ai_utils-1.3.4/eggs/finetune_llm/transformers_learning.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/gxl_knowledge_distill.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_knowledge_distill.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/gxl_paraformer_infer.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_paraformer_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/gxl_whisper_infer.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_whisper_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/handle_cmvn_gxl.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/handle_cmvn_gxl.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer/encoder.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/paraformer_infer.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/knowledge_distillation/whisper_ctc/main.py` & `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_lizhi_fm.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_lizhi_fm.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_qingting_fm.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_qingting_fm_new.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm_new.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_ximalaya.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_ximalaya_new.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya_new.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_yunting.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_yunting.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_zhihu.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/spider_zhihu_2.py` & `gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu_2.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/eggs/spider/test.py` & `gxl_ai_utils-1.3.4/eggs/spider/test.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/AiConstant.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/AiConstant.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/__init__.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/build_vocab.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/build_vocab.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/classify/data_handler.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/common_data_handler.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/common_data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/gxl_data_handler.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/gxl_data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_dataset/recognition/data_handler.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/classify/xvector.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/xvector.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/embedding.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/modules/subsampling.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/transformer/transformer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/config/gxl_config.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/config/gxl_config.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/alignment.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/alignment.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/average_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/average_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/recognize.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/cif/predictor.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/predictor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/init_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/init_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/k2/model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/paraformer/search.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/joint.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/joint.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/attention.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/search.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/swish.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/swish.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/common.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/common.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/config.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/config.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/executor.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/executor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/init_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/mask.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/mask.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/attentions.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/attentions.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/commons.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/commons.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/models.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/models.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_model_wenet/vits/modules.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/modules.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/__init__.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/audio.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/decoding.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/decoding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/normalizers/basic.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/basic.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/normalizers/english.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/english.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/timing.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/tokenizer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/transcribe.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/triton_ops.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/triton_ops.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/gxl_whisper/utils.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/fastformer/fastformer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/fastformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/component.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/component.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/decoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/encoder.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/model_warehouse/transformer/transformer.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/run/base_train_runner.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/run/base_train_runner.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/run/flask_template/flask_predict.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_predict.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/run/flask_template/flask_server.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_server.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/run/runner.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/run/runner_multi_template.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_multi_template.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/run/runner_single_template.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_single_template.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_data.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_data.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_data/store_dataset/store_dataset.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/store_dataset.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/attention_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/attention_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/cnn_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/cnn_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/mlp_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/mlp_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/rnn_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/rnn_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_class/store_model_class.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/store_model_class.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/store_model/store_model_name.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_name.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/thread/my_thread.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/thread/my_thread.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_data.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,15 @@
                              SI1279.WRD file -> "bricks are an alternative"
                              Else if trans_type is phn,
                              read from SI1279.PHN file ->
                              "sil b r ih sil k s aa r er n aa l
                              sil t er n ih sil t ih v sil)
     :return:
     """
-
+    os.makedirs(os.path.dirname(output_path), exist_ok=True)
     def exist_or_not(i, match_pos):
         start_pos = None
         end_pos = None
         for pos in match_pos:
             if pos[0] <= i < pos[1]:
                 start_pos = pos[0]
                 end_pos = pos[1]
@@ -453,17 +453,18 @@
 
     if text_scp_path is not None:
         f = codecs.open(text_scp_path, encoding="utf-8")
     else:
         f = codecs.getreader("utf-8")(
             sys.stdin if is_python2 else sys.stdin.buffer)
     buffer = GxlStringBuffer()
-    line = f.readline()
+    # line = f.readline()
     n = nchar
-    while line:
+    lines_totals = f.readlines()
+    for line in tqdm(lines_totals, total=len(lines_totals), desc='text2tokening'):
         x = line.split()
         buffer.print(' '.join(x[:skip_ncols]), end=" ")
         a = ' '.join(x[skip_ncols:])
 
         # get all matched positions
         match_pos = []
         for r in rs:
@@ -514,28 +515,29 @@
         for z in a:
             a_flat.append("".join(z))
 
         a_chars = [z.replace(' ', space) for z in a_flat]
         if trans_type == "phn":
             a_chars = [z.replace("sil", space) for z in a_chars]
         buffer.print(' '.join(a_chars))
-        line = f.readline()
+        # line = f.readline()
     lines = buffer.to_list_clean()
     cut_result = [line.split()[1:] for line in lines]
     # 将列表展平，并用换行符连接
     tr_result = "\n".join("\n".join(row) for row in cut_result)
     # 对行进行排序
     sort_result = "\n".join(sorted(tr_result.split("\n")))
     # 去除重复行
     uniq_result = "\n".join(sorted(set(sort_result.split("\n"))))
     # 过滤掉只包含空白字符的行
     grep_result = "\n".join(line for line in uniq_result.split("\n") if line.strip())
     # 在每一行末尾添加数字
     items = grep_result.split("\n")
-    awk_result = "\n".join(f"{line} {i + 1}" for i, line in enumerate(items))
+    awk_result = "<blk> 0\n"
+    awk_result += "\n".join(f"{line} {i + 1}" for i, line in enumerate(items))
     awk_result += f"\n<sos/eos> {len(items) + 1}\n"
     from .utils_file import makedir_for_file
     makedir_for_file(output_path)
     # 将结果追加到文件
     with open(output_path, "w", encoding='utf-8') as f:
         f.write(awk_result)
```

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_file.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import glob
+import gzip
 import hashlib
 import io
 import json
 import logging
 import multiprocessing
 import os
 import random
@@ -28,14 +29,15 @@
 import wave
 from torch import nn
 from tqdm import tqdm
 from ..thread.my_thread import GxlDynamicThreadPool, GxlFixedThreadPool
 
 HAS_SET_LOGGING = False
 
+
 # GLOGGER: logging.Logger = None
 def set_logging():
     """
     设置日志输出的格式
     :return: 
     """
     global HAS_SET_LOGGING, GLOGGER
@@ -105,14 +107,17 @@
 
 def load_first_row_clean(path: str):
     """
     得到不包含换行符的第一行,如果文件为空， 则返回“”
     :param path:
     :return:
     """
+    if not os.path.exists(path):
+        logging_print(f'load_first_row_clean()_{path}文件不存在')
+        return ""
     with codecs.open(path, 'r', encoding='utf=8') as f:
         cat_to_name: str = f.readline()
     return cat_to_name.strip()
 
 
 def load_list_file_unclean(path: str):
     """
@@ -135,33 +140,43 @@
     return cat_to_name
 
 
 def load_dict_list_from_jsonl(jsonl_file_path) -> list:
     """"""
     with codecs.open(jsonl_file_path, 'r', encoding='utf-8') as f:
         lines = f.readlines()
-        logging_print("load_dict_list_from_jsonl()_数据总条数为:", len(lines))
-        lines = [json.loads(x) for x in lines]
-        return lines
+        lines_res = []
+        for line in lines:
+            try:
+                line = json.loads(line)
+                lines_res.append(line)
+            except Exception as e:
+                print(e)
+                continue
+    return lines_res
 
 
 def load_dict_from_scp(label_scp_file: str) -> dict:
     """
     得到scp文件的内容,要求key value以空格分割， 第一个为key,剩下的都是value。
     :param label_scp_file:
     :return:
     """
     res = {}
     with codecs.open(label_scp_file, 'r', encoding='utf-8') as f:
-        lines = f.readlines()
+        try:
+            lines = f.readlines()
+        except Exception as e:
+            print(e)
+            return {}
         for line in lines:
             line = line.strip()
             items = line.split()
             if len(items) < 2:
-                logging_print('warning_gxl:, this row not conform to the regulation of scp(key content) and skip it:',
+                logging_print('load_dict_from_scp;warning_gxl:, this row not conform to the regulation of scp(key content) and skip it:',
                               line)
                 continue
             elif len(items) == 2:
                 res[items[0].strip()] = items[1].strip()
             else:
                 # logging_print(
                 #     'warning_gxl:, this row not conform to the regulation of'
@@ -995,14 +1010,19 @@
 
 
 def get_random_subdict(source_dict: dict, num_value: int):
     keys = list(source_dict.keys())
     random.shuffle(keys)
     return {key: source_dict[key] for key in keys[:num_value]}
 
+def do_get_random_subdict(source_dict: dict, num_value: int):
+    keys = list(source_dict.keys())
+    random.shuffle(keys)
+    return {key: source_dict[key] for key in keys[:num_value]}
+
 
 def get_subdict(source_dict: dict, start_i, end_i):
     return {key: source_dict[key] for key in list(source_dict.keys())[start_i:end_i]}
 
 
 def do_convert_jsonl_to_wav_text_scp(jsonl_path, scp_path=None, text_path=None):
     """
@@ -1083,47 +1103,364 @@
     将音频整理成标准格式， 16K采样， 单通道，补齐音频头
     :param input_file_path:
     :param output_file_path:
     :return:
     """
     os.system(f"ffmpeg -i '{input_file_path}' -ac 1 -ar 16000 -vn {output_file_path}")
 
+
 def is_windows_system():
     if sys.platform.startswith('win'):
         return True
     else:
         return False
 
+
 def is_linux_system():
     if sys.platform.startswith('linux'):
         return True
     else:
         return False
 
+
 def do_remove_punctuation(text):
     """使用正则表达式去除标点符号，只保留汉字、英文和数字"""
     # 使用正则表达式去除标点符号，只保留汉字、英文和数字
     return re.sub(r'[^\u4e00-\u9fa5a-zA-Z0-9]', '', text)
 
-def do_filter(text):
+
+def do_filter(text, only_zn=False, only_en=False, only_num=False):
     """使用正则表达式去除标点符号，只保留汉字、英文和数字"""
-    return do_remove_punctuation(text)
+    if only_zn:
+        return re.sub(r'[\u4e00-\u9fa5]', '', text)
+    if only_en:
+        return re.sub(r'[a-zA-Z]', '', text)
+    if only_num:
+        return re.sub(r'[0-9]', '', text)
+    return re.sub(r'[^\u4e00-\u9fa5a-zA-Z0-9]', '', text)
+
 
-def do_convert_text2chars_dict(text_scp_path, dict_file_path):
+def do_convert_text2chars_dict(text_scp_path, dict_file_path, blank_sym='<blank>'):
     """
     仅仅为中文服务
     :param text_scp_path:
     :param dict_file_path:
     :return:
     """
-    logging_print(f'开始便利{text_scp_path}中的所有句子，提取chars_dictionary')
+    logging_print(f'开始遍历{text_scp_path}中的所有句子，提取chars_dictionary')
+    makedir_for_file(dict_file_path)
     text_dict = load_dict_from_scp(text_scp_path)
     chars_set = set()
-    for value in tqdm(text_dict.values(),total=len(text_dict),desc='提取chars_dictionary'):
+    for value in tqdm(text_dict.values(), total=len(text_dict), desc='提取chars_dictionary'):
         for char_i in value:
             chars_set.add(char_i)
     with codecs.open(dict_file_path, 'w', encoding='utf-8') as f:
-        f.write('<blank> 0\n')
+        f.write(f'{blank_sym} 0\n')
         f.write('<unk> 1\n')
         f.write('<sos/eos> 2\n')
         for i, char in enumerate(sorted(chars_set)):
-            f.write(f'{char} {i + 3}\n')
+            f.write(f'{char} {i + 3}\n')
+
+
+def get_sample_count(audio_file_path: str):
+    """
+    得到路径所指音频的采样点数
+    output->
+    sample_count: 采样点数
+    sample_rate: 采样率
+    """
+    with wave.open(audio_file_path, 'rb') as audio_file:
+        sample_count = audio_file.getnframes()
+        sample_rate = audio_file.getframerate()
+    return sample_count, sample_rate
+
+
+def get_tsv_from_wav_scp(wav_scp_path, output_tsv_path, num_thread=32):
+    """"""
+    print_str = "dict,不予展示"
+    logging_print(
+        f"get_tsv_from_wav_scp:开始处理如下wav_scp: {wav_scp_path if isinstance(wav_scp_path, str) else print_str}, tsv_path: {output_tsv_path}")
+    makedir_sil(output_tsv_path)
+    if isinstance(wav_scp_path, str):
+        wav_dict = load_dict_from_scp(wav_scp_path)
+    elif isinstance(wav_scp_path, dict):
+        wav_dict = wav_scp_path
+    else:
+        raise ValueError("get_tsv_from_wav_scp: wav_scp_path must be str or dict")
+    res_list = ["/"]
+    wav_list = list(wav_dict.values())
+    list_list = do_split_list(wav_list, num_thread)
+    runner = GxlDynamicThreadPool()
+    for list_i in list_list:
+        """"""
+        runner.add_task(little_fun4get_tsv_from_wav_scp, [res_list, list_i])
+    runner.start()
+    write_list_to_file(res_list, "./all_data_with_sample.tsv")
+
+
+def little_fun4get_tsv_from_wav_scp(res_list, wav_path_list):
+    temp_list = []
+    for wav_path in tqdm(wav_path_list, total=len(wav_path_list)):
+        """"""
+        from gxl_ai_utils.utils.utils_data import get_sample_count
+        samples, _ = get_sample_count(wav_path)
+        temp_list.append(f"{wav_path}\t{samples}")
+    res_list.extend(temp_list)
+
+
+def remove_dir(directory_to_delete):
+    """递归删除一整个目录"""
+    logging_print('remove_dir():开始删除目录:%s' % directory_to_delete)
+    shutil.rmtree(directory_to_delete)
+    logging_print('remove_dir():目录结束删除:%s' % directory_to_delete)
+
+
+def do_compress_file_by_gzip(input_file, output_file):
+    logging_print(f'开始使用gzip压缩文件：{input_file},压缩到:{output_file}')
+    with open(input_file, 'rb') as f_in:
+        with gzip.open(output_file, 'wb') as f_out:
+            f_out.writelines(f_in)
+    logging_print(f'完成使用gzip压缩文件：{input_file},压缩到:{output_file}')
+
+
+def do_merge_file(*input_file_list):
+    """
+    最后一个参数为输出
+    :param input_file_list:
+    :return:
+    """
+    if len(input_file_list) == 1:
+        logging_print('只有一个文件，直接返回')
+        return input_file_list[0]
+    if len(input_file_list) == 0:
+        logging_print('没有文件，直接返回')
+        return None
+    output_file = input_file_list[-1]
+    input_file_list = input_file_list[:-1]
+    logging_print(f'开始合并文件：{input_file_list},输出到：{output_file}')
+    with open(output_file, 'wb') as f_out:
+        for input_file in input_file_list:
+            with open(input_file, 'rb') as f_in:
+                f_out.writelines(f_in)
+    logging_print(f'完成合并文件：{input_file_list},输出到：{output_file}')
+
+
+def do_get_random_sublist(input_list, num):
+    """"""
+    return [input_list[i] for i in sorted(random.sample(range(len(input_list)), num))]
+
+
+def _do_compute_fbank4icefall(
+        num_mel_bins: int = 80,
+        perturb_speed: bool = False,
+        whisper_fbank: bool = False,
+        fbank_dir: str = "data/fbank",
+        manifests_dir: str = "data/manifests",
+        prefix: str = "gxldata",
+        partition: str = "train",  # train dev test
+):
+    from lhotse import (
+        CutSet,
+        Fbank,
+        FbankConfig,
+        LilcomChunkyWriter,
+        WhisperFbank,
+        WhisperFbankConfig,
+    )
+    from lhotse.recipes.utils import read_manifests_if_cached
+    sys.path.insert(0, '/home/work_nfs8/xlgeng/new_workspace/icefall')
+    try:
+        from icefall.utils import get_executor, str2bool
+    except ImportError:
+        pass
+    torch.set_num_threads(1)
+    torch.set_num_interop_threads(1)
+    makedir_sil(fbank_dir)
+    src_dir = Path(manifests_dir)
+    output_dir = Path(fbank_dir)
+    num_jobs = min(15, os.cpu_count())
+    dataset_parts = (
+        f"{partition}",
+    )
+    prefix = prefix
+    suffix = "jsonl.gz"
+    manifests = read_manifests_if_cached(
+        dataset_parts=dataset_parts,
+        output_dir=src_dir,
+        prefix=prefix,
+        suffix=suffix,
+    )
+    assert manifests is not None
+
+    assert len(manifests) == len(dataset_parts), (
+        len(manifests),
+        len(dataset_parts),
+        list(manifests.keys()),
+        dataset_parts,
+    )
+    if whisper_fbank:
+        extractor = WhisperFbank(
+            WhisperFbankConfig(num_filters=num_mel_bins, device="cuda")
+        )
+    else:
+        extractor = Fbank(FbankConfig(num_mel_bins=num_mel_bins))
+    with get_executor() as ex:  # Initialize the executor only once.
+        for partition, m in manifests.items():
+            if (output_dir / f"{prefix}_cuts_{partition}.{suffix}").is_file():
+                logging.info(f"{partition} already exists - skipping.")
+                continue
+            logging.info(f"Processing {partition}")
+            cut_set = CutSet.from_manifests(
+                recordings=m["recordings"],
+                supervisions=m["supervisions"],
+            )
+            if "train" in partition and perturb_speed:
+                logging.info("Doing speed perturb")
+                cut_set = (
+                        cut_set + cut_set.perturb_speed(0.9) + cut_set.perturb_speed(1.1)
+                )
+            cut_set = cut_set.compute_and_store_features(
+                extractor=extractor,
+                storage_path=f"{output_dir}/{prefix}_feats_{partition}",
+                # when an executor is specified, make more partitions
+                num_jobs=num_jobs if ex is None else 80,
+                executor=ex,
+                storage_type=LilcomChunkyWriter,
+            )
+            cut_set.to_file(output_dir / f"{prefix}_cuts_{partition}.{suffix}")
+
+
+def _do_convert_scp_to_manifest4icefall(wav_scp_path, text_scp_path, wav_manifest_path, text_manifest_path):
+    def build_wav_dict_for_icefall(key, input_wav_path):
+        sample_num, sample_rate = get_sample_count(input_wav_path)
+        # file_name = utils_file.get_file_pure_name_from_path(input_wav_path)
+        duration = sample_num / sample_rate
+        res_dict = {}
+        res_dict['id'] = key
+        res_dict['sources'] = [dict(
+            type='file',
+            channels=[0],
+            source=input_wav_path,
+        )]
+        res_dict['sampling_rate'] = sample_rate
+        res_dict['num_samples'] = sample_num
+        res_dict['duration'] = duration
+        res_dict['channel_ids'] = [0]
+        return res_dict
+
+    def build_text_dict_for_icefall(key, input_text_str, duration_dict):
+        if key not in duration_dict:
+            # utils_file.logging_print('key not in duration dict,也就是text中有的key wav.scp没有: ' + key)
+            return {}
+        res_dict = {}
+        res_dict['id'] = key
+        res_dict['recording_id'] = key
+        res_dict['start'] = 0.0
+        res_dict['duration'] = duration_dict[key]
+        res_dict['channel'] = 0
+        res_dict['text'] = input_text_str
+        res_dict['language'] = 'Chinese'
+        res_dict['speaker'] = 'S0901'
+        return res_dict
+
+    def little_func4wav_convert(res_list, wav_dict):
+        temp_list = []
+        for key, wav_path in tqdm.tqdm(wav_dict.items(), total=len(wav_dict)):
+            temp_list.append(build_wav_dict_for_icefall(key, wav_path))
+        res_list.extend(temp_list)
+
+    def little_func4text_convert(res_list, wav_dict, duration_dict):
+        temp_list = []
+        for key, wav_path in tqdm.tqdm(wav_dict.items(), total=len(wav_dict)):
+            temp_dict = build_text_dict_for_icefall(key, wav_path, duration_dict)
+            if len(temp_dict) > 0:
+                temp_list.append(temp_dict)
+        res_list.extend(temp_list)
+
+    logging_print('开始 do_convert_scp_to_manifest4icefall')
+    makedir_for_file(wav_manifest_path)
+    makedir_for_file(text_manifest_path)
+    wav_dict = load_dict_from_scp(wav_scp_path)
+    res_wav_dict_list = []
+    runner = GxlDynamicThreadPool()
+    wav_dict_list = do_split_dict(wav_dict, 32)
+    for wav_dict_i in wav_dict_list:
+        runner.add_task(little_func4wav_convert, [res_wav_dict_list, wav_dict_i])
+    logging_print('do_convert_scp_to_manifest():开始执行为wav生成manifest')
+    runner.start()
+    write_dict_list_to_jsonl(res_wav_dict_list, wav_manifest_path)
+    wav_manifest_path_gz = wav_manifest_path + '.gz'
+    do_compress_file_by_gzip(wav_manifest_path, wav_manifest_path_gz)
+    # res_wav_dict_list = utils_file.load_dict_list_from_jsonl(wav_manifest_path)
+
+    # 得到duration信息的字典
+    logging_print('do_convert_scp_to_manifest():开始生成duration字典')
+    duration_dict = {}
+    for dict_i in tqdm.tqdm(res_wav_dict_list, total=len(res_wav_dict_list)):
+        id = dict_i['id']
+        duration = dict_i['duration']
+        duration_dict[id] = duration
+    logging_print('do_convert_scp_to_manifest():生成duration字典完成')
+
+    res_text_dict_list = []
+    text_dict = load_dict_from_scp(text_scp_path)
+    runner = GxlDynamicThreadPool()
+    text_dict_list = do_split_dict(text_dict, 32)
+    for text_dict_i in text_dict_list:
+        runner.add_task(little_func4text_convert, [res_text_dict_list, text_dict_i, duration_dict])
+    logging_print('do_convert_scp_to_manifest():开始执行为text生成manifest')
+    runner.start()
+    write_dict_list_to_jsonl(res_text_dict_list, text_manifest_path)
+    text_manifest_path_gz = text_manifest_path + '.gz'
+    do_compress_file_by_gzip(text_manifest_path, text_manifest_path_gz)
+
+
+def do_make_data4icefall(wav_scp_path,
+                         text_scp_path,
+                         manifest_dir=None,
+                         fbank_dir=None,
+                         parent_dir= None,
+                         partition: str = 'train',
+                         prefix: str = 'gxldata',
+                         only_manifest: bool = False,
+                         only_fbank: bool = False):
+    """
+
+    :param wav_scp_path:
+    :param text_scp_path:
+    :param manifest_dir:
+    :param fbank_dir:
+    :param parent_dir: 如果设置了parent_dir,则manifest_dir 和 fbank_dir无效, 使用parent_dir和默认的目录名
+    :param partition:
+    :param prefix:
+    :return:
+    """
+
+    def get_jsonl_filename4icefall(prefix: str = 'gxldata', partition: str = 'train'):
+        return f'{prefix}_recordings_{partition}.jsonl', f'{prefix}_supervisions_{partition}.jsonl'
+
+    logging_print('开始处理{}的数据'.format(partition))
+    makedir_sil(manifest_dir)
+    makedir_sil(fbank_dir)
+    if not only_fbank:
+        logging_print('首先得到manifest,文件为.jsonl.gz')
+        manifest_wav_filename, manifest_text_filename = get_jsonl_filename4icefall(prefix, partition)
+        manifest_wav_path = os.path.join(manifest_dir, manifest_wav_filename)
+        manifest_text_path = os.path.join(manifest_dir, manifest_text_filename)
+        _do_convert_scp_to_manifest4icefall(wav_scp_path, text_scp_path, manifest_wav_path, manifest_text_path)
+        logging_print('得到manifest完成')
+    else:
+        logging_print(f'only_fbank={only_fbank}')
+        return
+    if not only_manifest:
+        logging_print('开始生成fbank')
+        _do_compute_fbank4icefall(
+            manifests_dir=manifest_dir,
+            fbank_dir=fbank_dir,
+            partition=partition,
+            prefix=prefix,
+            perturb_speed=(partition == 'train')
+        )
+        logging_print('生成fbank完成')
+    else:
+        logging_print(f'only_manifest={only_manifest}')
+        return
```

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_model.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_showing.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_showing.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/gxl_ai_utils/utils/utils_spider.py` & `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,26 +90,25 @@
 
 def handle_xpath(html_text: str, xpath: str):
     try:
         tree = etree.HTML(html_text)
         datas = tree.xpath(xpath)
         # datas = tree.cssselect(xpath)
         if len(datas) == 0:
-            print("datas:", datas)
-            raise RuntimeError()
+            print("warning:datas为空, 没得到应有的数据:", datas)
         return datas
     except Exception as e:
         print('xpath处理失败')
         traceback.print_exc()
         return None
 
 
-def download_file(url: str, file_name: str):
+def download_file(url: str, file_path: str):
     response = send_request(url)
-    with open(file_name, 'wb') as f:
+    with open(file_path, 'wb') as f:
         f.write(response.content)
 
 
 def handle_css_select(html_text: str, css_selector: str):
     try:
         tree = etree.HTML(html_text)
         datas = tree.cssselect(css_selector)
```

### Comparing `gxl_ai_utils-1.3.3/license.txt` & `gxl_ai_utils-1.3.4/license.txt`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.3/setup.py` & `gxl_ai_utils-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # from distutils.core import setup
 from setuptools import setup, find_packages
 
 # packages = ['gxl_ai_utils', 'gxl_ai_utils.utils',
 #             'gxl_ai_utils.config', 'gxl_ai_utils.run',
 #             'gxl_ai_utils.thread' ]
 setup(name='gxl_ai_utils',
-      version='1.3.3',
+      version='1.3.4',
       author='Xuelong Geng',
-      description='这个是耿雪龙的工具包模块, update time: 2024-3-19',
+      description='这个是耿雪龙的工具包模块, update time: 2024-4-9',
       author_email='3349495429@qq.com',
       packages=find_packages(),
       package_dir={'requests': 'requests'}, )
```

