# Comparing `tmp/elevenlabs-1.0.4.tar.gz` & `tmp/elevenlabs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-1.0.4.tar", max compression
+gzip compressed data, was "elevenlabs-1.0.5.tar", max compression
```

## Comparing `elevenlabs-1.0.4.tar` & `elevenlabs-1.0.5.tar`

### file list

```diff
@@ -1,121 +1,122 @@
--rw-r--r--   0        0        0     1067 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/LICENSE
--rw-r--r--   0        0        0     9356 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/README.md
--rw-r--r--   0        0        0      659 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4689 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/__init__.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/audio_native/__init__.py
--rw-r--r--   0        0        0    13565 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/audio_native/client.py
--rw-r--r--   0        0        0     7523 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/base_client.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/chapters/__init__.py
--rw-r--r--   0        0        0    34318 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/chapters/client.py
--rw-r--r--   0        0        0    20882 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/client.py
--rw-r--r--   0        0        0      790 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/api_error.py
--rw-r--r--   0        0        0     1683 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/dubbing/__init__.py
--rw-r--r--   0        0        0    27796 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/dubbing/client.py
--rw-r--r--   0        0        0      164 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/environment.py
--rw-r--r--   0        0        0      170 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/history/__init__.py
--rw-r--r--   0        0        0    27725 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/history/client.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/models/__init__.py
--rw-r--r--   0        0        0     5069 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/models/client.py
--rw-r--r--   0        0        0     2715 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/play.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/projects/__init__.py
--rw-r--r--   0        0        0    54697 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/projects/client.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/pronunciation_dictionary/__init__.py
--rw-r--r--   0        0        0    13080 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/pronunciation_dictionary/client.py
--rw-r--r--   0        0        0        0 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/py.typed
--rw-r--r--   0        0        0     5093 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/realtime_tts.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/samples/__init__.py
--rw-r--r--   0        0        0    11145 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/samples/client.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/speech_to_speech/__init__.py
--rw-r--r--   0        0        0    20960 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/speech_to_speech/client.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/text_to_speech/__init__.py
--rw-r--r--   0        0        0    23081 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/text_to_speech/client.py
--rw-r--r--   0        0        0     6114 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/__init__.py
--rw-r--r--   0        0        0      191 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/accent.py
--rw-r--r--   0        0        0      978 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/add_project_response_model.py
--rw-r--r--   0        0        0     1058 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
--rw-r--r--   0        0        0      919 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/add_voice_response_model.py
--rw-r--r--   0        0        0      161 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/age.py
--rw-r--r--   0        0        0      980 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/audio_native_create_project_response_model.py
--rw-r--r--   0        0        0      130 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
--rw-r--r--   0        0        0     1560 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/audio_output.py
--rw-r--r--   0        0        0     1196 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_response.py
--rw-r--r--   0        0        0     1011 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshot_response.py
--rw-r--r--   0        0        0     1019 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshots_response.py
--rw-r--r--   0        0        0      164 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_state.py
--rw-r--r--   0        0        0     1029 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_statistics_response.py
--rw-r--r--   0        0        0      149 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/currency.py
--rw-r--r--   0        0        0      950 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/do_dubbing_response.py
--rw-r--r--   0        0        0      214 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
--rw-r--r--   0        0        0     1082 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/feedback_item.py
--rw-r--r--   0        0        0     1837 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/fine_tuning_response.py
--rw-r--r--   0        0        0      223 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/finetuning_state.py
--rw-r--r--   0        0        0      151 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/gender.py
--rw-r--r--   0        0        0     2288 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/generation_config.py
--rw-r--r--   0        0        0      988 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_chapters_response.py
--rw-r--r--   0        0        0     1048 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_library_voices_response.py
--rw-r--r--   0        0        0      988 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_projects_response.py
--rw-r--r--   0        0        0     1041 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
--rw-r--r--   0        0        0     1073 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_speech_history_response.py
--rw-r--r--   0        0        0      953 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_voices_response.py
--rw-r--r--   0        0        0      101 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/history.py
--rw-r--r--   0        0        0      992 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/history_item.py
--rw-r--r--   0        0        0     1010 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/http_validation_error.py
--rw-r--r--   0        0        0      948 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/invoice.py
--rw-r--r--   0        0        0      931 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/language_response.py
--rw-r--r--   0        0        0     1639 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/library_voice_response.py
--rw-r--r--   0        0        0     1011 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_file_response.py
--rw-r--r--   0        0        0     1086 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_response.py
--rw-r--r--   0        0        0     1671 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/model.py
--rw-r--r--   0        0        0     2207 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/normalized_alignment.py
--rw-r--r--   0        0        0      176 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/optimize_streaming_latency.py
--rw-r--r--   0        0        0      408 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/output_format.py
--rw-r--r--   0        0        0     1278 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_extended_response_model.py
--rw-r--r--   0        0        0     1259 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_response.py
--rw-r--r--   0        0        0      991 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_snapshot_response.py
--rw-r--r--   0        0        0     1019 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_snapshots_response.py
--rw-r--r--   0        0        0      164 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_state.py
--rw-r--r--   0        0        0      974 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
--rw-r--r--   0        0        0     1477 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/realtime_voice_settings.py
--rw-r--r--   0        0        0     1007 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/recording_response.py
--rw-r--r--   0        0        0      220 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/review_status.py
--rw-r--r--   0        0        0     2353 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/send_text.py
--rw-r--r--   0        0        0      147 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/source.py
--rw-r--r--   0        0        0     1865 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/speech_history_item_response.py
--rw-r--r--   0        0        0      226 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
--rw-r--r--   0        0        0     1079 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/sso_provider_db_model.py
--rw-r--r--   0        0        0      173 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/sso_provider_db_model_provider_type.py
--rw-r--r--   0        0        0     1879 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription.py
--rw-r--r--   0        0        0     1611 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription_response.py
--rw-r--r--   0        0        0      200 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription_response_model_billing_period.py
--rw-r--r--   0        0        0      256 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription_status.py
--rw-r--r--   0        0        0     1141 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/user.py
--rw-r--r--   0        0        0     1029 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1120 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/verification_attempt_response.py
--rw-r--r--   0        0        0     1991 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice.py
--rw-r--r--   0        0        0      946 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_option_response.py
--rw-r--r--   0        0        0     1325 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_response.py
--rw-r--r--   0        0        0      216 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_response_model_safety_control.py
--rw-r--r--   0        0        0     1102 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_sample.py
--rw-r--r--   0        0        0     1083 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_settings.py
--rw-r--r--   0        0        0     2354 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_sharing_response.py
--rw-r--r--   0        0        0      196 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_sharing_state.py
--rw-r--r--   0        0        0     1245 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_verification_response.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/user/__init__.py
--rw-r--r--   0        0        0     9207 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/user/client.py
--rw-r--r--   0        0        0       78 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/version.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voice_generation/__init__.py
--rw-r--r--   0        0        0    20238 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voice_generation/client.py
--rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voices/__init__.py
--rw-r--r--   0        0        0    58857 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voices/client.py
--rw-r--r--   0        0        0     9948 1970-01-01 00:00:00.000000 elevenlabs-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/LICENSE
+-rw-r--r--   0        0        0     9366 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/README.md
+-rw-r--r--   0        0        0      659 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4749 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/audio_native/__init__.py
+-rw-r--r--   0        0        0    13565 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/audio_native/client.py
+-rw-r--r--   0        0        0     7523 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/chapters/__init__.py
+-rw-r--r--   0        0        0    34318 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/chapters/client.py
+-rw-r--r--   0        0        0    20882 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/client.py
+-rw-r--r--   0        0        0      790 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/api_error.py
+-rw-r--r--   0        0        0     1683 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/dubbing/__init__.py
+-rw-r--r--   0        0        0    27974 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/dubbing/client.py
+-rw-r--r--   0        0        0      164 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/environment.py
+-rw-r--r--   0        0        0      170 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/history/__init__.py
+-rw-r--r--   0        0        0    28349 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/history/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/models/__init__.py
+-rw-r--r--   0        0        0     5069 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/models/client.py
+-rw-r--r--   0        0        0     2715 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/play.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/projects/__init__.py
+-rw-r--r--   0        0        0    54697 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/projects/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/pronunciation_dictionary/__init__.py
+-rw-r--r--   0        0        0    18330 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/pronunciation_dictionary/client.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/py.typed
+-rw-r--r--   0        0        0     5093 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/realtime_tts.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/samples/__init__.py
+-rw-r--r--   0        0        0    11145 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/samples/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/speech_to_speech/__init__.py
+-rw-r--r--   0        0        0    27928 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/speech_to_speech/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/text_to_speech/__init__.py
+-rw-r--r--   0        0        0    23081 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/text_to_speech/client.py
+-rw-r--r--   0        0        0     6208 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/accent.py
+-rw-r--r--   0        0        0      978 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/add_project_response_model.py
+-rw-r--r--   0        0        0     1058 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
+-rw-r--r--   0        0        0      919 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/add_voice_response_model.py
+-rw-r--r--   0        0        0      161 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/age.py
+-rw-r--r--   0        0        0      980 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/audio_native_create_project_response_model.py
+-rw-r--r--   0        0        0      130 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
+-rw-r--r--   0        0        0     1560 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/audio_output.py
+-rw-r--r--   0        0        0     1196 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_response.py
+-rw-r--r--   0        0        0     1011 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshot_response.py
+-rw-r--r--   0        0        0     1019 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshots_response.py
+-rw-r--r--   0        0        0      164 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_state.py
+-rw-r--r--   0        0        0     1029 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_statistics_response.py
+-rw-r--r--   0        0        0      149 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/currency.py
+-rw-r--r--   0        0        0      950 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/do_dubbing_response.py
+-rw-r--r--   0        0        0     1007 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/dubbing_metadata_response.py
+-rw-r--r--   0        0        0      214 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0     1082 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/feedback_item.py
+-rw-r--r--   0        0        0     1837 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/fine_tuning_response.py
+-rw-r--r--   0        0        0      223 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/finetuning_state.py
+-rw-r--r--   0        0        0      151 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/gender.py
+-rw-r--r--   0        0        0     2288 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/generation_config.py
+-rw-r--r--   0        0        0      988 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_chapters_response.py
+-rw-r--r--   0        0        0     1048 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_library_voices_response.py
+-rw-r--r--   0        0        0      988 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_projects_response.py
+-rw-r--r--   0        0        0     1068 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
+-rw-r--r--   0        0        0     1073 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_speech_history_response.py
+-rw-r--r--   0        0        0      953 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_voices_response.py
+-rw-r--r--   0        0        0      101 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/history.py
+-rw-r--r--   0        0        0      992 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/history_item.py
+-rw-r--r--   0        0        0     1010 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/http_validation_error.py
+-rw-r--r--   0        0        0      948 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/invoice.py
+-rw-r--r--   0        0        0      931 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/language_response.py
+-rw-r--r--   0        0        0     1639 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/library_voice_response.py
+-rw-r--r--   0        0        0     1011 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_file_response.py
+-rw-r--r--   0        0        0     1086 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_response.py
+-rw-r--r--   0        0        0     1671 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/model.py
+-rw-r--r--   0        0        0     2207 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/normalized_alignment.py
+-rw-r--r--   0        0        0      176 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/optimize_streaming_latency.py
+-rw-r--r--   0        0        0      408 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/output_format.py
+-rw-r--r--   0        0        0     1278 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_extended_response_model.py
+-rw-r--r--   0        0        0     1259 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_response.py
+-rw-r--r--   0        0        0      991 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_snapshot_response.py
+-rw-r--r--   0        0        0     1019 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_snapshots_response.py
+-rw-r--r--   0        0        0      164 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_state.py
+-rw-r--r--   0        0        0      974 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
+-rw-r--r--   0        0        0     1477 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/realtime_voice_settings.py
+-rw-r--r--   0        0        0     1007 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/recording_response.py
+-rw-r--r--   0        0        0      220 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/review_status.py
+-rw-r--r--   0        0        0     2353 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/send_text.py
+-rw-r--r--   0        0        0      147 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/source.py
+-rw-r--r--   0        0        0     1865 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/speech_history_item_response.py
+-rw-r--r--   0        0        0      226 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
+-rw-r--r--   0        0        0     1079 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/sso_provider_db_model.py
+-rw-r--r--   0        0        0      173 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/sso_provider_db_model_provider_type.py
+-rw-r--r--   0        0        0     1879 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription.py
+-rw-r--r--   0        0        0     1611 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription_response.py
+-rw-r--r--   0        0        0      200 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0      256 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription_status.py
+-rw-r--r--   0        0        0     1141 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/user.py
+-rw-r--r--   0        0        0     1029 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1120 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/verification_attempt_response.py
+-rw-r--r--   0        0        0     2089 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice.py
+-rw-r--r--   0        0        0      946 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_option_response.py
+-rw-r--r--   0        0        0     1325 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_response.py
+-rw-r--r--   0        0        0      216 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_response_model_safety_control.py
+-rw-r--r--   0        0        0     1102 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_sample.py
+-rw-r--r--   0        0        0     1083 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_settings.py
+-rw-r--r--   0        0        0     2354 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_sharing_response.py
+-rw-r--r--   0        0        0      196 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_sharing_state.py
+-rw-r--r--   0        0        0     1245 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_verification_response.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/user/__init__.py
+-rw-r--r--   0        0        0     9207 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/user/client.py
+-rw-r--r--   0        0        0       78 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/version.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voice_generation/__init__.py
+-rw-r--r--   0        0        0    20232 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voice_generation/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voices/__init__.py
+-rw-r--r--   0        0        0    59193 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voices/client.py
+-rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.0.5/PKG-INFO
```

### Comparing `elevenlabs-1.0.4/LICENSE` & `elevenlabs-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/README.md` & `elevenlabs-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## ⚙️ Install
 
 ```bash
 pip install elevenlabs
 ```
 
 ## v0.x to v1.x Migration Guide
-> The SDK was rewritten in v1 and is now programatically generated from our OpenAPI spec. As part of this release 
+> The SDK was rewritten in v1 and is now programmatically generated from our OpenAPI spec. As part of this release 
 > there are some breaking changes. 
 
 
 ### Client Instantiation
 The SDK now exports a client class that you must instantiate to call various
 endpoints in our API. 
 
@@ -139,15 +139,15 @@
 
 client = ElevenLabs(
   api_key="YOUR_API_KEY", # Defaults to ELEVEN_API_KEY
 )
 
 response = client.voices.get_all()
 audio = client.generate(text="Hello there!", voice=response.voices[0])
-print(voices)
+print(response.voices)
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
 [
   Voice(
```

### Comparing `elevenlabs-1.0.4/pyproject.toml` & `elevenlabs-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elevenlabs"
-version = "v1.0.4"
+version = "v1.0.5"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "elevenlabs", from = "src"}
 ]
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/__init__.py` & `elevenlabs-1.0.5/src/elevenlabs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ChapterResponse,
     ChapterSnapshotResponse,
     ChapterSnapshotsResponse,
     ChapterState,
     ChapterStatisticsResponse,
     Currency,
     DoDubbingResponse,
+    DubbingMetadataResponse,
     ExtendedSubscriptionResponseModelBillingPeriod,
     FeedbackItem,
     FineTuningResponse,
     FinetuningState,
     Gender,
     GenerationConfig,
     GetChaptersResponse,
@@ -105,14 +106,15 @@
     "ChapterResponse",
     "ChapterSnapshotResponse",
     "ChapterSnapshotsResponse",
     "ChapterState",
     "ChapterStatisticsResponse",
     "Currency",
     "DoDubbingResponse",
+    "DubbingMetadataResponse",
     "ElevenLabsEnvironment",
     "ExtendedSubscriptionResponseModelBillingPeriod",
     "FeedbackItem",
     "FineTuningResponse",
     "FinetuningState",
     "Gender",
     "GenerationConfig",
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/audio_native/client.py` & `elevenlabs-1.0.5/src/elevenlabs/audio_native/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/base_client.py` & `elevenlabs-1.0.5/src/elevenlabs/base_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/chapters/client.py` & `elevenlabs-1.0.5/src/elevenlabs/chapters/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/client.py` & `elevenlabs-1.0.5/src/elevenlabs/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/__init__.py` & `elevenlabs-1.0.5/src/elevenlabs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/client_wrapper.py` & `elevenlabs-1.0.5/src/elevenlabs/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "elevenlabs",
-            "X-Fern-SDK-Version": "v1.0.4",
+            "X-Fern-SDK-Version": "v1.0.5",
         }
         if self._api_key is not None:
             headers["xi-api-key"] = self._api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/datetime_utils.py` & `elevenlabs-1.0.5/src/elevenlabs/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/file.py` & `elevenlabs-1.0.5/src/elevenlabs/core/file.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/http_client.py` & `elevenlabs-1.0.5/src/elevenlabs/core/http_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/jsonable_encoder.py` & `elevenlabs-1.0.5/src/elevenlabs/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/core/request_options.py` & `elevenlabs-1.0.5/src/elevenlabs/core/request_options.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/dubbing/client.py` & `elevenlabs-1.0.5/src/elevenlabs/dubbing/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.do_dubbing_response import DoDubbingResponse
+from ..types.dubbing_metadata_response import DubbingMetadataResponse
 from ..types.http_validation_error import HttpValidationError
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -166,15 +167,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_dubbing_project_metadata(
         self, dubbing_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> DubbingMetadataResponse:
         """
         Returns metadata about a dubbing project, including whether it's still in progress or not
 
         Parameters:
             - dubbing_id: str. ID of the dubbing project.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -207,15 +208,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DubbingMetadataResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -270,17 +271,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_dubbed_file(
         self, dubbing_id: str, language_code: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> None:
         """
-        Returns dubbed file.
+        Returns dubbed file as a streamed file. Videos will be returned in MP4 format and audio only dubs will be returned in MP3.
 
         Parameters:
             - dubbing_id: str. ID of the dubbing project.
 
             - language_code: str. ID of the language.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -315,15 +316,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -472,15 +473,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_dubbing_project_metadata(
         self, dubbing_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> DubbingMetadataResponse:
         """
         Returns metadata about a dubbing project, including whether it's still in progress or not
 
         Parameters:
             - dubbing_id: str. ID of the dubbing project.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -513,15 +514,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DubbingMetadataResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -576,17 +577,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_dubbed_file(
         self, dubbing_id: str, language_code: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> None:
         """
-        Returns dubbed file.
+        Returns dubbed file as a streamed file. Videos will be returned in MP4 format and audio only dubs will be returned in MP3.
 
         Parameters:
             - dubbing_id: str. ID of the dubbing project.
 
             - language_code: str. ID of the language.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -621,15 +622,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/history/client.py` & `elevenlabs-1.0.5/src/elevenlabs/history/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,43 +247,52 @@
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def download(
-        self, *, history_item_ids: typing.Sequence[str], request_options: typing.Optional[RequestOptions] = None
+        self,
+        *,
+        history_item_ids: typing.Sequence[str],
+        output_format: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Download one or more history items. If one history item ID is provided, we will return a single audio file. If more than one history item IDs are provided, we will provide the history items packed into a .zip file.
 
         Parameters:
             - history_item_ids: typing.Sequence[str]. A list of history items to download, you can get IDs of history items and other metadata using the GET https://api.elevenlabs.io/v1/history endpoint.
 
+            - output_format: typing.Optional[str]. Output format to transcode the audio file, can be wav or default.
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.download(
             history_item_ids=["history_item_ids"],
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"history_item_ids": history_item_ids}
+        if output_format is not OMIT:
+            _request["output_format"] = output_format
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history/download"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"history_item_ids": history_item_ids})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"history_item_ids": history_item_ids}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -499,15 +508,15 @@
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.get_audio(
             history_item_id="string",
         )
         """
-        async with await self._client_wrapper.httpx_client.stream(
+        async with self._client_wrapper.httpx_client.stream(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}/audio"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
@@ -533,43 +542,52 @@
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def download(
-        self, *, history_item_ids: typing.Sequence[str], request_options: typing.Optional[RequestOptions] = None
+        self,
+        *,
+        history_item_ids: typing.Sequence[str],
+        output_format: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Download one or more history items. If one history item ID is provided, we will return a single audio file. If more than one history item IDs are provided, we will provide the history items packed into a .zip file.
 
         Parameters:
             - history_item_ids: typing.Sequence[str]. A list of history items to download, you can get IDs of history items and other metadata using the GET https://api.elevenlabs.io/v1/history endpoint.
 
+            - output_format: typing.Optional[str]. Output format to transcode the audio file, can be wav or default.
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.download(
             history_item_ids=["history_item_ids"],
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"history_item_ids": history_item_ids}
+        if output_format is not OMIT:
+            _request["output_format"] = output_format
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history/download"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"history_item_ids": history_item_ids})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"history_item_ids": history_item_ids}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/models/client.py` & `elevenlabs-1.0.5/src/elevenlabs/models/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/play.py` & `elevenlabs-1.0.5/src/elevenlabs/play.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/projects/client.py` & `elevenlabs-1.0.5/src/elevenlabs/projects/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/pronunciation_dictionary/client.py` & `elevenlabs-1.0.5/src/elevenlabs/pronunciation_dictionary/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -90,14 +90,70 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_pls_file_with_a_pronunciation_dictionary_version_rules(
+        self, dictionary_id: str, version_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> typing.Any:
+        """
+        Get PLS file with a pronunciation dictionary version rules
+
+        Parameters:
+            - dictionary_id: str. The id of the pronunciation dictionary
+
+            - version_id: str. The id of the version of the pronunciation dictionary
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from elevenlabs.client import ElevenLabs
+
+        client = ElevenLabs(
+            api_key="YOUR_API_KEY",
+        )
+        client.pronunciation_dictionary.get_pls_file_with_a_pronunciation_dictionary_version_rules(
+            dictionary_id="dictionary_id",
+            version_id="version_id",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"v1/pronunciation-dictionaries/{jsonable_encoder(dictionary_id)}/{jsonable_encoder(version_id)}/download",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def get_metadata_for_a_pronunciation_dictionary_v_1_pronunciation_dictionaries_pronunciation_dictionary_id_get(
         self, pronunciation_dictionary_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetPronunciationDictionaryMetadataResponse:
         """
         Get metadata for a pronunciation dictionary
 
         Parameters:
@@ -213,14 +269,70 @@
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_pls_file_with_a_pronunciation_dictionary_version_rules(
+        self, dictionary_id: str, version_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> typing.Any:
+        """
+        Get PLS file with a pronunciation dictionary version rules
+
+        Parameters:
+            - dictionary_id: str. The id of the pronunciation dictionary
+
+            - version_id: str. The id of the version of the pronunciation dictionary
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from elevenlabs.client import AsyncElevenLabs
+
+        client = AsyncElevenLabs(
+            api_key="YOUR_API_KEY",
+        )
+        await client.pronunciation_dictionary.get_pls_file_with_a_pronunciation_dictionary_version_rules(
+            dictionary_id="dictionary_id",
+            version_id="version_id",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"v1/pronunciation-dictionaries/{jsonable_encoder(dictionary_id)}/{jsonable_encoder(version_id)}/download",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_metadata_for_a_pronunciation_dictionary_v_1_pronunciation_dictionaries_pronunciation_dictionary_id_get(
         self, pronunciation_dictionary_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetPronunciationDictionaryMetadataResponse:
         """
         Get metadata for a pronunciation dictionary
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/realtime_tts.py` & `elevenlabs-1.0.5/src/elevenlabs/realtime_tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/samples/client.py` & `elevenlabs-1.0.5/src/elevenlabs/samples/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/speech_to_speech/client.py` & `elevenlabs-1.0.5/src/elevenlabs/text_to_speech/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,122 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..types.optimize_streaming_latency import OptimizeStreamingLatency
+from ..types.output_format import OutputFormat
+from ..types.pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
+from ..types.voice_settings import VoiceSettings
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class SpeechToSpeechClient:
+class TextToSpeechClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def convert(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        optimize_streaming_latency: OptimizeStreamingLatency,
+        output_format: OutputFormat,
+        text: str,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice.
+        Converts text into speech using a voice of your choice and returns audio.
 
         Parameters:
             - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
+            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-                                                                Defaults to 0.
-            - audio: core.File. See core.File for more documentation
+            - output_format: OutputFormat. The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+            - text: str. The text that will get converted into speech.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.speech_to_speech.convert(
+        client.text_to_speech.convert(
             voice_id="string",
-            optimize_streaming_latency=1,
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
+                        "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -110,76 +138,101 @@
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert_as_stream(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        optimize_streaming_latency: OptimizeStreamingLatency,
+        output_format: OutputFormat,
+        text: str,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice and returns an audio stream.
+        Converts text into speech using a voice of your choice and returns audio as an audio stream.
 
         Parameters:
             - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
+            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-                                                                Defaults to 0.
-            - audio: core.File. See core.File for more documentation
+            - output_format: OutputFormat. The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+            - text: str. The text that will get converted into speech.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.speech_to_speech.convert_as_stream(
+        client.text_to_speech.convert_as_stream(
             voice_id="string",
-            optimize_streaming_latency=1,
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
+                        "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -198,84 +251,109 @@
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncSpeechToSpeechClient:
+class AsyncTextToSpeechClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def convert(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        optimize_streaming_latency: OptimizeStreamingLatency,
+        output_format: OutputFormat,
+        text: str,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice.
+        Converts text into speech using a voice of your choice and returns audio.
 
         Parameters:
             - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
+            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-                                                                Defaults to 0.
-            - audio: core.File. See core.File for more documentation
+            - output_format: OutputFormat. The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+            - text: str. The text that will get converted into speech.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.speech_to_speech.convert(
+        await client.text_to_speech.convert(
             voice_id="string",
-            optimize_streaming_latency=1,
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
-        async with await self._client_wrapper.httpx_client.stream(
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
+        async with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
+                        "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -297,76 +375,101 @@
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert_as_stream(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        optimize_streaming_latency: OptimizeStreamingLatency,
+        output_format: OutputFormat,
+        text: str,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice and returns an audio stream.
+        Converts text into speech using a voice of your choice and returns audio as an audio stream.
 
         Parameters:
             - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
+            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-                                                                Defaults to 0.
-            - audio: core.File. See core.File for more documentation
+            - output_format: OutputFormat. The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+            - text: str. The text that will get converted into speech.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.speech_to_speech.convert_as_stream(
+        await client.text_to_speech.convert_as_stream(
             voice_id="string",
-            optimize_streaming_latency=1,
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="string",
+            model_id="string",
+            voice_settings=VoiceSettings(
+                stability=1.1,
+                similarity_boost=1.1,
+                style=1.1,
+                use_speaker_boost=True,
+            ),
+            pronunciation_dictionary_locators=[
+                PronunciationDictionaryVersionLocator(
+                    pronunciation_dictionary_id="string",
+                    version_id="string",
+                )
+            ],
         )
         """
-        async with await self._client_wrapper.httpx_client.stream(
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
+        async with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
+                        "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/text_to_speech/client.py` & `elevenlabs-1.0.5/src/elevenlabs/voice_generation/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,116 +5,133 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
-from ..types.optimize_streaming_latency import OptimizeStreamingLatency
-from ..types.output_format import OutputFormat
-from ..types.pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
-from ..types.voice_settings import VoiceSettings
+from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.age import Age
+from ..types.gender import Gender
+from ..types.http_validation_error import HttpValidationError
+from ..types.voice import Voice
+from ..types.voice_generation_parameter_response import VoiceGenerationParameterResponse
+
+try:
+    import pydantic.v1 as pydantic  # type: ignore
+except ImportError:
+    import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class TextToSpeechClient:
+class VoiceGenerationClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def convert(
+    def generate_parameters(
+        self, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> VoiceGenerationParameterResponse:
+        """
+        Get possible parameters for the /v1/voice-generation/generate-voice endpoint.
+
+        Parameters:
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from elevenlabs.client import ElevenLabs
+
+        client = ElevenLabs(
+            api_key="YOUR_API_KEY",
+        )
+        client.voice_generation.generate_parameters()
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice/parameters"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(VoiceGenerationParameterResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def generate(
         self,
-        voice_id: str,
         *,
-        optimize_streaming_latency: OptimizeStreamingLatency,
-        output_format: OutputFormat,
+        gender: Gender,
+        accent: str,
+        age: Age,
+        accent_strength: float,
         text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Converts text into speech using a voice of your choice and returns audio.
+        Generate a random voice based on parameters. This method returns a generated_voice_id in the response header, and a sample of the voice in the body. If you like the generated voice call /v1/voice-generation/create-voice with the generated_voice_id to create the voice.
 
         Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+            - gender: Gender. Category code corresponding to the gender of the generated voice. Possible values: female, male.
 
-            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+            - accent: str. Category code corresponding to the accent of the generated voice. Possible values: american, british, african, australian, indian.
 
-            - output_format: OutputFormat. The output format of the generated audio.
+            - age: Age. Category code corresponding to the age of the generated voice. Possible values: young, middle_aged, old.
 
-            - text: str. The text that will get converted into speech.
+            - accent_strength: float. The strength of the accent of the generated voice. Has to be between 0.3 and 2.0.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
-
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
-
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+            - text: str. Text to generate, text length has to be between 100 and 1000.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.text_to_speech.convert(
-            voice_id="string",
-            optimize_streaming_latency="0",
-            output_format="mp3_22050_32",
+        client.voice_generation.generate(
+            gender="male",
+            accent="string",
+            age="young",
+            accent_strength=1.1,
             text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "optimize_streaming_latency": optimize_streaming_latency,
-                        "output_format": output_format,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder(
+                {"gender": gender, "accent": accent, "age": age, "accent_strength": accent_strength, "text": text}
+            )
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder(
+                    {"gender": gender, "accent": accent, "age": age, "accent_strength": accent_strength, "text": text}
+                ),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -134,98 +151,60 @@
             _response.read()
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def convert_as_stream(
+    def create_a_previously_generated_voice(
         self,
-        voice_id: str,
         *,
-        optimize_streaming_latency: OptimizeStreamingLatency,
-        output_format: OutputFormat,
-        text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
+        voice_name: str,
+        voice_description: str,
+        generated_voice_id: str,
+        labels: typing.Optional[typing.Dict[str, str]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> typing.Iterator[bytes]:
+    ) -> Voice:
         """
-        Converts text into speech using a voice of your choice and returns audio as an audio stream.
+        Create a previously generated voice. This endpoint should be called after you fetched a generated_voice_id using /v1/voice-generation/generate-voice.
 
         Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+            - voice_name: str. Name to use for the created voice.
 
-            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+            - voice_description: str. Description to use for the created voice.
 
-            - output_format: OutputFormat. The output format of the generated audio.
+            - generated_voice_id: str. The generated_voice_id to create, call POST /v1/voice-generation/generate-voice and fetch the generated_voice_id from the response header if don't have one yet.
 
-            - text: str. The text that will get converted into speech.
-
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
-
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
-
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+            - labels: typing.Optional[typing.Dict[str, str]]. Optional, metadata to add to the created voice. Defaults to None.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.text_to_speech.convert_as_stream(
-            voice_id="string",
-            optimize_streaming_latency="0",
-            output_format="mp3_22050_32",
-            text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
+        client.voice_generation.create_a_previously_generated_voice(
+            voice_name="voice_name",
+            voice_description="voice_description",
+            generated_voice_id="generated_voice_id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
-        with self._client_wrapper.httpx_client.stream(
+        _request: typing.Dict[str, typing.Any] = {
+            "voice_name": voice_name,
+            "voice_description": voice_description,
+            "generated_voice_id": generated_voice_id,
+        }
+        if labels is not OMIT:
+            _request["labels"] = labels
+        _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/create-voice"),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "optimize_streaming_latency": optimize_streaming_latency,
-                        "output_format": output_format,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -238,120 +217,129 @@
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        ) as _response:
-            if 200 <= _response.status_code < 300:
-                for _chunk in _response.iter_bytes():
-                    yield _chunk
-                return
-            _response.read()
-            try:
-                _response_json = _response.json()
-            except JSONDecodeError:
-                raise ApiError(status_code=_response.status_code, body=_response.text)
-            raise ApiError(status_code=_response.status_code, body=_response_json)
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(Voice, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTextToSpeechClient:
+class AsyncVoiceGenerationClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def convert(
+    async def generate_parameters(
+        self, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> VoiceGenerationParameterResponse:
+        """
+        Get possible parameters for the /v1/voice-generation/generate-voice endpoint.
+
+        Parameters:
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from elevenlabs.client import AsyncElevenLabs
+
+        client = AsyncElevenLabs(
+            api_key="YOUR_API_KEY",
+        )
+        await client.voice_generation.generate_parameters()
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice/parameters"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(VoiceGenerationParameterResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def generate(
         self,
-        voice_id: str,
         *,
-        optimize_streaming_latency: OptimizeStreamingLatency,
-        output_format: OutputFormat,
+        gender: Gender,
+        accent: str,
+        age: Age,
+        accent_strength: float,
         text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Converts text into speech using a voice of your choice and returns audio.
+        Generate a random voice based on parameters. This method returns a generated_voice_id in the response header, and a sample of the voice in the body. If you like the generated voice call /v1/voice-generation/create-voice with the generated_voice_id to create the voice.
 
         Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+            - gender: Gender. Category code corresponding to the gender of the generated voice. Possible values: female, male.
 
-            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+            - accent: str. Category code corresponding to the accent of the generated voice. Possible values: american, british, african, australian, indian.
 
-            - output_format: OutputFormat. The output format of the generated audio.
+            - age: Age. Category code corresponding to the age of the generated voice. Possible values: young, middle_aged, old.
 
-            - text: str. The text that will get converted into speech.
+            - accent_strength: float. The strength of the accent of the generated voice. Has to be between 0.3 and 2.0.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
-
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
-
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+            - text: str. Text to generate, text length has to be between 100 and 1000.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.text_to_speech.convert(
-            voice_id="string",
-            optimize_streaming_latency="0",
-            output_format="mp3_22050_32",
+        await client.voice_generation.generate(
+            gender="male",
+            accent="string",
+            age="young",
+            accent_strength=1.1,
             text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "optimize_streaming_latency": optimize_streaming_latency,
-                        "output_format": output_format,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder(
+                {"gender": gender, "accent": accent, "age": age, "accent_strength": accent_strength, "text": text}
+            )
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder(
+                    {"gender": gender, "accent": accent, "age": age, "accent_strength": accent_strength, "text": text}
+                ),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -371,98 +359,60 @@
             await _response.aread()
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def convert_as_stream(
+    async def create_a_previously_generated_voice(
         self,
-        voice_id: str,
         *,
-        optimize_streaming_latency: OptimizeStreamingLatency,
-        output_format: OutputFormat,
-        text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
+        voice_name: str,
+        voice_description: str,
+        generated_voice_id: str,
+        labels: typing.Optional[typing.Dict[str, str]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> typing.AsyncIterator[bytes]:
+    ) -> Voice:
         """
-        Converts text into speech using a voice of your choice and returns audio as an audio stream.
+        Create a previously generated voice. This endpoint should be called after you fetched a generated_voice_id using /v1/voice-generation/generate-voice.
 
         Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+            - voice_name: str. Name to use for the created voice.
 
-            - optimize_streaming_latency: OptimizeStreamingLatency. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+            - voice_description: str. Description to use for the created voice.
 
-            - output_format: OutputFormat. The output format of the generated audio.
+            - generated_voice_id: str. The generated_voice_id to create, call POST /v1/voice-generation/generate-voice and fetch the generated_voice_id from the response header if don't have one yet.
 
-            - text: str. The text that will get converted into speech.
-
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
-
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
-
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+            - labels: typing.Optional[typing.Dict[str, str]]. Optional, metadata to add to the created voice. Defaults to None.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.text_to_speech.convert_as_stream(
-            voice_id="string",
-            optimize_streaming_latency="0",
-            output_format="mp3_22050_32",
-            text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
+        await client.voice_generation.create_a_previously_generated_voice(
+            voice_name="voice_name",
+            voice_description="voice_description",
+            generated_voice_id="generated_voice_id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
-        async with self._client_wrapper.httpx_client.stream(
+        _request: typing.Dict[str, typing.Any] = {
+            "voice_name": voice_name,
+            "voice_description": voice_description,
+            "generated_voice_id": generated_voice_id,
+        }
+        if labels is not OMIT:
+            _request["labels"] = labels
+        _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/create-voice"),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "optimize_streaming_latency": optimize_streaming_latency,
-                        "output_format": output_format,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -475,18 +425,17 @@
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        ) as _response:
-            if 200 <= _response.status_code < 300:
-                async for _chunk in _response.aiter_bytes():
-                    yield _chunk
-                return
-            await _response.aread()
-            try:
-                _response_json = _response.json()
-            except JSONDecodeError:
-                raise ApiError(status_code=_response.status_code, body=_response.text)
-            raise ApiError(status_code=_response.status_code, body=_response_json)
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(Voice, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/__init__.py` & `elevenlabs-1.0.5/src/elevenlabs/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .chapter_response import ChapterResponse
 from .chapter_snapshot_response import ChapterSnapshotResponse
 from .chapter_snapshots_response import ChapterSnapshotsResponse
 from .chapter_state import ChapterState
 from .chapter_statistics_response import ChapterStatisticsResponse
 from .currency import Currency
 from .do_dubbing_response import DoDubbingResponse
+from .dubbing_metadata_response import DubbingMetadataResponse
 from .extended_subscription_response_model_billing_period import ExtendedSubscriptionResponseModelBillingPeriod
 from .feedback_item import FeedbackItem
 from .fine_tuning_response import FineTuningResponse
 from .finetuning_state import FinetuningState
 from .gender import Gender
 from .generation_config import GenerationConfig
 from .get_chapters_response import GetChaptersResponse
@@ -84,14 +85,15 @@
     "ChapterResponse",
     "ChapterSnapshotResponse",
     "ChapterSnapshotsResponse",
     "ChapterState",
     "ChapterStatisticsResponse",
     "Currency",
     "DoDubbingResponse",
+    "DubbingMetadataResponse",
     "ExtendedSubscriptionResponseModelBillingPeriod",
     "FeedbackItem",
     "FineTuningResponse",
     "FinetuningState",
     "Gender",
     "GenerationConfig",
     "GetChaptersResponse",
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/add_project_response_model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/add_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/add_voice_response_model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/add_voice_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/audio_native_create_project_response_model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/audio_native_create_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/audio_output.py` & `elevenlabs-1.0.5/src/elevenlabs/types/audio_output.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/chapter_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/chapter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshot_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshots_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/chapter_statistics_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/chapter_statistics_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/do_dubbing_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/do_dubbing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/feedback_item.py` & `elevenlabs-1.0.5/src/elevenlabs/types/feedback_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/fine_tuning_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/generation_config.py` & `elevenlabs-1.0.5/src/elevenlabs/types/generation_config.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/get_chapters_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/get_chapters_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/get_library_voices_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/get_library_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/get_projects_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/invoice.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetPronunciationDictionaryMetadataResponse(pydantic.BaseModel):
-    id: str
-    name: str
-    created_by: str
-    creation_time_unix: int
-    description: typing.Optional[str] = None
+class Invoice(pydantic.BaseModel):
+    amount_due_cents: int
+    next_payment_attempt_unix: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/get_speech_history_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/get_speech_history_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/get_voices_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/get_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/history_item.py` & `elevenlabs-1.0.5/src/elevenlabs/types/history_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/http_validation_error.py` & `elevenlabs-1.0.5/src/elevenlabs/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/invoice.py` & `elevenlabs-1.0.5/src/elevenlabs/types/recording_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Invoice(pydantic.BaseModel):
-    amount_due_cents: int
-    next_payment_attempt_unix: int
+class RecordingResponse(pydantic.BaseModel):
+    recording_id: str
+    mime_type: str
+    size_bytes: int
+    upload_date_unix: int
+    transcription: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/language_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/language_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/library_voice_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/library_voice_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_file_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_file_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/normalized_alignment.py` & `elevenlabs-1.0.5/src/elevenlabs/types/normalized_alignment.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/project_extended_response_model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/project_extended_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/project_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/project_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/project_snapshot_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/project_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/project_snapshots_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/project_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/pronunciation_dictionary_version_locator.py` & `elevenlabs-1.0.5/src/elevenlabs/types/pronunciation_dictionary_version_locator.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/realtime_voice_settings.py` & `elevenlabs-1.0.5/src/elevenlabs/types/realtime_voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/recording_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_option_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class RecordingResponse(pydantic.BaseModel):
-    recording_id: str
-    mime_type: str
-    size_bytes: int
-    upload_date_unix: int
-    transcription: str
+class VoiceGenerationParameterOptionResponse(pydantic.BaseModel):
+    name: str
+    code: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/send_text.py` & `elevenlabs-1.0.5/src/elevenlabs/types/send_text.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/speech_history_item_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/speech_history_item_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/sso_provider_db_model.py` & `elevenlabs-1.0.5/src/elevenlabs/types/sso_provider_db_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/subscription.py` & `elevenlabs-1.0.5/src/elevenlabs/types/subscription.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/subscription_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/subscription_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/user.py` & `elevenlabs-1.0.5/src/elevenlabs/types/user.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/validation_error.py` & `elevenlabs-1.0.5/src/elevenlabs/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/verification_attempt_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/verification_attempt_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     preview_url: typing.Optional[str] = None
     available_for_tiers: typing.Optional[typing.List[str]] = None
     settings: typing.Optional[VoiceSettings] = None
     sharing: typing.Optional[VoiceSharingResponse] = None
     high_quality_base_model_ids: typing.Optional[typing.List[str]] = None
     safety_control: typing.Optional[VoiceResponseModelSafetyControl] = None
     voice_verification: typing.Optional[VoiceVerificationResponse] = None
+    owner_id: typing.Optional[str] = None
+    permission_on_resource: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_option_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/dubbing_metadata_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class VoiceGenerationParameterOptionResponse(pydantic.BaseModel):
+class DubbingMetadataResponse(pydantic.BaseModel):
+    dubbing_id: str
     name: str
-    code: str
+    status: str
+    error: str
+    target_languages: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice_sample.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice_sample.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice_settings.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice_sharing_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice_sharing_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     financial_rewards_enabled: typing.Optional[bool] = None
     free_users_allowed: typing.Optional[bool] = None
     live_moderation_enabled: typing.Optional[bool] = None
     rate: typing.Optional[float] = None
     notice_period: typing.Optional[int] = None
     disable_at_unix: typing.Optional[int] = None
     voice_mixing_allowed: typing.Optional[bool] = None
-    instagram_username: typing.Optional[str] = None
-    twitter_username: typing.Optional[str] = None
-    youtube_username: typing.Optional[str] = None
-    tiktok_username: typing.Optional[str] = None
     featured: typing.Optional[bool] = None
     ban_reason: typing.Optional[str] = None
     liked_by_count: typing.Optional[int] = None
     cloned_by_count: typing.Optional[int] = None
     name: typing.Optional[str] = None
     description: typing.Optional[str] = None
     labels: typing.Optional[typing.Dict[str, str]] = None
     review_status: typing.Optional[ReviewStatus] = None
     review_message: typing.Optional[str] = None
     enabled_in_library: typing.Optional[bool] = None
+    instagram_username: typing.Optional[str] = None
+    twitter_username: typing.Optional[str] = None
+    youtube_username: typing.Optional[str] = None
+    tiktok_username: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `elevenlabs-1.0.4/src/elevenlabs/types/voice_verification_response.py` & `elevenlabs-1.0.5/src/elevenlabs/types/voice_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/user/client.py` & `elevenlabs-1.0.5/src/elevenlabs/user/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.4/src/elevenlabs/voices/client.py` & `elevenlabs-1.0.5/src/elevenlabs/voices/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,36 +557,39 @@
         self,
         *,
         page_size: typing.Optional[int] = None,
         category: typing.Optional[str] = None,
         gender: typing.Optional[str] = None,
         age: typing.Optional[str] = None,
         accent: typing.Optional[str] = None,
+        language: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
         use_cases: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         descriptives: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         sort: typing.Optional[str] = None,
         featured: typing.Optional[bool] = None,
         page: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetLibraryVoicesResponse:
         """
         Gets a list of shared voices.
 
         Parameters:
-            - page_size: typing.Optional[int]. How many shared voices to return at maximum. Can not exceed 500, defaults to 30.
+            - page_size: typing.Optional[int]. How many shared voices to return at maximum. Can not exceed 100, defaults to 30.
 
             - category: typing.Optional[str]. voice category used for filtering
 
             - gender: typing.Optional[str]. gender used for filtering
 
             - age: typing.Optional[str]. age used for filtering
 
             - accent: typing.Optional[str]. accent used for filtering
 
+            - language: typing.Optional[str]. language used for filtering
+
             - search: typing.Optional[str]. search term used for filtering
 
             - use_cases: typing.Optional[typing.Union[str, typing.Sequence[str]]]. use-case used for filtering
 
             - descriptives: typing.Optional[typing.Union[str, typing.Sequence[str]]]. search term used for filtering
 
             - sort: typing.Optional[str]. sort criteria
@@ -611,14 +614,15 @@
                 remove_none_from_dict(
                     {
                         "page_size": page_size,
                         "category": category,
                         "gender": gender,
                         "age": age,
                         "accent": accent,
+                        "language": language,
                         "search": search,
                         "use_cases": use_cases,
                         "descriptives": descriptives,
                         "sort": sort,
                         "featured": featured,
                         "page": page,
                         **(
@@ -1186,36 +1190,39 @@
         self,
         *,
         page_size: typing.Optional[int] = None,
         category: typing.Optional[str] = None,
         gender: typing.Optional[str] = None,
         age: typing.Optional[str] = None,
         accent: typing.Optional[str] = None,
+        language: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
         use_cases: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         descriptives: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         sort: typing.Optional[str] = None,
         featured: typing.Optional[bool] = None,
         page: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetLibraryVoicesResponse:
         """
         Gets a list of shared voices.
 
         Parameters:
-            - page_size: typing.Optional[int]. How many shared voices to return at maximum. Can not exceed 500, defaults to 30.
+            - page_size: typing.Optional[int]. How many shared voices to return at maximum. Can not exceed 100, defaults to 30.
 
             - category: typing.Optional[str]. voice category used for filtering
 
             - gender: typing.Optional[str]. gender used for filtering
 
             - age: typing.Optional[str]. age used for filtering
 
             - accent: typing.Optional[str]. accent used for filtering
 
+            - language: typing.Optional[str]. language used for filtering
+
             - search: typing.Optional[str]. search term used for filtering
 
             - use_cases: typing.Optional[typing.Union[str, typing.Sequence[str]]]. use-case used for filtering
 
             - descriptives: typing.Optional[typing.Union[str, typing.Sequence[str]]]. search term used for filtering
 
             - sort: typing.Optional[str]. sort criteria
@@ -1240,14 +1247,15 @@
                 remove_none_from_dict(
                     {
                         "page_size": page_size,
                         "category": category,
                         "gender": gender,
                         "age": age,
                         "accent": accent,
+                        "language": language,
                         "search": search,
                         "use_cases": use_cases,
                         "descriptives": descriptives,
                         "sort": sort,
                         "featured": featured,
                         "page": page,
                         **(
```

### Comparing `elevenlabs-1.0.4/PKG-INFO` & `elevenlabs-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,15 +35,15 @@
 ## ⚙️ Install
 
 ```bash
 pip install elevenlabs
 ```
 
 ## v0.x to v1.x Migration Guide
-> The SDK was rewritten in v1 and is now programatically generated from our OpenAPI spec. As part of this release 
+> The SDK was rewritten in v1 and is now programmatically generated from our OpenAPI spec. As part of this release 
 > there are some breaking changes. 
 
 
 ### Client Instantiation
 The SDK now exports a client class that you must instantiate to call various
 endpoints in our API. 
 
@@ -157,15 +157,15 @@
 
 client = ElevenLabs(
   api_key="YOUR_API_KEY", # Defaults to ELEVEN_API_KEY
 )
 
 response = client.voices.get_all()
 audio = client.generate(text="Hello there!", voice=response.voices[0])
-print(voices)
+print(response.voices)
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
 [
   Voice(
```

