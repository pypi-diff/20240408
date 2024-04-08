# Comparing `tmp/haystack_ai-2.0.0rc1.tar.gz` & `tmp/haystack_ai-2.0.1rc1.tar.gz`

## Comparing `haystack_ai-2.0.0rc1.tar` & `haystack_ai-2.0.1rc1.tar`

### file list

```diff
@@ -1,168 +1,169 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/VERSION.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/errors.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/logging.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13706 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16195 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/azure.py
--rw-r--r--   0        0        0    10440 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    17612 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    17574 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/errors.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/serialization.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/type_utils.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/component/component.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/component/types.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    51706 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/dataclasses/document.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/marshal/yaml.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/__init__.py
--rw-r--r--   0        0        0    57589 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/factory.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/tracing/utils.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/auth.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/device.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/expit.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/filters.py
--rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/README.md
--rw-r--r--   0        0        0     9563 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 haystack_ai-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/VERSION.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/errors.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/logging.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13706 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16195 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0    12132 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    12720 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    17612 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    17574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/errors.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/types.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    53414 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    57626 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/device.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/filters.py
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/LICENSE
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/README.md
+-rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/PKG-INFO
```

### Comparing `haystack_ai-2.0.0rc1/haystack/__init__.py` & `haystack_ai-2.0.1rc1/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/lazy_imports.py` & `haystack_ai-2.0.1rc1/haystack/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/logging.py` & `haystack_ai-2.0.1rc1/haystack/logging.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/audio/whisper_local.py` & `haystack_ai-2.0.1rc1/haystack/components/audio/whisper_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.0.1rc1/haystack/components/audio/whisper_remote.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/builders/answer_builder.py` & `haystack_ai-2.0.1rc1/haystack/components/builders/answer_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/builders/prompt_builder.py` & `haystack_ai-2.0.1rc1/haystack/components/builders/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/caching/cache_checker.py` & `haystack_ai-2.0.1rc1/haystack/components/caching/cache_checker.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.0.1rc1/haystack/components/classifiers/document_language_classifier.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.0.1rc1/haystack/components/connectors/openapi_service.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/__init__.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/azure.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/html.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/html.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/markdown.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/markdown.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/openapi_functions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/output_adapter.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/output_adapter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/pypdf.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/pypdf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/tika.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/tika.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/txt.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/txt.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/converters/utils.py` & `haystack_ai-2.0.1rc1/haystack/components/converters/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/__init__.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/azure_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/azure_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import Document
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_secrets_inplace
 from haystack.utils.hf import HFModelType, check_valid_model
 
-with LazyImport(message="Run 'pip install transformers'") as transformers_import:
+with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\"'") as huggingface_hub_import:
     from huggingface_hub import InferenceClient
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class HuggingFaceTEIDocumentEmbedder:
@@ -75,15 +75,15 @@
         :param progress_bar:
             If True shows a progress bar when running.
         :param meta_fields_to_embed:
             List of meta fields that will be embedded along with the Document text.
         :param embedding_separator:
             Separator used to concatenate the meta fields to the Document text.
         """
-        transformers_import.check()
+        huggingface_hub_import.check()
 
         if url:
             r = urlparse(url)
             is_valid_url = all([r.scheme in ["http", "https"], r.netloc])
             if not is_valid_url:
                 raise ValueError(f"Invalid TEI endpoint URL provided: {url}")
```

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from urllib.parse import urlparse
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_secrets_inplace
 from haystack.utils.hf import HFModelType, check_valid_model
 
-with LazyImport(message="Run 'pip install transformers'") as transformers_import:
+with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\"'") as huggingface_hub_import:
     from huggingface_hub import InferenceClient
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class HuggingFaceTEITextEmbedder:
@@ -58,15 +58,15 @@
             The HuggingFace Hub token. This is needed if you are using a paid HF Inference Endpoint or serving
             a private or gated model.
         :param prefix:
             A string to add at the beginning of each text.
         :param suffix:
             A string to add at the end of each text.
         """
-        transformers_import.check()
+        huggingface_hub_import.check()
 
         if url:
             r = urlparse(url)
             is_valid_url = all([r.scheme in ["http", "https"], r.netloc])
             if not is_valid_url:
                 raise ValueError(f"Invalid TEI endpoint URL provided: {url}")
 
@@ -131,12 +131,12 @@
             raise TypeError(
                 "HuggingFaceTEITextEmbedder expects a string as an input."
                 "In case you want to embed a list of Documents, please use the HuggingFaceTEIDocumentEmbedder."
             )
 
         text_to_embed = self.prefix + text + self.suffix
 
-        embedding = self.client.feature_extraction(text=text_to_embed)
+        embeddings = self.client.feature_extraction(text=[text_to_embed])
         # The client returns a numpy array
-        embedding = embedding.tolist()
+        embedding = embeddings.tolist()[0]
 
         return {"embedding": embedding}
```

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/openai_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/openai_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.0.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.0.1rc1/haystack/components/extractors/named_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/fetchers/link_content.py` & `haystack_ai-2.0.1rc1/haystack/components/fetchers/link_content.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/azure.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_local.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Callable, Dict, List, Literal, Optional
 
 from haystack import component, default_from_dict, default_to_dict, logging
+from haystack.dataclasses import StreamingChunk
 from haystack.lazy_imports import LazyImport
-from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
-from haystack.utils.hf import deserialize_hf_model_kwargs, serialize_hf_model_kwargs
+from haystack.utils import (
+    ComponentDevice,
+    Secret,
+    deserialize_callable,
+    deserialize_secrets_inplace,
+    serialize_callable,
+)
+from haystack.utils.hf import HFTokenStreamingHandler, deserialize_hf_model_kwargs, serialize_hf_model_kwargs
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_TASKS = ["text-generation", "text2text-generation"]
 
 with LazyImport(message="Run 'pip install transformers[torch]'") as transformers_import:
     from huggingface_hub import model_info
@@ -44,14 +51,15 @@
         model: str = "google/flan-t5-base",
         task: Optional[Literal["text-generation", "text2text-generation"]] = None,
         device: Optional[ComponentDevice] = None,
         token: Optional[Secret] = Secret.from_env_var("HF_API_TOKEN", strict=False),
         generation_kwargs: Optional[Dict[str, Any]] = None,
         huggingface_pipeline_kwargs: Optional[Dict[str, Any]] = None,
         stop_words: Optional[List[str]] = None,
+        streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
     ):
         """
         Creates an instance of a HuggingFaceLocalGenerator.
 
         :param model: The name or path of a Hugging Face model for text generation,
         :param task: The task for the Hugging Face pipeline.
             Possible values are "text-generation" and "text2text-generation".
@@ -77,14 +85,15 @@
             for more information on the available kwargs.
             In this dictionary, you can also include `model_kwargs` to specify the kwargs for model initialization:
             [transformers.PreTrainedModel.from_pretrained](https://huggingface.co/docs/transformers/en/main_classes/model#transformers.PreTrainedModel.from_pretrained)
         :param stop_words: A list of stop words. If any one of the stop words is generated, the generation is stopped.
             If you provide this parameter, you should not specify the `stopping_criteria` in `generation_kwargs`.
             For some chat models, the output includes both the new text and the original prompt.
             In these cases, it's important to make sure your prompt has no stop words.
+        :param streaming_callback: An optional callable for handling streaming responses.
         """
         transformers_import.check()
 
         huggingface_pipeline_kwargs = huggingface_pipeline_kwargs or {}
         generation_kwargs = generation_kwargs or {}
 
         self.token = token
@@ -119,20 +128,22 @@
             generation_kwargs.setdefault("return_full_text", False)
 
         if stop_words and "stopping_criteria" in generation_kwargs:
             raise ValueError(
                 "Found both the `stop_words` init parameter and the `stopping_criteria` key in `generation_kwargs`. "
                 "Please specify only one of them."
             )
+        generation_kwargs.setdefault("max_new_tokens", 512)
 
         self.huggingface_pipeline_kwargs = huggingface_pipeline_kwargs
         self.generation_kwargs = generation_kwargs
         self.stop_words = stop_words
         self.pipeline = None
         self.stopping_criteria_list = None
+        self.streaming_callback = streaming_callback
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         if isinstance(self.huggingface_pipeline_kwargs["model"], str):
             return {"model": self.huggingface_pipeline_kwargs["model"]}
@@ -154,18 +165,20 @@
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
+        callback_name = serialize_callable(self.streaming_callback) if self.streaming_callback else None
         serialization_dict = default_to_dict(
             self,
             huggingface_pipeline_kwargs=self.huggingface_pipeline_kwargs,
             generation_kwargs=self.generation_kwargs,
+            streaming_callback=callback_name,
             stop_words=self.stop_words,
             token=self.token.to_dict() if self.token else None,
         )
 
         huggingface_pipeline_kwargs = serialization_dict["init_parameters"]["huggingface_pipeline_kwargs"]
         huggingface_pipeline_kwargs.pop("token", None)
 
@@ -180,14 +193,19 @@
         :param data:
             The dictionary to deserialize from.
         :returns:
             The deserialized component.
         """
         deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
         deserialize_hf_model_kwargs(data["init_parameters"]["huggingface_pipeline_kwargs"])
+        init_params = data.get("init_parameters", {})
+        serialized_callback_handler = init_params.get("streaming_callback")
+        if serialized_callback_handler:
+            data["init_parameters"]["streaming_callback"] = deserialize_callable(serialized_callback_handler)
+
         return default_from_dict(cls, data)
 
     @component.output_types(replies=List[str])
     def run(self, prompt: str, generation_kwargs: Optional[Dict[str, Any]] = None):
         """
         Run the text generation model on the given prompt.
 
@@ -205,14 +223,29 @@
 
         if not prompt:
             return {"replies": []}
 
         # merge generation kwargs from init method with those from run method
         updated_generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
 
+        if self.streaming_callback:
+            num_responses = updated_generation_kwargs.get("num_return_sequences", 1)
+            if num_responses > 1:
+                logger.warning(
+                    "Streaming is enabled, but the number of responses is set to %d. "
+                    "Streaming is only supported for single response generation. "
+                    "Setting the number of responses to 1.",
+                    num_responses,
+                )
+                updated_generation_kwargs["num_return_sequences"] = 1
+            # streamer parameter hooks into HF streaming, HFTokenStreamingHandler is an adapter to our streaming
+            updated_generation_kwargs["streamer"] = HFTokenStreamingHandler(
+                self.pipeline.tokenizer, self.streaming_callback, self.stop_words
+            )
+
         output = self.pipeline(prompt, stopping_criteria=self.stopping_criteria_list, **updated_generation_kwargs)
         replies = [o["generated_text"] for o in output if "generated_text" in o]
 
         if self.stop_words:
             # the output of the pipeline includes the stop word
             replies = [reply.replace(stop_word, "").rstrip() for reply in replies for stop_word in self.stop_words]
```

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_tgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import StreamingChunk
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 from haystack.utils.hf import HFModelType, check_generation_params, check_valid_model, list_inference_deployed_models
 
-with LazyImport(message="Run 'pip install transformers'") as transformers_import:
-    from huggingface_hub import InferenceClient
-    from huggingface_hub.inference._text_generation import TextGenerationResponse, TextGenerationStreamResponse, Token
+with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\" transformers'") as transformers_import:
+    from huggingface_hub import (
+        InferenceClient,
+        TextGenerationOutput,
+        TextGenerationOutputToken,
+        TextGenerationStreamOutput,
+    )
     from transformers import AutoTokenizer
 
 
 logger = logging.getLogger(__name__)
 
 
 @component
@@ -107,14 +111,15 @@
         check_valid_model(model, HFModelType.GENERATION, token)
 
         # handle generation kwargs setup
         generation_kwargs = generation_kwargs.copy() if generation_kwargs else {}
         check_generation_params(generation_kwargs, ["n"])
         generation_kwargs["stop_sequences"] = generation_kwargs.get("stop_sequences", [])
         generation_kwargs["stop_sequences"].extend(stop_words or [])
+        generation_kwargs.setdefault("max_new_tokens", 512)
 
         self.model = model
         self.url = url
         self.token = token
         self.generation_kwargs = generation_kwargs
         self.client = InferenceClient(url or model, token=token.resolve_value() if token else None)
         self.streaming_callback = streaming_callback
@@ -208,21 +213,21 @@
                 raise ValueError("Cannot stream multiple responses, please set n=1.")
 
             return self._run_streaming(prompt, prompt_token_count, generation_kwargs)
 
         return self._run_non_streaming(prompt, prompt_token_count, num_responses, generation_kwargs)
 
     def _run_streaming(self, prompt: str, prompt_token_count: int, generation_kwargs: Dict[str, Any]):
-        res_chunk: Iterable[TextGenerationStreamResponse] = self.client.text_generation(
+        res_chunk: Iterable[TextGenerationStreamOutput] = self.client.text_generation(
             prompt, details=True, stream=True, **generation_kwargs
         )
         chunks: List[StreamingChunk] = []
         # pylint: disable=not-an-iterable
         for chunk in res_chunk:
-            token: Token = chunk.token
+            token: TextGenerationOutputToken = chunk.token
             if token.special:
                 continue
             chunk_metadata = {**asdict(token), **(asdict(chunk.details) if chunk.details else {})}
             stream_chunk = StreamingChunk(token.text, chunk_metadata)
             chunks.append(stream_chunk)
             self.streaming_callback(stream_chunk)  # type: ignore # streaming_callback is not None (verified in the run method)
         metadata = {
@@ -238,20 +243,20 @@
 
     def _run_non_streaming(
         self, prompt: str, prompt_token_count: int, num_responses: int, generation_kwargs: Dict[str, Any]
     ):
         responses: List[str] = []
         all_metadata: List[Dict[str, Any]] = []
         for _i in range(num_responses):
-            tgr: TextGenerationResponse = self.client.text_generation(prompt, details=True, **generation_kwargs)
+            tgr: TextGenerationOutput = self.client.text_generation(prompt, details=True, **generation_kwargs)
             all_metadata.append(
                 {
                     "model": self.client.model,
                     "index": _i,
-                    "finish_reason": tgr.details.finish_reason.value,
+                    "finish_reason": tgr.details.finish_reason,
                     "usage": {
                         "completion_tokens": len(tgr.details.tokens),
                         "prompt_tokens": prompt_token_count,
                         "total_tokens": prompt_token_count + len(tgr.details.tokens),
                     },
                 }
             )
```

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/openai.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/utils.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/chat/__init__.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/chat/azure.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/chat/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 from haystack.utils.hf import HFModelType, check_generation_params, check_valid_model, list_inference_deployed_models
 
-with LazyImport(message="Run 'pip install transformers'") as transformers_import:
-    from huggingface_hub import InferenceClient
-    from huggingface_hub.inference._text_generation import TextGenerationResponse, TextGenerationStreamResponse, Token
+with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\" transformers'") as transformers_import:
+    from huggingface_hub import (
+        InferenceClient,
+        TextGenerationOutput,
+        TextGenerationOutputToken,
+        TextGenerationStreamOutput,
+    )
     from transformers import AutoTokenizer
 
 logger = logging.getLogger(__name__)
 
 
+@component
 class HuggingFaceTGIChatGenerator:
     """
     Enables text generation using HuggingFace Hub hosted chat-based LLMs. This component is designed to seamlessly
     inference chat-based models deployed on the Text Generation Inference (TGI) backend.
 
     You can use this component for chat LLMs hosted on Hugging Face inference endpoints, the rate-limited
     Inference API tier.
@@ -119,14 +124,15 @@
         check_valid_model(model, HFModelType.GENERATION, token)
 
         # handle generation kwargs setup
         generation_kwargs = generation_kwargs.copy() if generation_kwargs else {}
         check_generation_params(generation_kwargs, ["n"])
         generation_kwargs["stop_sequences"] = generation_kwargs.get("stop_sequences", [])
         generation_kwargs["stop_sequences"].extend(stop_words or [])
+        generation_kwargs.setdefault("max_new_tokens", 512)
 
         self.model = model
         self.url = url
         self.chat_template = chat_template
         self.token = token
         self.generation_kwargs = generation_kwargs
         self.client = InferenceClient(url or model, token=token.resolve_value() if token else None)
@@ -238,31 +244,31 @@
             return self._run_streaming(prepared_prompt, prompt_token_count, generation_kwargs)
 
         return self._run_non_streaming(prepared_prompt, prompt_token_count, num_responses, generation_kwargs)
 
     def _run_streaming(
         self, prepared_prompt: str, prompt_token_count: int, generation_kwargs: Dict[str, Any]
     ) -> Dict[str, List[ChatMessage]]:
-        res: Iterable[TextGenerationStreamResponse] = self.client.text_generation(
+        res: Iterable[TextGenerationStreamOutput] = self.client.text_generation(
             prepared_prompt, stream=True, details=True, **generation_kwargs
         )
         chunk = None
         # pylint: disable=not-an-iterable
         for chunk in res:
-            token: Token = chunk.token
+            token: TextGenerationOutputToken = chunk.token
             if token.special:
                 continue
             chunk_metadata = {**asdict(token), **(asdict(chunk.details) if chunk.details else {})}
             stream_chunk = StreamingChunk(token.text, chunk_metadata)
             self.streaming_callback(stream_chunk)  # type: ignore # streaming_callback is not None (verified in the run method)
 
         message = ChatMessage.from_assistant(chunk.generated_text)
         message.meta.update(
             {
-                "finish_reason": chunk.details.finish_reason.value,
+                "finish_reason": chunk.details.finish_reason,
                 "index": 0,
                 "model": self.client.model,
                 "usage": {
                     "completion_tokens": chunk.details.generated_tokens,
                     "prompt_tokens": prompt_token_count,
                     "total_tokens": prompt_token_count + chunk.details.generated_tokens,
                 },
@@ -271,21 +277,19 @@
         return {"replies": [message]}
 
     def _run_non_streaming(
         self, prepared_prompt: str, prompt_token_count: int, num_responses: int, generation_kwargs: Dict[str, Any]
     ) -> Dict[str, List[ChatMessage]]:
         chat_messages: List[ChatMessage] = []
         for _i in range(num_responses):
-            tgr: TextGenerationResponse = self.client.text_generation(
-                prepared_prompt, details=True, **generation_kwargs
-            )
+            tgr: TextGenerationOutput = self.client.text_generation(prepared_prompt, details=True, **generation_kwargs)
             message = ChatMessage.from_assistant(tgr.generated_text)
             message.meta.update(
                 {
-                    "finish_reason": tgr.details.finish_reason.value,
+                    "finish_reason": tgr.details.finish_reason,
                     "index": _i,
                     "model": self.client.model,
                     "usage": {
                         "completion_tokens": len(tgr.details.tokens),
                         "prompt_tokens": prompt_token_count,
                         "total_tokens": prompt_token_count + len(tgr.details.tokens),
                     },
```

### Comparing `haystack_ai-2.0.0rc1/haystack/components/generators/chat/openai.py` & `haystack_ai-2.0.1rc1/haystack/components/generators/chat/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.0.1rc1/haystack/components/joiners/document_joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/others/multiplexer.py` & `haystack_ai-2.0.1rc1/haystack/components/others/multiplexer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_splitter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.0.1rc1/haystack/components/preprocessors/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.0.1rc1/haystack/components/rankers/lost_in_the_middle.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/rankers/meta_field.py` & `haystack_ai-2.0.1rc1/haystack/components/rankers/meta_field.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.0.1rc1/haystack/components/rankers/transformers_similarity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/readers/extractive.py` & `haystack_ai-2.0.1rc1/haystack/components/readers/extractive.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.0.1rc1/haystack/components/retrievers/filter_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py` & `haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/routers/conditional_router.py` & `haystack_ai-2.0.1rc1/haystack/components/routers/conditional_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/routers/file_type_router.py` & `haystack_ai-2.0.1rc1/haystack/components/routers/file_type_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/routers/metadata_router.py` & `haystack_ai-2.0.1rc1/haystack/components/routers/metadata_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/routers/text_language_router.py` & `haystack_ai-2.0.1rc1/haystack/components/routers/text_language_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/samplers/top_p.py` & `haystack_ai-2.0.1rc1/haystack/components/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/validators/json_schema.py` & `haystack_ai-2.0.1rc1/haystack/components/validators/json_schema.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/websearch/searchapi.py` & `haystack_ai-2.0.1rc1/haystack/components/websearch/searchapi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.0.1rc1/haystack/components/websearch/serper_dev.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/components/writers/document_writer.py` & `haystack_ai-2.0.1rc1/haystack/components/writers/document_writer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/errors.py` & `haystack_ai-2.0.1rc1/haystack/core/errors.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/serialization.py` & `haystack_ai-2.0.1rc1/haystack/core/serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/type_utils.py` & `haystack_ai-2.0.1rc1/haystack/core/type_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/component/component.py` & `haystack_ai-2.0.1rc1/haystack/core/component/component.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/component/sockets.py` & `haystack_ai-2.0.1rc1/haystack/core/component/sockets.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/component/types.py` & `haystack_ai-2.0.1rc1/haystack/core/component/types.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/descriptions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/draw.py` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/draw.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/pipeline.py` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,21 +82,15 @@
         if not isinstance(other, Pipeline):
             return False
         return self.to_dict() == other.to_dict()
 
     def __repr__(self) -> str:
         """
         Returns a text representation of the Pipeline.
-        If this runs in a Jupyter notebook, it will instead display the Pipeline image.
         """
-        if is_in_jupyter():
-            # If we're in a Jupyter notebook we want to display the image instead of the text repr.
-            self.show()
-            return ""
-
         res = f"{object.__repr__(self)}\n"
         if self.metadata:
             res += "🧱 Metadata\n"
             for k, v in self.metadata.items():
                 res += f"  - {k}: {v}\n"
 
         res += "🚅 Components\n"
@@ -899,34 +893,37 @@
                     # It's important to check whether previous waitings are None as it could be that no
                     # Component has actually been run yet.
                     if (
                         before_last_waiting_for_input is not None
                         and last_waiting_for_input is not None
                         and before_last_waiting_for_input == last_waiting_for_input
                     ):
-                        # Are we actually stuck or there's a lazy variadic waiting for input?
-                        # This is our last resort, if there's no lazy variadic waiting for input
+                        # Are we actually stuck or there's a lazy variadic or a component with has only default inputs waiting for input?
+                        # This is our last resort, if there's no lazy variadic or component with only default inputs waiting for input
                         # we're stuck for real and we can't make any progress.
                         for name, comp in waiting_for_input:
                             is_variadic = any(socket.is_variadic for socket in comp.__haystack_input__._sockets_dict.values())  # type: ignore
-                            if is_variadic and not comp.__haystack_is_greedy__:  # type: ignore[attr-defined]
+                            has_only_defaults = all(
+                                not socket.is_mandatory for socket in comp.__haystack_input__._sockets_dict.values()  # type: ignore
+                            )
+                            if is_variadic and not comp.__haystack_is_greedy__ or has_only_defaults:  # type: ignore[attr-defined]
                                 break
                         else:
                             # We're stuck in a loop for real, we can't make any progress.
                             # BAIL!
                             break
 
                         if len(waiting_for_input) == 1:
-                            # We have a single component with variadic input waiting for input.
+                            # We have a single component with variadic input or only default inputs waiting for input.
                             # If we're at this point it means it has been waiting for input for at least 2 iterations.
                             # This will never run.
                             # BAIL!
                             break
 
-                        # There was a lazy variadic waiting for input, we can run it
+                        # There was a lazy variadic or a component with only default waiting for input, we can run it
                         waiting_for_input.remove((name, comp))
                         to_run.append((name, comp))
                         continue
 
                     before_last_waiting_for_input = (
                         last_waiting_for_input.copy() if last_waiting_for_input is not None else None
                     )
@@ -950,14 +947,34 @@
                                     )
                                     and not other_comp.__haystack_is_greedy__  # type: ignore[attr-defined]
                                 )
 
                             if not there_are_only_lazy_variadics:
                                 continue
 
+                        # Components that have defaults for all their inputs must be treated the same identical way as we treat
+                        # lazy variadic components. If there are only components with defaults we can run them.
+                        # If we don't do this the order of execution of the Pipeline's Components will be affected cause we
+                        # enqueue the Components in `to_run` at the start using the order they are added in the Pipeline.
+                        # If a Component A with defaults is added before a Component B that has no defaults, but in the Pipeline
+                        # logic A must be executed after B it could run instead before if we don't do this check.
+                        has_only_defaults = all(
+                            not socket.is_mandatory for socket in comp.__haystack_input__._sockets_dict.values()  # type: ignore
+                        )
+                        if has_only_defaults:
+                            there_are_only_components_with_defaults = True
+                            for other_name, other_comp in waiting_for_input:
+                                if name == other_name:
+                                    continue
+                                there_are_only_components_with_defaults &= all(
+                                    not s.is_mandatory for s in other_comp.__haystack_input__._sockets_dict.values()  # type: ignore
+                                )
+                            if not there_are_only_components_with_defaults:
+                                continue
+
                         # Find the first component that has all the inputs it needs to run
                         has_enough_inputs = True
                         for input_socket in comp.__haystack_input__._sockets_dict.values():  # type: ignore
                             if input_socket.is_mandatory and input_socket.name not in last_inputs[name]:
                                 has_enough_inputs = False
                                 break
                             if input_socket.is_mandatory:
```

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/template.py` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/template.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/dataclasses/answer.py` & `haystack_ai-2.0.1rc1/haystack/dataclasses/answer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.0.1rc1/haystack/dataclasses/byte_stream.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/dataclasses/chat_message.py` & `haystack_ai-2.0.1rc1/haystack/dataclasses/chat_message.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/dataclasses/document.py` & `haystack_ai-2.0.1rc1/haystack/dataclasses/document.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Dict, List, Optional
 
 from numpy import ndarray
 from pandas import DataFrame, read_json
 
 from haystack import logging
 from haystack.dataclasses.byte_stream import ByteStream
+from haystack.dataclasses.sparse_embedding import SparseEmbedding
 
 logger = logging.getLogger(__name__)
 
 
 class _BackwardCompatible(type):
     """
     Metaclass that handles Document backward compatibility.
@@ -53,24 +54,26 @@
 
     :param id: Unique identifier for the document. When not set, it's generated based on the Document fields' values.
     :param content: Text of the document, if the document contains text.
     :param dataframe: Pandas dataframe with the document's content, if the document contains tabular data.
     :param blob: Binary data associated with the document, if the document has any binary data associated with it.
     :param meta: Additional custom metadata for the document. Must be JSON-serializable.
     :param score: Score of the document. Used for ranking, usually assigned by retrievers.
-    :param embedding: Vector representation of the document.
+    :param embedding: dense vector representation of the document.
+    :param sparse_embedding: sparse vector representation of the document.
     """
 
     id: str = field(default="")
     content: Optional[str] = field(default=None)
     dataframe: Optional[DataFrame] = field(default=None)
     blob: Optional[ByteStream] = field(default=None)
     meta: Dict[str, Any] = field(default_factory=dict)
     score: Optional[float] = field(default=None)
     embedding: Optional[List[float]] = field(default=None)
+    sparse_embedding: Optional[SparseEmbedding] = field(default=None)
 
     def __repr__(self):
         fields = []
         if self.content is not None:
             fields.append(
                 f"content: '{self.content}'" if len(self.content) < 100 else f"content: '{self.content[:100]}...'"
             )
@@ -80,14 +83,16 @@
             fields.append(f"blob: {len(self.blob.data)} bytes")
         if len(self.meta) > 0:
             fields.append(f"meta: {self.meta}")
         if self.score is not None:
             fields.append(f"score: {self.score}")
         if self.embedding is not None:
             fields.append(f"embedding: vector of size {len(self.embedding)}")
+        if self.sparse_embedding is not None:
+            fields.append(f"sparse_embedding: vector with {len(self.sparse_embedding.indices)} non-zero elements")
         fields_str = ", ".join(fields)
         return f"{self.__class__.__name__}(id={self.id}, {fields_str})"
 
     def __eq__(self, other):
         """
         Compares Documents for equality.
 
@@ -110,15 +115,16 @@
         """
         text = self.content or None
         dataframe = self.dataframe.to_json() if self.dataframe is not None else None
         blob = self.blob.data if self.blob is not None else None
         mime_type = self.blob.mime_type if self.blob is not None else None
         meta = self.meta or {}
         embedding = self.embedding if self.embedding is not None else None
-        data = f"{text}{dataframe}{blob}{mime_type}{meta}{embedding}"
+        sparse_embedding = self.sparse_embedding.to_dict() if self.sparse_embedding is not None else ""
+        data = f"{text}{dataframe}{blob}{mime_type}{meta}{embedding}{sparse_embedding}"
         return hashlib.sha256(data.encode("utf-8")).hexdigest()
 
     def to_dict(self, flatten=True) -> Dict[str, Any]:
         """
         Converts Document into a dictionary.
 
         `dataframe` and `blob` fields are converted to JSON-serializable types.
@@ -128,14 +134,17 @@
         """
         data = asdict(self)
         if (dataframe := data.get("dataframe")) is not None:
             data["dataframe"] = dataframe.to_json()
         if (blob := data.get("blob")) is not None:
             data["blob"] = {"data": list(blob["data"]), "mime_type": blob["mime_type"]}
 
+        if (sparse_embedding := data.get("sparse_embedding")) is not None:
+            data["sparse_embedding"] = sparse_embedding.to_dict()
+
         if flatten:
             meta = data.pop("meta")
             return {**data, **meta}
 
         return data
 
     @classmethod
@@ -145,14 +154,17 @@
 
         The `dataframe` and `blob` fields are converted to their original types.
         """
         if (dataframe := data.get("dataframe")) is not None:
             data["dataframe"] = read_json(io.StringIO(dataframe))
         if blob := data.get("blob"):
             data["blob"] = ByteStream(data=bytes(blob["data"]), mime_type=blob["mime_type"])
+        if sparse_embedding := data.get("sparse_embedding"):
+            data["sparse_embedding"] = SparseEmbedding.from_dict(sparse_embedding)
+
         # Store metadata for a moment while we try un-flattening allegedly flatten metadata.
         # We don't expect both a `meta=` keyword and flatten metadata keys so we'll raise a
         # ValueError later if this is the case.
         meta = data.pop("meta", {})
         # Unflatten metadata if it was flattened. We assume any keyword argument that's not
         # a document field is a metadata key. We treat legacy fields as document fields
         # for backward compatibility.
```

### Comparing `haystack_ai-2.0.0rc1/haystack/dataclasses/streaming_chunk.py` & `haystack_ai-2.0.1rc1/haystack/dataclasses/streaming_chunk.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.0.1rc1/haystack/document_stores/in_memory/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/document_stores/types/protocol.py` & `haystack_ai-2.0.1rc1/haystack/document_stores/types/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/telemetry/_environment.py` & `haystack_ai-2.0.1rc1/haystack/telemetry/_environment.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/telemetry/_telemetry.py` & `haystack_ai-2.0.1rc1/haystack/telemetry/_telemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/document_store.py` & `haystack_ai-2.0.1rc1/haystack/testing/document_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1135,18 +1135,18 @@
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": "<=", "value": None})
         self.assert_documents_are_equal(result, [])
 
     # in comparator
     def test_comparison_in(self, document_store, filterable_docs):
         document_store.write_documents(filterable_docs)
-        result = document_store.filter_documents({"field": "meta.number", "operator": "in", "value": [9, 10]})
-        self.assert_documents_are_equal(
-            result, [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] in [9, 10]]
-        )
+        result = document_store.filter_documents({"field": "meta.number", "operator": "in", "value": [10, -10]})
+        assert len(result)
+        expected = [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] in [10, -10]]
+        self.assert_documents_are_equal(result, expected)
 
     def test_comparison_in_with_with_non_list(self, document_store, filterable_docs):
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents({"field": "meta.number", "operator": "in", "value": 9})
 
     def test_comparison_in_with_with_non_list_iterable(self, document_store, filterable_docs):
```

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/factory.py` & `haystack_ai-2.0.1rc1/haystack/testing/factory.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/test_utils.py` & `haystack_ai-2.0.1rc1/haystack/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/accumulate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/add_value.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/concatenate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/fstring.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/greet.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/greet.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/parity.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/parity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/remainder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/self_loop.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/self_loop.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/subtract.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.0.1rc1/haystack/testing/sample_components/threshold.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/tracing/datadog.py` & `haystack_ai-2.0.1rc1/haystack/tracing/datadog.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/tracing/opentelemetry.py` & `haystack_ai-2.0.1rc1/haystack/tracing/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/tracing/tracer.py` & `haystack_ai-2.0.1rc1/haystack/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/tracing/utils.py` & `haystack_ai-2.0.1rc1/haystack/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/__init__.py` & `haystack_ai-2.0.1rc1/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/auth.py` & `haystack_ai-2.0.1rc1/haystack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/callable_serialization.py` & `haystack_ai-2.0.1rc1/haystack/utils/callable_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/device.py` & `haystack_ai-2.0.1rc1/haystack/utils/device.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/filters.py` & `haystack_ai-2.0.1rc1/haystack/utils/filters.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/hf.py` & `haystack_ai-2.0.1rc1/haystack/utils/hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from haystack.lazy_imports import LazyImport
 from haystack.utils.auth import Secret
 from haystack.utils.device import ComponentDevice
 
 with LazyImport(message="Run 'pip install transformers[torch]'") as torch_import:
     import torch
 
-with LazyImport(message="Run 'pip install transformers'") as transformers_import:
-    from huggingface_hub import HfApi, InferenceClient
+with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\"'") as huggingface_hub_import:
+    from huggingface_hub import HfApi, InferenceClient, model_info
     from huggingface_hub.utils import RepositoryNotFoundError
 
 logger = logging.getLogger(__name__)
 
 
 class HFModelType(Enum):
     EMBEDDING = 1
@@ -125,15 +125,15 @@
     Also check if the model is an embedding or generation model.
 
     :param model_id: A string representing the HuggingFace model ID.
     :param model_type: the model type, HFModelType.EMBEDDING or HFModelType.GENERATION
     :param token: The optional authentication token.
     :raises ValueError: If the model is not found or is not a embedding model.
     """
-    transformers_import.check()
+    huggingface_hub_import.check()
 
     api = HfApi()
     try:
         model_info = api.model_info(model_id, token=token.resolve_value() if token else None)
     except RepositoryNotFoundError as e:
         raise ValueError(
             f"Model {model_id} not found on HuggingFace Hub. Please provide a valid HuggingFace model_id."
@@ -154,15 +154,15 @@
     """
     Check the provided generation parameters for validity.
 
     :param kwargs: A dictionary containing the generation parameters.
     :param additional_accepted_params: An optional list of strings representing additional accepted parameters.
     :raises ValueError: If any unknown text generation parameters are provided.
     """
-    transformers_import.check()
+    huggingface_hub_import.check()
 
     if kwargs:
         accepted_params = {
             param
             for param in inspect.signature(InferenceClient.text_generation).parameters.keys()
             if param not in ["self", "prompt"]
         }
@@ -171,15 +171,15 @@
         unknown_params = set(kwargs.keys()) - accepted_params
         if unknown_params:
             raise ValueError(
                 f"Unknown text generation parameters: {unknown_params}. The valid parameters are: {accepted_params}."
             )
 
 
-with LazyImport(message="Run 'pip install transformers[torch]'") as torch_and_transformers_import:
+with LazyImport(message="Run 'pip install transformers[torch]'") as transformers_import:
     from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast, StoppingCriteria, TextStreamer
 
     transformers_import.check()
     torch_import.check()
 
     class StopWordsCriteria(StoppingCriteria):
         """
```

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/jupyter.py` & `haystack_ai-2.0.1rc1/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/requests_utils.py` & `haystack_ai-2.0.1rc1/haystack/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/haystack/utils/type_serialization.py` & `haystack_ai-2.0.1rc1/haystack/utils/type_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/.gitignore` & `haystack_ai-2.0.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/LICENSE` & `haystack_ai-2.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.0rc1/README.md` & `haystack_ai-2.0.1rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-  <a href="https://www.deepset.ai/haystack/"><img src="docs/img/banner_20.png" alt="Haystack"></a>
+  <a href="https://www.deepset.ai/haystack/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Haystack"></a>
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | CI/CD   | [![Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/haystack?branch=main)                                                        |
 | Docs    | [![Website](https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)](https://docs.haystack.deepset.ai)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | Package | [![PyPI](https://img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/farm-haystack?logo=python&logoColor=gold) [![GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml) |
 | Meta    | [![Discord](https://img.shields.io/discord/993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://twitter.com/haystack_ai)                                                                                                                                                                                                                                                                                                                                                                                        |
@@ -53,15 +53,15 @@
 -   Perform **semantic search** and retrieve documents according to meaning.
 -   Build applications that can make complex decisions making to answer complex queries: such as systems that can resolve complex customer queries, do knowledge search on many disconnected resources and so on.
 -   Scale to millions of docs using retrievers and production-scale components.
 -   Use **off-the-shelf models** or **fine-tune** them to your data.
 -   Use **user feedback** to evaluate, benchmark, and continuously improve your models.
 
 > [!TIP]
-><img src="docs/img/deepset-cloud-logo-lightblue.png"  width=30% height=30%>
+><img src="https://github.com/deepset-ai/haystack/raw/main/docs/img/deepset-cloud-logo-lightblue.png"  width=30% height=30%>
 >
 > Are you looking for a managed solution that benefits from Haystack? [deepset Cloud](https://www.deepset.ai/deepset-cloud?utm_campaign=developer-relations&utm_source=haystack&utm_medium=readme) is our fully managed, end-to-end platform to integrate LLMs with your data, which uses Haystack for the LLM pipelines architecture.
 
 ## Telemetry
 
 Haystack collects **anonymous** usage statistics of pipeline components. We receive an event every time these components are initialized. This way, we know which components are most relevant to our community.
```

#### html2text {}

```diff
@@ -67,49 +67,50 @@
 granular answers in your documents. - Perform **semantic search** and retrieve
 documents according to meaning. - Build applications that can make complex
 decisions making to answer complex queries: such as systems that can resolve
 complex customer queries, do knowledge search on many disconnected resources
 and so on. - Scale to millions of docs using retrievers and production-scale
 components. - Use **off-the-shelf models** or **fine-tune** them to your data.
 - Use **user feedback** to evaluate, benchmark, and continuously improve your
-models. > [!TIP] >[docs/img/deepset-cloud-logo-lightblue.png] > > Are you
-looking for a managed solution that benefits from Haystack? [deepset Cloud]
-(https://www.deepset.ai/deepset-cloud?utm_campaign=developer-
-relations&utm_source=haystack&utm_medium=readme) is our fully managed, end-to-
-end platform to integrate LLMs with your data, which uses Haystack for the LLM
-pipelines architecture. ## Telemetry Haystack collects **anonymous** usage
-statistics of pipeline components. We receive an event every time these
-components are initialized. This way, we know which components are most
-relevant to our community. Read more about telemetry in Haystack or how you can
-opt out in [Haystack docs](https://docs.haystack.deepset.ai/v2.0/docs/
-telemetry). ## ð Community If you have a feature request or a bug report,
-feel free to open an [issue in Github](https://github.com/deepset-ai/haystack/
-issues). We regularly check these and you can expect a quick response. If you'd
-like to discuss a topic, or get more general advice on how to make Haystack
-work for your project, you can start a thread in [Github Discussions](https://
-github.com/deepset-ai/haystack/discussions) or our [Discord channel](https://
-discord.gg/haystack). We also check [ð (Twitter)](https://twitter.com/
-haystack_ai) and [Stack Overflow](https://stackoverflow.com/questions/tagged/
-haystack). ## Contributing to Haystack We are very open to the community's
-contributions - be it a quick fix of a typo, or a completely new feature! You
-don't need to be a Haystack expert to provide meaningful improvements. To learn
-how to get started, check out our [Contributor Guidelines](https://github.com/
-deepset-ai/haystack/blob/main/CONTRIBUTING.md) first. There are several ways
-you can contribute to Haystack: - Contribute to the main Haystack project -
-Contribute an integration on [haystack-core-integrations](https://github.com/
-deepset-ai/haystack-core-integrations) > [!TIP] >ð **[Check out the full
-list of issues that are open to contributions](https://github.com/orgs/deepset-
-ai/projects/14)** ## Who Uses Haystack Here's a list of projects and companies
-using Haystack. Want to add yours? Open a PR, add it to the list and let the
-world know that you use Haystack! - [Airbus](https://www.airbus.com/en) -
-[Alcatel-Lucent](https://www.al-enterprise.com/) - [Apple](https://
-www.apple.com/) - [BetterUp](https://www.betterup.com/) - [Databricks](https://
-www.databricks.com/) - [Deepset](https://deepset.ai/) - [Etalab](https://
-www.deepset.ai/blog/improving-on-site-search-for-government-agencies-etalab) -
-[Infineon](https://www.infineon.com/) - [Intel](https://github.com/intel/open-
-domain-question-and-answer#readme) - [Intelijus](https://www.intelijus.ai/) -
-[Intel Labs](https://github.com/IntelLabs/fastRAG#readme) - [LEGO](https://
-github.com/larsbaunwall/bricky#readme) - [Netflix](https://netflix.com) -
-[Nvidia](https://developer.nvidia.com/blog/reducing-development-time-for-
-intelligent-virtual-assistants-in-contact-centers/) - [PostHog](https://
-github.com/PostHog/max-ai#readme) - [Rakuten](https://www.rakuten.com/) -
-[Sooth.ai](https://www.deepset.ai/blog/advanced-neural-search-with-sooth-ai)
+models. > [!TIP] >[https://github.com/deepset-ai/haystack/raw/main/docs/img/
+deepset-cloud-logo-lightblue.png] > > Are you looking for a managed solution
+that benefits from Haystack? [deepset Cloud](https://www.deepset.ai/deepset-
+cloud?utm_campaign=developer-relations&utm_source=haystack&utm_medium=readme)
+is our fully managed, end-to-end platform to integrate LLMs with your data,
+which uses Haystack for the LLM pipelines architecture. ## Telemetry Haystack
+collects **anonymous** usage statistics of pipeline components. We receive an
+event every time these components are initialized. This way, we know which
+components are most relevant to our community. Read more about telemetry in
+Haystack or how you can opt out in [Haystack docs](https://
+docs.haystack.deepset.ai/v2.0/docs/telemetry). ## ð Community If you have a
+feature request or a bug report, feel free to open an [issue in Github](https:/
+/github.com/deepset-ai/haystack/issues). We regularly check these and you can
+expect a quick response. If you'd like to discuss a topic, or get more general
+advice on how to make Haystack work for your project, you can start a thread in
+[Github Discussions](https://github.com/deepset-ai/haystack/discussions) or our
+[Discord channel](https://discord.gg/haystack). We also check [ð (Twitter)]
+(https://twitter.com/haystack_ai) and [Stack Overflow](https://
+stackoverflow.com/questions/tagged/haystack). ## Contributing to Haystack We
+are very open to the community's contributions - be it a quick fix of a typo,
+or a completely new feature! You don't need to be a Haystack expert to provide
+meaningful improvements. To learn how to get started, check out our
+[Contributor Guidelines](https://github.com/deepset-ai/haystack/blob/main/
+CONTRIBUTING.md) first. There are several ways you can contribute to Haystack:
+- Contribute to the main Haystack project - Contribute an integration on
+[haystack-core-integrations](https://github.com/deepset-ai/haystack-core-
+integrations) > [!TIP] >ð **[Check out the full list of issues that are open
+to contributions](https://github.com/orgs/deepset-ai/projects/14)** ## Who Uses
+Haystack Here's a list of projects and companies using Haystack. Want to add
+yours? Open a PR, add it to the list and let the world know that you use
+Haystack! - [Airbus](https://www.airbus.com/en) - [Alcatel-Lucent](https://
+www.al-enterprise.com/) - [Apple](https://www.apple.com/) - [BetterUp](https://
+www.betterup.com/) - [Databricks](https://www.databricks.com/) - [Deepset]
+(https://deepset.ai/) - [Etalab](https://www.deepset.ai/blog/improving-on-site-
+search-for-government-agencies-etalab) - [Infineon](https://www.infineon.com/
+) - [Intel](https://github.com/intel/open-domain-question-and-answer#readme) -
+[Intelijus](https://www.intelijus.ai/) - [Intel Labs](https://github.com/
+IntelLabs/fastRAG#readme) - [LEGO](https://github.com/larsbaunwall/
+bricky#readme) - [Netflix](https://netflix.com) - [Nvidia](https://
+developer.nvidia.com/blog/reducing-development-time-for-intelligent-virtual-
+assistants-in-contact-centers/) - [PostHog](https://github.com/PostHog/max-
+ai#readme) - [Rakuten](https://www.rakuten.com/) - [Sooth.ai](https://
+www.deepset.ai/blog/advanced-neural-search-with-sooth-ai)
```

### Comparing `haystack_ai-2.0.0rc1/pyproject.toml` & `haystack_ai-2.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
 
 [tool.hatch.envs.default.scripts]
 format = "black ."
 format-check = "black --check ."
 
 [tool.hatch.envs.test]
 extra-dependencies = [
-  "transformers[torch,sentencepiece]==4.37.2",  # ExtractiveReader, TransformersSimilarityRanker, LocalWhisperTranscriber, HFGenerators...
+  "transformers[torch,sentencepiece]==4.38.2",  # ExtractiveReader, TransformersSimilarityRanker, LocalWhisperTranscriber, HFGenerators...
+  "huggingface_hub>=0.22.0", # TGI Generators and TEI Embedders
   "spacy>=3.7,<3.8",  # NamedEntityExtractor
   "spacy-curated-transformers>=0.2,<=0.3",  # NamedEntityExtractor
   "en-core-web-trf @ https://github.com/explosion/spacy-models/releases/download/en_core_web_trf-3.7.3/en_core_web_trf-3.7.3-py3-none-any.whl",  # NamedEntityExtractor
 
   # Converters
   "pypdf",  # PyPDFConverter
   "markdown-it-py",  # MarkdownToDocument
```

### Comparing `haystack_ai-2.0.0rc1/PKG-INFO` & `haystack_ai-2.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.0.0rc1
+Version: 2.0.1rc1
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
@@ -38,15 +38,15 @@
 Requires-Dist: requests
 Requires-Dist: tenacity
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions>=4.7
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <a href="https://www.deepset.ai/haystack/"><img src="docs/img/banner_20.png" alt="Haystack"></a>
+  <a href="https://www.deepset.ai/haystack/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Haystack"></a>
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | CI/CD   | [![Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/haystack?branch=main)                                                        |
 | Docs    | [![Website](https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)](https://docs.haystack.deepset.ai)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | Package | [![PyPI](https://img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/farm-haystack?logo=python&logoColor=gold) [![GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml) |
 | Meta    | [![Discord](https://img.shields.io/discord/993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://twitter.com/haystack_ai)                                                                                                                                                                                                                                                                                                                                                                                        |
@@ -96,15 +96,15 @@
 -   Perform **semantic search** and retrieve documents according to meaning.
 -   Build applications that can make complex decisions making to answer complex queries: such as systems that can resolve complex customer queries, do knowledge search on many disconnected resources and so on.
 -   Scale to millions of docs using retrievers and production-scale components.
 -   Use **off-the-shelf models** or **fine-tune** them to your data.
 -   Use **user feedback** to evaluate, benchmark, and continuously improve your models.
 
 > [!TIP]
-><img src="docs/img/deepset-cloud-logo-lightblue.png"  width=30% height=30%>
+><img src="https://github.com/deepset-ai/haystack/raw/main/docs/img/deepset-cloud-logo-lightblue.png"  width=30% height=30%>
 >
 > Are you looking for a managed solution that benefits from Haystack? [deepset Cloud](https://www.deepset.ai/deepset-cloud?utm_campaign=developer-relations&utm_source=haystack&utm_medium=readme) is our fully managed, end-to-end platform to integrate LLMs with your data, which uses Haystack for the LLM pipelines architecture.
 
 ## Telemetry
 
 Haystack collects **anonymous** usage statistics of pipeline components. We receive an event every time these components are initialized. This way, we know which components are most relevant to our community.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haystack-ai Version: 2.0.0rc1 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.0.1rc1 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
@@ -93,49 +93,50 @@
 granular answers in your documents. - Perform **semantic search** and retrieve
 documents according to meaning. - Build applications that can make complex
 decisions making to answer complex queries: such as systems that can resolve
 complex customer queries, do knowledge search on many disconnected resources
 and so on. - Scale to millions of docs using retrievers and production-scale
 components. - Use **off-the-shelf models** or **fine-tune** them to your data.
 - Use **user feedback** to evaluate, benchmark, and continuously improve your
-models. > [!TIP] >[docs/img/deepset-cloud-logo-lightblue.png] > > Are you
-looking for a managed solution that benefits from Haystack? [deepset Cloud]
-(https://www.deepset.ai/deepset-cloud?utm_campaign=developer-
-relations&utm_source=haystack&utm_medium=readme) is our fully managed, end-to-
-end platform to integrate LLMs with your data, which uses Haystack for the LLM
-pipelines architecture. ## Telemetry Haystack collects **anonymous** usage
-statistics of pipeline components. We receive an event every time these
-components are initialized. This way, we know which components are most
-relevant to our community. Read more about telemetry in Haystack or how you can
-opt out in [Haystack docs](https://docs.haystack.deepset.ai/v2.0/docs/
-telemetry). ## ð Community If you have a feature request or a bug report,
-feel free to open an [issue in Github](https://github.com/deepset-ai/haystack/
-issues). We regularly check these and you can expect a quick response. If you'd
-like to discuss a topic, or get more general advice on how to make Haystack
-work for your project, you can start a thread in [Github Discussions](https://
-github.com/deepset-ai/haystack/discussions) or our [Discord channel](https://
-discord.gg/haystack). We also check [ð (Twitter)](https://twitter.com/
-haystack_ai) and [Stack Overflow](https://stackoverflow.com/questions/tagged/
-haystack). ## Contributing to Haystack We are very open to the community's
-contributions - be it a quick fix of a typo, or a completely new feature! You
-don't need to be a Haystack expert to provide meaningful improvements. To learn
-how to get started, check out our [Contributor Guidelines](https://github.com/
-deepset-ai/haystack/blob/main/CONTRIBUTING.md) first. There are several ways
-you can contribute to Haystack: - Contribute to the main Haystack project -
-Contribute an integration on [haystack-core-integrations](https://github.com/
-deepset-ai/haystack-core-integrations) > [!TIP] >ð **[Check out the full
-list of issues that are open to contributions](https://github.com/orgs/deepset-
-ai/projects/14)** ## Who Uses Haystack Here's a list of projects and companies
-using Haystack. Want to add yours? Open a PR, add it to the list and let the
-world know that you use Haystack! - [Airbus](https://www.airbus.com/en) -
-[Alcatel-Lucent](https://www.al-enterprise.com/) - [Apple](https://
-www.apple.com/) - [BetterUp](https://www.betterup.com/) - [Databricks](https://
-www.databricks.com/) - [Deepset](https://deepset.ai/) - [Etalab](https://
-www.deepset.ai/blog/improving-on-site-search-for-government-agencies-etalab) -
-[Infineon](https://www.infineon.com/) - [Intel](https://github.com/intel/open-
-domain-question-and-answer#readme) - [Intelijus](https://www.intelijus.ai/) -
-[Intel Labs](https://github.com/IntelLabs/fastRAG#readme) - [LEGO](https://
-github.com/larsbaunwall/bricky#readme) - [Netflix](https://netflix.com) -
-[Nvidia](https://developer.nvidia.com/blog/reducing-development-time-for-
-intelligent-virtual-assistants-in-contact-centers/) - [PostHog](https://
-github.com/PostHog/max-ai#readme) - [Rakuten](https://www.rakuten.com/) -
-[Sooth.ai](https://www.deepset.ai/blog/advanced-neural-search-with-sooth-ai)
+models. > [!TIP] >[https://github.com/deepset-ai/haystack/raw/main/docs/img/
+deepset-cloud-logo-lightblue.png] > > Are you looking for a managed solution
+that benefits from Haystack? [deepset Cloud](https://www.deepset.ai/deepset-
+cloud?utm_campaign=developer-relations&utm_source=haystack&utm_medium=readme)
+is our fully managed, end-to-end platform to integrate LLMs with your data,
+which uses Haystack for the LLM pipelines architecture. ## Telemetry Haystack
+collects **anonymous** usage statistics of pipeline components. We receive an
+event every time these components are initialized. This way, we know which
+components are most relevant to our community. Read more about telemetry in
+Haystack or how you can opt out in [Haystack docs](https://
+docs.haystack.deepset.ai/v2.0/docs/telemetry). ## ð Community If you have a
+feature request or a bug report, feel free to open an [issue in Github](https:/
+/github.com/deepset-ai/haystack/issues). We regularly check these and you can
+expect a quick response. If you'd like to discuss a topic, or get more general
+advice on how to make Haystack work for your project, you can start a thread in
+[Github Discussions](https://github.com/deepset-ai/haystack/discussions) or our
+[Discord channel](https://discord.gg/haystack). We also check [ð (Twitter)]
+(https://twitter.com/haystack_ai) and [Stack Overflow](https://
+stackoverflow.com/questions/tagged/haystack). ## Contributing to Haystack We
+are very open to the community's contributions - be it a quick fix of a typo,
+or a completely new feature! You don't need to be a Haystack expert to provide
+meaningful improvements. To learn how to get started, check out our
+[Contributor Guidelines](https://github.com/deepset-ai/haystack/blob/main/
+CONTRIBUTING.md) first. There are several ways you can contribute to Haystack:
+- Contribute to the main Haystack project - Contribute an integration on
+[haystack-core-integrations](https://github.com/deepset-ai/haystack-core-
+integrations) > [!TIP] >ð **[Check out the full list of issues that are open
+to contributions](https://github.com/orgs/deepset-ai/projects/14)** ## Who Uses
+Haystack Here's a list of projects and companies using Haystack. Want to add
+yours? Open a PR, add it to the list and let the world know that you use
+Haystack! - [Airbus](https://www.airbus.com/en) - [Alcatel-Lucent](https://
+www.al-enterprise.com/) - [Apple](https://www.apple.com/) - [BetterUp](https://
+www.betterup.com/) - [Databricks](https://www.databricks.com/) - [Deepset]
+(https://deepset.ai/) - [Etalab](https://www.deepset.ai/blog/improving-on-site-
+search-for-government-agencies-etalab) - [Infineon](https://www.infineon.com/
+) - [Intel](https://github.com/intel/open-domain-question-and-answer#readme) -
+[Intelijus](https://www.intelijus.ai/) - [Intel Labs](https://github.com/
+IntelLabs/fastRAG#readme) - [LEGO](https://github.com/larsbaunwall/
+bricky#readme) - [Netflix](https://netflix.com) - [Nvidia](https://
+developer.nvidia.com/blog/reducing-development-time-for-intelligent-virtual-
+assistants-in-contact-centers/) - [PostHog](https://github.com/PostHog/max-
+ai#readme) - [Rakuten](https://www.rakuten.com/) - [Sooth.ai](https://
+www.deepset.ai/blog/advanced-neural-search-with-sooth-ai)
```

