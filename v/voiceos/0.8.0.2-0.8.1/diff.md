# Comparing `tmp/voiceos-0.8.0.2.tar.gz` & `tmp/voiceos-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voiceos-0.8.0.2.tar", last modified: Mon Apr  8 02:39:44 2024, max compression
+gzip compressed data, was "voiceos-0.8.1.tar", last modified: Mon Apr  8 02:44:24 2024, max compression
```

## Comparing `voiceos-0.8.0.2.tar` & `voiceos-0.8.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:39:44.877521 voiceos-0.8.0.2/
--rw-r--r--   0 jonah      (501) staff       (20)     2272 2024-04-08 02:39:44.877590 voiceos-0.8.0.2/PKG-INFO
--rw-r--r--   0 jonah      (501) staff       (20)     1992 2024-04-08 02:18:46.000000 voiceos-0.8.0.2/README.md
--rw-r--r--   0 jonah      (501) staff       (20)     1913 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/pyproject.toml
--rw-r--r--   0 jonah      (501) staff       (20)       69 2024-04-08 02:39:44.878005 voiceos-0.8.0.2/setup.cfg
--rw-r--r--   0 jonah      (501) staff       (20)      921 2024-04-08 02:38:56.000000 voiceos-0.8.0.2/setup.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:39:44.864098 voiceos-0.8.0.2/test/
--rw-r--r--   0 jonah      (501) staff       (20)     2352 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     2175 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent_configuration.py
--rw-r--r--   0 jonah      (501) staff       (20)     1508 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)      697 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent_language.py
--rw-r--r--   0 jonah      (501) staff       (20)     3083 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      697 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)     2711 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agent_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     1237 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_agents_api.py
--rw-r--r--   0 jonah      (501) staff       (20)      704 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_azure_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)      676 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_azure_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     1509 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_azure_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     1486 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_azure_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     1453 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_buy_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     3495 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_call_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1405 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_call_recording.py
--rw-r--r--   0 jonah      (501) staff       (20)     4036 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_call_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      676 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_call_status.py
--rw-r--r--   0 jonah      (501) staff       (20)      662 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_call_type.py
--rw-r--r--   0 jonah      (501) staff       (20)     1104 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_calls_api.py
--rw-r--r--   0 jonah      (501) staff       (20)     3483 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_calls_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      655 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_chat_gpt.py
--rw-r--r--   0 jonah      (501) staff       (20)     1489 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_create_call.py
--rw-r--r--   0 jonah      (501) staff       (20)      661 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_currency.py
--rw-r--r--   0 jonah      (501) staff       (20)      725 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_deepgram_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)      697 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_deepgram_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     1586 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_deepgram_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)      712 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_eleven_labs_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     1557 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_eleven_labs_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)      690 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_ended_reasons.py
--rw-r--r--   0 jonah      (501) staff       (20)      669 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_event_name.py
--rw-r--r--   0 jonah      (501) staff       (20)      726 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_event_variable_name.py
--rw-r--r--   0 jonah      (501) staff       (20)     1694 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_http_validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     1724 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_language_model_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1384 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_message.py
--rw-r--r--   0 jonah      (501) staff       (20)      683 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_message_role.py
--rw-r--r--   0 jonah      (501) staff       (20)      676 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_method_enum.py
--rw-r--r--   0 jonah      (501) staff       (20)     1615 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_open_ai.py
--rw-r--r--   0 jonah      (501) staff       (20)     2085 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_open_ai_function.py
--rw-r--r--   0 jonah      (501) staff       (20)     1701 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_open_ai_function_parameter.py
--rw-r--r--   0 jonah      (501) staff       (20)      734 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_open_ai_function_type.py
--rw-r--r--   0 jonah      (501) staff       (20)      661 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_operator.py
--rw-r--r--   0 jonah      (501) staff       (20)     2494 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     2874 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_phone_number_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)     2641 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_phone_number_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     1546 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_phone_number_to_buy.py
--rw-r--r--   0 jonah      (501) staff       (20)     1719 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_phone_numbers_api.py
--rw-r--r--   0 jonah      (501) staff       (20)     1502 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_rime_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     1621 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_synthesizer_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1599 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_telephony_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1476 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     1627 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_transcriber_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1539 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_twilio_telephony.py
--rw-r--r--   0 jonah      (501) staff       (20)     1997 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_update_agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     1422 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_update_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     1607 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     1456 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_validation_error_loc_inner.py
--rw-r--r--   0 jonah      (501) staff       (20)     1524 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_voice.py
--rw-r--r--   0 jonah      (501) staff       (20)      848 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_wako_api_models_language_model_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      834 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_wako_api_models_phone_number_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      833 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_wako_api_models_synthesizer_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      833 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/test/test_wako_api_models_transcriber_provider.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:39:44.865353 voiceos-0.8.0.2/voiceos/
--rw-r--r--   0 jonah      (501) staff       (20)     4023 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/__init__.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:39:44.866916 voiceos-0.8.0.2/voiceos/api/
--rw-r--r--   0 jonah      (501) staff       (20)      194 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/api/__init__.py
--rw-r--r--   0 jonah      (501) staff       (20)    53316 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/api/agents_api.py
--rw-r--r--   0 jonah      (501) staff       (20)    42990 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/api/calls_api.py
--rw-r--r--   0 jonah      (501) staff       (20)    66496 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/api/phone_numbers_api.py
--rw-r--r--   0 jonah      (501) staff       (20)    25749 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/api_client.py
--rw-r--r--   0 jonah      (501) staff       (20)      652 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/api_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      687 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/client.py
--rw-r--r--   0 jonah      (501) staff       (20)    15339 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/configuration.py
--rw-r--r--   0 jonah      (501) staff       (20)     5972 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/exceptions.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:39:44.877374 voiceos-0.8.0.2/voiceos/models/
--rw-r--r--   0 jonah      (501) staff       (20)     3938 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/__init__.py
--rw-r--r--   0 jonah      (501) staff       (20)     4809 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     4546 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent_configuration.py
--rw-r--r--   0 jonah      (501) staff       (20)     3109 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)      766 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent_language.py
--rw-r--r--   0 jonah      (501) staff       (20)     3265 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      728 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)     5213 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/agent_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     1336 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/azure_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)     2022 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/azure_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     3601 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/azure_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     3194 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/azure_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     3086 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/buy_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     5066 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/call_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     2573 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/call_recording.py
--rw-r--r--   0 jonah      (501) staff       (20)     5704 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/call_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      742 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/call_status.py
--rw-r--r--   0 jonah      (501) staff       (20)      794 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/call_type.py
--rw-r--r--   0 jonah      (501) staff       (20)     3273 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/calls_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      830 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/chat_gpt.py
--rw-r--r--   0 jonah      (501) staff       (20)     2885 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/create_call.py
--rw-r--r--   0 jonah      (501) staff       (20)      716 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/currency.py
--rw-r--r--   0 jonah      (501) staff       (20)      998 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/deepgram_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)     1224 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/deepgram_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     3678 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/deepgram_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     1084 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/eleven_labs_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     3503 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/eleven_labs_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)      828 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/ended_reasons.py
--rw-r--r--   0 jonah      (501) staff       (20)      860 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/event_name.py
--rw-r--r--   0 jonah      (501) staff       (20)      796 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/event_variable_name.py
--rw-r--r--   0 jonah      (501) staff       (20)     2976 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/http_validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     3479 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/language_model_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     2681 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/message.py
--rw-r--r--   0 jonah      (501) staff       (20)      746 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/message_role.py
--rw-r--r--   0 jonah      (501) staff       (20)      738 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/method_enum.py
--rw-r--r--   0 jonah      (501) staff       (20)     3744 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/open_ai.py
--rw-r--r--   0 jonah      (501) staff       (20)     3538 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/open_ai_function.py
--rw-r--r--   0 jonah      (501) staff       (20)     3155 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/open_ai_function_parameter.py
--rw-r--r--   0 jonah      (501) staff       (20)      742 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/open_ai_function_type.py
--rw-r--r--   0 jonah      (501) staff       (20)      716 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/operator.py
--rw-r--r--   0 jonah      (501) staff       (20)     4161 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     3312 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/phone_number_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)     4301 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/phone_number_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     3446 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/phone_number_to_buy.py
--rw-r--r--   0 jonah      (501) staff       (20)     3859 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/rime_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     3264 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/synthesizer_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     3238 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/telephony_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     5007 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     5030 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/transcriber1.py
--rw-r--r--   0 jonah      (501) staff       (20)     3269 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/transcriber_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     3636 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/twilio_telephony.py
--rw-r--r--   0 jonah      (501) staff       (20)     4672 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/update_agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     2708 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/update_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     3077 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     4901 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/validation_error_loc_inner.py
--rw-r--r--   0 jonah      (501) staff       (20)     5765 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/voice.py
--rw-r--r--   0 jonah      (501) staff       (20)     5794 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/voice1.py
--rw-r--r--   0 jonah      (501) staff       (20)      774 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/wako_api_models_language_model_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      770 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/wako_api_models_phone_number_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      816 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/wako_api_models_synthesizer_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      794 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/models/wako_api_models_transcriber_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)        0 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/py.typed
--rw-r--r--   0 jonah      (501) staff       (20)     9225 2024-04-07 03:49:32.000000 voiceos-0.8.0.2/voiceos/rest.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:39:44.866187 voiceos-0.8.0.2/voiceos.egg-info/
--rw-r--r--   0 jonah      (501) staff       (20)     2272 2024-04-08 02:39:44.000000 voiceos-0.8.0.2/voiceos.egg-info/PKG-INFO
--rw-r--r--   0 jonah      (501) staff       (20)     4422 2024-04-08 02:39:44.000000 voiceos-0.8.0.2/voiceos.egg-info/SOURCES.txt
--rw-r--r--   0 jonah      (501) staff       (20)        1 2024-04-08 02:39:44.000000 voiceos-0.8.0.2/voiceos.egg-info/dependency_links.txt
--rw-r--r--   0 jonah      (501) staff       (20)       76 2024-04-08 02:39:44.000000 voiceos-0.8.0.2/voiceos.egg-info/requires.txt
--rw-r--r--   0 jonah      (501) staff       (20)        8 2024-04-08 02:39:44.000000 voiceos-0.8.0.2/voiceos.egg-info/top_level.txt
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:44:24.636542 voiceos-0.8.1/
+-rw-r--r--   0 jonah      (501) staff       (20)     2266 2024-04-08 02:44:24.636613 voiceos-0.8.1/PKG-INFO
+-rw-r--r--   0 jonah      (501) staff       (20)     1992 2024-04-08 02:18:46.000000 voiceos-0.8.1/README.md
+-rw-r--r--   0 jonah      (501) staff       (20)     1913 2024-04-07 03:49:32.000000 voiceos-0.8.1/pyproject.toml
+-rw-r--r--   0 jonah      (501) staff       (20)       69 2024-04-08 02:44:24.636843 voiceos-0.8.1/setup.cfg
+-rw-r--r--   0 jonah      (501) staff       (20)      915 2024-04-08 02:43:27.000000 voiceos-0.8.1/setup.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:44:24.621914 voiceos-0.8.1/test/
+-rw-r--r--   0 jonah      (501) staff       (20)     2352 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2175 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent_configuration.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1508 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)      697 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent_language.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3083 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)      697 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2711 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agent_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1237 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_agents_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)      704 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_azure_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)      676 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_azure_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1509 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_azure_synthesizer.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1486 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_azure_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1453 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_buy_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3495 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_call_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1405 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_call_recording.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4036 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_call_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)      676 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_call_status.py
+-rw-r--r--   0 jonah      (501) staff       (20)      662 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_call_type.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1104 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_calls_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3483 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_calls_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)      655 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_chat_gpt.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1489 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_create_call.py
+-rw-r--r--   0 jonah      (501) staff       (20)      661 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_currency.py
+-rw-r--r--   0 jonah      (501) staff       (20)      725 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_deepgram_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)      697 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_deepgram_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1586 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_deepgram_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)      712 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_eleven_labs_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1557 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_eleven_labs_synthesizer.py
+-rw-r--r--   0 jonah      (501) staff       (20)      690 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_ended_reasons.py
+-rw-r--r--   0 jonah      (501) staff       (20)      669 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_event_name.py
+-rw-r--r--   0 jonah      (501) staff       (20)      726 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_event_variable_name.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1694 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_http_validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1724 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_language_model_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1384 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_message.py
+-rw-r--r--   0 jonah      (501) staff       (20)      683 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_message_role.py
+-rw-r--r--   0 jonah      (501) staff       (20)      676 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_method_enum.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1615 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_open_ai.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2085 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_open_ai_function.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1701 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_open_ai_function_parameter.py
+-rw-r--r--   0 jonah      (501) staff       (20)      734 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_open_ai_function_type.py
+-rw-r--r--   0 jonah      (501) staff       (20)      661 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_operator.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2494 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2874 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_phone_number_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2641 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_phone_number_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1546 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_phone_number_to_buy.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1719 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_phone_numbers_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1502 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_rime_synthesizer.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1621 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_synthesizer_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1599 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_telephony_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1476 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1627 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_transcriber_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1539 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_twilio_telephony.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1997 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_update_agent.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1422 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_update_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1607 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1456 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_validation_error_loc_inner.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1524 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)      848 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_wako_api_models_language_model_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      834 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_wako_api_models_phone_number_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      833 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_wako_api_models_synthesizer_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      833 2024-04-07 03:49:32.000000 voiceos-0.8.1/test/test_wako_api_models_transcriber_provider.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:44:24.623469 voiceos-0.8.1/voiceos/
+-rw-r--r--   0 jonah      (501) staff       (20)     4023 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/__init__.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:44:24.625217 voiceos-0.8.1/voiceos/api/
+-rw-r--r--   0 jonah      (501) staff       (20)      194 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/api/__init__.py
+-rw-r--r--   0 jonah      (501) staff       (20)    53316 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/api/agents_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)    42990 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/api/calls_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)    66496 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/api/phone_numbers_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)    25749 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/api_client.py
+-rw-r--r--   0 jonah      (501) staff       (20)      652 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/api_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)      687 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/client.py
+-rw-r--r--   0 jonah      (501) staff       (20)    15339 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/configuration.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5972 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/exceptions.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:44:24.636385 voiceos-0.8.1/voiceos/models/
+-rw-r--r--   0 jonah      (501) staff       (20)     3938 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/__init__.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4809 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4546 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent_configuration.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3109 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)      766 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent_language.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3265 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)      728 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5213 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/agent_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1336 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/azure_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2022 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/azure_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3601 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/azure_synthesizer.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3194 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/azure_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3086 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/buy_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5066 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/call_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2573 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/call_recording.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5704 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/call_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)      742 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/call_status.py
+-rw-r--r--   0 jonah      (501) staff       (20)      794 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/call_type.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3273 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/calls_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)      830 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/chat_gpt.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2885 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/create_call.py
+-rw-r--r--   0 jonah      (501) staff       (20)      716 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/currency.py
+-rw-r--r--   0 jonah      (501) staff       (20)      998 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/deepgram_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1224 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/deepgram_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3678 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/deepgram_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1084 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/eleven_labs_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3503 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/eleven_labs_synthesizer.py
+-rw-r--r--   0 jonah      (501) staff       (20)      828 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/ended_reasons.py
+-rw-r--r--   0 jonah      (501) staff       (20)      860 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/event_name.py
+-rw-r--r--   0 jonah      (501) staff       (20)      796 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/event_variable_name.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2976 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/http_validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3479 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/language_model_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2681 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/message.py
+-rw-r--r--   0 jonah      (501) staff       (20)      746 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/message_role.py
+-rw-r--r--   0 jonah      (501) staff       (20)      738 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/method_enum.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3744 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/open_ai.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3538 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/open_ai_function.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3155 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/open_ai_function_parameter.py
+-rw-r--r--   0 jonah      (501) staff       (20)      742 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/open_ai_function_type.py
+-rw-r--r--   0 jonah      (501) staff       (20)      716 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/operator.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4161 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3312 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/phone_number_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4301 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/phone_number_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3446 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/phone_number_to_buy.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3859 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/rime_synthesizer.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3264 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/synthesizer_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3238 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/telephony_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5007 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5030 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/transcriber1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3269 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/transcriber_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3636 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/twilio_telephony.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4672 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/update_agent.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2708 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/update_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3077 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4901 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/validation_error_loc_inner.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5765 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5794 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/voice1.py
+-rw-r--r--   0 jonah      (501) staff       (20)      774 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/wako_api_models_language_model_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      770 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/wako_api_models_phone_number_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      816 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/wako_api_models_synthesizer_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      794 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/models/wako_api_models_transcriber_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)        0 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/py.typed
+-rw-r--r--   0 jonah      (501) staff       (20)     9225 2024-04-07 03:49:32.000000 voiceos-0.8.1/voiceos/rest.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 02:44:24.624426 voiceos-0.8.1/voiceos.egg-info/
+-rw-r--r--   0 jonah      (501) staff       (20)     2266 2024-04-08 02:44:24.000000 voiceos-0.8.1/voiceos.egg-info/PKG-INFO
+-rw-r--r--   0 jonah      (501) staff       (20)     4422 2024-04-08 02:44:24.000000 voiceos-0.8.1/voiceos.egg-info/SOURCES.txt
+-rw-r--r--   0 jonah      (501) staff       (20)        1 2024-04-08 02:44:24.000000 voiceos-0.8.1/voiceos.egg-info/dependency_links.txt
+-rw-r--r--   0 jonah      (501) staff       (20)       76 2024-04-08 02:44:24.000000 voiceos-0.8.1/voiceos.egg-info/requires.txt
+-rw-r--r--   0 jonah      (501) staff       (20)        8 2024-04-08 02:44:24.000000 voiceos-0.8.1/voiceos.egg-info/top_level.txt
```

### Comparing `voiceos-0.8.0.2/PKG-INFO` & `voiceos-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: voiceos
-Version: 0.8.0.2
+Version: 0.8.1
 Summary: VoiceOS Python SDK
 Home-page: https://github.com/WakoAi/voiceos-python
-Author: WakoAI Inc
+Author: WakoAI
 Author-email: hello@wako.ai
 Keywords: VoiceOS,VoiceOS Python ClientSDK,VoiceOS Python
 Description-Content-Type: text/markdown
 
 # VoiceOS Python SDK
 
 This python client lets you build with [VoiceOS](https://voiceos.io)
```

### Comparing `voiceos-0.8.0.2/README.md` & `voiceos-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/pyproject.toml` & `voiceos-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/setup.py` & `voiceos-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 NAME = "voiceos"
-VERSION = "0.8.0.2"
+VERSION = "0.8.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="VoiceOS Python SDK",
-    author="WakoAI Inc",
+    author="WakoAI",
     author_email="hello@wako.ai",
     url="https://github.com/WakoAi/voiceos-python",
     keywords=["VoiceOS", "VoiceOS Python ClientSDK", "VoiceOS Python"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description_content_type='text/markdown',
```

### Comparing `voiceos-0.8.0.2/test/test_agent.py` & `voiceos-0.8.1/test/test_agent.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agent_configuration.py` & `voiceos-0.8.1/test/test_agent_configuration.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agent_cost.py` & `voiceos-0.8.1/test/test_agent_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agent_language.py` & `voiceos-0.8.1/test/test_agent_language.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agent_pagination.py` & `voiceos-0.8.1/test/test_agent_pagination.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agent_provider.py` & `voiceos-0.8.1/test/test_agent_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agent_response.py` & `voiceos-0.8.1/test/test_agent_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_agents_api.py` & `voiceos-0.8.1/test/test_agents_api.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_azure_languages.py` & `voiceos-0.8.1/test/test_azure_languages.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_azure_model.py` & `voiceos-0.8.1/test/test_azure_model.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_azure_synthesizer.py` & `voiceos-0.8.1/test/test_azure_synthesizer.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_azure_transcriber.py` & `voiceos-0.8.1/test/test_azure_transcriber.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_buy_phone_number.py` & `voiceos-0.8.1/test/test_buy_phone_number.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_call_cost.py` & `voiceos-0.8.1/test/test_call_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_call_recording.py` & `voiceos-0.8.1/test/test_call_recording.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_call_response.py` & `voiceos-0.8.1/test/test_call_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_call_status.py` & `voiceos-0.8.1/test/test_call_status.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_call_type.py` & `voiceos-0.8.1/test/test_call_type.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_calls_api.py` & `voiceos-0.8.1/test/test_calls_api.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_calls_pagination.py` & `voiceos-0.8.1/test/test_calls_pagination.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_chat_gpt.py` & `voiceos-0.8.1/test/test_chat_gpt.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_create_call.py` & `voiceos-0.8.1/test/test_create_call.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_currency.py` & `voiceos-0.8.1/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_deepgram_languages.py` & `voiceos-0.8.1/test/test_deepgram_languages.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_deepgram_model.py` & `voiceos-0.8.1/test/test_deepgram_model.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_deepgram_transcriber.py` & `voiceos-0.8.1/test/test_deepgram_transcriber.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_eleven_labs_model.py` & `voiceos-0.8.1/test/test_eleven_labs_model.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_eleven_labs_synthesizer.py` & `voiceos-0.8.1/test/test_eleven_labs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_ended_reasons.py` & `voiceos-0.8.1/test/test_ended_reasons.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_event_name.py` & `voiceos-0.8.1/test/test_event_name.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_event_variable_name.py` & `voiceos-0.8.1/test/test_event_variable_name.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_http_validation_error.py` & `voiceos-0.8.1/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_language_model_cost.py` & `voiceos-0.8.1/test/test_language_model_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_message.py` & `voiceos-0.8.1/test/test_message.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_message_role.py` & `voiceos-0.8.1/test/test_message_role.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_method_enum.py` & `voiceos-0.8.1/test/test_method_enum.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_open_ai.py` & `voiceos-0.8.1/test/test_open_ai.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_open_ai_function.py` & `voiceos-0.8.1/test/test_open_ai_function.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_open_ai_function_parameter.py` & `voiceos-0.8.1/test/test_open_ai_function_parameter.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_open_ai_function_type.py` & `voiceos-0.8.1/test/test_open_ai_function_type.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_operator.py` & `voiceos-0.8.1/test/test_operator.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_phone_number.py` & `voiceos-0.8.1/test/test_phone_number.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_phone_number_pagination.py` & `voiceos-0.8.1/test/test_phone_number_pagination.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_phone_number_response.py` & `voiceos-0.8.1/test/test_phone_number_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_phone_number_to_buy.py` & `voiceos-0.8.1/test/test_phone_number_to_buy.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_phone_numbers_api.py` & `voiceos-0.8.1/test/test_phone_numbers_api.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_rime_synthesizer.py` & `voiceos-0.8.1/test/test_rime_synthesizer.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_synthesizer_cost.py` & `voiceos-0.8.1/test/test_synthesizer_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_telephony_cost.py` & `voiceos-0.8.1/test/test_telephony_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_transcriber.py` & `voiceos-0.8.1/test/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_transcriber_cost.py` & `voiceos-0.8.1/test/test_transcriber_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_twilio_telephony.py` & `voiceos-0.8.1/test/test_twilio_telephony.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_update_agent.py` & `voiceos-0.8.1/test/test_update_agent.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_update_phone_number.py` & `voiceos-0.8.1/test/test_update_phone_number.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_validation_error.py` & `voiceos-0.8.1/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_validation_error_loc_inner.py` & `voiceos-0.8.1/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_voice.py` & `voiceos-0.8.1/test/test_voice.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_wako_api_models_language_model_provider.py` & `voiceos-0.8.1/test/test_wako_api_models_language_model_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_wako_api_models_phone_number_provider.py` & `voiceos-0.8.1/test/test_wako_api_models_phone_number_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_wako_api_models_synthesizer_provider.py` & `voiceos-0.8.1/test/test_wako_api_models_synthesizer_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/test/test_wako_api_models_transcriber_provider.py` & `voiceos-0.8.1/test/test_wako_api_models_transcriber_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/__init__.py` & `voiceos-0.8.1/voiceos/__init__.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/api/agents_api.py` & `voiceos-0.8.1/voiceos/api/agents_api.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/api/calls_api.py` & `voiceos-0.8.1/voiceos/api/calls_api.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/api/phone_numbers_api.py` & `voiceos-0.8.1/voiceos/api/phone_numbers_api.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/api_client.py` & `voiceos-0.8.1/voiceos/api_client.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/api_response.py` & `voiceos-0.8.1/voiceos/api_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/client.py` & `voiceos-0.8.1/voiceos/client.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/configuration.py` & `voiceos-0.8.1/voiceos/configuration.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/exceptions.py` & `voiceos-0.8.1/voiceos/exceptions.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/__init__.py` & `voiceos-0.8.1/voiceos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent.py` & `voiceos-0.8.1/voiceos/models/agent.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent_configuration.py` & `voiceos-0.8.1/voiceos/models/agent_configuration.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent_cost.py` & `voiceos-0.8.1/voiceos/models/agent_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent_language.py` & `voiceos-0.8.1/voiceos/models/agent_language.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent_pagination.py` & `voiceos-0.8.1/voiceos/models/agent_pagination.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent_provider.py` & `voiceos-0.8.1/voiceos/models/agent_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/agent_response.py` & `voiceos-0.8.1/voiceos/models/agent_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/azure_languages.py` & `voiceos-0.8.1/voiceos/models/azure_languages.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/azure_model.py` & `voiceos-0.8.1/voiceos/models/azure_model.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/azure_synthesizer.py` & `voiceos-0.8.1/voiceos/models/azure_synthesizer.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/azure_transcriber.py` & `voiceos-0.8.1/voiceos/models/azure_transcriber.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/buy_phone_number.py` & `voiceos-0.8.1/voiceos/models/buy_phone_number.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/call_cost.py` & `voiceos-0.8.1/voiceos/models/call_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/call_recording.py` & `voiceos-0.8.1/voiceos/models/call_recording.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/call_response.py` & `voiceos-0.8.1/voiceos/models/call_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/call_status.py` & `voiceos-0.8.1/voiceos/models/call_status.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/call_type.py` & `voiceos-0.8.1/voiceos/models/call_type.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/calls_pagination.py` & `voiceos-0.8.1/voiceos/models/calls_pagination.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/chat_gpt.py` & `voiceos-0.8.1/voiceos/models/chat_gpt.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/create_call.py` & `voiceos-0.8.1/voiceos/models/create_call.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/currency.py` & `voiceos-0.8.1/voiceos/models/currency.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/deepgram_languages.py` & `voiceos-0.8.1/voiceos/models/deepgram_languages.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/deepgram_model.py` & `voiceos-0.8.1/voiceos/models/deepgram_model.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/deepgram_transcriber.py` & `voiceos-0.8.1/voiceos/models/deepgram_transcriber.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/eleven_labs_model.py` & `voiceos-0.8.1/voiceos/models/eleven_labs_model.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/eleven_labs_synthesizer.py` & `voiceos-0.8.1/voiceos/models/eleven_labs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/ended_reasons.py` & `voiceos-0.8.1/voiceos/models/ended_reasons.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/event_name.py` & `voiceos-0.8.1/voiceos/models/event_name.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/event_variable_name.py` & `voiceos-0.8.1/voiceos/models/event_variable_name.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/http_validation_error.py` & `voiceos-0.8.1/voiceos/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/language_model_cost.py` & `voiceos-0.8.1/voiceos/models/language_model_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/message.py` & `voiceos-0.8.1/voiceos/models/message.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/message_role.py` & `voiceos-0.8.1/voiceos/models/message_role.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/method_enum.py` & `voiceos-0.8.1/voiceos/models/method_enum.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/open_ai.py` & `voiceos-0.8.1/voiceos/models/open_ai.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/open_ai_function.py` & `voiceos-0.8.1/voiceos/models/open_ai_function.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/open_ai_function_parameter.py` & `voiceos-0.8.1/voiceos/models/open_ai_function_parameter.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/open_ai_function_type.py` & `voiceos-0.8.1/voiceos/models/open_ai_function_type.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/operator.py` & `voiceos-0.8.1/voiceos/models/operator.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/phone_number.py` & `voiceos-0.8.1/voiceos/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/phone_number_pagination.py` & `voiceos-0.8.1/voiceos/models/phone_number_pagination.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/phone_number_response.py` & `voiceos-0.8.1/voiceos/models/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/phone_number_to_buy.py` & `voiceos-0.8.1/voiceos/models/phone_number_to_buy.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/rime_synthesizer.py` & `voiceos-0.8.1/voiceos/models/rime_synthesizer.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/synthesizer_cost.py` & `voiceos-0.8.1/voiceos/models/synthesizer_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/telephony_cost.py` & `voiceos-0.8.1/voiceos/models/telephony_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/transcriber.py` & `voiceos-0.8.1/voiceos/models/transcriber.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/transcriber1.py` & `voiceos-0.8.1/voiceos/models/transcriber1.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/transcriber_cost.py` & `voiceos-0.8.1/voiceos/models/transcriber_cost.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/twilio_telephony.py` & `voiceos-0.8.1/voiceos/models/twilio_telephony.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/update_agent.py` & `voiceos-0.8.1/voiceos/models/update_agent.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/update_phone_number.py` & `voiceos-0.8.1/voiceos/models/update_phone_number.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/validation_error.py` & `voiceos-0.8.1/voiceos/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/validation_error_loc_inner.py` & `voiceos-0.8.1/voiceos/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/voice.py` & `voiceos-0.8.1/voiceos/models/voice.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/voice1.py` & `voiceos-0.8.1/voiceos/models/voice1.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/wako_api_models_language_model_provider.py` & `voiceos-0.8.1/voiceos/models/wako_api_models_language_model_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/wako_api_models_phone_number_provider.py` & `voiceos-0.8.1/voiceos/models/wako_api_models_phone_number_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/wako_api_models_synthesizer_provider.py` & `voiceos-0.8.1/voiceos/models/wako_api_models_synthesizer_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/models/wako_api_models_transcriber_provider.py` & `voiceos-0.8.1/voiceos/models/wako_api_models_transcriber_provider.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos/rest.py` & `voiceos-0.8.1/voiceos/rest.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.0.2/voiceos.egg-info/PKG-INFO` & `voiceos-0.8.1/voiceos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: voiceos
-Version: 0.8.0.2
+Version: 0.8.1
 Summary: VoiceOS Python SDK
 Home-page: https://github.com/WakoAi/voiceos-python
-Author: WakoAI Inc
+Author: WakoAI
 Author-email: hello@wako.ai
 Keywords: VoiceOS,VoiceOS Python ClientSDK,VoiceOS Python
 Description-Content-Type: text/markdown
 
 # VoiceOS Python SDK
 
 This python client lets you build with [VoiceOS](https://voiceos.io)
```

### Comparing `voiceos-0.8.0.2/voiceos.egg-info/SOURCES.txt` & `voiceos-0.8.1/voiceos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

