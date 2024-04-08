# Comparing `tmp/cohere-5.2.2.tar.gz` & `tmp/cohere-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.2.2.tar", max compression
+gzip compressed data, was "cohere-5.2.3.tar", max compression
```

## Comparing `cohere-5.2.2.tar` & `cohere-5.2.3.tar`

### file list

```diff
@@ -1,173 +1,174 @@
--rw-r--r--   0        0        0     1062 2024-04-04 21:42:57.584772 cohere-5.2.2/LICENSE
--rw-r--r--   0        0        0     2359 2024-04-04 21:42:57.584772 cohere-5.2.2/README.md
--rw-r--r--   0        0        0      679 2024-04-04 21:42:57.592772 cohere-5.2.2/pyproject.toml
--rw-r--r--   0        0        0     7869 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/__init__.py
--rw-r--r--   0        0        0   198723 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/base_client.py
--rw-r--r--   0        0        0    19312 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    46750 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/connectors/client.py
--rw-r--r--   0        0        0      853 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/core/request_options.py
--rw-r--r--   0        0        0      289 2024-04-04 21:42:57.592772 cohere-5.2.2/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    33977 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      417 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0      945 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0      902 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1000 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      941 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    29728 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      172 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      253 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    56670 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1417 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      308 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1117 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1025 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1342 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2299 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1113 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1765 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1431 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1474 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1405 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1519 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      405 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      196 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1332 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1119 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     1948 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    12450 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/py.typed
--rw-r--r--   0        0        0    10138 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1111 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0      955 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1378 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0      171 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1873 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1127 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1805 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1364 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1588 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      171 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      173 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1652 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      192 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0      955 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1180 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1191 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1597 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0      999 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1417 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1861 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      228 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      837 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      179 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1658 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      198 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0      961 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1102 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1068 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1040 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1075 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      915 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      174 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1081 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2504 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      217 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      915 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      223 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3327 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/connector.py
--rw-r--r--   0        0        0      166 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1604 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1669 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      904 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1139 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0      991 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2153 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1592 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      474 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      225 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1012 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1360 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2223 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1308 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      214 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1808 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      210 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      159 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      171 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0      892 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      187 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1901 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      225 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      188 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      174 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1197 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1045 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1311 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      841 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      194 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      180 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1312 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1269 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1198 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/generation.py
--rw-r--r--   0        0        0      901 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2056 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1301 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1039 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      937 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1131 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0      968 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     2645 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1024 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      918 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0      945 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1144 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1286 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1000 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     2031 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1763 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1192 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      896 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     2963 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      182 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      173 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      176 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1145 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1071 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1872 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1165 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1275 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      904 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10025 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-04-04 21:42:57.596772 cohere-5.2.2/src/cohere/version.py
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 cohere-5.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-08 16:22:48.917201 cohere-5.2.3/LICENSE
+-rw-r--r--   0        0        0     2359 2024-04-08 16:22:48.917201 cohere-5.2.3/README.md
+-rw-r--r--   0        0        0      679 2024-04-08 16:22:48.925201 cohere-5.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7869 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/__init__.py
+-rw-r--r--   0        0        0   203898 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/base_client.py
+-rw-r--r--   0        0        0    19312 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    50199 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1006 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      289 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    34988 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      417 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1002 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0      959 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1057 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      998 2024-04-08 16:22:48.925201 cohere-5.2.3/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    31599 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      253 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    62127 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      305 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1175 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1083 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1400 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2357 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1171 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1823 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1489 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1532 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1463 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1577 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1390 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1177 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     1948 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    13071 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/py.typed
+-rw-r--r--   0        0        0    10138 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1167 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1011 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1434 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0      168 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1929 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1127 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1861 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1297 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1644 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      168 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      170 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1708 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1011 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1180 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1247 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1653 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1055 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1417 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1861 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      893 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1714 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1017 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1102 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1068 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1040 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1004 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      971 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1137 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2560 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      971 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3383 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1660 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1725 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      960 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1195 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1047 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2209 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1648 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      471 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1068 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1416 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2279 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1364 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1864 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1057 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1735 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1197 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1101 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1311 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      897 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1312 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1456 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1254 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      957 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     1975 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1256 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1095 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      993 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1187 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1024 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     2701 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1080 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      974 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1001 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1200 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1342 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1056 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1818 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1819 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1248 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      952 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     3157 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1201 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1127 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1928 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1221 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1331 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      960 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10025 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-04-08 16:22:48.929201 cohere-5.2.3/src/cohere/version.py
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 cohere-5.2.3/PKG-INFO
```

### Comparing `cohere-5.2.2/LICENSE` & `cohere-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/README.md` & `cohere-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/pyproject.toml` & `cohere-5.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "5.2.2"
+version = "5.2.3"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "cohere", from = "src"}
 ]
```

### Comparing `cohere-5.2.2/src/cohere/__init__.py` & `cohere-5.2.3/src/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/base_client.py` & `cohere-5.2.3/src/cohere/base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import httpx
 
 from .connectors.client import AsyncConnectorsClient, ConnectorsClient
 from .core.api_error import ApiError
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .core.jsonable_encoder import jsonable_encoder
-from .core.pydantic_utilities import pydantic_v1
 from .core.remove_none_from_dict import remove_none_from_dict
 from .core.request_options import RequestOptions
+from .core.unchecked_base_model import construct_type
 from .datasets.client import AsyncDatasetsClient, DatasetsClient
 from .embed_jobs.client import AsyncEmbedJobsClient, EmbedJobsClient
 from .environment import ClientEnvironment
 from .errors.bad_request_error import BadRequestError
 from .errors.internal_server_error import InternalServerError
 from .errors.too_many_requests_error import TooManyRequestsError
 from .finetuning.client import AsyncFinetuningClient, FinetuningClient
@@ -129,14 +129,15 @@
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
+        max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
@@ -209,14 +210,18 @@
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
 
+            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+
+                                                      Input will be truncated according to the `prompt_truncation` parameter.
+
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
             - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
@@ -297,14 +302,15 @@
                 )
             ],
             search_queries_only=True,
             documents=[{"string": "string"}],
             citation_quality="fast",
             temperature=1.1,
             max_tokens=1,
+            max_input_tokens=1,
             k=1,
             p=1.1,
             seed=1.1,
             stop_sequences=["string"],
             connectors_search_options=ChatStreamRequestConnectorsSearchOptions(
                 model={"key": "value"},
                 temperature={"key": "value"},
@@ -353,14 +359,16 @@
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
+        if max_input_tokens is not OMIT:
+            _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
             _request["k"] = k
         if p is not OMIT:
             _request["p"] = p
         if seed is not OMIT:
             _request["seed"] = seed
         if stop_sequences is not OMIT:
@@ -401,19 +409,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _text in _response.iter_lines():
                     if len(_text) == 0:
                         continue
-                    yield pydantic_v1.parse_obj_as(StreamedChatResponse, json.loads(_text))  # type: ignore
+                    yield typing.cast(StreamedChatResponse, construct_type(type_=StreamedChatResponse, object_=json.loads(_text)))  # type: ignore
                 return
             _response.read()
             if _response.status_code == 429:
-                raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise TooManyRequestsError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def chat(
@@ -426,14 +436,15 @@
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
+        max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
@@ -506,14 +517,18 @@
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
 
+            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+
+                                                      Input will be truncated according to the `prompt_truncation` parameter.
+
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
             - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
@@ -598,14 +613,16 @@
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
+        if max_input_tokens is not OMIT:
+            _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
             _request["k"] = k
         if p is not OMIT:
             _request["p"] = p
         if seed is not OMIT:
             _request["seed"] = seed
         if stop_sequences is not OMIT:
@@ -643,17 +660,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NonStreamedChatResponse, _response.json())  # type: ignore
+            return typing.cast(NonStreamedChatResponse, construct_type(type_=NonStreamedChatResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def generate_stream(
@@ -822,23 +841,29 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _text in _response.iter_lines():
                     if len(_text) == 0:
                         continue
-                    yield pydantic_v1.parse_obj_as(GenerateStreamedResponse, json.loads(_text))  # type: ignore
+                    yield typing.cast(GenerateStreamedResponse, construct_type(type_=GenerateStreamedResponse, object_=json.loads(_text)))  # type: ignore
                 return
             _response.read()
             if _response.status_code == 400:
-                raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise BadRequestError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             if _response.status_code == 429:
-                raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise TooManyRequestsError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             if _response.status_code == 500:
-                raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise InternalServerError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def generate(
@@ -990,21 +1015,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Generation, _response.json())  # type: ignore
+            return typing.cast(Generation, construct_type(type_=Generation, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def embed(
@@ -1103,21 +1134,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(EmbedResponse, _response.json())  # type: ignore
+            return typing.cast(EmbedResponse, construct_type(type_=EmbedResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def rerank(
@@ -1202,17 +1239,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(RerankResponse, _response.json())  # type: ignore
+            return typing.cast(RerankResponse, construct_type(type_=RerankResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def classify(
@@ -1328,21 +1367,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ClassifyResponse, _response.json())  # type: ignore
+            return typing.cast(ClassifyResponse, construct_type(type_=ClassifyResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def summarize(
@@ -1427,17 +1472,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SummarizeResponse, _response.json())  # type: ignore
+            return typing.cast(SummarizeResponse, construct_type(type_=SummarizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def tokenize(
@@ -1487,21 +1534,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(TokenizeResponse, _response.json())  # type: ignore
+            return typing.cast(TokenizeResponse, construct_type(type_=TokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detokenize(
@@ -1551,17 +1604,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DetokenizeResponse, _response.json())  # type: ignore
+            return typing.cast(DetokenizeResponse, construct_type(type_=DetokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -1635,14 +1690,15 @@
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
+        max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
@@ -1715,14 +1771,18 @@
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
 
+            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+
+                                                      Input will be truncated according to the `prompt_truncation` parameter.
+
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
             - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
@@ -1803,14 +1863,15 @@
                 )
             ],
             search_queries_only=True,
             documents=[{"string": "string"}],
             citation_quality="fast",
             temperature=1.1,
             max_tokens=1,
+            max_input_tokens=1,
             k=1,
             p=1.1,
             seed=1.1,
             stop_sequences=["string"],
             connectors_search_options=ChatStreamRequestConnectorsSearchOptions(
                 model={"key": "value"},
                 temperature={"key": "value"},
@@ -1859,14 +1920,16 @@
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
+        if max_input_tokens is not OMIT:
+            _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
             _request["k"] = k
         if p is not OMIT:
             _request["p"] = p
         if seed is not OMIT:
             _request["seed"] = seed
         if stop_sequences is not OMIT:
@@ -1907,19 +1970,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _text in _response.aiter_lines():
                     if len(_text) == 0:
                         continue
-                    yield pydantic_v1.parse_obj_as(StreamedChatResponse, json.loads(_text))  # type: ignore
+                    yield typing.cast(StreamedChatResponse, construct_type(type_=StreamedChatResponse, object_=json.loads(_text)))  # type: ignore
                 return
             await _response.aread()
             if _response.status_code == 429:
-                raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise TooManyRequestsError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def chat(
@@ -1932,14 +1997,15 @@
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
+        max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
@@ -2012,14 +2078,18 @@
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
 
+            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+
+                                                      Input will be truncated according to the `prompt_truncation` parameter.
+
             - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
                                        Defaults to `0`, min value of `0`, max value of `500`.
 
             - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
                                          Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
             - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinism cannot be totally guaranteed.
@@ -2104,14 +2174,16 @@
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
+        if max_input_tokens is not OMIT:
+            _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
             _request["k"] = k
         if p is not OMIT:
             _request["p"] = p
         if seed is not OMIT:
             _request["seed"] = seed
         if stop_sequences is not OMIT:
@@ -2149,17 +2221,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NonStreamedChatResponse, _response.json())  # type: ignore
+            return typing.cast(NonStreamedChatResponse, construct_type(type_=NonStreamedChatResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def generate_stream(
@@ -2328,23 +2402,29 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _text in _response.aiter_lines():
                     if len(_text) == 0:
                         continue
-                    yield pydantic_v1.parse_obj_as(GenerateStreamedResponse, json.loads(_text))  # type: ignore
+                    yield typing.cast(GenerateStreamedResponse, construct_type(type_=GenerateStreamedResponse, object_=json.loads(_text)))  # type: ignore
                 return
             await _response.aread()
             if _response.status_code == 400:
-                raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise BadRequestError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             if _response.status_code == 429:
-                raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise TooManyRequestsError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             if _response.status_code == 500:
-                raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+                raise InternalServerError(
+                    typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def generate(
@@ -2496,21 +2576,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Generation, _response.json())  # type: ignore
+            return typing.cast(Generation, construct_type(type_=Generation, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def embed(
@@ -2609,21 +2695,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(EmbedResponse, _response.json())  # type: ignore
+            return typing.cast(EmbedResponse, construct_type(type_=EmbedResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def rerank(
@@ -2708,17 +2800,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(RerankResponse, _response.json())  # type: ignore
+            return typing.cast(RerankResponse, construct_type(type_=RerankResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def classify(
@@ -2834,21 +2928,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ClassifyResponse, _response.json())  # type: ignore
+            return typing.cast(ClassifyResponse, construct_type(type_=ClassifyResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def summarize(
@@ -2933,17 +3033,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SummarizeResponse, _response.json())  # type: ignore
+            return typing.cast(SummarizeResponse, construct_type(type_=SummarizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def tokenize(
@@ -2993,21 +3095,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(TokenizeResponse, _response.json())  # type: ignore
+            return typing.cast(TokenizeResponse, construct_type(type_=TokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def detokenize(
@@ -3057,17 +3165,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DetokenizeResponse, _response.json())  # type: ignore
+            return typing.cast(DetokenizeResponse, construct_type(type_=DetokenizeResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.2.2/src/cohere/client.py` & `cohere-5.2.3/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/connectors/client.py` & `cohere-5.2.3/src/cohere/embed_jobs/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,79 +3,56 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
-from ..errors.forbidden_error import ForbiddenError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.not_found_error import NotFoundError
 from ..errors.too_many_requests_error import TooManyRequestsError
-from ..types.create_connector_o_auth import CreateConnectorOAuth
-from ..types.create_connector_response import CreateConnectorResponse
-from ..types.create_connector_service_auth import CreateConnectorServiceAuth
-from ..types.delete_connector_response import DeleteConnectorResponse
-from ..types.get_connector_response import GetConnectorResponse
-from ..types.list_connectors_response import ListConnectorsResponse
-from ..types.o_auth_authorize_response import OAuthAuthorizeResponse
-from ..types.update_connector_response import UpdateConnectorResponse
+from ..types.create_embed_job_response import CreateEmbedJobResponse
+from ..types.embed_input_type import EmbedInputType
+from ..types.embed_job import EmbedJob
+from ..types.embedding_type import EmbeddingType
+from ..types.list_embed_job_response import ListEmbedJobResponse
+from .types.create_embed_job_request_truncate import CreateEmbedJobRequestTruncate
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class ConnectorsClient:
+class EmbedJobsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
-        self,
-        *,
-        limit: typing.Optional[float] = None,
-        offset: typing.Optional[float] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListConnectorsResponse:
+    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListEmbedJobResponse:
         """
-        Returns a list of connectors ordered by descending creation date (newer first). See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
+        The list embed job endpoint allows users to view all embed jobs history for that specific user.
 
         Parameters:
-            - limit: typing.Optional[float]. Maximum number of connectors to return [0, 100].
-
-            - offset: typing.Optional[float]. Number of connectors to skip before returning results [0, inf].
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        client.connectors.list()
+        client.embed_jobs.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "offset": offset,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -84,89 +61,98 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListConnectorsResponse, _response.json())  # type: ignore
+            return typing.cast(ListEmbedJobResponse, construct_type(type_=ListEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 429:
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
-        name: str,
-        description: typing.Optional[str] = OMIT,
-        url: str,
-        excludes: typing.Optional[typing.Sequence[str]] = OMIT,
-        oauth: typing.Optional[CreateConnectorOAuth] = OMIT,
-        active: typing.Optional[bool] = OMIT,
-        continue_on_failure: typing.Optional[bool] = OMIT,
-        service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
+        model: str,
+        dataset_id: str,
+        input_type: EmbedInputType,
+        name: typing.Optional[str] = OMIT,
+        embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
+        truncate: typing.Optional[CreateEmbedJobRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> CreateConnectorResponse:
+    ) -> CreateEmbedJobResponse:
         """
-        Creates a new connector. The connector is tested during registration and will cancel registration when the test is unsuccessful. See ['Creating and Deploying a Connector'](https://docs.cohere.com/docs/creating-and-deploying-a-connector) for more information.
+        This API launches an async Embed job for a [Dataset](https://docs.cohere.com/docs/datasets) of type `embed-input`. The result of a completed embed job is new Dataset of type `embed-output`, which contains the original text entries and the corresponding embeddings.
 
         Parameters:
-            - name: str. A human-readable name for the connector.
+            - model: str. ID of the embedding model.
 
-            - description: typing.Optional[str]. A description of the connector.
+                          Available models and corresponding embedding dimensions:
 
-            - url: str. The URL of the connector that will be used to search for documents.
+                          - `embed-english-v3.0` : 1024
+                          - `embed-multilingual-v3.0` : 1024
+                          - `embed-english-light-v3.0` : 384
+                          - `embed-multilingual-light-v3.0` : 384
 
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
+            - dataset_id: str. ID of a [Dataset](https://docs.cohere.com/docs/datasets). The Dataset must be of type `embed-input` and must have a validation status `Validated`
 
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
+            - input_type: EmbedInputType.
 
-            - active: typing.Optional[bool]. Whether the connector is active or not.
+            - name: typing.Optional[str]. The name of the embed job.
 
-            - continue_on_failure: typing.Optional[bool]. Whether a chat request should continue or not if the request to this connector fails.
+            - embedding_types: typing.Optional[typing.Sequence[EmbeddingType]]. Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
 
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
+                                                                                * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
+                                                                                * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
+                                                                                * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
+                                                                                * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
+                                                                                * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
+            - truncate: typing.Optional[CreateEmbedJobRequestTruncate]. One of `START|END` to specify how the API will handle inputs longer than the maximum token length.
+
+                                                                        Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        client.connectors.create(
-            name="name",
-            url="url",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "url": url}
-        if description is not OMIT:
-            _request["description"] = description
-        if excludes is not OMIT:
-            _request["excludes"] = excludes
-        if oauth is not OMIT:
-            _request["oauth"] = oauth
-        if active is not OMIT:
-            _request["active"] = active
-        if continue_on_failure is not OMIT:
-            _request["continue_on_failure"] = continue_on_failure
-        if service_auth is not OMIT:
-            _request["service_auth"] = service_auth
+        client.embed_jobs.create(
+            model="model",
+            dataset_id="dataset_id",
+            input_type="search_document",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"model": model, "dataset_id": dataset_id, "input_type": input_type}
+        if name is not OMIT:
+            _request["name"] = name
+        if embedding_types is not OMIT:
+            _request["embedding_types"] = embedding_types
+        if truncate is not OMIT:
+            _request["truncate"] = truncate
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -183,51 +169,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(CreateConnectorResponse, _response.json())  # type: ignore
+            return typing.cast(CreateEmbedJobResponse, construct_type(type_=CreateEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 403:
-            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetConnectorResponse:
+    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> EmbedJob:
         """
-        Retrieve a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
+        This API retrieves the details about an embed job started by the same user.
 
         Parameters:
-            - id: str. The ID of the connector to retrieve.
+            - id: str. The ID of the embed job to retrieve.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        client.connectors.get(
+        client.embed_jobs.get(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -238,233 +228,63 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetConnectorResponse, _response.json())  # type: ignore
+            return typing.cast(EmbedJob, construct_type(type_=EmbedJob, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DeleteConnectorResponse:
+    def cancel(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Delete a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
+        This API allows users to cancel an active embed job. Once invoked, the embedding process will be terminated, and users will be charged for the embeddings processed up to the cancellation point. It's important to note that partial results will not be available to users after cancellation.
 
         Parameters:
-            - id: str. The ID of the connector to delete.
+            - id: str. The ID of the embed job to cancel.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        client.connectors.delete(
-            id="id",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DeleteConnectorResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 403:
-            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def update(
-        self,
-        id: str,
-        *,
-        name: typing.Optional[str] = OMIT,
-        url: typing.Optional[str] = OMIT,
-        excludes: typing.Optional[typing.Sequence[str]] = OMIT,
-        oauth: typing.Optional[CreateConnectorOAuth] = OMIT,
-        active: typing.Optional[bool] = OMIT,
-        continue_on_failure: typing.Optional[bool] = OMIT,
-        service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> UpdateConnectorResponse:
-        """
-        Update a connector by ID. Omitted fields will not be updated. See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
-
-        Parameters:
-            - id: str. The ID of the connector to update.
-
-            - name: typing.Optional[str]. A human-readable name for the connector.
-
-            - url: typing.Optional[str]. The URL of the connector that will be used to search for documents.
-
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
-
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
-
-            - active: typing.Optional[bool].
-
-            - continue_on_failure: typing.Optional[bool].
-
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from cohere.client import Client
-
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
-            token="YOUR_TOKEN",
-        )
-        client.connectors.update(
-            id="id",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if name is not OMIT:
-            _request["name"] = name
-        if url is not OMIT:
-            _request["url"] = url
-        if excludes is not OMIT:
-            _request["excludes"] = excludes
-        if oauth is not OMIT:
-            _request["oauth"] = oauth
-        if active is not OMIT:
-            _request["active"] = active
-        if continue_on_failure is not OMIT:
-            _request["continue_on_failure"] = continue_on_failure
-        if service_auth is not OMIT:
-            _request["service_auth"] = service_auth
-        _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UpdateConnectorResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 403:
-            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def o_auth_authorize(
-        self,
-        id: str,
-        *,
-        after_token_redirect: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> OAuthAuthorizeResponse:
-        """
-        Authorize the connector with the given ID for the connector oauth app. See ['Connector Authentication'](https://docs.cohere.com/docs/connector-authentication) for more information.
-
-        Parameters:
-            - id: str. The ID of the connector to authorize.
-
-            - after_token_redirect: typing.Optional[str]. The URL to redirect to after the connector has been authorized.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from cohere.client import Client
-
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
-            token="YOUR_TOKEN",
-        )
-        client.connectors.o_auth_authorize(
+        client.embed_jobs.cancel(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}/oauth/authorize"
+                f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}/cancel"
             ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "after_token_redirect": after_token_redirect,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -476,74 +296,62 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(OAuthAuthorizeResponse, _response.json())  # type: ignore
+            return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncConnectorsClient:
+class AsyncEmbedJobsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
-        self,
-        *,
-        limit: typing.Optional[float] = None,
-        offset: typing.Optional[float] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListConnectorsResponse:
+    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListEmbedJobResponse:
         """
-        Returns a list of connectors ordered by descending creation date (newer first). See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
+        The list embed job endpoint allows users to view all embed jobs history for that specific user.
 
         Parameters:
-            - limit: typing.Optional[float]. Maximum number of connectors to return [0, 100].
-
-            - offset: typing.Optional[float]. Number of connectors to skip before returning results [0, inf].
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        await client.connectors.list()
+        await client.embed_jobs.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "offset": offset,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -552,89 +360,98 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListConnectorsResponse, _response.json())  # type: ignore
+            return typing.cast(ListEmbedJobResponse, construct_type(type_=ListEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 429:
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
-        name: str,
-        description: typing.Optional[str] = OMIT,
-        url: str,
-        excludes: typing.Optional[typing.Sequence[str]] = OMIT,
-        oauth: typing.Optional[CreateConnectorOAuth] = OMIT,
-        active: typing.Optional[bool] = OMIT,
-        continue_on_failure: typing.Optional[bool] = OMIT,
-        service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
+        model: str,
+        dataset_id: str,
+        input_type: EmbedInputType,
+        name: typing.Optional[str] = OMIT,
+        embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
+        truncate: typing.Optional[CreateEmbedJobRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> CreateConnectorResponse:
+    ) -> CreateEmbedJobResponse:
         """
-        Creates a new connector. The connector is tested during registration and will cancel registration when the test is unsuccessful. See ['Creating and Deploying a Connector'](https://docs.cohere.com/docs/creating-and-deploying-a-connector) for more information.
+        This API launches an async Embed job for a [Dataset](https://docs.cohere.com/docs/datasets) of type `embed-input`. The result of a completed embed job is new Dataset of type `embed-output`, which contains the original text entries and the corresponding embeddings.
 
         Parameters:
-            - name: str. A human-readable name for the connector.
+            - model: str. ID of the embedding model.
+
+                          Available models and corresponding embedding dimensions:
 
-            - description: typing.Optional[str]. A description of the connector.
+                          - `embed-english-v3.0` : 1024
+                          - `embed-multilingual-v3.0` : 1024
+                          - `embed-english-light-v3.0` : 384
+                          - `embed-multilingual-light-v3.0` : 384
 
-            - url: str. The URL of the connector that will be used to search for documents.
+            - dataset_id: str. ID of a [Dataset](https://docs.cohere.com/docs/datasets). The Dataset must be of type `embed-input` and must have a validation status `Validated`
 
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
+            - input_type: EmbedInputType.
 
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
+            - name: typing.Optional[str]. The name of the embed job.
 
-            - active: typing.Optional[bool]. Whether the connector is active or not.
+            - embedding_types: typing.Optional[typing.Sequence[EmbeddingType]]. Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
 
-            - continue_on_failure: typing.Optional[bool]. Whether a chat request should continue or not if the request to this connector fails.
+                                                                                * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
+                                                                                * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
+                                                                                * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
+                                                                                * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
+                                                                                * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
+            - truncate: typing.Optional[CreateEmbedJobRequestTruncate]. One of `START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
+                                                                        Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        await client.connectors.create(
-            name="name",
-            url="url",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "url": url}
-        if description is not OMIT:
-            _request["description"] = description
-        if excludes is not OMIT:
-            _request["excludes"] = excludes
-        if oauth is not OMIT:
-            _request["oauth"] = oauth
-        if active is not OMIT:
-            _request["active"] = active
-        if continue_on_failure is not OMIT:
-            _request["continue_on_failure"] = continue_on_failure
-        if service_auth is not OMIT:
-            _request["service_auth"] = service_auth
+        await client.embed_jobs.create(
+            model="model",
+            dataset_id="dataset_id",
+            input_type="search_document",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"model": model, "dataset_id": dataset_id, "input_type": input_type}
+        if name is not OMIT:
+            _request["name"] = name
+        if embedding_types is not OMIT:
+            _request["embedding_types"] = embedding_types
+        if truncate is not OMIT:
+            _request["truncate"] = truncate
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -651,51 +468,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(CreateConnectorResponse, _response.json())  # type: ignore
+            return typing.cast(CreateEmbedJobResponse, construct_type(type_=CreateEmbedJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 403:
-            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetConnectorResponse:
+    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> EmbedJob:
         """
-        Retrieve a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
+        This API retrieves the details about an embed job started by the same user.
 
         Parameters:
-            - id: str. The ID of the connector to retrieve.
+            - id: str. The ID of the embed job to retrieve.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        await client.connectors.get(
+        await client.embed_jobs.get(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -706,235 +527,63 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetConnectorResponse, _response.json())  # type: ignore
+            return typing.cast(EmbedJob, construct_type(type_=EmbedJob, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> DeleteConnectorResponse:
+    async def cancel(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Delete a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
+        This API allows users to cancel an active embed job. Once invoked, the embedding process will be terminated, and users will be charged for the embeddings processed up to the cancellation point. It's important to note that partial results will not be available to users after cancellation.
 
         Parameters:
-            - id: str. The ID of the connector to delete.
+            - id: str. The ID of the embed job to cancel.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        await client.connectors.delete(
-            id="id",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DeleteConnectorResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 403:
-            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def update(
-        self,
-        id: str,
-        *,
-        name: typing.Optional[str] = OMIT,
-        url: typing.Optional[str] = OMIT,
-        excludes: typing.Optional[typing.Sequence[str]] = OMIT,
-        oauth: typing.Optional[CreateConnectorOAuth] = OMIT,
-        active: typing.Optional[bool] = OMIT,
-        continue_on_failure: typing.Optional[bool] = OMIT,
-        service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> UpdateConnectorResponse:
-        """
-        Update a connector by ID. Omitted fields will not be updated. See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
-
-        Parameters:
-            - id: str. The ID of the connector to update.
-
-            - name: typing.Optional[str]. A human-readable name for the connector.
-
-            - url: typing.Optional[str]. The URL of the connector that will be used to search for documents.
-
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
-
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
-
-            - active: typing.Optional[bool].
-
-            - continue_on_failure: typing.Optional[bool].
-
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from cohere.client import AsyncClient
-
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
-            token="YOUR_TOKEN",
-        )
-        await client.connectors.update(
-            id="id",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if name is not OMIT:
-            _request["name"] = name
-        if url is not OMIT:
-            _request["url"] = url
-        if excludes is not OMIT:
-            _request["excludes"] = excludes
-        if oauth is not OMIT:
-            _request["oauth"] = oauth
-        if active is not OMIT:
-            _request["active"] = active
-        if continue_on_failure is not OMIT:
-            _request["continue_on_failure"] = continue_on_failure
-        if service_auth is not OMIT:
-            _request["service_auth"] = service_auth
-        _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UpdateConnectorResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 403:
-            raise ForbiddenError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def o_auth_authorize(
-        self,
-        id: str,
-        *,
-        after_token_redirect: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> OAuthAuthorizeResponse:
-        """
-        Authorize the connector with the given ID for the connector oauth app. See ['Connector Authentication'](https://docs.cohere.com/docs/connector-authentication) for more information.
-
-        Parameters:
-            - id: str. The ID of the connector to authorize.
-
-            - after_token_redirect: typing.Optional[str]. The URL to redirect to after the connector has been authorized.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from cohere.client import AsyncClient
-
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
-            token="YOUR_TOKEN",
-        )
-        await client.connectors.o_auth_authorize(
+        await client.embed_jobs.cancel(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}/oauth/authorize"
+                f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}/cancel"
             ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "after_token_redirect": after_token_redirect,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -946,21 +595,29 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(OAuthAuthorizeResponse, _response.json())  # type: ignore
+            return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 429:
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.2.2/src/cohere/core/__init__.py` & `cohere-5.2.3/src/cohere/core/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
 from .pydantic_utilities import pydantic_v1
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
+from .unchecked_base_model import UncheckedBaseModel, UnionMetadata, construct_type
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
     "AsyncHttpClient",
     "BaseClientWrapper",
     "File",
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
+    "UncheckedBaseModel",
+    "UnionMetadata",
+    "construct_type",
     "convert_file_dict_to_httpx_tuples",
     "jsonable_encoder",
     "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `cohere-5.2.2/src/cohere/core/client_wrapper.py` & `cohere-5.2.3/src/cohere/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.2.2",
+            "X-Fern-SDK-Version": "5.2.3",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.2.2/src/cohere/core/datetime_utils.py` & `cohere-5.2.3/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/core/file.py` & `cohere-5.2.3/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/core/http_client.py` & `cohere-5.2.3/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/core/jsonable_encoder.py` & `cohere-5.2.3/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/core/request_options.py` & `cohere-5.2.3/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/datasets/client.py` & `cohere-5.2.3/src/cohere/datasets/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from json.decoder import JSONDecodeError
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.datetime_utils import serialize_datetime
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.dataset_type import DatasetType
 from .types.datasets_create_response import DatasetsCreateResponse
 from .types.datasets_get_response import DatasetsGetResponse
 from .types.datasets_get_usage_response import DatasetsGetUsageResponse
 from .types.datasets_list_response import DatasetsListResponse
 
@@ -92,17 +92,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsListResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsListResponse, construct_type(type_=DatasetsListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
@@ -203,17 +205,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsCreateResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsCreateResponse, construct_type(type_=DatasetsCreateResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_usage(self, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetUsageResponse:
@@ -248,17 +252,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsGetUsageResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsGetUsageResponse, construct_type(type_=DatasetsGetUsageResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetResponse:
@@ -297,17 +303,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsGetResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsGetResponse, construct_type(type_=DatasetsGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(
@@ -348,17 +356,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(typing.Dict[str, typing.Any], _response.json())  # type: ignore
+            return typing.cast(typing.Dict[str, typing.Any], construct_type(type_=typing.Dict[str, typing.Any], object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -430,17 +440,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsListResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsListResponse, construct_type(type_=DatasetsListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
@@ -541,17 +553,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsCreateResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsCreateResponse, construct_type(type_=DatasetsCreateResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_usage(self, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetUsageResponse:
@@ -586,17 +600,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsGetUsageResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsGetUsageResponse, construct_type(type_=DatasetsGetUsageResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetResponse:
@@ -635,17 +651,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DatasetsGetResponse, _response.json())  # type: ignore
+            return typing.cast(DatasetsGetResponse, construct_type(type_=DatasetsGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(
@@ -686,15 +704,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(typing.Dict[str, typing.Any], _response.json())  # type: ignore
+            return typing.cast(typing.Dict[str, typing.Any], construct_type(type_=typing.Dict[str, typing.Any], object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.2.2/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.2.3/src/cohere/types/chat_search_result_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class DatasetsCreateResponse(pydantic_v1.BaseModel):
-    id: typing.Optional[str] = pydantic_v1.Field(default=None)
+class ChatSearchResultConnector(UncheckedBaseModel):
     """
-    The dataset ID
+    The connector used for fetching documents.
+    """
+
+    id: str = pydantic_v1.Field()
+    """
+    The identifier of the connector.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.2.3/src/cohere/types/generate_stream_event.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...types.dataset import Dataset
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class DatasetsGetResponse(pydantic_v1.BaseModel):
-    dataset: Dataset
-
+class GenerateStreamEvent(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.2.3/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class DatasetsGetUsageResponse(pydantic_v1.BaseModel):
-    organization_usage: typing.Optional[str] = pydantic_v1.Field(default=None)
+class RerankRequestDocumentsItemText(UncheckedBaseModel):
+    text: str = pydantic_v1.Field()
     """
-    The total number of bytes used by the organization.
+    The text of the document to rerank.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.2.3/src/cohere/datasets/types/datasets_list_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from ...types.dataset import Dataset
 
 
-class DatasetsListResponse(pydantic_v1.BaseModel):
+class DatasetsListResponse(UncheckedBaseModel):
     datasets: typing.Optional[typing.List[Dataset]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/errors/__init__.py` & `cohere-5.2.3/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/finetuning/__init__.py` & `cohere-5.2.3/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .base_type import BaseType
 from .strategy import Strategy
 
 
-class BaseModel(pydantic_v1.BaseModel):
+class BaseModel(UncheckedBaseModel):
     """
     The base model used for fine-tuning.
     """
 
     name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The name of the base model.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class CreateFinetunedModelResponse(pydantic_v1.BaseModel):
+class GetFinetunedModelResponse(UncheckedBaseModel):
     """
-    Response to request to create a fine-tuned model.
+    Response to a request to get a fine-tuned model.
     """
 
     finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
     """
     Information about the fine-tuned model.
     """
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class Error(pydantic_v1.BaseModel):
+class Error(UncheckedBaseModel):
     """
     Error is the response for any unsuccessful event.
     """
 
     message: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A developer-facing error message.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .status import Status
 
 
-class Event(pydantic_v1.BaseModel):
+class Event(UncheckedBaseModel):
     """
     A change in status of a fine-tuned model.
     """
 
     user_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     ID of the user who initiated the event. Empty if initiated by the system.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .settings import Settings
 from .status import Status
 
 
-class FinetunedModel(pydantic_v1.BaseModel):
+class FinetunedModel(UncheckedBaseModel):
     """
     This resource represents a fine-tuned model.
     """
 
     id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     read-only. FinetunedModel ID.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class GetFinetunedModelResponse(pydantic_v1.BaseModel):
+class UpdateFinetunedModelResponse(UncheckedBaseModel):
     """
-    Response to a request to get a fine-tuned model.
+    Response to a request to update a fine-tuned model.
     """
 
     finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
     """
     Information about the fine-tuned model.
     """
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class Hyperparameters(pydantic_v1.BaseModel):
+class Hyperparameters(UncheckedBaseModel):
     """
     The fine-tuning hyperparameters.
     """
 
     early_stopping_patience: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Stops training if the loss metric does not improve beyond the value of
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .event import Event
 
 
-class ListEventsResponse(pydantic_v1.BaseModel):
+class ListEventsResponse(UncheckedBaseModel):
     """
     Response to a request to list events of a fine-tuned model.
     """
 
     events: typing.Optional[typing.List[Event]] = pydantic_v1.Field(default=None)
     """
     List of events for the fine-tuned model.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class ListFinetunedModelsResponse(pydantic_v1.BaseModel):
+class ListFinetunedModelsResponse(UncheckedBaseModel):
     """
     Response to a request to list fine-tuned models.
     """
 
     finetuned_models: typing.Optional[typing.List[FinetunedModel]] = pydantic_v1.Field(default=None)
     """
     List of fine-tuned models matching the request.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .training_step_metrics import TrainingStepMetrics
 
 
-class ListTrainingStepMetricsResponse(pydantic_v1.BaseModel):
+class ListTrainingStepMetricsResponse(UncheckedBaseModel):
     """
     Response to a request to list training-step metrics of a fine-tuned model.
     """
 
     step_metrics: typing.Optional[typing.List[TrainingStepMetrics]] = pydantic_v1.Field(default=None)
     """
     The metrics for each step the evaluation was run on.
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.2.3/src/cohere/types/api_meta_billed_units.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .base_model import BaseModel
-from .hyperparameters import Hyperparameters
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class Settings(pydantic_v1.BaseModel):
+class ApiMetaBilledUnits(UncheckedBaseModel):
+    input_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    The configuration used for fine-tuning.
+    The number of billed input tokens.
     """
 
-    base_model: BaseModel = pydantic_v1.Field()
+    output_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    The base model to fine-tune.
+    The number of billed output tokens.
     """
 
-    dataset_id: str = pydantic_v1.Field()
+    search_units: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    The data used for training and evaluating the fine-tuned model.
+    The number of billed search units.
     """
 
-    hyperparameters: typing.Optional[Hyperparameters] = pydantic_v1.Field(default=None)
+    classifications: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    Fine-tuning hyper-parameters.
-    """
-
-    multi_label: typing.Optional[bool] = pydantic_v1.Field(default=None)
-    """
-    read-only. Whether the model is single-label or multi-label (only for classification).
+    The number of billed classifications units.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.2.3/src/cohere/types/label_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class TrainingStepMetrics(pydantic_v1.BaseModel):
+class LabelMetric(UncheckedBaseModel):
+    total_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The evaluation metrics at a given step of the training of a fine-tuned model.
+    Total number of examples for this label
     """
 
-    created_at: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
+    label: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Creation timestamp.
+    value of the label
     """
 
-    step_number: typing.Optional[int] = pydantic_v1.Field(default=None)
+    samples: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
     """
-    Step number.
-    """
-
-    metrics: typing.Optional[typing.Dict[str, float]] = pydantic_v1.Field(default=None)
-    """
-    Map of names and values for each evaluation metrics.
+    samples for this label
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class UpdateFinetunedModelResponse(pydantic_v1.BaseModel):
+class CreateFinetunedModelResponse(UncheckedBaseModel):
     """
-    Response to a request to update a fine-tuned model.
+    Response to request to create a fine-tuned model.
     """
 
     finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
     """
     Information about the fine-tuned model.
     """
```

### Comparing `cohere-5.2.2/src/cohere/manually_maintained/cache.py` & `cohere-5.2.3/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.2.3/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/models/client.py` & `cohere-5.2.3/src/cohere/models/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.compatible_endpoint import CompatibleEndpoint
 from ..types.get_model_response import GetModelResponse
 from ..types.list_models_response import ListModelsResponse
 
@@ -58,21 +58,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetModelResponse, _response.json())  # type: ignore
+            return typing.cast(GetModelResponse, construct_type(type_=GetModelResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list(
@@ -131,17 +137,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListModelsResponse, _response.json())  # type: ignore
+            return typing.cast(ListModelsResponse, construct_type(type_=ListModelsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -185,21 +193,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetModelResponse, _response.json())  # type: ignore
+            return typing.cast(GetModelResponse, construct_type(type_=GetModelResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 500:
-            raise InternalServerError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise InternalServerError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list(
@@ -258,15 +272,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListModelsResponse, _response.json())  # type: ignore
+            return typing.cast(ListModelsResponse, construct_type(type_=ListModelsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 429:
-            raise TooManyRequestsError(pydantic_v1.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            raise TooManyRequestsError(
+                typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `cohere-5.2.2/src/cohere/overrides.py` & `cohere-5.2.3/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/__init__.py` & `cohere-5.2.3/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/api_meta.py` & `cohere-5.2.3/src/cohere/types/list_embed_job_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .api_meta_api_version import ApiMetaApiVersion
-from .api_meta_billed_units import ApiMetaBilledUnits
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .embed_job import EmbedJob
 
 
-class ApiMeta(pydantic_v1.BaseModel):
-    api_version: typing.Optional[ApiMetaApiVersion] = None
-    billed_units: typing.Optional[ApiMetaBilledUnits] = None
-    warnings: typing.Optional[typing.List[str]] = None
+class ListEmbedJobResponse(UncheckedBaseModel):
+    embed_jobs: typing.Optional[typing.List[EmbedJob]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/api_meta_api_version.py` & `cohere-5.2.3/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ApiMetaApiVersion(pydantic_v1.BaseModel):
-    version: str
-    is_deprecated: typing.Optional[bool] = None
-    is_experimental: typing.Optional[bool] = None
+class SingleGenerationTokenLikelihoodsItem(UncheckedBaseModel):
+    token: str
+    likelihood: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/api_meta_billed_units.py` & `cohere-5.2.3/src/cohere/types/dataset_part.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ApiMetaBilledUnits(pydantic_v1.BaseModel):
-    input_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
+class DatasetPart(UncheckedBaseModel):
+    id: str = pydantic_v1.Field()
     """
-    The number of billed input tokens.
+    The dataset part ID
     """
 
-    output_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
+    name: str = pydantic_v1.Field()
     """
-    The number of billed output tokens.
+    The name of the dataset part
     """
 
-    search_units: typing.Optional[float] = pydantic_v1.Field(default=None)
+    url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The number of billed search units.
+    The download url of the file
     """
 
-    classifications: typing.Optional[float] = pydantic_v1.Field(default=None)
+    index: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    The number of billed classifications units.
+    The index of the file
+    """
+
+    size_bytes: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The size of the file in bytes
+    """
+
+    num_rows: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The number of rows in the file
+    """
+
+    original_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The download url of the original file
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_citation.py` & `cohere-5.2.3/src/cohere/types/chat_citation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatCitation(pydantic_v1.BaseModel):
+class ChatCitation(UncheckedBaseModel):
     """
     A section of the generated reply which cites external knowledge.
     """
 
     start: int = pydantic_v1.Field()
     """
     The index of text that the citation starts at, counting from zero. For example, a generation of `Hello, world!` with a citation on `world` would have a start value of `7`. This is because the citation starts at `w`, which is the seventh character.
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.2.3/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/chat_connector.py` & `cohere-5.2.3/src/cohere/types/chat_connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatConnector(pydantic_v1.BaseModel):
+class ChatConnector(UncheckedBaseModel):
     """
     The connector used for fetching documents.
     """
 
     id: str = pydantic_v1.Field()
     """
     The identifier of the connector.
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_data_metrics.py` & `cohere-5.2.3/src/cohere/types/chat_data_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatDataMetrics(pydantic_v1.BaseModel):
-    num_train_turns: typing.Optional[str] = pydantic_v1.Field(alias="numTrainTurns", default=None)
+class ChatDataMetrics(UncheckedBaseModel):
+    num_train_turns: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The sum of all turns of valid train examples.
     """
 
-    num_eval_turns: typing.Optional[str] = pydantic_v1.Field(alias="numEvalTurns", default=None)
+    num_eval_turns: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The sum of all turns of valid eval examples.
     """
 
     preamble: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The preamble of this dataset.
@@ -30,11 +31,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_message.py` & `cohere-5.2.3/src/cohere/types/chat_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .chat_message_role import ChatMessageRole
 
 
-class ChatMessage(pydantic_v1.BaseModel):
+class ChatMessage(UncheckedBaseModel):
     """
     Represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
 
     The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
     """
 
     role: ChatMessageRole = pydantic_v1.Field()
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.2.3/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatRequestConnectorsSearchOptions(pydantic_v1.BaseModel):
+class ChatRequestConnectorsSearchOptions(UncheckedBaseModel):
     """
     (internal) Sets inference and model options for RAG search query and tool use generations. Defaults are used when options are not specified here, meaning that other parameters outside of connectors_search_options are ignored (such as model= or temperature=).
     """
 
     model: typing.Optional[typing.Any] = None
     temperature: typing.Optional[typing.Any] = None
     max_tokens: typing.Optional[typing.Any] = None
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.2.3/src/cohere/types/get_connector_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .tool_call import ToolCall
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .connector import Connector
 
 
-class ChatRequestToolResultsItem(pydantic_v1.BaseModel):
-    call: ToolCall
-    outputs: typing.List[typing.Dict[str, typing.Any]]
+class GetConnectorResponse(UncheckedBaseModel):
+    connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.2.3/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/chat_search_query.py` & `cohere-5.2.3/src/cohere/types/chat_search_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatSearchQuery(pydantic_v1.BaseModel):
+class ChatSearchQuery(UncheckedBaseModel):
     """
     The generated search query. Contains the text of the query and a unique identifier for the query.
     """
 
     text: str = pydantic_v1.Field()
     """
     The text of the search query.
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_search_result.py` & `cohere-5.2.3/src/cohere/types/chat_search_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .chat_search_query import ChatSearchQuery
 from .chat_search_result_connector import ChatSearchResultConnector
 
 
-class ChatSearchResult(pydantic_v1.BaseModel):
+class ChatSearchResult(UncheckedBaseModel):
     search_query: typing.Optional[ChatSearchQuery] = None
     connector: ChatSearchResultConnector = pydantic_v1.Field()
     """
     The connector from which this result comes from.
     """
 
     document_ids: typing.List[str] = pydantic_v1.Field()
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_search_result_connector.py` & `cohere-5.2.3/src/cohere/types/generate_stream_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .finish_reason import FinishReason
+from .generate_stream_event import GenerateStreamEvent
 
 
-class ChatSearchResultConnector(pydantic_v1.BaseModel):
+class GenerateStreamError(GenerateStreamEvent):
+    index: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    The connector used for fetching documents.
+    Refers to the nth generation. Only present when `num_generations` is greater than zero.
     """
 
-    id: str = pydantic_v1.Field()
+    is_finished: bool
+    finish_reason: FinishReason
+    err: str = pydantic_v1.Field()
     """
-    The identifier of the connector.
+    Error message
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_search_results_event.py` & `cohere-5.2.3/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/chat_stream_end_event.py` & `cohere-5.2.3/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/chat_stream_event.py` & `cohere-5.2.3/src/cohere/types/parse_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatStreamEvent(pydantic_v1.BaseModel):
+class ParseInfo(UncheckedBaseModel):
+    separator: typing.Optional[str] = None
+    delimiter: typing.Optional[str] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.2.3/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatStreamRequestConnectorsSearchOptions(pydantic_v1.BaseModel):
+class ChatStreamRequestConnectorsSearchOptions(UncheckedBaseModel):
     """
     (internal) Sets inference and model options for RAG search query and tool use generations. Defaults are used when options are not specified here, meaning that other parameters outside of connectors_search_options are ignored (such as model= or temperature=).
     """
 
     model: typing.Optional[typing.Any] = None
     temperature: typing.Optional[typing.Any] = None
     max_tokens: typing.Optional[typing.Any] = None
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.2.3/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .tool_call import ToolCall
 
 
-class ChatStreamRequestToolResultsItem(pydantic_v1.BaseModel):
+class ChatStreamRequestToolResultsItem(UncheckedBaseModel):
     call: ToolCall
     outputs: typing.List[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/chat_stream_start_event.py` & `cohere-5.2.3/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/chat_text_generation_event.py` & `cohere-5.2.3/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.2.3/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/classify_data_metrics.py` & `cohere-5.2.3/src/cohere/types/chat_stream_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .label_metric import LabelMetric
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ClassifyDataMetrics(pydantic_v1.BaseModel):
-    label_metrics: typing.Optional[typing.List[LabelMetric]] = pydantic_v1.Field(alias="labelMetrics", default=None)
-
+class ChatStreamEvent(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/classify_example.py` & `cohere-5.2.3/src/cohere/types/api_meta_api_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ClassifyExample(pydantic_v1.BaseModel):
-    text: typing.Optional[str] = None
-    label: typing.Optional[str] = None
+class ApiMetaApiVersion(UncheckedBaseModel):
+    version: str
+    is_deprecated: typing.Optional[bool] = None
+    is_experimental: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/classify_response.py` & `cohere-5.2.3/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .api_meta import ApiMeta
-from .classify_response_classifications_item import ClassifyResponseClassificationsItem
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ClassifyResponse(pydantic_v1.BaseModel):
-    id: str
-    classifications: typing.List[ClassifyResponseClassificationsItem]
-    meta: typing.Optional[ApiMeta] = None
+class ClassifyResponseClassificationsItemLabelsValue(UncheckedBaseModel):
+    confidence: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.2.3/src/cohere/types/classify_response_classifications_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .classify_response_classifications_item_classification_type import (
     ClassifyResponseClassificationsItemClassificationType,
 )
 from .classify_response_classifications_item_labels_value import ClassifyResponseClassificationsItemLabelsValue
 
 
-class ClassifyResponseClassificationsItem(pydantic_v1.BaseModel):
+class ClassifyResponseClassificationsItem(UncheckedBaseModel):
     id: str
     input: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The input text that was classified
     """
 
     prediction: typing.Optional[str] = pydantic_v1.Field(default=None)
```

### Comparing `cohere-5.2.2/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.2.3/src/cohere/types/create_connector_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .connector import Connector
 
 
-class ClassifyResponseClassificationsItemLabelsValue(pydantic_v1.BaseModel):
-    confidence: typing.Optional[float] = None
+class CreateConnectorResponse(UncheckedBaseModel):
+    connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/connector.py` & `cohere-5.2.3/src/cohere/types/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .connector_auth_status import ConnectorAuthStatus
 from .connector_o_auth import ConnectorOAuth
 
 
-class Connector(pydantic_v1.BaseModel):
+class Connector(UncheckedBaseModel):
     """
     A connector allows you to integrate data sources with the '/chat' endpoint to create grounded generations with citations to the data source.
     documents to help answer users.
     """
 
     id: str = pydantic_v1.Field()
     """
```

### Comparing `cohere-5.2.2/src/cohere/types/connector_o_auth.py` & `cohere-5.2.3/src/cohere/types/create_connector_o_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ConnectorOAuth(pydantic_v1.BaseModel):
+class CreateConnectorOAuth(UncheckedBaseModel):
     client_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The OAuth 2.0 client ID. This field is encrypted at rest.
+    The OAuth 2.0 client ID. This fields is encrypted at rest.
     """
 
     client_secret: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth 2.0 client Secret. This field is encrypted at rest and never returned in a response.
     """
 
-    authorize_url: str = pydantic_v1.Field()
+    authorize_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth 2.0 /authorize endpoint to use when users authorize the connector.
     """
 
-    token_url: str = pydantic_v1.Field()
+    token_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth 2.0 /token endpoint to use when users authorize the connector.
     """
 
     scope: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth scopes to request when users authorize the connector.
```

### Comparing `cohere-5.2.2/src/cohere/types/create_connector_o_auth.py` & `cohere-5.2.3/src/cohere/types/connector_o_auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class CreateConnectorOAuth(pydantic_v1.BaseModel):
+class ConnectorOAuth(UncheckedBaseModel):
     client_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The OAuth 2.0 client ID. This fields is encrypted at rest.
+    The OAuth 2.0 client ID. This field is encrypted at rest.
     """
 
     client_secret: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth 2.0 client Secret. This field is encrypted at rest and never returned in a response.
     """
 
-    authorize_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    authorize_url: str = pydantic_v1.Field()
     """
     The OAuth 2.0 /authorize endpoint to use when users authorize the connector.
     """
 
-    token_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    token_url: str = pydantic_v1.Field()
     """
     The OAuth 2.0 /token endpoint to use when users authorize the connector.
     """
 
     scope: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth scopes to request when users authorize the connector.
```

### Comparing `cohere-5.2.2/src/cohere/types/create_connector_response.py` & `cohere-5.2.3/src/cohere/types/update_connector_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .connector import Connector
 
 
-class CreateConnectorResponse(pydantic_v1.BaseModel):
+class UpdateConnectorResponse(UncheckedBaseModel):
     connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/types/create_connector_service_auth.py` & `cohere-5.2.3/src/cohere/types/o_auth_authorize_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .auth_token_type import AuthTokenType
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class CreateConnectorServiceAuth(pydantic_v1.BaseModel):
-    type: AuthTokenType
-    token: str = pydantic_v1.Field()
+class OAuthAuthorizeResponse(UncheckedBaseModel):
+    redirect_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The token that will be used in the HTTP Authorization header when making requests to the connector. This field is encrypted at rest and never returned in a response.
+    The OAuth 2.0 redirect url. Redirect the user to this url to authorize the connector.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/types/create_embed_job_response.py` & `cohere-5.2.3/src/cohere/types/create_embed_job_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 
 
-class CreateEmbedJobResponse(pydantic_v1.BaseModel):
+class CreateEmbedJobResponse(UncheckedBaseModel):
     """
     Response from creating an embed job.
     """
 
     job_id: str
     meta: typing.Optional[ApiMeta] = None
```

### Comparing `cohere-5.2.2/src/cohere/types/dataset.py` & `cohere-5.2.3/src/cohere/types/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .dataset_part import DatasetPart
 from .dataset_type import DatasetType
 from .dataset_validation_status import DatasetValidationStatus
 
 
-class Dataset(pydantic_v1.BaseModel):
+class Dataset(UncheckedBaseModel):
     id: str = pydantic_v1.Field()
     """
     The dataset ID
     """
 
     name: str = pydantic_v1.Field()
     """
```

### Comparing `cohere-5.2.2/src/cohere/types/dataset_part.py` & `cohere-5.2.3/src/cohere/types/embed_job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
+from .embed_job_status import EmbedJobStatus
+from .embed_job_truncate import EmbedJobTruncate
 
 
-class DatasetPart(pydantic_v1.BaseModel):
-    id: str = pydantic_v1.Field()
+class EmbedJob(UncheckedBaseModel):
+    job_id: str = pydantic_v1.Field()
     """
-    The dataset part ID
+    ID of the embed job
     """
 
-    name: str = pydantic_v1.Field()
+    name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The name of the dataset part
+    The name of the embed job
     """
 
-    url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    status: EmbedJobStatus = pydantic_v1.Field()
     """
-    The download url of the file
+    The status of the embed job
     """
 
-    index: typing.Optional[int] = pydantic_v1.Field(default=None)
+    created_at: dt.datetime = pydantic_v1.Field()
     """
-    The index of the file
+    The creation date of the embed job
     """
 
-    size_bytes: typing.Optional[int] = pydantic_v1.Field(default=None)
+    input_dataset_id: str = pydantic_v1.Field()
     """
-    The size of the file in bytes
+    ID of the input dataset
     """
 
-    num_rows: typing.Optional[int] = pydantic_v1.Field(default=None)
+    output_dataset_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The number of rows in the file
+    ID of the resulting output dataset
     """
 
-    original_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    model: str = pydantic_v1.Field()
     """
-    The download url of the original file
+    ID of the model used to embed
     """
 
+    truncate: EmbedJobTruncate = pydantic_v1.Field()
+    """
+    The truncation option used
+    """
+
+    meta: typing.Optional[ApiMeta] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/detokenize_response.py` & `cohere-5.2.3/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from .api_meta import ApiMeta
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class DetokenizeResponse(pydantic_v1.BaseModel):
-    text: str = pydantic_v1.Field()
+class DatasetsGetUsageResponse(UncheckedBaseModel):
+    organization_usage: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    A string representing the list of tokens.
+    The total number of bytes used by the organization.
     """
 
-    meta: typing.Optional[ApiMeta] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/embed_by_type_response.py` & `cohere-5.2.3/src/cohere/types/embed_floats_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
-from .embed_by_type_response_embeddings import EmbedByTypeResponseEmbeddings
 
 
-class EmbedByTypeResponse(pydantic_v1.BaseModel):
+class EmbedFloatsResponse(UncheckedBaseModel):
     id: str
-    embeddings: EmbedByTypeResponseEmbeddings = pydantic_v1.Field()
+    embeddings: typing.List[typing.List[float]] = pydantic_v1.Field()
     """
-    An object with different embedding types. The length of each embedding type array will be the same as the length of the original `texts` array.
+    An array of embeddings, where each embedding is an array of floats. The length of the `embeddings` array will be the same as the length of the original `texts` array.
     """
 
     texts: typing.List[str] = pydantic_v1.Field()
     """
     The text entries for which embeddings were returned.
     """
```

### Comparing `cohere-5.2.2/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.2.3/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class EmbedByTypeResponseEmbeddings(pydantic_v1.BaseModel):
+class EmbedByTypeResponseEmbeddings(UncheckedBaseModel):
     """
     An object with different embedding types. The length of each embedding type array will be the same as the length of the original `texts` array.
     """
 
     float_: typing.Optional[typing.List[typing.List[float]]] = pydantic_v1.Field(alias="float", default=None)
     """
     An array of float embeddings.
```

### Comparing `cohere-5.2.2/src/cohere/types/embed_floats_response.py` & `cohere-5.2.3/src/cohere/types/tokenize_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 
 
-class EmbedFloatsResponse(pydantic_v1.BaseModel):
-    id: str
-    embeddings: typing.List[typing.List[float]] = pydantic_v1.Field()
+class TokenizeResponse(UncheckedBaseModel):
+    tokens: typing.List[int] = pydantic_v1.Field()
     """
-    An array of embeddings, where each embedding is an array of floats. The length of the `embeddings` array will be the same as the length of the original `texts` array.
-    """
-
-    texts: typing.List[str] = pydantic_v1.Field()
-    """
-    The text entries for which embeddings were returned.
+    An array of tokens, where each token is an integer.
     """
 
+    token_strings: typing.List[str]
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/types/embed_job.py` & `cohere-5.2.3/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .api_meta import ApiMeta
-from .embed_job_status import EmbedJobStatus
-from .embed_job_truncate import EmbedJobTruncate
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class EmbedJob(pydantic_v1.BaseModel):
-    job_id: str = pydantic_v1.Field()
+class ToolParameterDefinitionsValue(UncheckedBaseModel):
+    description: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    ID of the embed job
+    The description of the parameter.
     """
 
-    name: typing.Optional[str] = pydantic_v1.Field(default=None)
+    type: str = pydantic_v1.Field()
     """
-    The name of the embed job
+    The type of the parameter. Must be a valid Python type.
     """
 
-    status: EmbedJobStatus = pydantic_v1.Field()
+    required: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
-    The status of the embed job
+    Denotes whether the parameter is always present (required) or not. Defaults to not required.
     """
 
-    created_at: dt.datetime = pydantic_v1.Field()
-    """
-    The creation date of the embed job
-    """
-
-    input_dataset_id: str = pydantic_v1.Field()
-    """
-    ID of the input dataset
-    """
-
-    output_dataset_id: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    ID of the resulting output dataset
-    """
-
-    model: str = pydantic_v1.Field()
-    """
-    ID of the model used to embed
-    """
-
-    truncate: EmbedJobTruncate = pydantic_v1.Field()
-    """
-    The truncation option used
-    """
-
-    meta: typing.Optional[ApiMeta] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.2.3/src/cohere/types/finetune_dataset_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class FinetuneDatasetMetrics(pydantic_v1.BaseModel):
-    trainable_token_count: typing.Optional[str] = pydantic_v1.Field(alias="trainableTokenCount", default=None)
+class FinetuneDatasetMetrics(UncheckedBaseModel):
+    trainable_token_count: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The number of tokens of valid examples that can be used for training.
     """
 
-    total_examples: typing.Optional[str] = pydantic_v1.Field(alias="totalExamples", default=None)
+    total_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The overall number of examples.
     """
 
-    train_examples: typing.Optional[str] = pydantic_v1.Field(alias="trainExamples", default=None)
+    train_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The number of training examples.
     """
 
-    train_size_bytes: typing.Optional[str] = pydantic_v1.Field(alias="trainSizeBytes", default=None)
+    train_size_bytes: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The size in bytes of all training examples.
     """
 
-    eval_examples: typing.Optional[str] = pydantic_v1.Field(alias="evalExamples", default=None)
+    eval_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Number of evaluation examples.
     """
 
-    eval_size_bytes: typing.Optional[str] = pydantic_v1.Field(alias="evalSizeBytes", default=None)
+    eval_size_bytes: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The size in bytes of all eval examples.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -45,11 +46,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/generate_stream_end.py` & `cohere-5.2.3/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/generate_stream_end_response.py` & `cohere-5.2.3/src/cohere/types/generate_stream_end_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .single_generation_in_stream import SingleGenerationInStream
 
 
-class GenerateStreamEndResponse(pydantic_v1.BaseModel):
+class GenerateStreamEndResponse(UncheckedBaseModel):
     id: str
     prompt: typing.Optional[str] = None
     generations: typing.Optional[typing.List[SingleGenerationInStream]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/generate_stream_error.py` & `cohere-5.2.3/src/cohere/types/single_generation_in_stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .finish_reason import FinishReason
-from .generate_stream_event import GenerateStreamEvent
 
 
-class GenerateStreamError(GenerateStreamEvent):
+class SingleGenerationInStream(UncheckedBaseModel):
+    id: str
+    text: str = pydantic_v1.Field()
+    """
+    Full text of the generation.
+    """
+
     index: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Refers to the nth generation. Only present when `num_generations` is greater than zero.
     """
 
-    is_finished: bool
     finish_reason: FinishReason
-    err: str = pydantic_v1.Field()
-    """
-    Error message
-    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/generate_stream_event.py` & `cohere-5.2.3/src/cohere/datasets/types/datasets_get_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from ...types.dataset import Dataset
 
 
-class GenerateStreamEvent(pydantic_v1.BaseModel):
+class DatasetsGetResponse(UncheckedBaseModel):
+    dataset: Dataset
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/generate_stream_text.py` & `cohere-5.2.3/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/src/cohere/types/generation.py` & `cohere-5.2.3/src/cohere/types/summarize_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
-from .single_generation import SingleGeneration
 
 
-class Generation(pydantic_v1.BaseModel):
-    id: str
-    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
+class SummarizeResponse(UncheckedBaseModel):
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Prompt used for generations.
+    Generated ID for the summary
     """
 
-    generations: typing.List[SingleGeneration] = pydantic_v1.Field()
+    summary: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    List of generated results
+    Generated summary for the text
     """
 
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/get_connector_response.py` & `cohere-5.2.3/src/cohere/types/embed_by_type_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .connector import Connector
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
+from .embed_by_type_response_embeddings import EmbedByTypeResponseEmbeddings
+
+
+class EmbedByTypeResponse(UncheckedBaseModel):
+    id: str
+    embeddings: EmbedByTypeResponseEmbeddings = pydantic_v1.Field()
+    """
+    An object with different embedding types. The length of each embedding type array will be the same as the length of the original `texts` array.
+    """
+
+    texts: typing.List[str] = pydantic_v1.Field()
+    """
+    The text entries for which embeddings were returned.
+    """
 
-
-class GetConnectorResponse(pydantic_v1.BaseModel):
-    connector: Connector
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/get_model_response.py` & `cohere-5.2.3/src/cohere/types/get_model_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .compatible_endpoint import CompatibleEndpoint
 
 
-class GetModelResponse(pydantic_v1.BaseModel):
+class GetModelResponse(UncheckedBaseModel):
     """
     Contains information about the model and which API endpoints it can be used with.
     """
 
     name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Specify this name in the `model` parameter of API requests to use your chosen model.
@@ -29,19 +30,14 @@
     """
 
     context_length: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     The maximum number of tokens that the model can process in a single request. Note that not all of these tokens are always available due to special tokens and preambles that Cohere has added by default.
     """
 
-    tokenizer: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The name of the tokenizer used for the model.
-    """
-
     tokenizer_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Public URL to the tokenizer's configuration file.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/label_metric.py` & `cohere-5.2.3/src/cohere/datasets/types/datasets_create_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class LabelMetric(pydantic_v1.BaseModel):
-    total_examples: typing.Optional[str] = pydantic_v1.Field(alias="totalExamples", default=None)
+class DatasetsCreateResponse(UncheckedBaseModel):
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Total number of examples for this label
-    """
-
-    label: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    value of the label
-    """
-
-    samples: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
-    """
-    samples for this label
+    The dataset ID
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/list_connectors_response.py` & `cohere-5.2.3/src/cohere/types/generation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .connector import Connector
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
+from .single_generation import SingleGeneration
 
 
-class ListConnectorsResponse(pydantic_v1.BaseModel):
-    connectors: typing.List[Connector]
-    total_count: typing.Optional[float] = pydantic_v1.Field(default=None)
+class Generation(UncheckedBaseModel):
+    id: str
+    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Total number of connectors.
+    Prompt used for generations.
     """
 
+    generations: typing.List[SingleGeneration] = pydantic_v1.Field()
+    """
+    List of generated results
+    """
+
+    meta: typing.Optional[ApiMeta] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/list_embed_job_response.py` & `cohere-5.2.3/src/cohere/types/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .embed_job import EmbedJob
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .finetune_dataset_metrics import FinetuneDatasetMetrics
 
 
-class ListEmbedJobResponse(pydantic_v1.BaseModel):
-    embed_jobs: typing.Optional[typing.List[EmbedJob]] = None
+class Metrics(UncheckedBaseModel):
+    finetune_dataset_metrics: typing.Optional[FinetuneDatasetMetrics] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/list_models_response.py` & `cohere-5.2.3/src/cohere/types/list_models_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .get_model_response import GetModelResponse
 
 
-class ListModelsResponse(pydantic_v1.BaseModel):
+class ListModelsResponse(UncheckedBaseModel):
     models: typing.List[GetModelResponse]
     next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A token to retrieve the next page of results. Provide in the page_token parameter of the next request.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `cohere-5.2.2/src/cohere/types/metrics.py` & `cohere-5.2.3/src/cohere/types/chat_request_tool_results_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .finetune_dataset_metrics import FinetuneDatasetMetrics
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .tool_call import ToolCall
 
 
-class Metrics(pydantic_v1.BaseModel):
-    finetune_dataset_metrics: typing.Optional[FinetuneDatasetMetrics] = None
+class ChatRequestToolResultsItem(UncheckedBaseModel):
+    call: ToolCall
+    outputs: typing.List[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.2.3/src/cohere/types/non_streamed_chat_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .chat_citation import ChatCitation
 from .chat_document import ChatDocument
 from .chat_message import ChatMessage
 from .chat_search_query import ChatSearchQuery
 from .chat_search_result import ChatSearchResult
 from .finish_reason import FinishReason
 from .tool_call import ToolCall
 
 
-class NonStreamedChatResponse(pydantic_v1.BaseModel):
+class NonStreamedChatResponse(UncheckedBaseModel):
     text: str = pydantic_v1.Field()
     """
     Contents of the reply generated by the model.
     """
 
     generation_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
```

### Comparing `cohere-5.2.2/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.2.3/src/cohere/types/detokenize_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
 
 
-class OAuthAuthorizeResponse(pydantic_v1.BaseModel):
-    redirect_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+class DetokenizeResponse(UncheckedBaseModel):
+    text: str = pydantic_v1.Field()
     """
-    The OAuth 2.0 redirect url. Redirect the user to this url to authorize the connector.
+    A string representing the list of tokens.
     """
 
+    meta: typing.Optional[ApiMeta] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/parse_info.py` & `cohere-5.2.3/src/cohere/types/classify_data_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .label_metric import LabelMetric
 
 
-class ParseInfo(pydantic_v1.BaseModel):
-    separator: typing.Optional[str] = None
-    delimiter: typing.Optional[str] = None
+class ClassifyDataMetrics(UncheckedBaseModel):
+    label_metrics: typing.Optional[typing.List[LabelMetric]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.2.3/src/cohere/types/rerank_response_results_item_document.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class RerankRequestDocumentsItemText(pydantic_v1.BaseModel):
+class RerankResponseResultsItemDocument(UncheckedBaseModel):
+    """
+    The doc object which was ranked
+    """
+
     text: str = pydantic_v1.Field()
     """
-    The text of the document to rerank.
+    The text of the document to rerank
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/types/rerank_response.py` & `cohere-5.2.3/src/cohere/types/rerank_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 from .rerank_response_results_item import RerankResponseResultsItem
 
 
-class RerankResponse(pydantic_v1.BaseModel):
+class RerankResponse(UncheckedBaseModel):
     id: typing.Optional[str] = None
     results: typing.List[RerankResponseResultsItem] = pydantic_v1.Field()
     """
     An ordered list of ranked documents
     """
 
     meta: typing.Optional[ApiMeta] = None
```

### Comparing `cohere-5.2.2/src/cohere/types/rerank_response_results_item.py` & `cohere-5.2.3/src/cohere/types/rerank_response_results_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .rerank_response_results_item_document import RerankResponseResultsItemDocument
 
 
-class RerankResponseResultsItem(pydantic_v1.BaseModel):
+class RerankResponseResultsItem(UncheckedBaseModel):
     document: typing.Optional[RerankResponseResultsItemDocument] = pydantic_v1.Field(default=None)
     """
     The doc object which was ranked
     """
 
     index: int = pydantic_v1.Field()
     """
```

### Comparing `cohere-5.2.2/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.2.3/src/cohere/types/list_connectors_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .connector import Connector
 
 
-class RerankResponseResultsItemDocument(pydantic_v1.BaseModel):
+class ListConnectorsResponse(UncheckedBaseModel):
+    connectors: typing.List[Connector]
+    total_count: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    The doc object which was ranked
-    """
-
-    text: str = pydantic_v1.Field()
-    """
-    The text of the document to rerank
+    Total number of connectors.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.2/src/cohere/types/reranker_data_metrics.py` & `cohere-5.2.3/src/cohere/types/reranker_data_metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class RerankerDataMetrics(pydantic_v1.BaseModel):
-    num_train_queries: typing.Optional[str] = pydantic_v1.Field(alias="numTrainQueries", default=None)
+class RerankerDataMetrics(UncheckedBaseModel):
+    num_train_queries: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The number of training queries.
     """
 
-    num_train_relevant_passages: typing.Optional[str] = pydantic_v1.Field(
-        alias="numTrainRelevantPassages", default=None
-    )
+    num_train_relevant_passages: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The sum of all relevant passages of valid training examples.
     """
 
-    num_train_hard_negatives: typing.Optional[str] = pydantic_v1.Field(alias="numTrainHardNegatives", default=None)
+    num_train_hard_negatives: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The sum of all hard negatives of valid training examples.
     """
 
-    num_eval_queries: typing.Optional[str] = pydantic_v1.Field(alias="numEvalQueries", default=None)
+    num_eval_queries: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The number of evaluation queries.
     """
 
-    num_eval_relevant_passages: typing.Optional[str] = pydantic_v1.Field(alias="numEvalRelevantPassages", default=None)
+    num_eval_relevant_passages: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The sum of all relevant passages of valid eval examples.
     """
 
-    num_eval_hard_negatives: typing.Optional[str] = pydantic_v1.Field(alias="numEvalHardNegatives", default=None)
+    num_eval_hard_negatives: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The sum of all hard negatives of valid eval examples.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -47,11 +46,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.2.2/src/cohere/types/single_generation.py` & `cohere-5.2.3/src/cohere/types/single_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .single_generation_token_likelihoods_item import SingleGenerationTokenLikelihoodsItem
 
 
-class SingleGeneration(pydantic_v1.BaseModel):
+class SingleGeneration(UncheckedBaseModel):
     id: str
     text: str
     index: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Refers to the nth generation. Only present when `num_generations` is greater than zero.
     """
```

### Comparing `cohere-5.2.2/src/cohere/types/single_generation_in_stream.py` & `cohere-5.2.3/src/cohere/types/create_connector_service_auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .finish_reason import FinishReason
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .auth_token_type import AuthTokenType
 
 
-class SingleGenerationInStream(pydantic_v1.BaseModel):
-    id: str
-    text: str = pydantic_v1.Field()
+class CreateConnectorServiceAuth(UncheckedBaseModel):
+    type: AuthTokenType
+    token: str = pydantic_v1.Field()
     """
-    Full text of the generation.
+    The token that will be used in the HTTP Authorization header when making requests to the connector. This field is encrypted at rest and never returned in a response.
     """
 
-    index: typing.Optional[int] = pydantic_v1.Field(default=None)
-    """
-    Refers to the nth generation. Only present when `num_generations` is greater than zero.
-    """
-
-    finish_reason: FinishReason
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.2/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.2.3/src/cohere/types/classify_example.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SingleGenerationTokenLikelihoodsItem(pydantic_v1.BaseModel):
-    token: str
-    likelihood: float
+class ClassifyExample(UncheckedBaseModel):
+    text: typing.Optional[str] = None
+    label: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/streamed_chat_response.py` & `cohere-5.2.3/src/cohere/types/streamed_chat_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
+import typing_extensions
+
+from ..core.unchecked_base_model import UnionMetadata
 from .chat_citation_generation_event import ChatCitationGenerationEvent
 from .chat_search_queries_generation_event import ChatSearchQueriesGenerationEvent
 from .chat_search_results_event import ChatSearchResultsEvent
 from .chat_stream_end_event import ChatStreamEndEvent
 from .chat_stream_start_event import ChatStreamStartEvent
 from .chat_text_generation_event import ChatTextGenerationEvent
 from .chat_tool_calls_generation_event import ChatToolCallsGenerationEvent
@@ -79,16 +82,19 @@
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
-StreamedChatResponse = typing.Union[
-    StreamedChatResponse_StreamStart,
-    StreamedChatResponse_SearchQueriesGeneration,
-    StreamedChatResponse_SearchResults,
-    StreamedChatResponse_TextGeneration,
-    StreamedChatResponse_CitationGeneration,
-    StreamedChatResponse_ToolCallsGeneration,
-    StreamedChatResponse_StreamEnd,
+StreamedChatResponse = typing_extensions.Annotated[
+    typing.Union[
+        StreamedChatResponse_StreamStart,
+        StreamedChatResponse_SearchQueriesGeneration,
+        StreamedChatResponse_SearchResults,
+        StreamedChatResponse_TextGeneration,
+        StreamedChatResponse_CitationGeneration,
+        StreamedChatResponse_ToolCallsGeneration,
+        StreamedChatResponse_StreamEnd,
+    ],
+    UnionMetadata(discriminant="event_type"),
 ]
```

### Comparing `cohere-5.2.2/src/cohere/types/summarize_response.py` & `cohere-5.2.3/src/cohere/types/tool_call.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .api_meta import ApiMeta
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SummarizeResponse(pydantic_v1.BaseModel):
-    id: typing.Optional[str] = pydantic_v1.Field(default=None)
+class ToolCall(UncheckedBaseModel):
     """
-    Generated ID for the summary
+    Contains the tool calls generated by the model. Use it to invoke your tools.
     """
 
-    summary: typing.Optional[str] = pydantic_v1.Field(default=None)
+    name: str = pydantic_v1.Field()
     """
-    Generated summary for the text
+    Name of the tool to call.
     """
 
-    meta: typing.Optional[ApiMeta] = None
+    parameters: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    The name and value of the parameters to use when invoking a tool.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/tokenize_response.py` & `cohere-5.2.3/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from .api_meta import ApiMeta
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class TokenizeResponse(pydantic_v1.BaseModel):
-    tokens: typing.List[int] = pydantic_v1.Field()
+class TrainingStepMetrics(UncheckedBaseModel):
     """
-    An array of tokens, where each token is an integer.
+    The evaluation metrics at a given step of the training of a fine-tuned model.
     """
 
-    token_strings: typing.List[str]
-    meta: typing.Optional[ApiMeta] = None
+    created_at: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
+    """
+    Creation timestamp.
+    """
+
+    step_number: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Step number.
+    """
+
+    metrics: typing.Optional[typing.Dict[str, float]] = pydantic_v1.Field(default=None)
+    """
+    Map of names and values for each evaluation metrics.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.2.2/src/cohere/types/tool.py` & `cohere-5.2.3/src/cohere/types/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .tool_parameter_definitions_value import ToolParameterDefinitionsValue
 
 
-class Tool(pydantic_v1.BaseModel):
+class Tool(UncheckedBaseModel):
     name: str = pydantic_v1.Field()
     """
     The name of the tool to be called. Valid names contain only the characters `a-z`, `A-Z`, `0-9`, `_` and must not begin with a digit.
     """
 
     description: str = pydantic_v1.Field()
     """
```

### Comparing `cohere-5.2.2/src/cohere/utils.py` & `cohere-5.2.3/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.2/PKG-INFO` & `cohere-5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.2.2
+Version: 5.2.3
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

