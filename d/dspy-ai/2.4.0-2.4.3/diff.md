# Comparing `tmp/dspy-ai-2.4.0.tar.gz` & `tmp/dspy-ai-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspy-ai-2.4.0.tar", last modified: Fri Mar  8 16:06:56 2024, max compression
+gzip compressed data, was "dist/dspy-ai-2.4.3.tar", last modified: Mon Apr  8 16:49:27 2024, max compression
```

## Comparing `dspy-ai-2.4.0.tar` & `dspy-ai-2.4.3.tar`

### file list

```diff
@@ -1,151 +1,164 @@
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.868605 dspy-ai-2.4.0/
--rw-r--r--   0 okhattab (19845) future   (20099)     1085 2023-12-17 18:54:52.000000 dspy-ai-2.4.0/LICENSE
--rw-r--r--   0 okhattab (19845) future   (20099)    35248 2024-03-08 16:06:56.867606 dspy-ai-2.4.0/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)    34398 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/README.md
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.583618 dspy-ai-2.4.0/dsp/
--rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.588618 dspy-ai-2.4.0/dsp/evaluation/
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dsp/evaluation/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/evaluation/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.634616 dspy-ai-2.4.0/dsp/modules/
--rw-r--r--   0 okhattab (19845) future   (20099)      416 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/aws_lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/azure_openai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/azurecognitivesearch.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3025 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/bedrock.py
--rw-r--r--   0 okhattab (19845) future   (20099)      964 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/cache_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/clarifai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/cohere.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/colbertv2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/databricks.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.639616 dspy-ai-2.4.0/dsp/modules/finetuning/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dsp/modules/finetuning/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/finetuning/finetune_hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/google.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/gpt3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6544 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/hf_client.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2087 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dsp/modules/hf_server.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3209 2024-03-02 23:17:54.000000 dspy-ai-2.4.0/dsp/modules/lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/ollama.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/modules/pyserini.py
--rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-03-02 23:17:54.000000 dspy-ai-2.4.0/dsp/modules/sbert.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-03-02 23:17:54.000000 dspy-ai-2.4.0/dsp/modules/sentence_vectorizer.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.655615 dspy-ai-2.4.0/dsp/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/primitives/compiler.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/primitives/demonstrate.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/primitives/inspect.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7948 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/primitives/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/primitives/primitives.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-03-02 23:17:54.000000 dspy-ai-2.4.0/dsp/primitives/search.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.665615 dspy-ai-2.4.0/dsp/templates/
--rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/templates/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/templates/template_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/templates/template_v3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/templates/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.681614 dspy-ai-2.4.0/dsp/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-03-02 23:17:55.000000 dspy-ai-2.4.0/dsp/utils/ann_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/utils/dpr.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/utils/metrics.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3287 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/utils/settings.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/utils/settings_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dsp/utils/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.683614 dspy-ai-2.4.0/dspy/
--rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.694614 dspy-ai-2.4.0/dspy/adapters/
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/adapters/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/adapters/basic_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/adapters/chatml_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/adapters/vicuna_adapter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.707613 dspy-ai-2.4.0/dspy/datasets/
--rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/datasets/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/datasets/colors.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/datasets/dataloader.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/datasets/dataset.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/datasets/gsm8k.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/datasets/hotpotqa.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.716612 dspy-ai-2.4.0/dspy/evaluate/
--rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/evaluate/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10075 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/evaluate/evaluate.py
--rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/evaluate/metrics.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.722612 dspy-ai-2.4.0/dspy/experimental/
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/experimental/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6845 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/experimental/synthesizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/experimental/synthetic_data.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.727612 dspy-ai-2.4.0/dspy/functional/
--rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/functional/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    18631 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/functional/functional.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.754611 dspy-ai-2.4.0/dspy/predict/
--rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/aggregation.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/chain_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/knn.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/langchain.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0 okhattab (19845) future   (20099)       58 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/predict/parameter.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/program_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/react.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/predict/retry.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.771610 dspy-ai-2.4.0/dspy/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/primitives/assertions.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7779 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/primitives/box.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-03-02 23:17:56.000000 dspy-ai-2.4.0/dspy/primitives/example.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2490 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/primitives/module.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/primitives/prediction.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/primitives/program.py
--rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/primitives/python_interpreter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.807608 dspy-ai-2.4.0/dspy/retrieve/
--rw-r--r--   0 okhattab (19845) future   (20099)       30 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/retrieve/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4588 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-03-02 23:17:57.000000 dspy-ai-2.4.0/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5825 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/databricks_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/deeplake_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6617 2024-02-26 16:17:11.000000 dspy-ai-2.4.0/dspy/retrieve/faiss_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3454 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/marqo_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/retrieve.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/vectara_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-01-31 22:17:45.000000 dspy-ai-2.4.0/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/retrieve/you_rm.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.814608 dspy-ai-2.4.0/dspy/signatures/
--rw-r--r--   0 okhattab (19845) future   (20099)       46 2023-12-17 18:55:00.000000 dspy-ai-2.4.0/dspy/signatures/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2556 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/signatures/field.py
--rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/signatures/signature.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.847607 dspy-ai-2.4.0/dspy/teleprompt/
--rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/dspy/teleprompt/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9384 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/teleprompt/bootstrap.py
--rw-r--r--   0 okhattab (19845) future   (20099)    17283 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1385 2024-03-02 23:17:58.000000 dspy-ai-2.4.0/dspy/teleprompt/ensemble.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6211 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/teleprompt/finetune.py
--rw-r--r--   0 okhattab (19845) future   (20099)      807 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0 okhattab (19845) future   (20099)    29365 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7923 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/teleprompt/random_search.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2578 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/dspy/teleprompt/signature_opt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3280 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11790 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0 okhattab (19845) future   (20099)       60 2024-03-02 23:17:59.000000 dspy-ai-2.4.0/dspy/teleprompt/teleprompt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3097 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0 okhattab (19845) future   (20099)      950 2024-03-02 23:17:59.000000 dspy-ai-2.4.0/dspy/teleprompt/vanilla.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.852606 dspy-ai-2.4.0/dspy/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-03-02 22:57:11.000000 dspy-ai-2.4.0/dspy/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-03-08 15:43:30.000000 dspy-ai-2.4.0/dspy/utils/dummies.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-03-08 16:06:56.864606 dspy-ai-2.4.0/dspy_ai.egg-info/
--rw-r--r--   0 okhattab (19845) future   (20099)    35248 2024-03-08 16:06:56.000000 dspy-ai-2.4.0/dspy_ai.egg-info/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)     3470 2024-03-08 16:06:56.000000 dspy-ai-2.4.0/dspy_ai.egg-info/SOURCES.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-03-08 16:06:56.000000 dspy-ai-2.4.0/dspy_ai.egg-info/dependency_links.txt
--rw-r--r--   0 okhattab (19845) future   (20099)      604 2024-03-08 16:06:56.000000 dspy-ai-2.4.0/dspy_ai.egg-info/requires.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-03-08 16:06:56.000000 dspy-ai-2.4.0/dspy_ai.egg-info/top_level.txt
--rw-r--r--   0 okhattab (19845) future   (20099)     6499 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/pyproject.toml
--rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-03-08 16:06:56.868605 dspy-ai-2.4.0/setup.cfg
--rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-03-08 16:06:54.000000 dspy-ai-2.4.0/setup.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.3/LICENSE
+-rw-r--r--   0 okhattab (19845) future   (20099)    35537 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)    34661 2024-04-08 16:37:16.000000 dspy-ai-2.4.3/README.md
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/evaluation/
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/evaluation/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/evaluation/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/modules/
+-rw-r--r--   0 okhattab (19845) future   (20099)      497 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4516 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/anthropic.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6803 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/aws_lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9539 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/azure_openai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3135 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/azurecognitivesearch.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3195 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/bedrock.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1018 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/cache_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/clarifai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3214 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/cohere.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/colbertv2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5278 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/databricks.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/modules/finetuning/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/finetuning/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/finetuning/finetune_hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/google.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8610 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/gpt3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5023 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/groq_client.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15430 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/hf_client.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/hf_server.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3601 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3655 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/mistral.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/ollama.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/pyserini.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/sbert.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/sentence_vectorizer.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/compiler.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/demonstrate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/inspect.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8432 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/primitives.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2727 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/search.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/templates/
+-rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/template_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/template_v3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/ann_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/dpr.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/metrics.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3285 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/settings.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/settings_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/
+-rw-r--r--   0 okhattab (19845) future   (20099)      891 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/adapters/
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/basic_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/chatml_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/llamachat_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/vicuna_adapter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/datasets/
+-rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/colors.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4949 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/dataloader.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/dataset.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/gsm8k.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/hotpotqa.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/evaluate/
+-rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/evaluate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/metrics.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/experimental/
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9723 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4237 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthetic_data.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/functional/
+-rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/functional/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    18768 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/functional/functional.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/predict/
+-rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/aggregation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/chain_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/knn.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/langchain.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/parameter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5583 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7603 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/program_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/react.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2827 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/retry.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/assertions.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/box.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/example.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/module.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/prediction.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/program.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/python_interpreter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/retrieve/
+-rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9126 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/azureaisearch_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4812 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3275 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3897 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0 okhattab (19845) future   (20099)     6548 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5930 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3264 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2425 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/ragatouille_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1442 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/retrieve.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4491 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/you_rm.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/signatures/
+-rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/signatures/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/signatures/field.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    14464 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/signatures/signature.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/teleprompt/
+-rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/ensemble.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/finetune.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/random_search.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/vanilla.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/utils/dummies.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3378 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/utils/logging.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy_ai.egg-info/
+-rw-r--r--   0 okhattab (19845) future   (20099)    35537 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)     3890 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)      664 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/requires.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/top_level.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)     7129 2024-04-08 16:38:10.000000 dspy-ai-2.4.3/pyproject.toml
+-rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/setup.cfg
+-rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 16:38:10.000000 dspy-ai-2.4.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dspy-ai-2.4.0/LICENSE` & `dspy-ai-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/PKG-INFO` & `dspy-ai-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.0
+Version: 2.4.3
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,15 @@
 Provides-Extra: chromadb
 Provides-Extra: qdrant
 Provides-Extra: marqo
 Provides-Extra: mongodb
 Provides-Extra: pinecone
 Provides-Extra: weaviate
 Provides-Extra: faiss-cpu
+Provides-Extra: anthropic
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
@@ -57,15 +58,16 @@
 
 If you need help thinking about your task, we recently created a [Discord server](https://discord.gg/VzS6RHHK6F) for the community.
 
 1. **[Installation](#1-installation)**
 1. **[Tutorials & Documentation](#2-documentation)**
 1. **[Framework Syntax](#3-syntax-youre-in-charge-of-the-workflowits-free-form-python-code)**
 1. **[Compiling: Two Powerful Concepts](#4-two-powerful-concepts-signatures--teleprompters)**
-1. **[FAQ: Is DSPy right for me?](#5-faq-is-dspy-right-for-me)**
+1. **[Pydantic Types](#5-pydantic-types)** 
+1. **[FAQ: Is DSPy right for me?](#6-faq-is-dspy-right-for-me)**
 
 
 
 ### Analogy to Neural Networks
 
 When we build neural networks, we don't write manual _for-loops_ over lists of _hand-tuned_ floats. Instead, you might use a framework like [PyTorch](https://pytorch.org/) to compose declarative layers (e.g., `Convolution` or `Dropout`) and then use optimizers (e.g., SGD or Adam) to learn the parameters of the network.
 
@@ -120,14 +122,15 @@
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
 - Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
+- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
```

### Comparing `dspy-ai-2.4.0/README.md` & `dspy-ai-2.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
 If you need help thinking about your task, we recently created a [Discord server](https://discord.gg/VzS6RHHK6F) for the community.
 
 1. **[Installation](#1-installation)**
 1. **[Tutorials & Documentation](#2-documentation)**
 1. **[Framework Syntax](#3-syntax-youre-in-charge-of-the-workflowits-free-form-python-code)**
 1. **[Compiling: Two Powerful Concepts](#4-two-powerful-concepts-signatures--teleprompters)**
-1. **[FAQ: Is DSPy right for me?](#5-faq-is-dspy-right-for-me)**
+1. **[Pydantic Types](#5-pydantic-types)** 
+1. **[FAQ: Is DSPy right for me?](#6-faq-is-dspy-right-for-me)**
 
 
 
 ### Analogy to Neural Networks
 
 When we build neural networks, we don't write manual _for-loops_ over lists of _hand-tuned_ floats. Instead, you might use a framework like [PyTorch](https://pytorch.org/) to compose declarative layers (e.g., `Convolution` or `Dropout`) and then use optimizers (e.g., SGD or Adam) to learn the parameters of the network.
 
@@ -92,14 +93,15 @@
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
 - Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
+- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
```

### Comparing `dspy-ai-2.4.0/dsp/__init__.py` & `dspy-ai-2.4.3/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/evaluation/utils.py` & `dspy-ai-2.4.3/dsp/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/aws_lm.py` & `dspy-ai-2.4.3/dsp/modules/aws_lm.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 import json
 import logging
 from abc import abstractmethod
-from typing import Any, Literal
+from typing import Any, Literal, Optional
 
 from dsp.modules.lm import LM
 
 # Heuristic translating number of chars to tokens
 # ~4 chars = 1 token
 CHARS2TOKENS: int = 4
 
@@ -23,14 +23,15 @@
 
     def __init__(
         self,
         model: str,
         region_name: str,
         service_name: str,
         max_new_tokens: int,
+        profile_name: Optional[str] = None,
         truncate_long_prompts: bool = False,
         input_output_ratio: int = 3,
         batch_n: bool = True,
     ) -> None:
         """_summary_
 
         Args:
@@ -51,15 +52,20 @@
         self._max_new_tokens: int = max_new_tokens
         self._model_name: str = model
         self._truncate_long_prompt_prompts: bool = truncate_long_prompts
         self._batch_n: bool = batch_n
 
         import boto3
 
-        self.predictor = boto3.client(service_name, region_name=region_name)
+        if profile_name is None:
+            self.predictor = boto3.client(service_name, region_name=region_name)
+        else:
+            self.predictor = boto3.Session(profile_name=profile_name).client(
+                service_name, region_name=region_name,
+            )
 
     @abstractmethod
     def _create_body(self, prompt: str, **kwargs):
         pass
 
     def _sanitize_kwargs(self, query_kwargs: dict[str, Any]) -> dict[str, Any]:
         """Ensure that input kwargs can be used by Bedrock or Sagemaker."""
```

### Comparing `dspy-ai-2.4.0/dsp/modules/azure_openai.py` & `dspy-ai-2.4.3/dsp/modules/azure_openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-import logging
-
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[logging.FileHandler("azure_openai_usage.log")],
-)
-
 import functools
 import json
+import logging
 from typing import Any, Literal, Optional, cast
 
 import backoff
 import openai
 
 import dsp
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
@@ -112,14 +104,18 @@
             "top_p": 1,
             "frequency_penalty": 0,
             "presence_penalty": 0,
             "n": 1,
             **kwargs,
         }  # TODO: add kwargs above for </s>
 
+        self.api_base = api_base
+        self.api_version = api_version
+        self.api_key = api_key
+
         self.history: list[dict[str, Any]] = []
 
     def _openai_client(self):
         if OPENAI_LEGACY:
             return openai
 
         return self.client
@@ -223,14 +219,27 @@
                 avglog = sum(logprobs) / len(logprobs)
                 scored_completions.append((avglog, self._get_choice_text(c)))
 
             scored_completions = sorted(scored_completions, reverse=True)
             completions = [c for _, c in scored_completions]
 
         return completions
+    
+    def copy(self, **kwargs):
+        """Returns a copy of the language model with the same parameters."""
+        kwargs = {**self.kwargs, **kwargs}
+        model = kwargs.pop("model")
+
+        return self.__class__(
+            model=model, 
+            api_key=self.api_key, 
+            api_version=self.api_version, 
+            api_base=self.api_base, 
+            **kwargs,
+        )
 
 
 @CacheMemory.cache
 def cached_gpt3_request_v2(**kwargs):
     return openai.Completion.create(**kwargs)
```

### Comparing `dspy-ai-2.4.0/dsp/modules/azurecognitivesearch.py` & `dspy-ai-2.4.3/dsp/modules/azurecognitivesearch.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     from azure.search.documents._paging import SearchItemPaged
 except ImportError:
     raise ImportError(
         "You need to install azure-search-documents library"
         "Please use the command: pip install azure-search-documents",
     )
 
+# Deprecated: This module is scheduled for removal in future releases.
+# Please use the AzureAISearchRM class from dspy.retrieve.azureaisearch_rm instead.
+# For more information, refer to the updated documentation.
+
 class AzureCognitiveSearch:
     """Wrapper for the Azure Cognitive Search Retrieval."""
 
     def __init__(
         self,
         search_service_name: str,
         search_api_key: str,
@@ -33,17 +37,20 @@
         # Create a client
         self.credential = AzureKeyCredential(self.search_api_key)
         self.client = SearchClient(endpoint=self.endpoint,
                         index_name=self.search_index_name,
                         credential=self.credential)
 
     def __call__(self, query: str, k: int = 10) -> Union[list[str], list[dotdict]]:
-        
+        print("""# Deprecated: This module is scheduled for removal in future releases.
+                Please use the AzureAISearchRM class from dspy.retrieve.azureaisearch_rm instead.
+                For more information, refer to the updated documentation.""")
+
         topk: list[dict[str, Any]] = azure_search_request(self.field_text, self.field_score, self.client, query, k)
-        topk = [{**d, "long_text": d["text"]} for d in topk]            
+        topk = [{**d, "long_text": d["text"]} for d in topk]
 
         return [dotdict(psg) for psg in topk]
 
 def azure_search_request(key_content: str, key_score: str,  client: SearchClient, query: str, top: int =1):
     '''
     Search in Azure Cognitive Search Index
     '''
@@ -61,10 +68,10 @@
         tmp = {}
         for key, value in result.items():
             if(key == content_key):
                 tmp["text"] = value # assign content
             elif(key == content_score):
                 tmp["score"] = value
             else:
-                tmp[key] = value            
+                tmp[key] = value
         res.append(tmp)
-    return res 
+    return res
```

### Comparing `dspy-ai-2.4.0/dsp/modules/bedrock.py` & `dspy-ai-2.4.3/dsp/modules/bedrock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import json
-from typing import Any
+from typing import Any, Optional
 
 from dsp.modules.aws_lm import AWSLM
 
 
 class Bedrock(AWSLM):
     def __init__(
         self,
         region_name: str,
         model: str,
+        profile_name: Optional[str] = None,
         input_output_ratio: int = 3,
         max_new_tokens: int = 1500,
     ) -> None:
         """Use an AWS Bedrock language model.
         NOTE: You must first configure your AWS credentials with the AWS CLI before using this model!
 
         Args:
@@ -24,20 +25,22 @@
             input_output_ratio (int, optional): The rough size of the number of input tokens to output tokens in the worst case. Defaults to 3.
             max_new_tokens (int, optional): The maximum number of tokens to be sampled from the LM.
         """
         super().__init__(
             model=model,
             service_name="bedrock-runtime",
             region_name=region_name,
+            profile_name=profile_name,
             truncate_long_prompts=False,
             input_output_ratio=input_output_ratio,
             max_new_tokens=max_new_tokens,
             batch_n=True,  # Bedrock does not support the `n` parameter
         )
         self._validate_model(model)
+        self.provider = "claude" if "claude" in model.lower() else "bedrock"
 
     def _validate_model(self, model: str) -> None:
         if "claude" not in model.lower():
             raise NotImplementedError("Only claude models are supported as of now")
 
     def _create_body(self, prompt: str, **kwargs) -> dict[str, str | float]:
         base_args: dict[str, Any] = {
```

### Comparing `dspy-ai-2.4.0/dsp/modules/cache_utils.py` & `dspy-ai-2.4.3/dsp/modules/cache_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import wraps
 from pathlib import Path
 
 from joblib import Memory
 
 from dsp.utils import dotdict
 
-cache_turn_on = True
+cache_turn_on = os.environ.get('DSP_CACHEBOOL', 'True').lower() != 'false'
 
 
 def noop_decorator(arg=None, *noop_args, **noop_kwargs):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
```

### Comparing `dspy-ai-2.4.0/dsp/modules/clarifai.py` & `dspy-ai-2.4.3/dsp/modules/clarifai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/cohere.py` & `dspy-ai-2.4.3/dsp/modules/mistral.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import math
 from typing import Any, Optional
 
 import backoff
 
 from dsp.modules.lm import LM
 
 try:
-    import cohere
-    cohere_api_error = cohere.CohereAPIError
+    import mistralai
+    from mistralai.client import MistralClient
+    from mistralai.exceptions import MistralAPIException
+    from mistralai.models.chat_completion import ChatCompletionResponse, ChatMessage
+    mistralai_api_error = MistralAPIException
 except ImportError:
-    cohere_api_error = Exception
-    # print("Not loading Cohere because it is not installed.")
+    mistralai_api_error = Exception
 
 
 def backoff_hdlr(details):
     """Handler from https://pypi.org/project/backoff/"""
     print(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with kwargs "
@@ -25,121 +26,104 @@
 def giveup_hdlr(details):
     """wrapper function that decides when to give up on retry"""
     if "rate limits" in details.message:
         return False
     return True
 
 
-class Cohere(LM):
-    """Wrapper around Cohere's API.
+class Mistral(LM):
+    """Wrapper around Mistral AI's API.
 
-    Currently supported models include `command`, `command-nightly`, `command-light`, `command-light-nightly`.
+    Currently supported models include `mistral-small-latest`, `mistral-medium-latest`, `mistral-large-latest`.
     """
 
     def __init__(
         self,
-        model: str = "command-nightly",
+        model: str = "mistral-medium-latest",
         api_key: Optional[str] = None,
-        stop_sequences: list[str] = [],
         **kwargs,
     ):
         """
         Parameters
         ----------
         model : str
-            Which pre-trained model from Cohere to use?
-            Choices are [`command`, `command-nightly`, `command-light`, `command-light-nightly`]
+            Which pre-trained model from Mistral AI to use?
+            Choices are [`mistral-small-latest`, `mistral-medium-latest`, `mistral-large-latest`]
         api_key : str
-            The API key for Cohere.
-            It can be obtained from https://dashboard.cohere.ai/register.
-        stop_sequences : list of str
-            Additional stop tokens to end generation.
+            The API key for Mistral AI.
         **kwargs: dict
             Additional arguments to pass to the API provider.
         """
         super().__init__(model)
-        self.co = cohere.Client(api_key)
-        self.provider = "cohere"
+
+        if mistralai_api_error == Exception:
+            raise ImportError("Not loading Mistral AI because it is not installed. Install it with `pip install mistralai`.")
+
+        self.client = MistralClient(api_key=api_key)
+
+        self.provider = "mistral"
         self.kwargs = {
             "model": model,
-            "temperature": 0.0,
+            "temperature": 0.17,
             "max_tokens": 150,
-            "p": 1,
-            "frequency_penalty": 0,
-            "presence_penalty": 0,
-            "num_generations": 1,
             **kwargs,
         }
-        self.stop_sequences = stop_sequences
-        self.max_num_generations = 5
 
         self.history: list[dict[str, Any]] = []
 
     def basic_request(self, prompt: str, **kwargs):
+        """Basic request to Mistral AI's API."""
         raw_kwargs = kwargs
         kwargs = {
             **self.kwargs,
-            "stop_sequences": self.stop_sequences,
-            "prompt": prompt,
+            "messages": [ChatMessage(role="user", content=prompt)],
             **kwargs,
         }
-        response = self.co.generate(**kwargs)
+
+        # Mistral disallows "n" arguments
+        n = kwargs.pop("n", None)
+        if n is not None and n > 1 and kwargs['temperature'] == 0.0:
+            kwargs['temperature'] = 0.7
+
+        response = self.client.chat(**kwargs)
 
         history = {
             "prompt": prompt,
             "response": response,
             "kwargs": kwargs,
             "raw_kwargs": raw_kwargs,
         }
         self.history.append(history)
 
         return response
 
     @backoff.on_exception(
         backoff.expo,
-        (cohere_api_error),
+        (mistralai_api_error),
         max_time=1000,
         on_backoff=backoff_hdlr,
         giveup=giveup_hdlr,
     )
     def request(self, prompt: str, **kwargs):
-        """Handles retrieval of completions from Cohere whilst handling API errors"""
+        """Handles retrieval of completions from Mistral AI whilst handling API errors."""
+        prompt = prompt + "Follow the format only once !"
         return self.basic_request(prompt, **kwargs)
 
     def __call__(
         self,
         prompt: str,
         only_completed: bool = True,
         return_sorted: bool = False,
         **kwargs,
     ):
+
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
 
-        # Cohere uses 'num_generations' whereas dsp.generate() uses 'n'
         n = kwargs.pop("n", 1)
 
-        # Cohere can generate upto self.max_num_generations completions at a time
-        choices = []
-        num_iters = math.ceil(n / self.max_num_generations)
-        remainder = n % self.max_num_generations
-        for i in range(num_iters):
-            if i == (num_iters - 1):
-                kwargs["num_generations"] = (
-                    remainder if remainder != 0 else self.max_num_generations
-                )
-            else:
-                kwargs["num_generations"] = self.max_num_generations
+        completions = []
+        for _ in range(n):
             response = self.request(prompt, **kwargs)
-            choices.extend(response.generations)
-        completions = [c.text for c in choices]
-
-        if return_sorted and kwargs.get("num_generations", 1) > 1:
-            scored_completions = []
-
-            for c in choices:
-                scored_completions.append((c.likelihood, c.text))
-
-            scored_completions = sorted(scored_completions, reverse=True)
-            completions = [c for _, c in scored_completions]
+            completions.append(response.choices[0].message.content)
 
         return completions
```

### Comparing `dspy-ai-2.4.0/dsp/modules/colbertv2.py` & `dspy-ai-2.4.3/dsp/modules/colbertv2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/databricks.py` & `dspy-ai-2.4.3/dsp/modules/databricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-import logging
-
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(message)s',
-    handlers=[
-        logging.FileHandler('openai_usage.log'),
-    ],
-)
-
 import functools
 import json
 from typing import Literal, Optional
 
 import openai
 
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
```

### Comparing `dspy-ai-2.4.0/dsp/modules/finetuning/finetune_hf.py` & `dspy-ai-2.4.3/dsp/modules/finetuning/finetune_hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/google.py` & `dspy-ai-2.4.3/dsp/modules/google.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/gpt3.py` & `dspy-ai-2.4.3/dsp/modules/gpt3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-import logging
-
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[logging.FileHandler("openai_usage.log")],
-)
-
 import functools
 import json
+import logging
 from typing import Any, Literal, Optional, cast
 
 import backoff
 import openai
 
 import dsp
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
@@ -58,20 +50,23 @@
     def __init__(
         self,
         model: str = "gpt-3.5-turbo-instruct",
         api_key: Optional[str] = None,
         api_provider: Literal["openai"] = "openai",
         api_base: Optional[str] = None,
         model_type: Literal["chat", "text"] = None,
+        system_prompt: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(model)
         self.provider = "openai"
         openai.api_type = api_provider
 
+        self.system_prompt = system_prompt
+
         assert (
             api_provider != "azure"
         ), "Azure functionality with base OpenAI has been deprecated, please use dspy.AzureOpenAI instead."
 
         default_model_type = (
             "chat"
             if ("gpt-3.5" in model or "turbo" in model or "gpt-4" in model)
@@ -114,15 +109,18 @@
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
 
         kwargs = {**self.kwargs, **kwargs}
         if self.model_type == "chat":
             # caching mechanism requires hashable kwargs
-            kwargs["messages"] = [{"role": "user", "content": prompt}]
+            messages = [{"role": "user", "content": prompt}]
+            if self.system_prompt:
+                messages.insert(0, {"role": "system", "content": self.system_prompt})
+            kwargs["messages"] = messages
             kwargs = {"stringify_request": json.dumps(kwargs)}
             response = chat_request(**kwargs)
 
         else:
             kwargs["prompt"] = prompt
             response = completions_request(**kwargs)
```

### Comparing `dspy-ai-2.4.0/dsp/modules/hf.py` & `dspy-ai-2.4.3/dsp/modules/hf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # from peft import PeftConfig, PeftModel
 # from transformers import AutoModelForSeq2SeqLM, AutoModelForCausalLM, AutoTokenizer, AutoConfig
+import os
 from typing import Literal, Optional
 
 from dsp.modules.lm import LM
 
 # from dsp.modules.finetuning.finetune_hf import preprocess_prompt
 
+
 def openai_to_hf(**kwargs):
     hf_kwargs = {}
     for k, v in kwargs.items():
         if k == "n":
             hf_kwargs["num_return_sequences"] = v
         elif k == "frequency_penalty":
             hf_kwargs["repetition_penalty"] = 1.0 - v
@@ -22,74 +24,117 @@
         else:
             hf_kwargs[k] = v
 
     return hf_kwargs
 
 
 class HFModel(LM):
-    def __init__(self, model: str, checkpoint: Optional[str] = None, is_client: bool = False,
-                 hf_device_map: Literal["auto", "balanced", "balanced_low_0", "sequential"] = "auto"):
+    def __init__(
+        self,
+        model: str,
+        checkpoint: Optional[str] = None,
+        is_client: bool = False,
+        hf_device_map: Literal[
+            "auto",
+            "balanced",
+            "balanced_low_0",
+            "sequential",
+        ] = "auto",
+        token: Optional[str] = None,
+    ):
         """wrapper for Hugging Face models
 
         Args:
             model (str): HF model identifier to load and use
             checkpoint (str, optional): load specific checkpoints of the model. Defaults to None.
             is_client (bool, optional): whether to access models via client. Defaults to False.
             hf_device_map (str, optional): HF config strategy to load the model.
                 Recommeded to use "auto", which will help loading large models using accelerate. Defaults to "auto".
         """
 
         super().__init__(model)
         self.provider = "hf"
         self.is_client = is_client
         self.device_map = hf_device_map
+
+        hf_autoconfig_kwargs = dict(token=token or os.environ.get("HF_TOKEN"))
+        hf_autotokenizer_kwargs = hf_autoconfig_kwargs.copy()
+        hf_automodel_kwargs = hf_autoconfig_kwargs.copy()
         if not self.is_client:
             try:
                 import torch
                 from transformers import AutoConfig, AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
             except ImportError as exc:
                 raise ModuleNotFoundError(
                     "You need to install Hugging Face transformers library to use HF models.",
                 ) from exc
             self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
             try:
-                architecture = AutoConfig.from_pretrained(model).__dict__["architectures"][0]
-                self.encoder_decoder_model = ("ConditionalGeneration" in architecture) or ("T5WithLMHeadModel" in architecture)
+                architecture = AutoConfig.from_pretrained(
+                    model,
+                    **hf_autoconfig_kwargs,
+                ).__dict__["architectures"][0]
+                self.encoder_decoder_model = ("ConditionalGeneration" in architecture) or (
+                    "T5WithLMHeadModel" in architecture
+                )
                 self.decoder_only_model = ("CausalLM" in architecture) or ("GPT2LMHeadModel" in architecture)
-                assert self.encoder_decoder_model or self.decoder_only_model, f"Unknown HuggingFace model class: {model}"
-                self.tokenizer = AutoTokenizer.from_pretrained(model if checkpoint is None else checkpoint)
+                assert (
+                    self.encoder_decoder_model or self.decoder_only_model
+                ), f"Unknown HuggingFace model class: {model}"
+                self.tokenizer = AutoTokenizer.from_pretrained(
+                    model if checkpoint is None else checkpoint,
+                    **hf_autotokenizer_kwargs,
+                )
 
                 self.rationale = True
                 AutoModelClass = AutoModelForSeq2SeqLM if self.encoder_decoder_model else AutoModelForCausalLM
                 if checkpoint:
                     # with open(os.path.join(checkpoint, '..', 'compiler_config.json'), 'r') as f:
                     #     config = json.load(f)
-                    self.rationale = False #config['rationale']
+                    self.rationale = False  # config['rationale']
                     # if config['peft']:
                     #     peft_config = PeftConfig.from_pretrained(checkpoint)
                     #     self.model = AutoModelClass.from_pretrained(peft_config.base_model_name_or_path, return_dict=True, load_in_8bit=True, device_map=hf_device_map)
                     #     self.model = PeftModel.from_pretrained(self.model, checkpoint)
                     # else:
                     if self.device_map:
-                        self.model = AutoModelClass.from_pretrained(checkpoint, device_map=self.device_map)
+                        self.model = AutoModelClass.from_pretrained(
+                            checkpoint,
+                            device_map=self.device_map,
+                            **hf_automodel_kwargs,
+                        )
                     else:
-                        self.model = AutoModelClass.from_pretrained(checkpoint).to(self.device)
+                        self.model = AutoModelClass.from_pretrained(
+                            checkpoint,
+                            **hf_automodel_kwargs,
+                        ).to(self.device)
                 else:
                     if self.device_map:
-                        self.model = AutoModelClass.from_pretrained(model, device_map=self.device_map)
+                        self.model = AutoModelClass.from_pretrained(
+                            model,
+                            device_map=self.device_map,
+                            **hf_automodel_kwargs,
+                        )
                     else:
-                        self.model = AutoModelClass.from_pretrained(model).to(self.device)
+                        self.model = AutoModelClass.from_pretrained(
+                            model,
+                            **hf_automodel_kwargs,
+                        ).to(self.device)
                 self.drop_prompt_from_output = False
             except ValueError:
                 self.model = AutoModelForCausalLM.from_pretrained(
                     model if checkpoint is None else checkpoint,
                     device_map=self.device_map,
+                    **hf_automodel_kwargs,
                 )
                 self.drop_prompt_from_output = True
-                self.tokenizer = AutoTokenizer.from_pretrained(model)
+                self.tokenizer = AutoTokenizer.from_pretrained(
+                    model,
+                    **hf_autotokenizer_kwargs,
+                )
                 self.drop_prompt_from_output = True
         self.history = []
 
     def basic_request(self, prompt, **kwargs):
         raw_kwargs = kwargs
         kwargs = {**self.kwargs, **kwargs}
         response = self._generate(prompt, **kwargs)
@@ -107,28 +152,25 @@
     def _generate(self, prompt, **kwargs):
         assert not self.is_client
         # TODO: Add caching
         kwargs = {**openai_to_hf(**self.kwargs), **openai_to_hf(**kwargs)}
         # print(prompt)
         if isinstance(prompt, dict):
             try:
-                prompt = prompt['messages'][0]['content']
+                prompt = prompt["messages"][0]["content"]
             except (KeyError, IndexError, TypeError):
                 print("Failed to extract 'content' from the prompt.")
         inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
 
         # print(kwargs)
         outputs = self.model.generate(**inputs, **kwargs)
         if self.drop_prompt_from_output:
             input_length = inputs.input_ids.shape[1]
             outputs = outputs[:, input_length:]
-        completions = [
-            {"text": c}
-            for c in self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
-        ]
+        completions = [{"text": c} for c in self.tokenizer.batch_decode(outputs, skip_special_tokens=True)]
         response = {
             "prompt": prompt,
             "choices": completions,
         }
         return response
 
     def __call__(self, prompt, only_completed=True, return_sorted=False, **kwargs):
```

### Comparing `dspy-ai-2.4.0/dsp/modules/hf_client.py` & `dspy-ai-2.4.3/dsp/modules/hf_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,29 +112,44 @@
 def send_hftgi_request_v00(arg, **kwargs):
     return requests.post(arg, **kwargs)
 
 
 class HFClientVLLM(HFModel):
     def __init__(self, model, port, url="http://localhost", **kwargs):
         super().__init__(model=model, is_client=True)
-        self.url = f"{url}:{port}"
+
+        if isinstance(url, list):
+            self.urls = url
+        
+        elif isinstance(url, str):
+            self.urls = [f'{url}:{port}']
+        
+        else:
+            raise ValueError(f"The url provided to `HFClientVLLM` is neither a string nor a list of strings. It is of type {type(url)}.")
+        
         self.headers = {"Content-Type": "application/json"}
+        self.kwargs |= kwargs
+
 
     def _generate(self, prompt, **kwargs):
         kwargs = {**self.kwargs, **kwargs}
 
         payload = {
-            "model": kwargs["model"],
+            "model": self.kwargs["model"],
             "prompt": prompt,
-            "max_tokens": kwargs["max_tokens"],
-            "temperature": kwargs["temperature"],
+            **kwargs,
         }
 
+        
+        # Round robin the urls.
+        url = self.urls.pop(0)
+        self.urls.append(url)
+
         response = send_hfvllm_request_v00(
-            f"{self.url}/v1/completions",
+            f"{url}/v1/completions",
             json=payload,
             headers=self.headers,
         )
 
         try:
             json_response = response.json()
             completions = json_response["choices"]
@@ -416,8 +431,8 @@
         except Exception:
             print("Failed to parse JSON response:", response.text)
             raise Exception("Received invalid JSON response from server")
 
 
 @CacheMemory.cache
 def send_hfsglang_request_v00(arg, **kwargs):
-    return requests.post(arg, **kwargs)
+    return requests.post(arg, **kwargs)
```

### Comparing `dspy-ai-2.4.0/dsp/modules/hf_server.py` & `dspy-ai-2.4.3/dsp/modules/hf_server.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/lm.py` & `dspy-ai-2.4.3/dsp/modules/lm.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,83 +22,89 @@
     def basic_request(self, prompt, **kwargs):
         pass
 
     def request(self, prompt, **kwargs):
         return self.basic_request(prompt, **kwargs)
 
     def print_green(self, text: str, end: str = "\n"):
-        print("\x1b[32m" + str(text) + "\x1b[0m", end=end)
+        return "\x1b[32m" + str(text) + "\x1b[0m" + end
 
     def print_red(self, text: str, end: str = "\n"):
-        print("\x1b[31m" + str(text) + "\x1b[0m", end=end)
+        return "\x1b[31m" + str(text) + "\x1b[0m" + end
 
     def inspect_history(self, n: int = 1, skip: int = 0):
         """Prints the last n prompts and their completions.
-        TODO: print the valid choice that contains filled output field instead of the first
+
+        TODO: print the valid choice that contains filled output field instead of the first.
         """
         provider: str = self.provider
 
         last_prompt = None
         printed = []
         n = n + skip
 
         for x in reversed(self.history[-100:]):
             prompt = x["prompt"]
 
             if prompt != last_prompt:
-
                 if provider == "clarifai" or provider == "google":
-                    printed.append(
-                        (
-                            prompt,
-                            x['response'],
-                        ),
-                    )
+                    printed.append((prompt, x["response"]))
+                elif provider == "anthropic":
+                    blocks = [{"text": block.text} for block in x["response"].content if block.type == "text"]
+                    printed.append((prompt, blocks))
+                elif provider == "cohere":
+                    printed.append((prompt, x["response"].text))
+                elif provider == "mistral":
+                    printed.append((prompt, x['response'].choices))
                 else:
-                    printed.append(
-                        (
-                            prompt,
-                            x["response"].generations
-                            if provider == "cohere"
-                            else x["response"]["choices"],
-                        ),
-                    )
+                    printed.append((prompt, x["response"]["choices"]))
 
             last_prompt = prompt
 
             if len(printed) >= n:
                 break
 
         for idx, (prompt, choices) in enumerate(reversed(printed)):
+            printing_value = ""
+
             # skip the first `skip` prompts
             if (n - idx - 1) < skip:
                 continue
 
-            print("\n\n\n")
-            print(prompt, end="")
+            printing_value += "\n\n\n"
+            printing_value += prompt
+
             text = ""
             if provider == "cohere":
-                text = choices[0].text
+                text = choices
             elif provider == "openai" or provider == "ollama":
                 text = ' ' + self._get_choice_text(choices[0]).strip()
-            elif provider == "clarifai":
+            elif provider == "clarifai" or provider == "claude" :
                 text=choices
+            elif provider == "groq":
+                text = ' ' + choices
             elif provider == "google":
                 text = choices[0].parts[0].text
+            elif provider == "mistral":
+                text = choices[0].message.content
             else:
                 text = choices[0]["text"]
-            self.print_green(text, end="")
+            printing_value += self.print_green(text, end="")
 
             if len(choices) > 1:
-                self.print_red(f" \t (and {len(choices)-1} other completions)", end="")
-            print("\n\n\n")
+                printing_value += self.print_red(f" \t (and {len(choices)-1} other completions)", end="")
+
+            printing_value += "\n\n\n"
+
+        print(printing_value)
+        return printing_value
 
     @abstractmethod
     def __call__(self, prompt, only_completed=True, return_sorted=False, **kwargs):
         pass
 
     def copy(self, **kwargs):
         """Returns a copy of the language model with the same parameters."""
         kwargs = {**self.kwargs, **kwargs}
-        model = kwargs.pop('model')
+        model = kwargs.pop("model")
 
         return self.__class__(model=model, **kwargs)
```

### Comparing `dspy-ai-2.4.0/dsp/modules/ollama.py` & `dspy-ai-2.4.3/dsp/modules/ollama.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/pyserini.py` & `dspy-ai-2.4.3/dsp/modules/pyserini.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/sbert.py` & `dspy-ai-2.4.3/dsp/modules/sbert.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/modules/sentence_vectorizer.py` & `dspy-ai-2.4.3/dsp/modules/sentence_vectorizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/primitives/compiler.py` & `dspy-ai-2.4.3/dsp/primitives/compiler.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/primitives/demonstrate.py` & `dspy-ai-2.4.3/dsp/primitives/demonstrate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/primitives/inspect.py` & `dspy-ai-2.4.3/dsp/primitives/inspect.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/primitives/predict.py` & `dspy-ai-2.4.3/dsp/primitives/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,19 +94,28 @@
         # If none of the completions is completed (i.e., none has the final field set).
         if last_field_idx < len(field_names):
             # Pick the first completion that has gone farthest.
             completion = completions[0]
             completion[field_names[last_field_idx]] = ""
 
             # Recurse with greedy decoding and a shorter length.
-            max_tokens = kwargs.get("max_tokens", dsp.settings.lm.kwargs["max_tokens"])
+            max_tokens = (kwargs.get("max_tokens") or 
+                        kwargs.get("max_output_tokens") or
+                        dsp.settings.lm.kwargs.get("max_tokens") or 
+                        dsp.settings.lm.kwargs.get('max_output_tokens'))
+
+
+            if max_tokens is None:
+                raise ValueError("Required 'max_tokens' or 'max_output_tokens' not specified in settings.")
             max_tokens = min(max(75, max_tokens // 2), max_tokens)
+            keys = list(kwargs.keys()) + list(dsp.settings.lm.kwargs.keys()) 
+            max_tokens_key = "max_tokens" if "max_tokens" in keys else "max_output_tokens"
             new_kwargs = {
                 **kwargs,
-                "max_tokens": max_tokens,
+                max_tokens_key: max_tokens,
                 "n": 1,
                 "temperature": 0.0,
             }
 
             assert max_depth > 0
             return generate(template, **new_kwargs)(
                 completion,
```

### Comparing `dspy-ai-2.4.0/dsp/primitives/primitives.py` & `dspy-ai-2.4.3/dsp/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/primitives/search.py` & `dspy-ai-2.4.3/dsp/primitives/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,49 +20,49 @@
         passages_cs_scores = dsp.settings.reranker(query, passages)
         passages_cs_scores_sorted = np.argsort(passages_cs_scores)[::-1]
         passages = [passages[idx] for idx in passages_cs_scores_sorted]
 
     return passages
 
 
-def retrieveRerankEnsemble(queries: list[str], k: int) -> list[str]:
+def retrieveRerankEnsemble(queries: list[str], k: int,**kwargs) -> list[str]:
     if not (dsp.settings.rm and dsp.settings.reranker):
         raise AssertionError("Both RM and Reranker are needed to retrieve & re-rank.")
     queries = [q for q in queries if q]
     passages = {}
     for query in queries:
-        retrieved_passages = dsp.settings.rm(query, k=k*3)
+        retrieved_passages = dsp.settings.rm(query, k=k*3,**kwargs)
         passages_cs_scores = dsp.settings.reranker(query, [psg.long_text for psg in retrieved_passages])
         for idx in np.argsort(passages_cs_scores)[::-1]:
             psg = retrieved_passages[idx]
             passages[psg.long_text] = passages.get(psg.long_text, []) + [
                 passages_cs_scores[idx],
             ]
 
     passages = [(np.average(score), text) for text, score in passages.items()]
     return [text for _, text in sorted(passages, reverse=True)[:k]]
 
 
-def retrieveEnsemble(queries: list[str], k: int, by_prob: bool = True) -> list[str]:
+def retrieveEnsemble(queries: list[str], k: int, by_prob: bool = True,**kwargs) -> list[str]:
     """Retrieves passages from the RM for each query in queries and returns the top k passages
     based on the probability or score.
     """
     if not dsp.settings.rm:
         raise AssertionError("No RM is loaded.")
     if dsp.settings.reranker:
         return retrieveRerankEnsemble(queries, k)
     
     queries = [q for q in queries if q]
 
     if len(queries) == 1:
-        return retrieve(queries[0], k)
+        return retrieve(queries[0], k, **kwargs)
 
     passages = {}
     for q in queries:
-        for psg in dsp.settings.rm(q, k=k * 3):
+        for psg in dsp.settings.rm(q, k=k * 3,**kwargs):
             if by_prob:
                 passages[psg.long_text] = passages.get(psg.long_text, 0.0) + psg.prob
             else:
                 passages[psg.long_text] = passages.get(psg.long_text, 0.0) + psg.score
 
     passages = [(score, text) for text, score in passages.items()]
     passages = sorted(passages, reverse=True)[:k]
```

### Comparing `dspy-ai-2.4.0/dsp/templates/template_v2.py` & `dspy-ai-2.4.3/dsp/templates/template_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/templates/template_v3.py` & `dspy-ai-2.4.3/dsp/templates/template_v3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/templates/utils.py` & `dspy-ai-2.4.3/dsp/templates/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/utils/ann_utils.py` & `dspy-ai-2.4.3/dsp/utils/ann_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/utils/dpr.py` & `dspy-ai-2.4.3/dsp/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/utils/metrics.py` & `dspy-ai-2.4.3/dsp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/utils/settings.py` & `dspy-ai-2.4.3/dsp/utils/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 rm=None,
                 branch_idx=0,
                 reranker=None,
                 compiled_lm=None,
                 force_reuse_cached_compilation=False,
                 compiling=False,
                 skip_logprobs=False,
-                trace=None,
+                trace=[],
                 release=0,
                 log_openai_usage=False,
                 bypass_assert=False,
                 bypass_suggest=False,
                 assert_failures=0,
                 suggest_failures=0,
                 langchain_history=[],
```

### Comparing `dspy-ai-2.4.0/dsp/utils/settings_v2.py` & `dspy-ai-2.4.3/dsp/utils/settings_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dsp/utils/utils.py` & `dspy-ai-2.4.3/dsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/__init__.py` & `dspy-ai-2.4.3/dspy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from .predict import *
 from .primitives import *
 from .retrieve import *
 from .signatures import *
 
 # Functional must be imported after primitives, predict and signatures
 from .functional import * # isort: skip
+from .utils.logging import logger, set_log_level, set_log_output
 
 settings = dsp.settings
 
 AzureOpenAI = dsp.AzureOpenAI
 OpenAI = dsp.GPT3
+Mistral = dsp.Mistral
 Databricks = dsp.Databricks
 Cohere = dsp.Cohere
 ColBERTv2 = dsp.ColBERTv2
 Pyserini = dsp.PyseriniRetriever
 Clarifai = dsp.ClarifaiLLM
 Google = dsp.Google
+GROQ = dsp.GroqLM
 
 HFClientTGI = dsp.HFClientTGI
 HFClientVLLM = HFClientVLLM
 
 Anyscale = dsp.Anyscale
 Together = dsp.Together
 HFModel = dsp.HFModel
```

### Comparing `dspy-ai-2.4.0/dspy/datasets/colors.py` & `dspy-ai-2.4.3/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/datasets/dataloader.py` & `dspy-ai-2.4.3/dspy/datasets/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,21 @@
         dataset = load_dataset("json", data_files=file_path)["train"]
         
         if not fields:
             fields = list(dataset.features)
         
         return [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
 
+    def from_parquet(self, file_path: str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
+        dataset = load_dataset("parquet", data_files=file_path)["train"]
+
+        if not fields:
+            fields = list(dataset.features)
+
+        return [dspy.Example({field: row[field] for field in fields}).with_inputs(input_keys) for row in dataset]
 
     def sample(
         self,
         dataset: List[dspy.Example],
         n: int,
         *args,
         **kwargs,
```

### Comparing `dspy-ai-2.4.0/dspy/datasets/dataset.py` & `dspy-ai-2.4.3/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/datasets/gsm8k.py` & `dspy-ai-2.4.3/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/datasets/hotpotqa.py` & `dspy-ai-2.4.3/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/evaluate/auto_evaluation.py` & `dspy-ai-2.4.3/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/evaluate/evaluate.py` & `dspy-ai-2.4.3/dspy/evaluate/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,18 @@
         data = [
             merge_dicts(example, prediction) | {"correct": score} for _, example, prediction, score in predicted_devset
         ]
 
         df = pd.DataFrame(data)
 
         # Truncate every cell in the DataFrame
-        df = df.applymap(truncate_cell)
+        if hasattr(df, "map"):  # DataFrame.applymap was renamed to DataFrame.map in Pandas 2.1.0
+            df = df.map(truncate_cell)
+        else:
+            df = df.applymap(truncate_cell)
 
         # Rename the 'correct' column to the name of the metric object
         assert callable(metric)
         metric_name = metric.__name__ if isinstance(
             metric, types.FunctionType) else metric.__class__.__name__
         df.rename(columns={"correct": metric_name}, inplace=True)
 
@@ -215,15 +218,15 @@
                     margin: 10px 0;'>
                     ... {truncated_rows} more rows not displayed ...
                 </div>
                 """
                 ipython_display(HTML(message))
 
         if return_all_scores and return_outputs:
-            return round(100 * ncorrect / ntotal, 2), results
+            return round(100 * ncorrect / ntotal, 2), results, [score for *_, score in reordered_devset]
         elif return_all_scores:
             return round(100 * ncorrect / ntotal, 2), [score for *_, score in reordered_devset]
         elif return_outputs:
             return round(100 * ncorrect / ntotal, 2), results
 
         return round(100 * ncorrect / ntotal, 2)
```

### Comparing `dspy-ai-2.4.0/dspy/evaluate/metrics.py` & `dspy-ai-2.4.3/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/experimental/synthetic_data.py` & `dspy-ai-2.4.3/dspy/experimental/synthetic_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,89 @@
+import logging
 import random
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 import dspy
 
 
-class descriptionSignature(dspy.Signature):
-  field_name = dspy.InputField(desc="name of a field")
-  example = dspy.InputField(desc="an example value for the field")
-  description = dspy.OutputField(desc="a short text only description of what the field contains")
+class DescriptionSignature(dspy.Signature):
+    field_name = dspy.InputField(desc="name of a field")
+    example = dspy.InputField(desc="an example value for the field")
+    description = dspy.OutputField(desc="a short text only description of what the field contains")
+
 
 class SyntheticDataGenerator:
     def __init__(self, schema_class: Optional[BaseModel] = None, examples: Optional[List[dspy.Example]] = None):
         self.schema_class = schema_class
         self.examples = examples
 
     def generate(self, sample_size: int) -> List[dspy.Example]:
+        """Generate synthetic examples.
+
+        Args:
+            sample_size (int): number of examples to generate
+        Raises:
+            ValueError: either a schema_class or examples should be provided
+        Returns:
+            List[dspy.Example]: list of synthetic examples generated
+        """
         if not self.schema_class and not self.examples:
             raise ValueError("Either a schema_class or examples must be provided.")
         if self.examples and len(self.examples) >= sample_size:
-            print("No additional data generation needed.")
+            logging.info("No additional data generation needed.")
             return self.examples[:sample_size]
 
         additional_samples_needed = sample_size - (len(self.examples) if self.examples else 0)
         generated_examples = self._generate_additional_examples(additional_samples_needed)
 
         return self.examples + generated_examples if self.examples else generated_examples
 
     def _define_or_infer_fields(self):
+        """Define fields to generate if a schema class is provided.
+        Infer fields to generate if an inital sample of examples is provided.
+
+        Returns:
+            dict: dictionary of fields to generate
+        """  # noqa: D205
         if self.schema_class:
             data_schema = self.schema_class.model_json_schema()
             properties = data_schema['properties']
         elif self.examples:
             inferred_schema = self.examples[0].__dict__['_store']
-            descriptor = dspy.Predict(descriptionSignature)
+            descriptor = dspy.Predict(DescriptionSignature)
             properties = {field: {'description': str((descriptor(field_name=field, example=str(inferred_schema[field]))).description)}
                           for field in inferred_schema.keys()}
         else:
             properties = {}
         return properties
 
     def _generate_additional_examples(self, additional_samples_needed: int) -> List[dspy.Example]:
+        """Generate additional examples if needed.
+
+        Args:
+            additional_samples_needed (int): the difference between the desired
+            number of examples and the current number of examples
+        Returns:
+            List[dspy.Example]: list of synthetic examples
+        """
         properties = self._define_or_infer_fields()
         class_name = f"{self.schema_class.__name__ if self.schema_class else 'Inferred'}Signature"
         fields = self._prepare_fields(properties)
 
         signature_class = type(class_name, (dspy.Signature,), fields)
         generator = dspy.Predict(signature_class, n=additional_samples_needed)
         response = generator(sindex=str(random.randint(1, additional_samples_needed)))
 
         return [dspy.Example({field_name: getattr(completion, field_name) for field_name in properties.keys()})
                 for completion in response.completions]
 
     def _prepare_fields(self, properties) -> dict:
+        """Prepare fields to generate in an appropriate format."""
         return {
             '__doc__': f"Generates the following outputs: {{{', '.join(properties.keys())}}}.",
             'sindex': dspy.InputField(desc="a random string"),
             **{field_name: dspy.OutputField(desc=properties[field_name].get('description', 'No description'))
                for field_name in properties.keys()},
         }
```

### Comparing `dspy-ai-2.4.0/dspy/functional/functional.py` & `dspy-ai-2.4.3/dspy/functional/functional.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import inspect
 import json
-import os
+import textwrap
 import typing
-from typing import Annotated, List, Tuple  # noqa: UP035
+from typing import Annotated, List, Tuple, Union  # noqa: UP035
 
-import openai
 import pydantic
 import ujson
+from pydantic.fields import FieldInfo
 
 import dspy
 from dsp.templates import passages2text
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, make_signature
 
-# Some improvement ideas:
-# - Increase the temperature on error
-
 
 def predictor(func) -> dspy.Module:
     """Decorator that creates a predictor module based on the provided function."""
     signature = _func_to_signature(func)
     *_, output_key = signature.output_fields.keys()
     return _StripOutput(TypedPredictor(signature), output_key)
 
@@ -52,69 +49,161 @@
         super().__init__()
         for name in dir(self):
             attr = getattr(self, name)
             if isinstance(attr, dspy.Module):
                 self.__dict__[name] = attr.copy()
 
 
-def TypedChainOfThought(signature, max_retries=3) -> dspy.Module:  # noqa: N802
+def TypedChainOfThought(signature, instructions=None, *, max_retries=3) -> dspy.Module:  # noqa: N802
     """Just like TypedPredictor, but adds a ChainOfThought OutputField."""
-    signature = ensure_signature(signature)
+    signature = ensure_signature(signature, instructions)
     output_keys = ", ".join(signature.output_fields.keys())
     return TypedPredictor(
         signature.prepend(
             "reasoning",
             dspy.OutputField(
                 prefix="Reasoning: Let's think step by step in order to",
                 desc="${produce the " + output_keys + "}. We ...",
             ),
         ),
         max_retries=max_retries,
     )
 
 
 class TypedPredictor(dspy.Module):
-    def __init__(self, signature, max_retries=3):
+    def __init__(self, signature, instructions=None, *, max_retries=3, wrap_json=False, explain_errors=False):
+        """Like dspy.Predict, but enforces type annotations in the signature.
+
+        Args:
+            signature: The signature of the module. Can use type annotations.
+            max_retries: The number of times to retry the prediction if the output is invalid.
+            wrap_json: If True, json objects in the input will be wrapped in ```json ... ```
+        """
         super().__init__()
-        self.signature = ensure_signature(signature)
+        self.signature = ensure_signature(signature, instructions)
         self.predictor = dspy.Predict(signature)
         self.max_retries = max_retries
+        self.wrap_json = wrap_json
+        self.explain_errors = explain_errors
 
     def copy(self) -> "TypedPredictor":
-        return TypedPredictor(self.signature, self.max_retries)
+        return TypedPredictor(
+            self.signature,
+            max_retries=self.max_retries,
+            wrap_json=self.wrap_json,
+            explain_errors=self.explain_errors,
+        )
+
+    def __repr__(self):
+        """Return a string representation of the TypedPredictor object."""
+        return f"TypedPredictor({self.signature})"
 
-    @staticmethod
-    def _make_example(type_) -> str:
+    def _make_example(self, type_) -> str:
         # Note: DSPy will cache this call so we only pay the first time TypedPredictor is called.
+        schema = json.dumps(type_.model_json_schema())
+        if self.wrap_json:
+            schema = "```json\n" + schema + "\n```\n"
         json_object = dspy.Predict(
             make_signature(
                 "json_schema -> json_object",
                 "Make a very succinct json object that validates with the following schema",
             ),
-        )(json_schema=json.dumps(type_.model_json_schema())).json_object
+        )(json_schema=schema).json_object
         # We use the model_validate_json method to make sure the example is valid
         try:
             type_.model_validate_json(_unwrap_json(json_object))
         except (pydantic.ValidationError, ValueError):
             return ""  # Unable to make an example
         return json_object
         # TODO: Another fun idea is to only (but automatically) do this if the output fails.
         # We could also have a more general "suggest solution" prompt that tries to fix the output
         # More directly.
         # TODO: Instead of using a language model to create the example, we can also just use a
         # library like https://pypi.org/project/polyfactory/ that's made exactly to do this.
 
+    def _format_error(
+        self,
+        error: Exception,
+        task_description: Union[str, FieldInfo],
+        model_output: str,
+        lm_explain: bool,
+    ) -> str:
+        if isinstance(error, pydantic.ValidationError):
+            errors = []
+            for e in error.errors():
+                fields = ", ".join(map(str, e["loc"]))
+                errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
+            error_text = "; ".join(errors)
+        else:
+            error_text = repr(error)
+
+        if self.explain_errors and lm_explain:
+            if isinstance(task_description, FieldInfo):
+                args = task_description.json_schema_extra
+                task_description = args["prefix"] + " " + args["desc"]
+            return (
+                error_text
+                + "\n"
+                + self._make_explanation(
+                    task_description=task_description,
+                    model_output=model_output,
+                    error=error_text,
+                )
+            )
+
+        return error_text
+
+    def _make_explanation(self, task_description: str, model_output: str, error: str) -> str:
+        class Signature(dspy.Signature):
+            __doc__ = textwrap.dedent(
+                """
+                I gave my language model a task, but it failed. Figure out what went wrong,
+                and write instructions to help it avoid the error next time.""",
+            )
+
+            task_description: str = dspy.InputField(desc="What I asked the model to do")
+            language_model_output: str = dspy.InputField(desc="The output of the model")
+            error: str = dspy.InputField(desc="The validation error trigged by the models output")
+            explanation: str = dspy.OutputField(desc="Explain what the model did wrong")
+            advice: str = dspy.OutputField(
+                desc="Instructions for the model to do better next time. A single paragraph.",
+            )
+
+        # TODO: We could also try repair the output here. For example, if the output is a float, but the
+        # model returned a "float + explanation", the repair could be to remove the explanation.
+
+        return dspy.Predict(Signature)(
+            task_description=task_description,
+            language_model_output=model_output,
+            error=error,
+        ).advice
+
     def _prepare_signature(self) -> dspy.Signature:
         """Add formats and parsers to the signature fields, based on the type annotations of the fields."""
         signature = self.signature
         for name, field in self.signature.fields.items():
             is_output = field.json_schema_extra["__dspy_field_type"] == "output"
             type_ = field.annotation
             if is_output:
-                if type_ in (str, int, float, bool):
+                if type_ is bool:
+
+                    def parse(x):
+                        x = x.strip().lower()
+                        if x not in ("true", "false"):
+                            raise ValueError("Respond with true or false")
+                        return x == "true"
+
+                    signature = signature.with_updated_fields(
+                        name,
+                        desc=field.json_schema_extra.get("desc", "")
+                        + (" (Respond with true or false)" if type_ != str else ""),
+                        format=lambda x: x if isinstance(x, str) else str(x),
+                        parser=parse,
+                    )
+                elif type_ in (str, int, float, bool):
                     signature = signature.with_updated_fields(
                         name,
                         desc=field.json_schema_extra.get("desc", "")
                         + (f" (Respond with a single {type_.__name__} value)" if type_ != str else ""),
                         format=lambda x: x if isinstance(x, str) else str(x),
                         parser=type_,
                     )
@@ -140,37 +229,45 @@
                         to_json = lambda x, type_=type_: type_(value=x).model_dump_json()
                         from_json = lambda x, type_=type_: type_.model_validate_json(x).value
                         schema = json.dumps(type_.model_json_schema())
                     else:
                         to_json = lambda x: x.model_dump_json()
                         from_json = lambda x, type_=type_: type_.model_validate_json(x)
                         schema = json.dumps(type_.model_json_schema())
+                    if self.wrap_json:
+                        to_json = lambda x, inner=to_json: "```json\n" + inner(x) + "\n```\n"
+                        schema = "```json\n" + schema + "\n```"
                     signature = signature.with_updated_fields(
                         name,
                         desc=field.json_schema_extra.get("desc", "")
                         + (". Respond with a single JSON object. JSON Schema: " + schema),
                         format=lambda x, to_json=to_json: (x if isinstance(x, str) else to_json(x)),
                         parser=lambda x, from_json=from_json: from_json(_unwrap_json(x)),
                         type_=type_,
                     )
             else:  # If input field
+                is_json = False
                 format_ = lambda x: x if isinstance(x, str) else str(x)
                 if type_ in (List[str], list[str], Tuple[str], tuple[str]):
                     format_ = passages2text
                 # Special formatting for lists of known types. Maybe the output fields sohuld have this too?
                 elif typing.get_origin(type_) in (List, list, Tuple, tuple):
                     (inner_type,) = typing.get_args(type_)
                     if inspect.isclass(inner_type) and issubclass(inner_type, pydantic.BaseModel):
                         format_ = (
                             lambda x: x if isinstance(x, str) else "[" + ",".join(i.model_dump_json() for i in x) + "]"
                         )
                     else:
                         format_ = lambda x: x if isinstance(x, str) else json.dumps(x)
+                    is_json = True
                 elif inspect.isclass(type_) and issubclass(type_, pydantic.BaseModel):
                     format_ = lambda x: x if isinstance(x, str) else x.model_dump_json()
+                    is_json = True
+                if self.wrap_json and is_json:
+                    format_ = lambda x, inner=format_: x if isinstance(x, str) else "```json\n" + inner(x) + "\n```\n"
                 signature = signature.with_updated_fields(name, format=format_)
 
         return signature
 
     def forward(self, **kwargs) -> dspy.Prediction:
         modified_kwargs = kwargs.copy()
         # We have to re-prepare the signature on every forward call, because the base
@@ -185,15 +282,21 @@
                 parsed = {}
                 for name, field in signature.output_fields.items():
                     try:
                         value = completion[name]
                         parser = field.json_schema_extra.get("parser", lambda x: x)
                         parsed[name] = parser(value)
                     except (pydantic.ValidationError, ValueError) as e:
-                        errors[name] = _format_error(e)
+                        errors[name] = self._format_error(
+                            e,
+                            signature.fields[name],
+                            value,
+                            lm_explain=try_i + 1 < self.max_retries,
+                        )
+
                         # If we can, we add an example to the error message
                         current_desc = field.json_schema_extra.get("desc", "")
                         i = current_desc.find("JSON Schema: ")
                         if i == -1:
                             continue  # Only add examples to JSON objects
                         suffix, current_desc = current_desc[i:], current_desc[:i]
                         prefix = "You MUST use this format: "
@@ -208,221 +311,90 @@
                             )
                 # No reason trying to parse the general signature, or run more completions, if we already have errors
                 if errors:
                     break
                 # Instantiate the actual signature with the parsed values.
                 # This allow pydantic to validate the fields defined in the signature.
                 try:
-                    _dummy = self.signature(**kwargs, **parsed)
+                    _ = self.signature(**kwargs, **parsed)
                     parsed_results.append(parsed)
                 except pydantic.ValidationError as e:
-                    errors["general"] = _format_error(e)
+                    errors["general"] = self._format_error(
+                        e,
+                        signature.instructions,
+                        "\n\n".join(
+                            "> " + field.json_schema_extra["prefix"] + " " + completion[name]
+                            for name, field in signature.output_fields.items()
+                        ),
+                        lm_explain=try_i + 1 < self.max_retries,
+                    )
             if errors:
                 # Add new fields for each error
                 for name, error in errors.items():
                     modified_kwargs[f"error_{name}_{try_i}"] = error
+                    if name == "general":
+                        error_prefix = "General:"
+                    else:
+                        error_prefix = signature.output_fields[name].json_schema_extra["prefix"]
+                    number = "" if try_i == 0 else f" ({try_i+1})"
                     signature = signature.append(
                         f"error_{name}_{try_i}",
                         dspy.InputField(
-                            prefix="Past Error " + (f"({name}):" if try_i == 0 else f"({name}, {try_i+1}):"),
+                            prefix=f"Past Error{number} in {error_prefix}",
                             desc="An error to avoid in the future",
                         ),
                     )
             else:
                 # If there are no errors, we return the parsed results
                 return Prediction.from_completions(
                     {key: [r[key] for r in parsed_results] for key in signature.output_fields},
                 )
         raise ValueError(
             "Too many retries trying to get the correct output format. " + "Try simplifying the requirements.",
             errors,
         )
 
 
-def _format_error(error: Exception):
-    if isinstance(error, pydantic.ValidationError):
-        errors = []
-        for e in error.errors():
-            fields = ", ".join(map(str, e["loc"]))
-            errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
-        return "; ".join(errors)
-    else:
-        return repr(error)
-
-
 def _func_to_signature(func):
     """Make a dspy.Signature based on a function definition."""
     sig = inspect.signature(func)
-    annotations = typing.get_type_hints(func)
+    annotations = typing.get_type_hints(func, include_extras=True)
     output_key = func.__name__
     instructions = func.__doc__
     fields = {}
 
     # Input fields
     for param in sig.parameters.values():
         if param.name == "self":
             continue
         # We default to str as the type of the input
         annotation = annotations.get(param.name, str)
         kwargs = {}
         if typing.get_origin(annotation) is Annotated:
-            annotation, kwargs["desc"] = typing.get_args(annotation)
+            desc = next((arg for arg in typing.get_args(annotation) if isinstance(arg, str)), None)
+            if desc is not None:
+                kwargs["desc"] = desc
         fields[param.name] = (annotation, dspy.InputField(**kwargs))
 
     # Output field
     kwargs = {}
     annotation = annotations.get("return", str)
     if typing.get_origin(annotation) is Annotated:
-        annotation, kwargs["desc"] = typing.get_args(annotation)
+        desc = next((arg for arg in typing.get_args(annotation) if isinstance(arg, str)), None)
+        if desc is not None:
+            kwargs["desc"] = desc
     fields[output_key] = (annotation, dspy.OutputField(**kwargs))
 
     return dspy.Signature(fields, instructions)
 
 
 def _unwrap_json(output):
     output = output.strip()
     if output.startswith("```"):
         if not output.startswith("```json"):
             raise ValueError("json output should start with ```json")
         if not output.endswith("```"):
-            raise ValueError("json output should end with ```")
+            raise ValueError("Don't write anything after the final json ```")
         output = output[7:-3].strip()
     if not output.startswith("{") or not output.endswith("}"):
         raise ValueError("json output should start and end with { and }")
     return ujson.dumps(ujson.loads(output))  # ujson is a bit more robust than the standard json
-
-
-################################################################################
-# Example usage
-################################################################################
-
-
-def main() -> None:
-    class Answer(pydantic.BaseModel):
-        value: float
-        certainty: float
-        comments: list[str] = pydantic.Field(description="At least two comments about the answer")
-
-    class QA(dspy.Module):
-        @predictor
-        def hard_question(self, topic: str) -> str:
-            """Think of a hard factual question about a topic. It should be answerable with a number."""
-
-        @cot
-        def answer(self, question: Annotated[str, "Question to answer"]) -> Answer:
-            pass
-
-        def forward(self, **kwargs):
-            question = self.hard_question(**kwargs)
-            return (question, self.answer(question=question))
-
-    openai.api_key = os.getenv("OPENAI_API_KEY")
-    lm = dspy.OpenAI(model="gpt-3.5-turbo", max_tokens=4000)
-    # lm = dspy.OpenAI(model="gpt-4", max_tokens=4000)
-    # lm = dspy.OpenAI(model="gpt-4-preview-1106", max_tokens=4000)
-    with dspy.context(lm=lm):
-        qa = QA()
-        question, answer = qa(topic="Physics")
-        # lm.inspect_history(n=5)
-
-        print("Question:", question)  # noqa: T201
-        print("Answer:", answer)  # noqa: T201
-
-
-################################################################################
-# HotpotQA example with SimpleBaleen
-################################################################################
-
-
-def validate_context_and_answer_and_hops(example, pred, trace=None) -> bool:
-    if not dspy.evaluate.answer_exact_match(example, pred):
-        return False
-    if not dspy.evaluate.answer_passage_match(example, pred):
-        return False
-
-    hops = [example.question] + [outputs.query for *_, outputs in trace if "query" in outputs]
-
-    if max([len(h) for h in hops]) > 100:
-        return False
-    if any(dspy.evaluate.answer_exact_match_str(hops[idx], hops[:idx], frac=0.8) for idx in range(2, len(hops))):
-        return False
-
-    return True
-
-
-def gold_passages_retrieved(example, pred, _trace=None) -> bool:
-    gold_titles = set(map(dspy.evaluate.normalize_text, example["gold_titles"]))
-    found_titles = set(map(dspy.evaluate.normalize_text, [c.split(" | ")[0] for c in pred.context]))
-
-    return gold_titles.issubset(found_titles)
-
-
-def hotpot() -> None:
-    import dspy.evaluate
-    from dsp.utils import deduplicate
-    from dspy.datasets import HotPotQA
-    from dspy.evaluate.evaluate import Evaluate
-    from dspy.teleprompt.bootstrap import BootstrapFewShot
-
-    print("Load the dataset.")  # noqa: T201
-    dataset = HotPotQA(train_seed=1, train_size=20, eval_seed=2023, dev_size=50, test_size=0)
-    trainset = [x.with_inputs("question") for x in dataset.train]
-    devset = [x.with_inputs("question") for x in dataset.dev]
-    print("Done")  # noqa: T201
-
-    class SimplifiedBaleen(FunctionalModule):
-        def __init__(self, passages_per_hop=3, max_hops=1):
-            super().__init__()
-            self.retrieve = dspy.Retrieve(k=passages_per_hop)
-            self.max_hops = max_hops
-
-        @cot
-        def generate_query(self, context: list[str], question) -> str:
-            """Write a simple search query that will help answer a complex question."""
-            pass
-
-        @cot
-        def generate_answer(self, context: list[str], question) -> str:
-            """Answer questions with short factoid answers."""
-            pass
-
-        def forward(self, question):
-            context = []
-
-            for _ in range(self.max_hops):
-                query = self.generate_query(context=context, question=question)
-                passages = self.retrieve(query).passages
-                context = deduplicate(context + passages)
-
-            answer = self.generate_answer(context=context, question=question)
-            return dspy.Prediction(context=context, answer=answer)
-
-    openai.api_key = os.getenv("OPENAI_API_KEY")
-    rm = dspy.ColBERTv2(url="http://20.102.90.50:2017/wiki17_abstracts")
-    lm = dspy.OpenAI(model="gpt-3.5-turbo", max_tokens=4000)
-    dspy.settings.configure(lm=lm, rm=rm, trace=[])
-
-    evaluate_on_hotpotqa = Evaluate(devset=devset, num_threads=10, display_progress=True, display_table=5)
-
-    # uncompiled (i.e., zero-shot) program
-    uncompiled_baleen = SimplifiedBaleen()
-    print(  # noqa: T201
-        "Uncompiled Baleen retrieval score:",
-        evaluate_on_hotpotqa(uncompiled_baleen, metric=gold_passages_retrieved),
-    )
-
-    # compiled (i.e., few-shot) program
-    compiled_baleen = BootstrapFewShot(metric=validate_context_and_answer_and_hops).compile(
-        SimplifiedBaleen(),
-        teacher=SimplifiedBaleen(passages_per_hop=2),
-        trainset=trainset,
-    )
-    print(  # noqa: T201
-        "Compiled Baleen retrieval score:",
-        evaluate_on_hotpotqa(compiled_baleen, metric=gold_passages_retrieved),
-    )
-    # lm.inspect_history(n=5)
-
-
-if __name__ == "__main__":
-    # main()
-    hotpot()
```

### Comparing `dspy-ai-2.4.0/dspy/predict/aggregation.py` & `dspy-ai-2.4.3/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/chain_of_thought.py` & `dspy-ai-2.4.3/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/chain_of_thought_with_hint.py` & `dspy-ai-2.4.3/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/knn.py` & `dspy-ai-2.4.3/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/langchain.py` & `dspy-ai-2.4.3/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/multi_chain_comparison.py` & `dspy-ai-2.4.3/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/predict.py` & `dspy-ai-2.4.3/dspy/predict/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import random
 
+from pydantic import BaseModel
+
 import dsp
 from dspy.predict.parameter import Parameter
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, signature_to_template
 
 
 class Predict(Parameter):
@@ -16,17 +18,27 @@
     def reset(self):
         self.lm = None
         self.traces = []
         self.train = []
         self.demos = []
 
     def dump_state(self):
-        state_keys = ["lm", "traces", "train", "demos"]
+        state_keys = ["lm", "traces", "train"]
         state = {k: getattr(self, k) for k in state_keys}
 
+        state["demos"] = []
+        for demo in self.demos:
+            demo = demo.copy()
+
+            for field in demo:
+                if isinstance(demo[field], BaseModel):
+                    demo[field] = demo[field].model_dump_json()
+
+            state["demos"].append(demo)
+
         # Cache the signature instructions and the last field's name.
         state["signature_instructions"] = self.signature.instructions
 
         *_, last_key = self.signature.fields.keys()
         state["signature_prefix"] = self.signature.fields[last_key].json_schema_extra["prefix"]
 
         return state
```

### Comparing `dspy-ai-2.4.0/dspy/predict/program_of_thought.py` & `dspy-ai-2.4.3/dspy/predict/program_of_thought.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from dspy.signatures.signature import ensure_signature
 
 from ..primitives.program import Module
 from ..primitives.python_interpreter import CodePrompt, PythonInterpreter
 
 
 class ProgramOfThought(Module):
-    def __init__(self, signature, max_iters=3):
+    def __init__(self, signature, max_iters=3, import_white_list=None):
         super().__init__()
         self.signature = signature = ensure_signature(signature)
         self.max_iters = max_iters
+        self.import_white_list = import_white_list
 
         self.input_fields = signature.input_fields
         self.output_fields = signature.output_fields
 
+        assert len(self.output_fields) == 1, "PoT only supports one output field."
+
+        self.output_field_name = next(iter(self.output_fields))
         inputs_ = ", ".join(
             [f"`{field_name}`" for field_name in self.input_fields.keys()],
         )
-        outputs_ = ", ".join(
-            [f"`{field_name}`" for field_name in self.output_fields.keys()],
-        )
+        outputs_ = f"`{self.output_field_name}`"
 
         assert len(self.output_fields) == 1, "PoT only supports one output field."
 
         instr = []
         instr.append(
             f"You will be given {inputs_} and you will respond with {outputs_}.",
         )
@@ -51,15 +53,14 @@
         )
         self.generate_answer = dspy.ChainOfThought(
             dspy.Signature(
                 self._generate_signature("answer").fields,
                 self._generate_instruction("answer"),
             ),
         )
-
     def _generate_signature(self, mode):
         signature_dict = dict(self.input_fields)
         fields_for_mode = {
             "generate": {
                 "generated_code": dspy.OutputField(
                     prefix="Code:",
                     desc="python code that answers the question",
@@ -88,51 +89,47 @@
                     desc="python code that answers the question",
                     format=str,
                 ),
                 "code_output": dspy.InputField(
                     prefix="Code Output:",
                     desc="output of previously-generated python code",
                 ),
-                "answer": self.signature.fields["answer"],
+                self.output_field_name: self.signature.fields[self.output_field_name],
             },
         }
         signature_dict.update(fields_for_mode[mode])
         return dspy.Signature(signature_dict)
 
     def _generate_instruction(self, mode):
         mode_inputs = ", ".join(
             [
                 f"`{field_name}`"
                 for field_name in self._generate_signature(mode).input_fields
             ],
         )
-        mode_outputs = ", ".join(
-            [
-                f"`{field_name}`"
-                for field_name in self._generate_signature(mode).output_fields
-            ],
-        )
+        mode_outputs = f"`{self.output_field_name}`"
         if mode == "generate":
             instr = [
                 f"You will be given {mode_inputs} and you will respond with {mode_outputs}.",
                 f"Generating executable Python code that programmatically computes the correct {mode_outputs}.",
                 f"After you're done with the computation, make sure the last line in your code evaluates to the correct value for {mode_outputs}.",
             ]
         elif mode == "regenerate":
             instr = [
                 f"You are given {mode_inputs} due to an error in previous code.",
-                f"Your task is to correct the error and provide the new {mode_outputs}.",
+                "Your task is to correct the error and provide the new `generated_code`.",
             ]
         else:  # mode == 'answer'
             instr = [
                 f"Given the final code {mode_inputs}, provide the final {mode_outputs}.",
             ]
 
         return "\n".join(instr)
 
+
     def parse_code(self, code_data):
         code = (
             code_data.get("generated_code", "").split("---", 1)[0].split("\n\n\n", 1)[0]
         )
         code_match = re.search(r"```python[ \n](.*?)[ \n]```?", code, re.DOTALL)
         code_block = (code_match.group(1) if code_match else code).replace("\\n", "\n")
         if not code_block:
@@ -152,36 +149,37 @@
             )
         return code_block, None
 
     def execute_code(self, code):
         if not code:
             return code, None, "Error: Empty code before execution."
         code_prompt = CodePrompt(code, code_type="python")
-        interpreter = PythonInterpreter(action_space={"print": print})
+        interpreter = PythonInterpreter(action_space={"print": print}, import_white_list=self.import_white_list)
         try:
             output = str(code_prompt.execute(interpreter=interpreter)[0])
+            print
             return code, output, None
         except Exception as e:
             return code, None, str(e)
-
     def forward(self, **kwargs):
-        code_data = self.code_generate(question=kwargs["question"])
+        input_kwargs = {
+            field_name: kwargs[field_name] for field_name in self.input_fields
+        }
+        code_data = self.code_generate(**input_kwargs)
         parsed_code, error = self.parse_code(code_data)
         # FIXME: Don't try to execute the code if it didn't parse
         code, output, error = self.execute_code(parsed_code)
         hop = 0
         while hop < self.max_iters and error:
             print("Error in code execution")
-            code_data = self.code_regenerate(
-                question=kwargs["question"], previous_code=code, error=error,
-            )
+            input_kwargs.update({"previous_code": code, "error": error})
+            code_data = self.code_regenerate(**input_kwargs)
             parsed_code, error = self.parse_code(code_data)
             # FIXME: Don't try to execute the code if it didn't parse
             code, output, error = self.execute_code(parsed_code)
             hop += 1
             if hop == self.max_iters:
                 print("Max hops reached. Error persists.")
                 return None
-        answer_gen_result = self.generate_answer(
-            question=kwargs["question"], final_generated_code=code, code_output=output,
-        )
-        return answer_gen_result
+        input_kwargs.update({"final_generated_code": code, "code_output": output})
+        answer_gen_result = self.generate_answer(**input_kwargs)
+        return answer_gen_result
```

### Comparing `dspy-ai-2.4.0/dspy/predict/react.py` & `dspy-ai-2.4.3/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/predict/retry.py` & `dspy-ai-2.4.3/dspy/predict/retry.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,31 @@
             desc="Some instructions you must satisfy",
             format=str,
         ))
 
         return signature
 
     def forward(self, *, past_outputs, **kwargs):
+        # Take into account the possible new signature, as in TypedPredictor
+        new_signature = kwargs.pop("new_signature", None)
+        if new_signature:
+            self.original_signature = new_signature
+            self.new_signature = self._create_new_signature(self.original_signature)
+
         # Convert the dict past_outputs={"answer": ...} to kwargs
         # {past_answer=..., ...}
         for key, value in past_outputs.items():
             past_key = f"past_{key}"
             if past_key in self.new_signature.input_fields:
                 kwargs[past_key] = value
         # Tell the wrapped module to use the new signature.
         # Note: This only works if the wrapped module is a Predict or ChainOfThought.
         kwargs["new_signature"] = self.new_signature
         return self.original_forward(**kwargs)
-    
+
     def __call__(self, **kwargs):
         cached_kwargs = copy.deepcopy(kwargs)
         kwargs["_trace"] = False
         kwargs.setdefault("demos", self.demos if self.demos is not None else [])
 
         # perform backtracking
         if dspy.settings.backtrack_to == self:
@@ -55,14 +61,14 @@
             pred = self.forward(**kwargs)
         else:
             pred = self.module(**kwargs)
 
         # now pop multiple reserved keys
         # NOTE(shangyin) past_outputs seems not useful to include in demos,
         # therefore dropped
-        for key in ["_trace", "demos", "signature", "config", "lm", "past_outputs"]:
+        for key in ["_trace", "demos", "signature", "new_signature", "config", "lm", "past_outputs"]:
             kwargs.pop(key, None)
 
         if dsp.settings.trace is not None:
             trace = dsp.settings.trace
             trace.append((self, {**kwargs}, pred))
         return pred
```

### Comparing `dspy-ai-2.4.0/dspy/primitives/assertions.py` & `dspy-ai-2.4.3/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/primitives/box.py` & `dspy-ai-2.4.3/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/primitives/example.py` & `dspy-ai-2.4.3/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/primitives/prediction.py` & `dspy-ai-2.4.3/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/primitives/program.py` & `dspy-ai-2.4.3/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/primitives/python_interpreter.py` & `dspy-ai-2.4.3/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/retrieve/chromadb_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/chromadb_rm.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,19 +68,19 @@
 
     def __init__(
         self,
         collection_name: str,
         persist_directory: str,
         embedding_function: Optional[
             EmbeddingFunction[Embeddable]
-        ] = None,
+        ] = ef.DefaultEmbeddingFunction(),
         k: int = 7,
     ):
         self._init_chromadb(collection_name, persist_directory)
-        self.ef = embedding_function or self._chromadb_collection.embedding_function
+        self.ef = embedding_function
 
         super().__init__(k=k)
 
     def _init_chromadb(
         self,
         collection_name: str,
         persist_directory: str,
@@ -118,15 +118,15 @@
 
         Returns:
             List[List[float]]: List of embeddings corresponding to each query.
         """
         return self.ef(queries)
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs,
     ) -> dspy.Prediction:
         """Search with db for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
@@ -138,13 +138,17 @@
             else query_or_queries
         )
         queries = [q for q in queries if q]  # Filter empty queries
         embeddings = self._get_embeddings(queries)
 
         k = self.k if k is None else k
         results = self._chromadb_collection.query(
-            query_embeddings=embeddings, n_results=k,
+            query_embeddings=embeddings, n_results=k,**kwargs,
         )
 
-        passages = [dotdict({"long_text": x}) for x in results["documents"][0]]
-
-        return passages
+        zipped_results = zip(
+            results["ids"][0], 
+            results["distances"][0], 
+            results["documents"][0], 
+            results["metadatas"][0])
+        results = [dotdict({"id": id, "score": dist, "long_text": doc, "metadatas": meta }) for id, dist, doc, meta in zipped_results]
+        return results
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/clarifai_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/clarifai_rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         header = {"Authorization": f"Key {self.pat}"}
         request = requests.get(hits.input.data.text.url, headers=header)
         request.encoding = request.apparent_encoding
         requested_text = request.text
         return requested_text
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs,
     ) -> dspy.Prediction:
         """Uses clarifai-python SDK search function and retrieves top_k similar passages for given query,
         Args:
              query_or_queries : single query or list of queries
              k : Top K relevant documents to return
 
         Returns:
@@ -81,15 +81,15 @@
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         passages = []
         queries = [q for q in queries if q]
 
         for query in queries:
-            search_response = self.clarifai_search.query(ranks=[{"text_raw": query}])
+            search_response = self.clarifai_search.query(ranks=[{"text_raw": query}],**kwargs)
 
             # Retrieve hits
             hits = [hit for data in search_response for hit in data.hits]
             with ThreadPoolExecutor(max_workers=10) as executor:
                 results = list(executor.map(self.retrieve_hits, hits))
             passages.extend(dotdict({"long_text": d}) for d in results)
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/databricks_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/databricks_rm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 from collections import defaultdict
 from typing import List, Union
 
 import requests
 
 import dspy
@@ -15,14 +16,16 @@
     Args:
         databricks_index_name (str): Databricks vector search index to query
         databricks_endpoint (str): Databricks index endpoint url
         databricks_token (str): Databricks authentication token
         columns (list[str]): Column names to include in response
         filters_json (str, optional): JSON string for query filters
         k (int, optional): Number of top embeddings to retrieve. Defaults to 3.
+        docs_id_column_name (str, optional): Column name for retrieved doc_ids to return.
+        text_column_name (str, optional): Column name for retrieved text to return.
 
     Examples:
         Below is a code snippet that shows how to configure Databricks Vector Search endpoints:
 
         (example adapted from "Databricks: How to create and query a Vector Search Index: 
         https://docs.databricks.com/en/generative-ai/create-query-vector-search.html#create-a-vector-search-index)
 
@@ -35,15 +38,15 @@
 
         client.create_endpoint(
             name="your_vector_search_endpoint_name",
             endpoint_type="STANDARD"
         )
 
         #Creating Vector Search Index using Python SDK 
-        #Example for Direct Vector Acces Index
+        #Example for Direct Vector Access Index
 
         index = client.create_direct_access_index(
             endpoint_name="your_databricks_host_url",
             index_name="your_index_name",
             primary_key="id",
             embedding_dimension=1024,
             embedding_vector_column="text_vector",
@@ -61,15 +64,15 @@
         ```
 
         Below is a code snippet that shows how to query the Databricks Direct Vector Access Index using the forward() function.
         ```python
         self.retrieve = DatabricksRM(query=[1, 2, 3], query_type = 'vector')
         ```
     """
-    def __init__(self, databricks_index_name = None, databricks_endpoint = None, databricks_token = None, columns = None, filters_json = None, k = 3):
+    def __init__(self, databricks_index_name = None, databricks_endpoint = None, databricks_token = None, columns = None, filters_json = None, k = 3, docs_id_column_name = 'id', text_column_name = 'text'):
         super().__init__(k=k)
         if not databricks_token and not os.environ.get("DATABRICKS_TOKEN"):
             raise ValueError("You must supply databricks_token or set environment variable DATABRICKS_TOKEN")
         if not databricks_endpoint and not os.environ.get("DATABRICKS_HOST"):
             raise ValueError("You must supply databricks_endpoint or set environment variable DATABRICKS_HOST")
         if not databricks_index_name:
             raise ValueError("You must supply vector index name")
@@ -77,14 +80,16 @@
             raise ValueError("You must specify a list of column names to be included in the response")
         self.databricks_token = databricks_token if databricks_token else os.environ["DATABRICKS_TOKEN"]
         self.databricks_endpoint = databricks_endpoint if databricks_endpoint else os.environ["DATABRICKS_HOST"]
         self.databricks_index_name = databricks_index_name
         self.columns = columns
         self.filters_json = filters_json
         self.k = k
+        self.docs_id_column_name = docs_id_column_name
+        self.text_column_name = text_column_name
 
     def forward(self, query: Union[str, List[float]], query_type: str = 'vector') -> dspy.Prediction:
         """Search with Databricks Vector Search Client for self.k top results for query
 
         Args:
             query (Union[str, List[float]]): query to search for.
             query_type (str): 'vector' for Direct Vector Access Index and Delta Sync Index using self-managed vectors or 'text' for Delta Sync Index using model endpoint.
@@ -116,18 +121,24 @@
             f"{self.databricks_endpoint}/api/2.0/vector-search/indexes/{self.databricks_index_name}/query",
             json=payload,
             headers=headers,
         )
         results = response.json()
 
         docs = defaultdict(float)
+        doc_ids = []
         text, score = None, None
         for data_row in results["result"]["data_array"]:
             for col, val in zip(results["manifest"]["columns"], data_row):
-                if col["name"] == 'text':
+                if col["name"] == self.docs_id_column_name:
+                    if self.docs_id_column_name == 'metadata':
+                        docs_dict = json.loads(val)
+                        doc_ids.append(str(docs_dict["document_id"]))
+                    else:
+                        doc_ids.append(str(val))
                     text = val
                 if col["name"] == 'score':
                     score = val
             docs[text] += score
 
         sorted_docs = sorted(docs.items(), key=lambda x: x[1], reverse=True)[:self.k]
-        return Prediction(docs=[doc for doc, _ in sorted_docs])
+        return Prediction(docs=[doc for doc, _ in sorted_docs], doc_ids = doc_ids)
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/deeplake_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/deeplake_rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         texts = [t.replace("\n", " ") for t in texts]
         return [
             data["embedding"]
             for data in openai.Embedding.create(input=texts, model=model)["data"]
         ]
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int],
+        self, query_or_queries: Union[str, List[str]], k: Optional[int],**kwargs,
     ) -> dspy.Prediction:
         
         """Search with DeepLake for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
@@ -102,15 +102,15 @@
 
         passages = defaultdict(float)
         #deeplake doesn't support batch querying, manually querying each query and storing them
         for query in queries:
             results = self._deeplake_client(
             path=self._deeplake_vectorstore_name,
             embedding_function=self.embedding_function,
-            ).search(query, k=k)
+            ).search(query, k=k,**kwargs)
 
             for score,text in zip(results.get('score',0.0),results.get('text',"")):
                 passages[text] += score
 
         sorted_passages = sorted(
             passages.items(), key=lambda x: x[1], reverse=True)[:k]
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/faiss_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/faiss_rm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Retriever model for faiss: https://github.com/facebookresearch/faiss.
 Author: Jagane Sundar: https://github.com/jagane.
 """
 
 import logging
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 
 import dspy
 from dsp.modules.sentence_vectorizer import SentenceTransformersVectorizer
 from dsp.utils import dotdict
 
@@ -103,54 +103,48 @@
             indices = index_list[i]
             distances = distance_list[i]
             logging.debug(f"Query: {queries[i]}")
             for j in range(len(indices)):
                 logging.debug(f"    Hit {j} = {indices[j]}/{distances[j]}: {self._document_chunks[indices[j]]}")
         return
 
-    def forward(self, query_or_queries: Union[str, list[str]]) -> dspy.Prediction:
-        """Search the faiss index for self.k top passages for query.
+    def forward(self, query_or_queries: Union[str, list[str]], k: Optional[int] = None,**kwargs) -> dspy.Prediction:
+        """Search the faiss index for k or self.k top passages for query.
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
         """
         queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [q for q in queries if q]  # Filter empty queries
         embeddings = self._vectorizer(queries)
         emb_npa = np.array(embeddings)
         # For single query, just look up the top k passages
         if len(queries) == 1:
-            distance_list, index_list = self._faiss_index.search(emb_npa, self.k)
+            distance_list, index_list = self._faiss_index.search(emb_npa, k or self.k)
             # self._dump_raw_results(queries, index_list, distance_list)
             passages = [(self._document_chunks[ind], ind) for ind in index_list[0]]
-            passages = [dotdict({"long_text": passage[0], "index": passage[1]}) for passage in passages]
-            return dspy.Prediction(passages=passages)
+            return [dotdict({"long_text": passage[0], "index": passage[1]}) for passage in passages]
 
-        distance_list, index_list = self._faiss_index.search(emb_npa, self.k * 3)
+        distance_list, index_list = self._faiss_index.search(emb_npa, (k or self.k) * 3,**kwargs)
         # self._dump_raw_results(queries, index_list, distance_list)
         passage_scores = {}
         for emb in range(len(embeddings)):
             indices = index_list[emb]  # indices of neighbors for embeddings[emb] - this is an array of k*3 integers
             distances = distance_list[
                 emb
             ]  # distances of neighbors for embeddings[emb] - this is an array of k*3 floating point numbers
-            for res in range(self.k * 3):
+            for res in range((k or self.k) * 3):
                 neighbor = indices[res]
                 distance = distances[res]
                 if neighbor in passage_scores:
                     passage_scores[neighbor].append(distance)
                 else:
                     passage_scores[neighbor] = [distance]
         # Note re. sorting:
         # first degree sort: number of queries that got a hit with any particular document chunk. More
         # is a better match. This is len(queries)-len(x[1])
         # second degree sort: sum of the distances of each hit returned by faiss. Smaller distance is a better match
-        sorted_passages = sorted(passage_scores.items(), key=lambda x: (len(queries) - len(x[1]), sum(x[1])))[: self.k]
-        return dspy.Prediction(
-            passages=[
-                dotdict({"long_text": self._document_chunks[passage_index], "index": passage_index})
-                for passage_index, _ in sorted_passages
-            ],
-        )
+        sorted_passages = sorted(passage_scores.items(), key=lambda x: (len(queries) - len(x[1]), sum(x[1])))[: k or self.k]
+        return [ dotdict({"long_text": self._document_chunks[passage_index], "index": passage_index}) for passage_index, _ in sorted_passages ]
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/marqo_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/marqo_rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 from typing import List, Union
 
 import dspy
-from dspy import dotdict
+from dsp.utils import dotdict
 
 try:
     import marqo
 except ImportError:
     raise ImportError(
         "The 'marqo' extra is required to use MarqoRM. Install it with `pip install dspy-ai[marqo]`",
     )
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/mongodb_atlas_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/retrieve/pinecone_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/retrieve/qdrant_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/qdrant_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         k: int = 3,
     ):
         self._qdrant_collection_name = qdrant_collection_name
         self._qdrant_client = qdrant_client
 
         super().__init__(k=k)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int]) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int],**kwargs) -> dspy.Prediction:
         """Search with Qdrant for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -67,15 +67,15 @@
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         queries = [q for q in queries if q]  # Filter empty queries
 
         k = k if k is not None else self.k
         batch_results = self._qdrant_client.query_batch(
-            self._qdrant_collection_name, query_texts=queries, limit=k)
+            self._qdrant_collection_name, query_texts=queries, limit=k,**kwargs)
 
         passages_scores = defaultdict(float)
         for batch in batch_results:
             for result in batch:
                 # If a passage is returned multiple times, the score is accumulated.
                 passages_scores[result.document] += result.score
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/retrieve.py` & `dspy-ai-2.4.3/dspy/retrieve/retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     def load_state(self, state):
         for name, value in state.items():
             setattr(self, name, value)
 
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None) -> Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs) -> Prediction:
         queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [query.strip().split('\n')[0].strip() for query in queries]
 
         # print(queries)
         # TODO: Consider removing any quote-like markers that surround the query too.
         k = k if k is not None else self.k
-        passages = dsp.retrieveEnsemble(queries, k=k)
+        passages = dsp.retrieveEnsemble(queries, k=k,**kwargs)
         return Prediction(passages=passages)
 
 # TODO: Consider doing Prediction.from_completions with the individual sets of passages (per query) too.
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/vectara_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/retrieve/weaviate_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/weaviate_rm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Optional, Union
 
 import dspy
 from dsp.utils import dotdict
 
 try:
     import weaviate
+    import weaviate.classes as wvc
+    from weaviate.collections.classes.grpc import HybridFusion
 except ImportError:
     raise ImportError(
         "The 'weaviate' extra is required to use WeaviateRM. Install it with `pip install dspy-ai[weaviate]`",
     )
 
 
 class WeaviateRM(dspy.Retrieve):
@@ -18,14 +20,17 @@
     Assumes that a Weaviate collection has been created and populated with the following payload:
         - content: The text of the passage
 
     Args:
         weaviate_collection_name (str): The name of the Weaviate collection.
         weaviate_client (WeaviateClient): An instance of the Weaviate client.
         k (int, optional): The default number of top passages to retrieve. Defaults to 3.
+        weaviate_collection_text_key (str, optional): The key in the collection with the content. Defaults to content.
+        weaviate_alpha (float, optional): The alpha value for the hybrid query. Defaults to 0.5.
+        weaviate_fusion_type (wvc.HybridFusion, optional): The fusion type for the query. Defaults to RELATIVE_SCORE.
 
     Examples:
         Below is a code snippet that shows how to use Weaviate as the default retriver:
         ```python
         import weaviate
 
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
@@ -40,24 +45,28 @@
         ```python
         self.retrieve = WeaviateRM("my_collection_name", weaviate_client=weaviate_client, k=num_passages)
         ```
     """
 
     def __init__(self, 
                  weaviate_collection_name: str, 
-                 weaviate_client: weaviate.Client, 
+                 weaviate_client: weaviate.WeaviateClient,
                  k: int = 3,
                  weaviate_collection_text_key: Optional[str] = "content",
+                 weaviate_alpha: Optional[float] = 0.5,
+                 weaviate_fusion_type: Optional[HybridFusion] = HybridFusion.RELATIVE_SCORE,
         ):
         self._weaviate_collection_name = weaviate_collection_name
         self._weaviate_client = weaviate_client
         self._weaviate_collection_text_key = weaviate_collection_text_key
+        self._weaviate_alpha = weaviate_alpha
+        self._weaviate_fusion_type = weaviate_fusion_type
         super().__init__(k=k)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int]) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs) -> dspy.Prediction:
         """Search with Weaviate for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -68,18 +77,22 @@
             [query_or_queries]
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         queries = [q for q in queries if q]
         passages = []
         for query in queries:
-            results = self._weaviate_client.query\
-                .get(self._weaviate_collection_name, [self._weaviate_collection_text_key])\
-                .with_hybrid(query=query)\
-                .with_limit(k)\
-                .do()
+            collection = self._weaviate_client.collections.get(self._weaviate_collection_name)
+            results = collection.query.hybrid(query=query,
+                                              limit=k,
+                                              alpha=self._weaviate_alpha,
+                                              fusion_type=self._weaviate_fusion_type,
+                                              return_metadata=wvc.query.MetadataQuery(
+                                                  distance=True, score=True),
+                                              **kwargs,
+                                              )
 
-            results = results["data"]["Get"][self._weaviate_collection_name]
-            parsed_results = [result[self._weaviate_collection_text_key] for result in results]
+            parsed_results = [result.properties[self._weaviate_collection_text_key] for result in results.objects]
             passages.extend(dotdict({"long_text": d}) for d in parsed_results)
 
+        # Return type not changed, needs to be a Prediction object. But other code will break if we change it.
         return passages
```

### Comparing `dspy-ai-2.4.0/dspy/retrieve/you_rm.py` & `dspy-ai-2.4.3/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy/signatures/field.py` & `dspy-ai-2.4.3/dspy/signatures/field.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     pydantic_kwargs = {}
     json_schema_extra = {}
     for k, v in kwargs.items():
         if k in DSPY_FIELD_ARG_NAMES:
             json_schema_extra[k] = v
         else:
             pydantic_kwargs[k] = v
+    # Also copy over the pydantic "description" if no dspy "desc" is given.
+    if "description" in kwargs and "desc" not in json_schema_extra:
+        json_schema_extra["desc"] = kwargs["description"]
     pydantic_kwargs["json_schema_extra"] = json_schema_extra
     return pydantic_kwargs
 
 
 def InputField(**kwargs):
     return pydantic.Field(**move_kwargs(**kwargs, __dspy_field_type="input"))
```

### Comparing `dspy-ai-2.4.0/dspy/signatures/signature.py` & `dspy-ai-2.4.3/dspy/signatures/signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -202,19 +202,21 @@
     ""  # noqa: D419
 
     # Note: Don't put a docstring here, as it will become the default instructions
     # for any signature that doesn't define it's own instructions.
     pass
 
 
-def ensure_signature(signature: Union[str, Type[Signature]]) -> Signature:
+def ensure_signature(signature: Union[str, Type[Signature]], instructions=None) -> Signature:
     if signature is None:
         return None
     if isinstance(signature, str):
-        return Signature(signature)
+        return Signature(signature, instructions)
+    if instructions is not None:
+        raise ValueError("Don't specify instructions when initializing with a Signature")
     return signature
 
 
 def make_signature(
     signature: Union[str, Dict[str, Tuple[type, FieldInfo]]],
     instructions: str = None,
     signature_name: str = "StringSignature",
@@ -273,44 +275,39 @@
     )
 
 
 def _parse_signature(signature: str) -> Tuple[Type, Field]:
     if signature.count("->") != 1:
         raise ValueError(f"Invalid signature format: '{signature}', must contain exactly one '->'.")
 
+    inputs_str, outputs_str = signature.split("->")
+
     fields = {}
-    inputs_str, outputs_str = map(str.strip, signature.split("->"))
-    inputs = [v.strip() for v in inputs_str.split(",") if v.strip()]
-    outputs = [v.strip() for v in outputs_str.split(",") if v.strip()]
-    for name_type in inputs:
-        name, type_ = _parse_named_type_node(name_type)
+    for name, type_ in _parse_arg_string(inputs_str):
         fields[name] = (type_, InputField())
-    for name_type in outputs:
-        name, type_ = _parse_named_type_node(name_type)
+    for name, type_ in _parse_arg_string(outputs_str):
         fields[name] = (type_, OutputField())
 
     return fields
 
 
-def _parse_named_type_node(node, names=None) -> Any:
-    parts = node.split(":")
-    if len(parts) == 1:
-        return parts[0], str
-    name, type_str = parts
-    type_ = _parse_type_node(ast.parse(type_str), names)
-    return name, type_
+def _parse_arg_string(string: str, names=None) -> Dict[str, str]:
+    args = ast.parse("def f(" + string + "): pass").body[0].args.args
+    names = [arg.arg for arg in args]
+    types = [str if arg.annotation is None else _parse_type_node(arg.annotation) for arg in args]
+    return zip(names, types)
 
 
 def _parse_type_node(node, names=None) -> Any:
     """Recursively parse an AST node representing a type annotation.
 
     without using structural pattern matching introduced in Python 3.10.
     """
     if names is None:
-        names = {}
+        names = typing.__dict__
 
     if isinstance(node, ast.Module):
         body = node.body
         if len(body) != 1:
             raise ValueError(f"Code is not syntactically valid: {node}")
         return _parse_type_node(body[0], names)
 
@@ -321,24 +318,31 @@
     if isinstance(node, ast.Name):
         id_ = node.id
         if id_ in names:
             return names[id_]
         for type_ in [int, str, float, bool, list, tuple, dict]:
             if type_.__name__ == id_:
                 return type_
+        raise ValueError(f"Unknown name: {id_}")
 
-    elif isinstance(node, ast.Subscript):
+    if isinstance(node, ast.Subscript):
         base_type = _parse_type_node(node.value, names)
         arg_type = _parse_type_node(node.slice, names)
         return base_type[arg_type]
 
-    elif isinstance(node, ast.Tuple):
+    if isinstance(node, ast.Tuple):
         elts = node.elts
         return tuple(_parse_type_node(elt, names) for elt in elts)
 
+    if isinstance(node, ast.Call):
+        if node.func.id == "Field":
+            keys = [kw.arg for kw in node.keywords]
+            values = [kw.value.value for kw in node.keywords]
+            return Field(**dict(zip(keys, values)))
+
     raise ValueError(f"Code is not syntactically valid: {node}")
 
 
 def infer_prefix(attribute_name: str) -> str:
     """Infer a prefix from an attribute name."""
     # Convert camelCase to snake_case, but handle sequences of capital letters properly
     s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", attribute_name)
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/bootstrap.py` & `dspy-ai-2.4.3/dspy/teleprompt/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,32 @@
 # TODO: When this bootstraps for another teleprompter like finetune, we want all demos we gather.
 # But when it's for direct use we may want to sample ONE demo per predictor--example pair. This is important for "multi-use" modules.
 
 # TODO: Add baselines=[...]
 
 
 class BootstrapFewShot(Teleprompter):
-    def __init__(self, metric=None, metric_threshold=None, teacher_settings={}, max_bootstrapped_demos=4, max_labeled_demos=16, max_rounds=1, max_errors=5):
+    def __init__(
+        self,
+        metric=None,
+        metric_threshold=None,
+        teacher_settings={},
+        max_bootstrapped_demos=4,
+        max_labeled_demos=16,
+        max_rounds=1,
+        max_errors=5,
+    ):
         self.metric = metric
         self.metric_threshold = metric_threshold
         self.teacher_settings = teacher_settings
 
         self.max_bootstrapped_demos = max_bootstrapped_demos
         self.max_labeled_demos = max_labeled_demos
         self.max_rounds = max_rounds
-        self.max_errors= max_errors
+        self.max_errors = max_errors
         self.error_count = 0
         self.error_lock = threading.Lock()
 
     def compile(self, student, *, teacher=None, trainset, valset=None):
         self.trainset = trainset
         self.valset = valset
 
@@ -55,45 +64,49 @@
         self.student._compiled = True
 
         # set assert_failures and suggest_failures as attributes of student w/ value 0
         self.student._assert_failures = 0
         self.student._suggest_failures = 0
 
         return self.student
-    
+
     def _prepare_student_and_teacher(self, student, teacher):
         self.student = student.reset_copy()
         self.teacher = teacher.deepcopy() if teacher is not None else student.reset_copy()
 
-        assert getattr(self.student, '_compiled', False) is False, "Student must be uncompiled."
+        assert getattr(self.student, "_compiled", False) is False, "Student must be uncompiled."
 
-        if self.max_labeled_demos and getattr(self.teacher, '_compiled', False) is False:
+        if self.max_labeled_demos and getattr(self.teacher, "_compiled", False) is False:
             teleprompter = LabeledFewShot(k=self.max_labeled_demos)
             self.teacher = teleprompter.compile(self.teacher.reset_copy(), trainset=self.trainset)
 
     def _prepare_predictor_mappings(self):
         name2predictor, predictor2name = {}, {}
         student, teacher = self.student, self.teacher
 
-        assert len(student.predictors()) == len(teacher.predictors()), "Student and teacher must have the same number of predictors."
+        assert len(student.predictors()) == len(
+            teacher.predictors(),
+        ), "Student and teacher must have the same number of predictors."
 
         for (name1, predictor1), (name2, predictor2) in zip(student.named_predictors(), teacher.named_predictors()):
             assert name1 == name2, "Student and teacher must have the same program structure."
-            assert predictor1.signature.equals(predictor2.signature), f"Student and teacher must have the same signatures. {type(predictor1.signature)} != {type(predictor2.signature)}"
+            assert predictor1.signature.equals(
+                predictor2.signature,
+            ), f"Student and teacher must have the same signatures. {type(predictor1.signature)} != {type(predictor2.signature)}"
             assert id(predictor1) != id(predictor2), "Student and teacher must be different objects."
 
-            name2predictor[name1] = None # dict(student=predictor1, teacher=predictor2)
+            name2predictor[name1] = None  # dict(student=predictor1, teacher=predictor2)
             predictor2name[id(predictor1)] = name1
 
             # FIXME(shangyint): This is an ugly hack to bind traces of
             # retry.module to retry
             # if isinstance(predictor1, Retry):
             #     predictor2name[id(predictor1.module)] = name1
 
-            predictor2name[id(predictor2)] = name2            
+            predictor2name[id(predictor2)] = name2
 
         self.name2predictor = name2predictor
         self.predictor2name = predictor2name
 
     def _bootstrap(self, *, max_bootstraps=None):
         max_bootstraps = max_bootstraps or self.max_bootstrapped_demos
 
@@ -107,30 +120,30 @@
 
                 if example_idx not in bootstrapped:
                     success = self._bootstrap_one_example(example, round_idx)
 
                     if success:
                         bootstrapped[example_idx] = True
 
-        print(f'Bootstrapped {len(bootstrapped)} full traces after {example_idx+1} examples in round {round_idx}.')
-        
+        print(f"Bootstrapped {len(bootstrapped)} full traces after {example_idx+1} examples in round {round_idx}.")
+
         # Unbootstrapped training examples
 
         self.validation = [x for idx, x in enumerate(self.trainset) if idx not in bootstrapped]
         random.Random(0).shuffle(self.validation)
 
         self.validation = self.valset or self.validation
 
         # NOTE: Can't yet use evaluate because we need to trace *per example*
         # evaluate = Evaluate(program=self.teacher, metric=self.metric, num_threads=12)
         # score = evaluate(self.metric, display_table=False, display_progress=True)
-    
+
     def _bootstrap_one_example(self, example, round_idx=0):
         name2traces = self.name2traces
-        teacher = self.teacher #.deepcopy()
+        teacher = self.teacher  # .deepcopy()
         predictor_cache = {}
 
         try:
             with dsp.settings.context(trace=[], **self.teacher_settings):
                 lm = dsp.settings.lm
                 lm = lm.copy(temperature=0.7 + 0.001 * round_idx) if round_idx > 0 else lm
                 new_settings = dict(lm=lm) if round_idx > 0 else {}
@@ -141,15 +154,15 @@
                         predictor.demos = [x for x in predictor.demos if x != example]
 
                     prediction = teacher(**example.inputs())
                     trace = dsp.settings.trace
 
                     for name, predictor in teacher.named_predictors():
                         predictor.demos = predictor_cache[name]
-                
+
                 if self.metric:
                     metric_val = self.metric(example, prediction, trace)
                     if self.metric_threshold:
                         success = metric_val >= self.metric_threshold
                     else:
                         success = metric_val
                 else:
@@ -158,52 +171,56 @@
         except Exception as e:
             success = False
             with self.error_lock:
                 self.error_count += 1
                 current_error_count = self.error_count
             if current_error_count >= self.max_errors:
                 raise e
-            print(f'Failed to run or to evaluate example {example} with {self.metric} due to {e}.')
-        
+            print(f"Failed to run or to evaluate example {example} with {self.metric} due to {e}.")
+
         if success:
             for step in trace:
                 predictor, inputs, outputs = step
 
-                if 'dspy_uuid' in example:
+                if "dspy_uuid" in example:
                     demo = Example(augmented=True, dspy_uuid=example.dspy_uuid, **inputs, **outputs)
                 else:
                     # TODO: FIXME: This is a hack. RandomSearch will complain for now in this edge case.
                     demo = Example(augmented=True, **inputs, **outputs)
 
                 try:
                     predictor_name = self.predictor2name[id(predictor)]
                 except KeyError as e:
-                    continue # FIXME: !
+                    continue  # FIXME: !
 
                     # TODO: Look closer into this. It's a bit tricky to reproduce.
-                    print(f'Failed to find predictor {predictor} in {self.predictor2name}.')
-                    print('Are you doing this in a notebook (Jupyter)? This might be caused by redefining values by rerunning cells.')
-                    print('Try restarting the notebook, or open an issue.')
-                    raise KeyError(f'Failed to find predictor {id(predictor)} {predictor} in {self.predictor2name}.') from e
+                    print(f"Failed to find predictor {predictor} in {self.predictor2name}.")
+                    print(
+                        "Are you doing this in a notebook (Jupyter)? This might be caused by redefining values by rerunning cells.",
+                    )
+                    print("Try restarting the notebook, or open an issue.")
+                    raise KeyError(
+                        f"Failed to find predictor {id(predictor)} {predictor} in {self.predictor2name}.",
+                    ) from e
 
                 name2traces[predictor_name].append(demo)
-        
+
         return success
 
     def _train(self):
         rng = random.Random(0)
         raw_demos = self.validation
 
         for name, predictor in self.student.named_predictors():
-            augmented_demos = self.name2traces[name][:self.max_bootstrapped_demos]
-            
+            augmented_demos = self.name2traces[name][: self.max_bootstrapped_demos]
+
             sample_size = min(self.max_labeled_demos - len(augmented_demos), len(raw_demos))
             sample_size = max(0, sample_size)
 
             raw_demos = rng.sample(raw_demos, sample_size)
-            
+
             if dspy.settings.release >= 20230928:
                 predictor.demos = raw_demos + augmented_demos
             else:
                 predictor.demos = augmented_demos + raw_demos
 
         return self.student
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/copro_optimizer.py` & `dspy-ai-2.4.3/dspy/teleprompt/copro_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,32 +27,49 @@
 * track_stats: Tells the method whether or not to track statistics about the optimization process.
                 If True, the method will track the following statistics:
                     * results_best: The min,max,avg,stddev of top 10 scores for each predictor at each depth.
                     * results_latest: The min,max,avg,stddev of newest prompt scores for each predictor at each depth.
                     * total_calls: The total number of calls to the task metric.
                 These statistics will be returned as attributes of the best program.
 """
+
+
 class BasicGenerateInstruction(Signature):
     """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
 
     basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
     proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
+    proposed_prefix_for_output_field = dspy.OutputField(
+        desc="The string at the end of the prompt, which will help the model start solving the task",
+    )
+
 
 class GenerateInstructionGivenAttempts(dspy.Signature):
-        """You are an instruction optimizer for large language models. I will give some task instructions I've tried, along with their corresponding validation scores. The instructions are arranged in increasing order based on their scores, where higher scores indicate better quality.
+    """You are an instruction optimizer for large language models. I will give some task instructions I've tried, along with their corresponding validation scores. The instructions are arranged in increasing order based on their scores, where higher scores indicate better quality.
+
+    Your task is to propose a new instruction that will lead a good language model to perform the task even better. Don't be afraid to be creative."""
 
-Your task is to propose a new instruction that will lead a good language model to perform the task even better. Don't be afraid to be creative."""
+    attempted_instructions = dspy.InputField(format=dsp.passages2text)
+    proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
+    proposed_prefix_for_output_field = dspy.OutputField(
+        desc="The string at the end of the prompt, which will help the model start solving the task",
+    )
 
-        attempted_instructions = dspy.InputField(format=dsp.passages2text)
-        proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-        proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class COPRO(Teleprompter):
-    def __init__(self, prompt_model=None, metric=None, breadth=10, depth=3, init_temperature=1.4, verbose=False, track_stats=False):
+    def __init__(
+        self,
+        prompt_model=None,
+        metric=None,
+        breadth=10,
+        depth=3,
+        init_temperature=1.4,
+        verbose=False,
+        track_stats=False,
+    ):
         if breadth <= 1:
             raise ValueError("Breadth must be greater than 1")
         self.metric = metric
         self.breadth = breadth
         self.depth = depth
         self.init_temperature = init_temperature
         self.prompt_model = prompt_model
@@ -71,231 +88,276 @@
 
     def _drop_duplicates(self, candidates):
         final_candidates = []
         last_batch = []
         last_batch_score = -1
         for c in candidates:
             repeat = False
-            if c['score'] == last_batch_score:
+            if c["score"] == last_batch_score:
                 for c2 in last_batch:
-                    if (self._check_candidates_equal(c, c2)):
+                    if self._check_candidates_equal(c, c2):
                         repeat = True
                         break
                 if not repeat:
                     last_batch.append(c)
             else:
                 last_batch = [c]
-                last_batch_score = c['score']
+                last_batch_score = c["score"]
             if not repeat:
                 final_candidates.append(c)
         return final_candidates
 
     def _print_signature(self, predictor):
         if self.verbose:
             signature = self._get_signature(predictor)
             print(f"i: {signature.instructions}")
             print(f"p: {list(signature.fields.values())[-1].json_schema_extra['prefix']}")
             print()
-    
+
     def _get_signature(self, predictor):
-        if (hasattr(predictor, 'extended_signature')):
+        if hasattr(predictor, "extended_signature"):
             return predictor.extended_signature
-        elif (hasattr(predictor, 'signature')):
+        elif hasattr(predictor, "signature"):
             return predictor.signature
-    
+
     def _set_signature(self, predictor, updated_signature):
-        if (hasattr(predictor, 'extended_signature')):
+        if hasattr(predictor, "extended_signature"):
             predictor.extended_signature = updated_signature
-        elif (hasattr(predictor, 'signature')):
+        elif hasattr(predictor, "signature"):
             predictor.signature = updated_signature
 
-    
     def compile(self, student, *, trainset, eval_kwargs):
         """student is a program that needs to be optimized, note that it may be zero-shot or already pre-optimized for demos != []"""
         module = student.deepcopy()
         evaluate = Evaluate(devset=trainset, metric=self.metric, **eval_kwargs)
         total_calls = 0
-        results_best = {id(p):{"depth": [], "max": [], "average": [], "min":[], "std": []} for p in module.predictors()}
-        results_latest = {id(p):{"depth": [], "max": [], "average": [], "min":[], "std": []} for p in module.predictors()}
+        results_best = {
+            id(p): {"depth": [], "max": [], "average": [], "min": [], "std": []} for p in module.predictors()
+        }
+        results_latest = {
+            id(p): {"depth": [], "max": [], "average": [], "min": [], "std": []} for p in module.predictors()
+        }
 
         if self.track_stats:
             import numpy as np
 
-
         candidates = {}
         evaluated_candidates = defaultdict(dict)
 
         # Seed the prompt optimizer zero shot with just the instruction, generate BREADTH new prompts
         for predictor in module.predictors():
             basic_instruction = None
             basic_prefix = None
             *_, last_key = self._get_signature(predictor).fields.keys()
             basic_instruction = self._get_signature(predictor).instructions
-            basic_prefix = self._get_signature(predictor).fields[last_key].json_schema_extra['prefix']
-            if self.prompt_model: 
+            basic_prefix = self._get_signature(predictor).fields[last_key].json_schema_extra["prefix"]
+            if self.prompt_model:
                 with dspy.settings.context(lm=self.prompt_model):
-                    instruct = dspy.Predict(BasicGenerateInstruction, n=self.breadth-1, temperature=self.init_temperature)(basic_instruction=basic_instruction)
+                    instruct = dspy.Predict(
+                        BasicGenerateInstruction,
+                        n=self.breadth - 1,
+                        temperature=self.init_temperature,
+                    )(basic_instruction=basic_instruction)
             else:
-                instruct = dspy.Predict(BasicGenerateInstruction, n=self.breadth-1, temperature=self.init_temperature)(basic_instruction=basic_instruction)
+                instruct = dspy.Predict(
+                    BasicGenerateInstruction,
+                    n=self.breadth - 1,
+                    temperature=self.init_temperature,
+                )(basic_instruction=basic_instruction)
             # Add in our initial prompt as a candidate as well
             instruct.completions.proposed_instruction.append(basic_instruction)
             instruct.completions.proposed_prefix_for_output_field.append(basic_prefix)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
-        
-        if self.verbose and self.prompt_model: print(f"{self.prompt_model.inspect_history(n=1)}")
+
+        if self.verbose and self.prompt_model:
+            print(f"{self.prompt_model.inspect_history(n=1)}")
 
         latest_candidates = candidates
         all_candidates = candidates
-        
+
         module_clone = module.deepcopy()
 
         # For each iteration in depth...
-        for d in range(self.depth): # TODO: fix this so that we eval the new batch of predictors with the new best followoing predictors
+        for d in range(
+            self.depth,
+        ):  # TODO: fix this so that we eval the new batch of predictors with the new best followoing predictors
             print(f"Iteration Depth: {d+1}/{self.depth}.")
 
             latest_scores = []
-        
+
             # Go through our module's predictors
             for p_i, (p_old, p_new) in enumerate(zip(module.predictors(), module_clone.predictors())):
-                candidates_ = latest_candidates[id(p_old)] # Use the most recently generated candidates for evaluation 
+                candidates_ = latest_candidates[id(p_old)]  # Use the most recently generated candidates for evaluation
                 if len(module.predictors()) > 1:
-                    candidates_ = all_candidates[id(p_old)] # Unless our program has multiple predictors, in which case we need to reevaluate all prompts with the new prompt(s) for the other predictor(s)   
+                    candidates_ = all_candidates[
+                        id(p_old)
+                    ]  # Unless our program has multiple predictors, in which case we need to reevaluate all prompts with the new prompt(s) for the other predictor(s)
 
                 # For each candidate
-                for c_i, c in enumerate(candidates_):                    
-                    # Get the candidate instruction and prefix 
-                    instruction, prefix = c.proposed_instruction.strip('"').strip(), c.proposed_prefix_for_output_field.strip('"').strip()
+                for c_i, c in enumerate(candidates_):
+                    # Get the candidate instruction and prefix
+                    instruction, prefix = (
+                        c.proposed_instruction.strip('"').strip(),
+                        c.proposed_prefix_for_output_field.strip('"').strip(),
+                    )
 
-                    # Set this new module with our instruction / prefix 
+                    # Set this new module with our instruction / prefix
                     *_, last_key = self._get_signature(p_new).fields.keys()
-                    updated_signature = self._get_signature(p_new) \
-                        .with_instructions(instruction) \
+                    updated_signature = (
+                        self._get_signature(p_new)
+                        .with_instructions(instruction)
                         .with_updated_fields(last_key, prefix=prefix)
+                    )
                     self._set_signature(p_new, updated_signature)
 
-                    # Score the instruction / prefix 
-                    if self.verbose: print("----------------")
-                    for i,predictor in enumerate(module_clone.predictors()):
-                        if self.verbose: print(f"Predictor {i+1}")
+                    # Score the instruction / prefix
+                    if self.verbose:
+                        print("----------------")
+                    for i, predictor in enumerate(module_clone.predictors()):
+                        if self.verbose:
+                            print(f"Predictor {i+1}")
                         self._print_signature(predictor)
-                    print(f"At Depth {d+1}/{self.depth}, Evaluating Prompt Candidate #{c_i+1}/{len(candidates_)} for Predictor {p_i+1} of {len(module.predictors())}.")
+                    print(
+                        f"At Depth {d+1}/{self.depth}, Evaluating Prompt Candidate #{c_i+1}/{len(candidates_)} for Predictor {p_i+1} of {len(module.predictors())}.",
+                    )
                     score = evaluate(module_clone, devset=trainset, **eval_kwargs)
-                    if self.verbose and self.prompt_model: print(f"prompt_model.inspect_history(n=1) {self.prompt_model.inspect_history(n=1)}")
+                    if self.verbose and self.prompt_model:
+                        print(f"prompt_model.inspect_history(n=1) {self.prompt_model.inspect_history(n=1)}")
                     total_calls += 1
-                    if self.verbose: print("----------------")
+                    if self.verbose:
+                        print("----------------")
 
                     replace_entry = True
-                    if self.verbose: print(f"(instruction, prefix) {(instruction, prefix)}")
+                    if self.verbose:
+                        print(f"(instruction, prefix) {(instruction, prefix)}")
                     # if verbose: print(f"evaluated_candidates[id(p_old)] {evaluated_candidates[id(p_old)]}")
-                    if ((instruction, prefix) in evaluated_candidates[id(p_old)]):
+                    if (instruction, prefix) in evaluated_candidates[id(p_old)]:
                         # if verbose: print(f"if evaluated_candidates[id(p_old)][(instruction, prefix)] {evaluated_candidates[id(p_old)][(instruction, prefix)]}")
                         if evaluated_candidates[id(p_old)][(instruction, prefix)]["score"] >= score:
                             replace_entry = False
 
                     if replace_entry:
                         # Add it to our evaluated candidates list
                         evaluated_candidates[id(p_old)][(instruction, prefix)] = {
                             "score": score,
                             "program": module_clone.deepcopy(),
                             "instruction": instruction,
                             "prefix": prefix,
                             "depth": d,
                         }
-                    
-                    if (len(candidates_)-self.breadth <= c_i):
+
+                    if len(candidates_) - self.breadth <= c_i:
                         latest_scores.append(score)
 
                 if self.track_stats:
                     results_latest[id(p_old)]["depth"].append(d)
                     results_latest[id(p_old)]["max"].append(max(latest_scores))
-                    results_latest[id(p_old)]["average"].append(sum(latest_scores)/len(latest_scores))
+                    results_latest[id(p_old)]["average"].append(sum(latest_scores) / len(latest_scores))
                     results_latest[id(p_old)]["min"].append(min(latest_scores))
                     results_latest[id(p_old)]["std"].append(np.std(latest_scores))
-                
+
                 # Now that we've evaluated the candidates, set this predictor to the best performing version
                 # to ensure the next round of scores reflect the best possible version
-                best_candidate = max(evaluated_candidates[id(p_old)].values(), key=lambda candidate: candidate['score'])
+                best_candidate = max(evaluated_candidates[id(p_old)].values(), key=lambda candidate: candidate["score"])
                 *_, last_key = self._get_signature(p_old).fields.keys()
-                updated_signature = self._get_signature(p_new) \
-                    .with_instructions(best_candidate["instruction"]) \
+                updated_signature = (
+                    self._get_signature(p_new)
+                    .with_instructions(best_candidate["instruction"])
                     .with_updated_fields(last_key, prefix=best_candidate["prefix"])
+                )
                 self._set_signature(p_new, updated_signature)
-                if self.verbose: print(f"Updating Predictor {id(p_old)} to:\ni: {best_candidate['instruction']}\np: {best_candidate['prefix']}")
-                if self.verbose: print("Full predictor with update: ")
-                for i,predictor in enumerate(module_clone.predictors()):
-                    if self.verbose: print(f"Predictor {i}")
+                if self.verbose:
+                    print(
+                        f"Updating Predictor {id(p_old)} to:\ni: {best_candidate['instruction']}\np: {best_candidate['prefix']}",
+                    )
+                if self.verbose:
+                    print("Full predictor with update: ")
+                for i, predictor in enumerate(module_clone.predictors()):
+                    if self.verbose:
+                        print(f"Predictor {i}")
                     self._print_signature(predictor)
 
-            if d == self.depth-1:
+            if d == self.depth - 1:
                 break
 
-            
             new_candidates = {}
             for p_base in module.predictors():
                 # Build Few-Shot Example of Optimized Prompts
                 attempts = []
                 shortest_len = self.breadth
-                shortest_len = min(len(evaluated_candidates[id(p_base)]),shortest_len)
+                shortest_len = min(len(evaluated_candidates[id(p_base)]), shortest_len)
                 best_predictors = list(evaluated_candidates[id(p_base)].values())
 
                 # best_predictors = evaluated_candidates[id(p_base)].values()[:]
-                best_predictors.sort(key=lambda x: x['score'], reverse=True)
+                best_predictors.sort(key=lambda x: x["score"], reverse=True)
 
                 if self.track_stats:
-                    scores = [x['score'] for x in best_predictors][:10]
+                    scores = [x["score"] for x in best_predictors][:10]
                     results_best[id(p_base)]["depth"].append(d)
                     results_best[id(p_base)]["max"].append(max(scores))
-                    results_best[id(p_base)]["average"].append(sum(scores)/len(scores))
+                    results_best[id(p_base)]["average"].append(sum(scores) / len(scores))
                     results_best[id(p_base)]["min"].append(min(scores))
                     results_best[id(p_base)]["std"].append(np.std(scores))
-                
-                for i in range(shortest_len-1,-1,-1):
+
+                for i in range(shortest_len - 1, -1, -1):
                     # breakpoint()
                     attempts.append(f'Instruction #{shortest_len-i}: {best_predictors[i]["instruction"]}')
                     attempts.append(f'Prefix #{shortest_len-i}: {best_predictors[i]["prefix"]}')
                     attempts.append(f'Resulting Score #{shortest_len-i}: {best_predictors[i]["score"]}')
-            
+
                 # Generate next batch of potential prompts to optimize, with previous attempts as input
-                if self.prompt_model: 
+                if self.prompt_model:
                     with dspy.settings.context(lm=self.prompt_model):
-                        instr = dspy.Predict(GenerateInstructionGivenAttempts, n=self.breadth, temperature=self.init_temperature)(attempted_instructions=attempts)
+                        instr = dspy.Predict(
+                            GenerateInstructionGivenAttempts,
+                            n=self.breadth,
+                            temperature=self.init_temperature,
+                        )(attempted_instructions=attempts)
                 else:
-                    instr = dspy.Predict(GenerateInstructionGivenAttempts, n=self.breadth, temperature=self.init_temperature)(attempted_instructions=attempts)
+                    instr = dspy.Predict(
+                        GenerateInstructionGivenAttempts,
+                        n=self.breadth,
+                        temperature=self.init_temperature,
+                    )(attempted_instructions=attempts)
 
-                if self.verbose and self.prompt_model: print(f"{self.prompt_model.inspect_history(n=1)}")
+                if self.verbose and self.prompt_model:
+                    print(f"{self.prompt_model.inspect_history(n=1)}")
                 # Get candidates for each predictor
                 new_candidates[id(p_base)] = instr.completions
                 all_candidates[id(p_base)].proposed_instruction.extend(instr.completions.proposed_instruction)
-                all_candidates[id(p_base)].proposed_prefix_for_output_field.extend(instr.completions.proposed_prefix_for_output_field)
+                all_candidates[id(p_base)].proposed_prefix_for_output_field.extend(
+                    instr.completions.proposed_prefix_for_output_field,
+                )
 
-            if self.verbose and self.prompt_model: print(f"{self.prompt_model.inspect_history(n=1)}")
+            if self.verbose and self.prompt_model:
+                print(f"{self.prompt_model.inspect_history(n=1)}")
             latest_candidates = new_candidates
-        
+
         candidates = []
         for predictor in module.predictors():
             candidates.extend(list(evaluated_candidates[id(predictor)].values()))
 
             if self.track_stats:
                 best_predictors = list(evaluated_candidates[id(predictor)].values())
-                best_predictors.sort(key=lambda x: x['score'], reverse=True)
+                best_predictors.sort(key=lambda x: x["score"], reverse=True)
 
-                scores = [x['score'] for x in best_predictors][:10]
+                scores = [x["score"] for x in best_predictors][:10]
                 results_best[id(predictor)]["depth"].append(d)
                 results_best[id(predictor)]["max"].append(max(scores))
-                results_best[id(predictor)]["average"].append(sum(scores)/len(scores))
+                results_best[id(predictor)]["average"].append(sum(scores) / len(scores))
                 results_best[id(predictor)]["min"].append(min(scores))
                 results_best[id(predictor)]["std"].append(np.std(scores))
 
         # if verbose: print(f"candidates: {candidates}")
-        candidates.sort(key=lambda x: x['score'], reverse=True)
+        candidates.sort(key=lambda x: x["score"], reverse=True)
 
         candidates = self._drop_duplicates(candidates)
 
         best_program = candidates[0]["program"]
         best_program.candidate_programs = candidates
         best_program.total_calls = total_calls
         if self.track_stats:
             best_program.results_best = results_best
             best_program.results_latest = results_latest
 
-        return best_program
+        return best_program
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/ensemble.py` & `dspy-ai-2.4.3/dspy/teleprompt/ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 
 from dspy.teleprompt.teleprompt import Teleprompter
 
 """
 TODO: The EnsembledProgram should actually imitate the structure of the individual programs (IF they are all compatible). This allows compiling with an ensemble program as a (singular) teacher. Basically the top majority-compatible trace will end up being used, if dspy.majority is the reduce_fn.
 """
 
+
 class Ensemble(Teleprompter):
     def __init__(self, *, reduce_fn=None, size=None, deterministic=False):
         """A common reduce_fn is dspy.majority."""
-        
+
         assert deterministic is False, "TODO: Implement example hashing for deterministic ensemble."
-        
+
         self.reduce_fn = reduce_fn
         self.size = size
         self.deterministic = deterministic
 
     def compile(self, programs):
         size = self.size
         reduce_fn = self.reduce_fn
 
         import dspy
+
         class EnsembledProgram(dspy.Module):
             def __init__(self):
                 super().__init__()
                 self.programs = programs
-            
+
             def forward(self, *args, **kwargs):
                 programs = random.sample(self.programs, size) if size else self.programs
                 outputs = [prog(*args, **kwargs) for prog in programs]
 
                 if reduce_fn:
                     return reduce_fn(outputs)
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/finetune.py` & `dspy-ai-2.4.3/dspy/teleprompt/finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from .teleprompt import Teleprompter
 
 # from .vanilla import LabeledFewShot
 
 # from dspy.evaluate.evaluate import Evaluate
 
 
-if os.environ.get('DSP_NOTEBOOK_CACHEDIR'):
-    training_data_directory = os.path.join(os.environ.get('DSP_NOTEBOOK_CACHEDIR'), 'compiler')
+if os.environ.get("DSP_NOTEBOOK_CACHEDIR"):
+    training_data_directory = os.path.join(os.environ.get("DSP_NOTEBOOK_CACHEDIR"), "compiler")
     print(training_data_directory)
 else:
-    training_data_directory = 'local_cache/compiler'
+    training_data_directory = "local_cache/compiler"
 
 if not os.path.exists(training_data_directory):
     os.makedirs(training_data_directory)
 
 
 """
 TODO: Reduce and document the dependencies.
@@ -50,40 +50,56 @@
 class BootstrapFinetune(Teleprompter):
     def __init__(self, metric=None, teacher_settings={}, multitask=True):
         self.metric = metric
         self.teacher_settings = teacher_settings
         self.multitask = multitask
 
         metric = metric or (lambda *args: True)
-        self.teleprompter = BootstrapFewShot(metric=metric,
-                                             max_bootstrapped_demos=999999,
-                                             max_labeled_demos=0,  # FIXME: TODO: Make this zero? or param, with default as 16 or 0?
-                                             teacher_settings=teacher_settings)
-        
-
-    def compile(self, student, *, teacher=None, trainset, valset=None,
-                target='t5-large', bsize=12, accumsteps=1, lr=5e-5, epochs=1, bf16=False, int8=False, peft=False, path_prefix=None):
-
+        self.teleprompter = BootstrapFewShot(
+            metric=metric,
+            max_bootstrapped_demos=999999,
+            max_labeled_demos=0,  # FIXME: TODO: Make this zero? or param, with default as 16 or 0?
+            teacher_settings=teacher_settings,
+        )
+
+    def compile(
+        self,
+        student,
+        *,
+        teacher=None,
+        trainset,
+        valset=None,
+        target="t5-large",
+        bsize=12,
+        accumsteps=1,
+        lr=5e-5,
+        epochs=1,
+        bf16=False,
+        int8=False,
+        peft=False,
+        path_prefix=None,
+    ):
         # It's usually better to supply a few-shot teacher, rather than uncompiled module (the student).
         if teacher is None:
-            print("WARNING: Using a vanilla teacher. "
-                  "Are you sure you want to use BootstrapFinetune without a compiled teacher?")
-
+            print(
+                "WARNING: Using a vanilla teacher. "
+                "Are you sure you want to use BootstrapFinetune without a compiled teacher?",
+            )
 
         teachers = teacher if isinstance(teacher, list) else [teacher]
         finetune_data = {}
 
         for teacher in teachers:
             # Dummy compilation to get bootstraps.
             compiled = self.teleprompter.compile(student, teacher=teacher, trainset=trainset)
             multitask = self.multitask
 
             # Prepare finetune <prompt, completion> pairs.
             for name, predictor in compiled.named_predictors():
-                name_ = 'all' if multitask else name
+                name_ = "all" if multitask else name
                 finetune_data[name_] = [] if name_ not in finetune_data else finetune_data[name_]
 
                 for demo in predictor.demos:
                     demo = dict(demo)
 
                     # TODO: FIXME: generalize.
                     template = signature_to_template(predictor.signature)
@@ -92,79 +108,82 @@
 
                     finetune_data[name_].append(dict(prompt=prompt, completion=completion))
 
         for name_ in finetune_data:
             random.Random(0).shuffle(finetune_data[name_])
             print(name_, len(finetune_data[name_]))
 
-
         #
         # Dump as files.
-        # 
+        #
         finetune_paths = {}
 
         for name in finetune_data:
             data = finetune_data[name]
-            hashed_name = name + '.' + Hasher.hash(data)
-            output_path = os.path.join(training_data_directory, f'{hashed_name}.jsonl')
+            hashed_name = name + "." + Hasher.hash(data)
+            output_path = os.path.join(training_data_directory, f"{hashed_name}.jsonl")
             print(output_path)
 
-            with open(output_path, 'w') as f:
+            with open(output_path, "w") as f:
                 for line in data:
-                    f.write(ujson.dumps(line) + '\n')
-            
+                    f.write(ujson.dumps(line) + "\n")
+
             finetune_paths[name] = output_path
-        
 
         #
         # Train!
         #
         import string
+
         compiler_config = {
-            'save': ''.join(random.Random(time.time()).choices(string.ascii_uppercase + string.digits, k=13)), # https://stackoverflow.com/a/2257449/1493011
-            'peft': peft,
-            'fp16': False,
-            'bf16': bf16,
-            'int8': int8,
-            'fid': False,
-            'rationale': False,
-            'batch_size': bsize,
-            'epochs': epochs,
-            'gradient_accumulation_steps': accumsteps, # 2,
-            'lr': lr,
+            "save": "".join(
+                random.Random(time.time()).choices(string.ascii_uppercase + string.digits, k=13),
+            ),  # https://stackoverflow.com/a/2257449/1493011
+            "peft": peft,
+            "fp16": False,
+            "bf16": bf16,
+            "int8": int8,
+            "fid": False,
+            "rationale": False,
+            "batch_size": bsize,
+            "epochs": epochs,
+            "gradient_accumulation_steps": accumsteps,  # 2,
+            "lr": lr,
         }
 
-        compiler_config['save'] = os.path.join(path_prefix, compiler_config['save']) if path_prefix else compiler_config['save']
+        compiler_config["save"] = (
+            os.path.join(path_prefix, compiler_config["save"]) if path_prefix else compiler_config["save"]
+        )
 
         from dsp.modules.finetuning import finetune_hf
 
         target = target
         finetune_models = {}
 
         for name in finetune_data:
             training_data_path = finetune_paths[name]
             compiler_config_ = dict(compiler_config)
-            compiler_config_['save'] = compiler_config['save'] + '.' + name
+            compiler_config_["save"] = compiler_config["save"] + "." + name
             best_ckpt_path = finetune_hf(training_data_path, target, compiler_config_)
 
             print(f"#> Best checkpoint path: {best_ckpt_path} for {name}")
-            finetune_models[name] = dsp.HFModel(model=target, checkpoint=best_ckpt_path) # best_ckpt_path
+            finetune_models[name] = dsp.HFModel(model=target, checkpoint=best_ckpt_path)  # best_ckpt_path
 
         #
         # Set the LMs to the finetuned ones, per module
         #
         compiled2 = compiled.reset_copy()
 
         assert len(compiled.named_predictors()) == len(compiled2.named_predictors())
 
         for (name, predictor), (name2, predictor2) in zip(compiled.named_predictors(), compiled2.named_predictors()):
             assert name == name2
-            name = 'all' if multitask else name
+            name = "all" if multitask else name
 
             # TODO: FIXME: When we assign .lm, the Predict.forward will also set only_query=True.
             # This is correct for here but we may want to make it more explicitly restricted to finetuned models.
             print(f"Assigning the LM of predictor {name}.")
 
             predictor2.lm = finetune_models[name]
             assert predictor2.demos == []
-        
+
         return compiled2
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/knn_fewshot.py` & `dspy-ai-2.4.3/dspy/teleprompt/knn_fewshot.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,12 +13,17 @@
 
     def compile(self, student, *, teacher=None, trainset, valset=None):
         student_copy = student.reset_copy()
 
         def forward_pass(*args, **kwargs):
             knn_trainset = self.KNN(**kwargs)
             few_shot_bootstrap = BootstrapFewShot()
-            compiled_program = few_shot_bootstrap.compile(student, teacher=teacher, trainset=knn_trainset, valset=valset)
+            compiled_program = few_shot_bootstrap.compile(
+                student,
+                teacher=teacher,
+                trainset=knn_trainset,
+                valset=valset,
+            )
             return compiled_program(**kwargs)
-        
+
         student_copy.forward = types.MethodType(forward_pass, student_copy)
-        return student_copy
+        return student_copy
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/mipro_optimizer.py` & `dspy-ai-2.4.3/dspy/teleprompt/mipro_optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import random
 import sys
 import textwrap
 from collections import defaultdict
+from typing import Any
 
 import optuna
 
 import dsp
 import dspy
 from dspy.evaluate.evaluate import Evaluate
 from dspy.signatures import Signature
@@ -39,123 +40,168 @@
                 and a value containing a dict with the following keys:
                     * program: the program being evaluated at a given trial
                     * score: the last average evaluated score for the program
                     * pruned: whether or not this program was pruned
                 This information will be returned as attributes of the best program.
 """
 
+
 class BasicGenerateInstruction(Signature):
     """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
 
     basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
     proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
+    proposed_prefix_for_output_field = dspy.OutputField(
+        desc="The string at the end of the prompt, which will help the model start solving the task",
+    )
+
 
 class BasicGenerateInstructionWithDataObservations(Signature):
     """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English.  I will also give you some ``observations`` I have made about the dataset and task. Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
 
     basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
     observations = dspy.InputField(desc="Observations about the dataset and task")
     proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
+    proposed_prefix_for_output_field = dspy.OutputField(
+        desc="The string at the end of the prompt, which will help the model start solving the task",
+    )
+
 
 class BasicGenerateInstructionWithExamples(dspy.Signature):
-        ("""You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will also provide you with the current ``basic instruction`` that is being used for this task. I will also provide you with some ``examples`` of the expected inputs and outputs.
+    """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will also provide you with the current ``basic instruction`` that is being used for this task. I will also provide you with some ``examples`` of the expected inputs and outputs.
+
+    Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
+
+    # attempted_instructions = dspy.InputField(format=str, desc="Previously attempted task instructions, along with their resulting validation score, and an example of the instruction in use on a sample from our dataset.")
+    basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
+    # examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
+    examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
+    proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
+    proposed_prefix_for_output_field = dspy.OutputField(
+        desc="The string at the end of the prompt, which will help the model start solving the task",
+    )
 
-Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative.""")
-        # attempted_instructions = dspy.InputField(format=str, desc="Previously attempted task instructions, along with their resulting validation score, and an example of the instruction in use on a sample from our dataset.")
-        basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
-        # examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
-        examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
-        proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-        proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class BasicGenerateInstructionWithExamplesAndDataObservations(dspy.Signature):
-        ("""You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will give you some ``observations`` I have made about the dataset and task, along with some ``examples`` of the expected inputs and outputs. I will also provide you with the current ``basic instruction`` that is being used for this task.
+    """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will give you some ``observations`` I have made about the dataset and task, along with some ``examples`` of the expected inputs and outputs. I will also provide you with the current ``basic instruction`` that is being used for this task.
+
+    Your task is to propose a new improved instruction and prefix for the output field that will lead a good language model to perform the task well. Don't be afraid to be creative."""
+
+    observations = dspy.InputField(desc="Observations about the dataset and task")
+    examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
+    basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
+    proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
+    proposed_prefix_for_output_field = dspy.OutputField(
+        desc="The string at the end of the prompt, which will help the model start solving the task",
+    )
 
-Your task is to propose a new improved instruction and prefix for the output field that will lead a good language model to perform the task well. Don't be afraid to be creative.""")
-        observations = dspy.InputField(desc="Observations about the dataset and task")
-        examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
-        basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
-        proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-        proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class ObservationSummarizer(dspy.Signature):
-    ("""Given a series of observations I have made about my dataset, please summarize them into a brief 2-3 sentence summary which highlights only the most important details.""")
+    """Given a series of observations I have made about my dataset, please summarize them into a brief 2-3 sentence summary which highlights only the most important details."""
+
     observations = dspy.InputField(desc="Observations I have made about my dataset")
-    summary = dspy.OutputField(desc="Two to Three sentence summary of only the most significant highlights of my observations")
+    summary = dspy.OutputField(
+        desc="Two to Three sentence summary of only the most significant highlights of my observations",
+    )
+
 
 class DatasetDescriptor(dspy.Signature):
-    ("""Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
-    """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
-    """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative""")
-    
+    (
+        """Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
+        """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
+        """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative"""
+    )
+
     examples = dspy.InputField(desc="Sample data points from the dataset")
     observations = dspy.OutputField(desc="Somethings that holds true for most or all of the data you observed")
 
+
 class DatasetDescriptorWithPriorObservations(dspy.Signature):
-    ("""Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
-    """I will also provide you with a few observations I have already made.  Please add your own observations or if you feel the observations are comprehensive say 'COMPLETE' """
-    """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
-    """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative""")
-    
+    (
+        """Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
+        """I will also provide you with a few observations I have already made.  Please add your own observations or if you feel the observations are comprehensive say 'COMPLETE' """
+        """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
+        """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative"""
+    )
+
     examples = dspy.InputField(desc="Sample data points from the dataset")
     prior_observations = dspy.InputField(desc="Some prior observations I made about the data")
-    observations = dspy.OutputField(desc="Somethings that holds true for most or all of the data you observed or COMPLETE if you have nothing to add")
+    observations = dspy.OutputField(
+        desc="Somethings that holds true for most or all of the data you observed or COMPLETE if you have nothing to add",
+    )
+
 
 class MIPRO(Teleprompter):
-    def __init__(self, metric, prompt_model=None, task_model=None, teacher_settings={}, num_candidates=10, init_temperature=1.0, verbose=False, track_stats=True, view_data_batch_size=10):
+    def __init__(
+        self,
+        metric,
+        prompt_model=None,
+        task_model=None,
+        teacher_settings={},
+        num_candidates=10,
+        init_temperature=1.0,
+        verbose=False,
+        track_stats=True,
+        view_data_batch_size=10,
+    ):
         self.num_candidates = num_candidates
         self.metric = metric
         self.init_temperature = init_temperature
         self.prompt_model = prompt_model if prompt_model is not None else dspy.settings.lm
         self.task_model = task_model if task_model is not None else dspy.settings.lm
         self.verbose = verbose
         self.track_stats = track_stats
         self.teacher_settings = teacher_settings
         self.view_data_batch_size = view_data_batch_size
-        
+
     def _print_full_program(self, program):
-        for i,predictor in enumerate(program.predictors()):
-            if self.verbose: print(f"Predictor {i}")
-            if self.verbose: print(f"i: {self._get_signature(predictor).instructions}")
+        for i, predictor in enumerate(program.predictors()):
+            if self.verbose:
+                print(f"Predictor {i}")
+            if self.verbose:
+                print(f"i: {self._get_signature(predictor).instructions}")
             *_, last_field = self._get_signature(predictor).fields.values()
-            if self.verbose: print(f"p: {last_field.json_schema_extra['prefix']}")
-            if self.verbose: print("\n")
-    
+            if self.verbose:
+                print(f"p: {last_field.json_schema_extra['prefix']}")
+            if self.verbose:
+                print("\n")
+
     def _print_model_history(self, model, n=1):
-        if self.verbose: print(f"Model ({model}) History:")
+        if self.verbose:
+            print(f"Model ({model}) History:")
         model.inspect_history(n=n)
 
     def _observe_data(self, trainset, max_iterations=10):
         upper_lim = min(len(trainset), self.view_data_batch_size)
         observation = dspy.Predict(DatasetDescriptor, n=1, temperature=1.0)(examples=(trainset[0:upper_lim].__repr__()))
         observations = observation["observations"]
 
         skips = 0
         iterations = 0
         for b in range(self.view_data_batch_size, len(trainset), self.view_data_batch_size):
-            upper_lim = min(len(trainset), b+self.view_data_batch_size)
-            output = dspy.Predict(DatasetDescriptorWithPriorObservations, n=1, temperature=1.0)(prior_observations=observations, examples=(trainset[b:upper_lim].__repr__()))
+            upper_lim = min(len(trainset), b + self.view_data_batch_size)
+            output = dspy.Predict(DatasetDescriptorWithPriorObservations, n=1, temperature=1.0)(
+                prior_observations=observations,
+                examples=(trainset[b:upper_lim].__repr__()),
+            )
             iterations += 1
             if len(output["observations"]) >= 8 and output["observations"][:8].upper() == "COMPLETE":
                 skips += 1
                 if skips >= 5:
                     break
                 continue
             if iterations >= max_iterations:
                 break
             observations += output["observations"]
 
         summary = dspy.Predict(ObservationSummarizer, n=1, temperature=1.0)(observations=observations)
 
         return summary.summary
-    
-    def _create_example_string(self, fields, example):
 
+    def _create_example_string(self, fields, example):
         # Building the output string
         output = []
         for field in fields:
             name = field.name
             separator = field.separator
             input_variable = field.input_variable
 
@@ -163,71 +209,79 @@
             value = example.get(input_variable)
 
             # Construct the string for the current field
             field_str = f"{name}{separator}{value}"
             output.append(field_str)
 
         # Joining all the field strings
-        return '\n'.join(output)
+        return "\n".join(output)
 
     def _get_signature(self, predictor):
-        if (hasattr(predictor, 'extended_signature')):
+        if hasattr(predictor, "extended_signature"):
             return predictor.extended_signature
-        elif (hasattr(predictor, 'signature')):
+        elif hasattr(predictor, "signature"):
             return predictor.signature
-    
+        return None
+
     def _set_signature(self, predictor, updated_signature):
-        if (hasattr(predictor, 'extended_signature')):
+        if hasattr(predictor, "extended_signature"):
             predictor.extended_signature = updated_signature
-        elif (hasattr(predictor, 'signature')):
+        elif hasattr(predictor, "signature"):
             predictor.signature = updated_signature
-    
-    def _generate_first_N_candidates(self, module, N, view_data, view_examples, demo_candidates, devset):
+
+    def _generate_first_N_candidates(  # noqa: N802
+        self,
+        module: dspy.Module,
+        N: int,  # noqa: N803
+        view_data: bool,
+        view_examples: bool,
+        demo_candidates: dict,
+        devset,
+    ) -> tuple[dict, dict]:
         candidates = {}
         evaluated_candidates = defaultdict(dict)
 
         if view_data:
             # Create data observations
             self.observations = None
             with dspy.settings.context(lm=self.prompt_model):
-                self.observations = self._observe_data(devset).replace("Observations:","").replace("Summary:","")
-            
+                self.observations = self._observe_data(devset).replace("Observations:", "").replace("Summary:", "")
+
         if view_examples:
             example_sets = {}
             for predictor in module.predictors():
                 # Get all augmented examples
                 example_set = {}
-                all_sets_of_examples = demo_candidates[id(predictor)] # Get all generated sets of examples
+                all_sets_of_examples = demo_candidates[id(predictor)]  # Get all generated sets of examples
                 for example_set_i, set_of_examples in enumerate(all_sets_of_examples):
-                    if example_set_i != 0: # Skip the no examples case
-                        for example in set_of_examples: # Get each individual example in the set
-                            if "augmented" in example.keys():
-                                if example["augmented"]:
-                                    if example_set_i not in example_set:
-                                        example_set[example_set_i] = []
-                                    fields_to_use = signature_to_template(predictor.signature).fields
-                                    input_variable_names = list(self._get_signature(predictor).input_fields.keys())
-                                    example_string = self._create_example_string(fields_to_use, example)
-                                    example_set[example_set_i].append(example_string)
-                        example_sets[id(predictor)] = example_set  
+                    if example_set_i != 0:  # Skip the no examples case
+                        for example in set_of_examples:  # Get each individual example in the set
+                            if "augmented" in example and example["augmented"]:
+                                if example_set_i not in example_set:
+                                    example_set[example_set_i] = []
+                                fields_to_use = signature_to_template(predictor.signature).fields
+                                _input_variable_names = list(self._get_signature(predictor).input_fields.keys())
+                                example_string = self._create_example_string(fields_to_use, example)
+                                example_set[example_set_i].append(example_string)
+                        example_sets[id(predictor)] = example_set
                     else:
                         example_set[example_set_i] = []
                         example_sets[id(predictor)] = example_set
 
         # Seed the prompt optimizer zero shot with just the instruction, generate BREADTH new prompts
         for predictor in module.predictors():
             basic_instruction = None
             basic_prefix = None
             basic_instruction = self._get_signature(predictor).instructions
             *_, last_field = self._get_signature(predictor).fields.values()
             basic_prefix = last_field.json_schema_extra["prefix"]
             with dspy.settings.context(lm=self.prompt_model):
                 # Data & Examples
                 if view_data and view_examples:
-                    if 1 not in example_sets[id(predictor)].keys():
+                    if 1 not in example_sets[id(predictor)]:
                         raise ValueError("No examples found for the given predictor")
                     instruct = None
                     for i in range(1, self.num_candidates):
                         new_instruct = dspy.Predict(
                             BasicGenerateInstructionWithExamplesAndDataObservations,
                             n=1,
                             temperature=self.init_temperature,
@@ -235,61 +289,91 @@
                             basic_instruction=basic_instruction,
                             observations=self.observations,
                             examples=example_sets[id(predictor)][i],
                         )
                         if not instruct:
                             instruct = new_instruct
                         else:
-                            instruct.completions.proposed_instruction.extend(new_instruct.completions.proposed_instruction)
-                            instruct.completions.proposed_prefix_for_output_field.extend(new_instruct.completions.proposed_prefix_for_output_field)
+                            instruct.completions.proposed_instruction.extend(
+                                new_instruct.completions.proposed_instruction,
+                            )
+                            instruct.completions.proposed_prefix_for_output_field.extend(
+                                new_instruct.completions.proposed_prefix_for_output_field,
+                            )
                 # Just data
-                elif view_data: 
-                    instruct = dspy.Predict(BasicGenerateInstructionWithDataObservations, n=N-1, temperature=self.init_temperature)(basic_instruction=basic_instruction, observations=self.observations)
+                elif view_data:
+                    instruct = dspy.Predict(
+                        BasicGenerateInstructionWithDataObservations,
+                        n=N - 1,
+                        temperature=self.init_temperature,
+                    )(basic_instruction=basic_instruction, observations=self.observations)
                 # Just examples
-                elif view_examples: 
+                elif view_examples:
                     instruct = None
-                    for i in range(1,self.num_candidates): # Note: skip over the first example set which is empty
+                    for i in range(1, self.num_candidates):  # Note: skip over the first example set which is empty
                         new_instruct = dspy.Predict(
                             BasicGenerateInstructionWithExamples,
                             n=1,
                             temperature=self.init_temperature,
                         )(
                             basic_instruction=basic_instruction,
                             examples=example_sets[id(predictor)][i],
                         )
                         if not instruct:
                             instruct = new_instruct
                         else:
-                            instruct.completions.proposed_instruction.extend(new_instruct.completions.proposed_instruction)
-                            instruct.completions.proposed_prefix_for_output_field.extend(new_instruct.completions.proposed_prefix_for_output_field)
+                            instruct.completions.proposed_instruction.extend(
+                                new_instruct.completions.proposed_instruction,
+                            )
+                            instruct.completions.proposed_prefix_for_output_field.extend(
+                                new_instruct.completions.proposed_prefix_for_output_field,
+                            )
                 # Neither
-                else: 
-                    instruct = dspy.Predict(BasicGenerateInstruction, n=N-1, temperature=self.init_temperature)(basic_instruction=basic_instruction)
-            
+                else:
+                    instruct = dspy.Predict(BasicGenerateInstruction, n=N - 1, temperature=self.init_temperature)(
+                        basic_instruction=basic_instruction,
+                    )
+
             # Add in our initial prompt as a candidate as well
             instruct.completions.proposed_instruction.insert(0, basic_instruction)
             instruct.completions.proposed_prefix_for_output_field.insert(0, basic_prefix)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
-        
-        if self.verbose: self._print_model_history(self.prompt_model)
-        
+
+        if self.verbose:
+            self._print_model_history(self.prompt_model)
+
         return candidates, evaluated_candidates
 
-    def compile(self, student, *, trainset, num_trials, max_bootstrapped_demos, max_labeled_demos, eval_kwargs, seed=42, view_data=True, view_examples=True, requires_permission_to_run=True):
+    def compile(
+        self,
+        student: dspy.Program,
+        *,
+        trainset: list[dspy.Example],
+        num_trials: int,
+        max_bootstrapped_demos: int,
+        max_labeled_demos: int,
+        eval_kwargs: dict[str, Any],
+        seed=42,
+        view_data=True,
+        view_examples=True,
+        requires_permission_to_run=True,
+    ) -> dspy.Program:
         # Define ANSI escape codes for colors
-        YELLOW = '\033[93m'
-        BLUE = '\033[94m'
-        BOLD = '\033[1m'
-        ENDC = '\033[0m'  # Resets the color to default
+        YELLOW = "\033[93m"
+        BLUE = "\033[94m"
+        BOLD = "\033[1m"
+        ENDC = "\033[0m"  # Resets the color to default
 
         random.seed(seed)
-        
+
         estimated_task_model_calls_wo_module_calls = len(trainset) * num_trials  # M * T * P
-        estimated_prompt_model_calls = 10 + self.num_candidates * len(student.predictors()) # num data summary calls + N * P
+        estimated_prompt_model_calls = 10 + self.num_candidates * len(
+            student.predictors(),
+        )  # num data summary calls + N * P
 
         user_message = textwrap.dedent(f"""\
             {YELLOW}{BOLD}WARNING: Projected Language Model (LM) Calls{ENDC}
 
             Please be advised that based on the parameters you have set, the maximum number of LM calls is projected as follows:
 
             {YELLOW}- Task Model: {BLUE}{BOLD}{len(trainset)}{ENDC}{YELLOW} examples in dev set * {BLUE}{BOLD}{num_trials}{ENDC}{YELLOW} trials * {BLUE}{BOLD}# of LM calls in your program{ENDC}{YELLOW} = ({BLUE}{BOLD}{estimated_task_model_calls_wo_module_calls} * # of LM calls in your program{ENDC}{YELLOW}) task model calls{ENDC}
@@ -301,177 +385,212 @@
                         + (Number of calls to prompt model * (Avg Input Token Length per Call * Task Prompt Price per Input Token + Avg Output Token Length per Call * Prompt Model Price per Output Token).{ENDC}
 
             For a preliminary estimate of potential costs, we recommend you perform your own calculations based on the task
             and prompt models you intend to use. If the projected costs exceed your budget or expectations, you may consider:
 
             {YELLOW}- Reducing the number of trials (`num_trials`), the size of the trainset, or the number of LM calls in your program.{ENDC}
             {YELLOW}- Using a cheaper task model to optimize the prompt.{ENDC}""")
-        
+
         user_confirmation_message = textwrap.dedent(f"""\
             To proceed with the execution of this program, please confirm by typing {BLUE}'y'{ENDC} for yes or {BLUE}'n'{ENDC} for no.
 
             If you would like to bypass this confirmation step in future executions, set the {YELLOW}`requires_permission_to_run`{ENDC} flag to {YELLOW}`False`.{ENDC}
 
             {YELLOW}Awaiting your input...{ENDC}
         """)
 
         print(user_message)
-        
-        sys.stdout.flush()  # Flush the output buffer to force the message to print
 
+        sys.stdout.flush()  # Flush the output buffer to force the message to print
 
-        run=True
+        run = True
         if requires_permission_to_run:
             print(user_confirmation_message)
             user_input = input("Do you wish to continue? (y/n): ").strip().lower()
-            if user_input != 'y':
+            if user_input != "y":
                 print("Compilation aborted by the user.")
-                run=False
+                run = False
 
         if run:
             # Set up program and evaluation function
             module = student.deepcopy()
             evaluate = Evaluate(devset=trainset, metric=self.metric, **eval_kwargs)
-            
+
             # In the case where the bootstrapped and labeled demos are set to 0, we'll stil bootstrap examples to use in our meta prompt
-            if max_bootstrapped_demos==0 and max_labeled_demos==0: #TODO: address case when max_bootstrapped alone is 0
-                max_bootstrapped_demos_for_candidate_gen = 1 
-                max_labeled_demos_for_candidate_gen = 1 #TODO: this might only need to be 0
+            if (
+                max_bootstrapped_demos == 0 and max_labeled_demos == 0
+            ):  # TODO: address case when max_bootstrapped alone is 0
+                max_bootstrapped_demos_for_candidate_gen = 1
+                max_labeled_demos_for_candidate_gen = 1  # TODO: this might only need to be 0
             else:
-                max_bootstrapped_demos_for_candidate_gen = max_bootstrapped_demos 
+                max_bootstrapped_demos_for_candidate_gen = max_bootstrapped_demos
                 max_labeled_demos_for_candidate_gen = max_labeled_demos
 
             # Generate N few shot example sets
             demo_candidates = {}
             for i in range(self.num_candidates):
-                if i == 0: # Story empty set of demos as default for index 0
+                if i == 0:  # Story empty set of demos as default for index 0
                     for module_p in module.predictors():
                         if id(module_p) not in demo_candidates:
                             demo_candidates[id(module_p)] = []
                         demo_candidates[id(module_p)].append([])
                 else:
-                    if self.verbose: print(f"Creating basic bootstrap: {i}/{self.num_candidates-1}")
+                    if self.verbose:
+                        print(f"Creating basic bootstrap: {i}/{self.num_candidates-1}")
 
                     # Create a new basic bootstrap few - shot program .
                     rng = random.Random(i)
                     shuffled_trainset = trainset[:]  # Create a copy of devset
                     rng.shuffle(shuffled_trainset)  # Shuffle the copy
-                    tp = BootstrapFewShot(metric = self.metric, max_bootstrapped_demos=max_bootstrapped_demos_for_candidate_gen, max_labeled_demos=max_labeled_demos_for_candidate_gen, teacher_settings=self.teacher_settings)
+                    tp = BootstrapFewShot(
+                        metric=self.metric,
+                        max_bootstrapped_demos=max_bootstrapped_demos_for_candidate_gen,
+                        max_labeled_demos=max_labeled_demos_for_candidate_gen,
+                        teacher_settings=self.teacher_settings,
+                    )
                     candidate_program = tp.compile(student=module.deepcopy(), trainset=shuffled_trainset)
 
                     # Store the candidate demos
                     for module_p, candidate_p in zip(module.predictors(), candidate_program.predictors()):
                         if id(module_p) not in demo_candidates:
                             demo_candidates[id(module_p)] = []
                         demo_candidates[id(module_p)].append(candidate_p.demos)
-                
+
             # Generate N candidate prompts
-            instruction_candidates, _ = self._generate_first_N_candidates(module, self.num_candidates, view_data, view_examples, demo_candidates, trainset)
+            instruction_candidates, _ = self._generate_first_N_candidates(
+                module,
+                self.num_candidates,
+                view_data,
+                view_examples,
+                demo_candidates,
+                trainset,
+            )
 
             # Reset demo_candidates to None for our optimization if the user asked for no fewshot examples
-            if max_bootstrapped_demos==0 and max_labeled_demos==0:
+            if max_bootstrapped_demos == 0 and max_labeled_demos == 0:
                 demo_candidates = None
 
             # Initialize variables to store the best program and its score
-            best_score = float('-inf')
+            best_score = float("-inf")
             best_program = None
             trial_num = 0
 
             trial_logs = {}
 
             # Define our trial objective
             def create_objective(baseline_program, instruction_candidates, demo_candidates, evaluate, trainset):
                 def objective(trial):
                     nonlocal best_program, best_score, trial_num, trial_logs  # Allow access to the outer variables
                     candidate_program = baseline_program.deepcopy()
 
-                    # Suggest the instruction to use for our predictor 
+                    # Suggest the instruction to use for our predictor
                     print(f"Starting trial #{trial_num}")
                     trial_logs[trial_num] = {}
 
                     for p_old, p_new in zip(baseline_program.predictors(), candidate_program.predictors()):
-
                         # Get instruction candidates for our given predictor
                         p_instruction_candidates = instruction_candidates[id(p_old)]
-                        if demo_candidates: p_demo_candidates = demo_candidates[id(p_old)]
+                        if demo_candidates:
+                            p_demo_candidates = demo_candidates[id(p_old)]
 
                         # Suggest the index of the instruction candidate to use in our trial
-                        instruction_idx = trial.suggest_categorical(f"{id(p_old)}_predictor_instruction",range(len(p_instruction_candidates)))
-                        if demo_candidates: demos_idx = trial.suggest_categorical(f"{id(p_old)}_predictor_demos",range(len(p_demo_candidates)))
+                        instruction_idx = trial.suggest_categorical(
+                            f"{id(p_old)}_predictor_instruction",
+                            range(len(p_instruction_candidates)),
+                        )
+                        if demo_candidates:
+                            demos_idx = trial.suggest_categorical(
+                                f"{id(p_old)}_predictor_demos",
+                                range(len(p_demo_candidates)),
+                            )
                         trial_logs[trial_num][f"{id(p_old)}_predictor_instruction"] = instruction_idx
-                        if demo_candidates: trial_logs[trial_num][f"{id(p_old)}_predictor_demos"] = demos_idx
+                        if demo_candidates:
+                            trial_logs[trial_num][f"{id(p_old)}_predictor_demos"] = demos_idx
 
-                        # Get the selected instruction candidate 
+                        # Get the selected instruction candidate
                         selected_candidate = p_instruction_candidates[instruction_idx]
                         selected_instruction = selected_candidate.proposed_instruction.strip('"').strip()
                         selected_prefix = selected_candidate.proposed_prefix_for_output_field.strip('"').strip()
 
                         # Use this candidates in our program
                         *_, last_field = self._get_signature(p_new).fields.keys()
-                        updated_signature = self._get_signature(p_new).with_instructions(selected_instruction).with_updated_fields(last_field, prefix=selected_prefix)
+                        updated_signature = (
+                            self._get_signature(p_new)
+                            .with_instructions(selected_instruction)
+                            .with_updated_fields(last_field, prefix=selected_prefix)
+                        )
                         self._set_signature(p_new, updated_signature)
 
                         # Get the selected demos
-                        if demo_candidates: selected_demos = p_demo_candidates[demos_idx]
+                        if demo_candidates:
+                            selected_demos = p_demo_candidates[demos_idx]
 
                         # Use these demos in our program
-                        if demo_candidates: p_new.demos = selected_demos
-                        
-                    if self.verbose: print("Evaling the following program:")
-                    if self.verbose: self._print_full_program(candidate_program)
+                        if demo_candidates:
+                            p_new.demos = selected_demos
+
+                    if self.verbose:
+                        print("Evaling the following program:")
+                    if self.verbose:
+                        self._print_full_program(candidate_program)
                     trial_logs[trial_num]["program"] = candidate_program
 
                     # Evaluate with the new prompts
                     total_score = 0
                     batch_size = 100
                     num_batches = math.ceil(len(trainset) / batch_size)
 
                     for i in range(num_batches):
                         start_index = i * batch_size
                         end_index = min((i + 1) * batch_size, len(trainset))
                         split_trainset = trainset[start_index:end_index]
                         split_score = evaluate(candidate_program, devset=split_trainset, display_table=0)
-                        if self.verbose: print(f"{i}st split score: {split_score}")
+                        if self.verbose:
+                            print(f"{i}st split score: {split_score}")
 
                         total_score += split_score * len(split_trainset)
-                        curr_weighted_avg_score = total_score / min((i+1)*100,len(trainset))
-                        if self.verbose: print(f"curr average score: {curr_weighted_avg_score}")
+                        curr_weighted_avg_score = total_score / min((i + 1) * 100, len(trainset))
+                        if self.verbose:
+                            print(f"curr average score: {curr_weighted_avg_score}")
 
                         trial.report(curr_weighted_avg_score, i)
 
                         # Handle pruning based on the intermediate value.
                         if trial.should_prune():
                             print("Trial pruned.")
                             trial_logs[trial_num]["score"] = curr_weighted_avg_score
                             trial_logs[trial_num]["pruned"] = True
-                            trial_num += 1 
+                            trial_num += 1
                             raise optuna.TrialPruned()
-                    
-                    if self.verbose: print(f"Fully evaled score: {curr_weighted_avg_score}")
-                    if self.verbose: self._print_model_history(self.task_model, n=1)
+
+                    if self.verbose:
+                        print(f"Fully evaled score: {curr_weighted_avg_score}")
+                    if self.verbose:
+                        self._print_model_history(self.task_model, n=1)
                     score = curr_weighted_avg_score
-                    
+
                     trial_logs[trial_num]["score"] = curr_weighted_avg_score
                     trial_logs[trial_num]["pruned"] = False
-                    
+
                     # Update the best program if the current score is better
                     if score > best_score:
                         best_score = score
                         best_program = candidate_program.deepcopy()
-                    
-                    trial_num += 1 
+
+                    trial_num += 1
 
                     return score
 
                 return objective
 
-            # Run the trial 
+            # Run the trial
             objective_function = create_objective(module, instruction_candidates, demo_candidates, evaluate, trainset)
             sampler = optuna.samplers.TPESampler(seed=seed)
             study = optuna.create_study(direction="maximize", sampler=sampler)
-            score = study.optimize(objective_function, n_trials=num_trials)
+            _score = study.optimize(objective_function, n_trials=num_trials)
 
             if best_program is not None and self.track_stats:
                 best_program.trial_logs = trial_logs
 
             print(f"Returning {best_program} from continue_program")
-            return best_program
+            return best_program
+        return None
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/random_search.py` & `dspy-ai-2.4.3/dspy/teleprompt/random_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,27 @@
 # Progressive elimination sounds about right: after 50 examples, drop bottom third, after 100, another third, etc.
 # until only 3--5 are left for the end. Could also be systematic and add (earlier) stopping based on error bounds.
 # In general, though, the early filtering is just saying: either there are some really bad ones, or some really really
 # good ones, or most things are pretty close. In all of these cases, dropping the bottom third is not going to hurt.
 
 
 class BootstrapFewShotWithRandomSearch(Teleprompter):
-    def __init__(self, metric, teacher_settings={}, max_bootstrapped_demos=4, max_labeled_demos=16, max_rounds=1, num_candidate_programs=16, num_threads=6, max_errors=10, stop_at_score=None, metric_threshold=None):
+    def __init__(
+        self,
+        metric,
+        teacher_settings={},
+        max_bootstrapped_demos=4,
+        max_labeled_demos=16,
+        max_rounds=1,
+        num_candidate_programs=16,
+        num_threads=6,
+        max_errors=10,
+        stop_at_score=None,
+        metric_threshold=None,
+    ):
         self.metric = metric
         self.teacher_settings = teacher_settings
         self.max_rounds = max_rounds
 
         self.num_threads = num_threads
         self.stop_at_score = stop_at_score
         self.metric_threshold = metric_threshold
@@ -60,92 +72,105 @@
                 continue
 
             trainset2 = list(self.trainset)
 
             if seed == -3:
                 # zero-shot
                 program2 = student.reset_copy()
-            
+
             elif seed == -2:
                 # labels only
                 teleprompter = LabeledFewShot(k=self.max_labeled_demos)
                 program2 = teleprompter.compile(student, trainset=trainset2, sample=labeled_sample)
-            
+
             elif seed == -1:
                 # unshuffled few-shot
-                program = BootstrapFewShot(metric=self.metric, metric_threshold=self.metric_threshold, max_bootstrapped_demos=self.max_num_samples,
-                                           max_labeled_demos=self.max_labeled_demos,
-                                           teacher_settings=self.teacher_settings, max_rounds=self.max_rounds)
+                program = BootstrapFewShot(
+                    metric=self.metric,
+                    metric_threshold=self.metric_threshold,
+                    max_bootstrapped_demos=self.max_num_samples,
+                    max_labeled_demos=self.max_labeled_demos,
+                    teacher_settings=self.teacher_settings,
+                    max_rounds=self.max_rounds,
+                )
                 program2 = program.compile(student, teacher=teacher, trainset=trainset2)
 
             else:
                 assert seed >= 0, seed
 
                 random.Random(seed).shuffle(trainset2)
                 size = random.Random(seed).randint(self.min_num_samples, self.max_num_samples)
 
-                teleprompter = BootstrapFewShot(metric=self.metric, metric_threshold=self.metric_threshold, max_bootstrapped_demos=size,
-                                                max_labeled_demos=self.max_labeled_demos,
-                                                teacher_settings=self.teacher_settings,
-                                                max_rounds=self.max_rounds)
+                teleprompter = BootstrapFewShot(
+                    metric=self.metric,
+                    metric_threshold=self.metric_threshold,
+                    max_bootstrapped_demos=size,
+                    max_labeled_demos=self.max_labeled_demos,
+                    teacher_settings=self.teacher_settings,
+                    max_rounds=self.max_rounds,
+                )
 
                 program2 = teleprompter.compile(student, teacher=teacher, trainset=trainset2)
 
-            evaluate = Evaluate(devset=self.valset, metric=self.metric, num_threads=self.num_threads,
-                                max_errors=self.max_errors, display_table=False, display_progress=True)
+            evaluate = Evaluate(
+                devset=self.valset,
+                metric=self.metric,
+                num_threads=self.num_threads,
+                max_errors=self.max_errors,
+                display_table=False,
+                display_progress=True,
+            )
 
             score, subscores = evaluate(program2, return_all_scores=True)
 
             all_subscores.append(subscores)
 
             ############ Assertion-aware Optimization ############
-            if hasattr(program2, '_suggest_failures'):
+            if hasattr(program2, "_suggest_failures"):
                 score = score - program2._suggest_failures * 0.2
-            if hasattr(program2, '_assert_failures'):
+            if hasattr(program2, "_assert_failures"):
                 score = 0 if program2._assert_failures > 0 else score
             ######################################################
 
-            print('Score:', score, 'for set:', [len(predictor.demos) for predictor in program2.predictors()])
+            print("Score:", score, "for set:", [len(predictor.demos) for predictor in program2.predictors()])
 
             if len(scores) == 0 or score > max(scores):
-                print('New best score:', score, 'for seed', seed)
+                print("New best score:", score, "for seed", seed)
                 best_program = program2
 
             scores.append(score)
             print(f"Scores so far: {scores}")
 
-            print('Best score:', max(scores))
+            print("Best score:", max(scores))
 
             score_data.append((score, subscores, seed, program2))
 
             if len(score_data) > 2:  # We check if there are at least 3 scores to consider
                 for k in [1, 2, 3, 5, 8, 9999]:
                     top_3_scores = sorted(score_data, key=lambda x: x[0], reverse=True)[:k]
 
                     # Transpose the subscores to get max per entry and then calculate their average
                     transposed_subscores = zip(*[subscores for _, subscores, *_ in top_3_scores if subscores])
                     avg_of_max_per_entry = sum(max(entry) for entry in transposed_subscores) / len(top_3_scores[0][1])
 
-                    print(f'Average of max per entry across top {k} scores: {avg_of_max_per_entry}')
-            
+                    print(f"Average of max per entry across top {k} scores: {avg_of_max_per_entry}")
+
             if self.stop_at_score is not None and score >= self.stop_at_score:
                 print(f"Stopping early because score {score} is >= stop_at_score {self.stop_at_score}")
                 break
 
         # To best program, attach all program candidates in decreasing average score
         best_program.candidate_programs = score_data
         best_program.candidate_programs = sorted(best_program.candidate_programs, key=lambda x: x[0], reverse=True)
 
         print(len(best_program.candidate_programs), "candidate programs found.")
 
         return best_program
 
 
-
-
 # sample between 4 and 10 examples from traces
 # TODO: FIXME: The max number of demos should be determined in part by the LM's tokenizer + max_length.
 # This does require executing the program, or at least the predictor.
 # # # # # # (Actually we can just combine the token counts of the traces, when formatted via signature/adapter).
 # Alternatively, we can keep track of the (zero-shot) number of tokens when we bootstrap.
 # As another option, we can just try a wide range and handle failures as penalties on the score.
 # The number "24" of traces to collect can also be affected. If we only need 3x10, some overlap is ok.
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/signature_opt.py` & `dspy-ai-2.4.3/dspy/teleprompt/signature_opt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from .copro_optimizer import COPRO
 
 """
 ===============================================================
 DEPRECATED!!!
 PLEASE USE COPRO INSTEAD.
 ===============================================================
@@ -28,14 +27,26 @@
                 If True, the method will track the following statistics:
                     * results_best: The min,max,avg,stddev of top 10 scores for each predictor at each depth.
                     * results_latest: The min,max,avg,stddev of newest prompt scores for each predictor at each depth.
                     * total_calls: The total number of calls to the task metric.
                 These statistics will be returned as attributes of the best program.
 """
 
+
 class SignatureOptimizer(COPRO):
-    def __init__(self, prompt_model=None, metric=None, breadth=10, depth=3, init_temperature=1.4, verbose=False, track_stats=False):
-        print("\u001b[31m[WARNING] SignatureOptimizer has been deprecated and replaced with COPRO.  SignatureOptimizer will be removed in a future release. \u001b[31m")
+    def __init__(
+        self,
+        prompt_model=None,
+        metric=None,
+        breadth=10,
+        depth=3,
+        init_temperature=1.4,
+        verbose=False,
+        track_stats=False,
+    ):
+        print(
+            "\u001b[31m[WARNING] SignatureOptimizer has been deprecated and replaced with COPRO.  SignatureOptimizer will be removed in a future release. \u001b[31m",
+        )
         super().__init__(prompt_model, metric, breadth, depth, init_temperature, verbose, track_stats)
 
     def compile(self, student, *, devset, eval_kwargs):
-        return super().compile(student, trainset=devset, eval_kwargs=eval_kwargs)
+        return super().compile(student, trainset=devset, eval_kwargs=eval_kwargs)
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/signature_opt_bayesian.py` & `dspy-ai-2.4.3/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dspy.teleprompt.mipro_optimizer import MIPRO
 
 """
 ===============================================================
 DEPRECATED!!!
 PLEASE USE MIPRO INSTEAD.
 ===============================================================
@@ -31,15 +30,64 @@
                 and a value containing a dict with the following keys:
                     * program: the program being evaluated at a given trial
                     * score: the last average evaluated score for the program
                     * pruned: whether or not this program was pruned
                 This information will be returned as attributes of the best program.
 """
 
-class BayesianSignatureOptimizer(MIPRO):
-    def __init__(self, prompt_model=None, task_model=None, teacher_settings={}, n=10, metric=None, init_temperature=1.0, verbose=False, track_stats=True, view_data_batch_size=10):
-        print("\u001b[31m[WARNING] BayesianSignatureOptimizer has been deprecated and replaced with MIPRO.  BayesianSignatureOptimizer will be removed in a future release. \u001b[31m")
-
-        super().__init__(prompt_model, task_model, teacher_settings,n,metric,init_temperature,verbose,track_stats,view_data_batch_size)
 
-    def compile(self, student, *, devset, max_bootstrapped_demos, max_labeled_demos, eval_kwargs, seed=42, optuna_trials_num, view_data=True, view_examples=True, requires_permission_to_run=False, num_trials=None):
-        return super().compile(student, trainset=devset, max_bootstrapped_demos=max_bootstrapped_demos, max_labeled_demos=max_labeled_demos, eval_kwargs=eval_kwargs, seed=seed, view_data=view_data, view_examples=view_examples, requires_permission_to_run=requires_permission_to_run, num_trials=optuna_trials_num)
+class BayesianSignatureOptimizer(MIPRO):
+    def __init__(
+        self,
+        prompt_model=None,
+        task_model=None,
+        teacher_settings={},
+        n=10,
+        metric=None,
+        init_temperature=1.0,
+        verbose=False,
+        track_stats=True,
+        view_data_batch_size=10,
+    ):
+        print(
+            "\u001b[31m[WARNING] BayesianSignatureOptimizer has been deprecated and replaced with MIPRO.  BayesianSignatureOptimizer will be removed in a future release. \u001b[31m",
+        )
+
+        super().__init__(
+            metric=metric,
+            prompt_model=prompt_model,
+            task_model=task_model,
+            teacher_settings=teacher_settings,
+            num_candidates=n,
+            init_temperature=init_temperature,
+            verbose=verbose,
+            track_stats=track_stats,
+            view_data_batch_size=view_data_batch_size,
+        )
+
+    def compile(
+        self,
+        student,
+        *,
+        devset,
+        max_bootstrapped_demos,
+        max_labeled_demos,
+        eval_kwargs,
+        seed=42,
+        optuna_trials_num,
+        view_data=True,
+        view_examples=True,
+        requires_permission_to_run=False,
+        num_trials=None,
+    ):
+        return super().compile(
+            student,
+            trainset=devset,
+            max_bootstrapped_demos=max_bootstrapped_demos,
+            max_labeled_demos=max_labeled_demos,
+            eval_kwargs=eval_kwargs,
+            seed=seed,
+            view_data=view_data,
+            view_examples=view_examples,
+            requires_permission_to_run=requires_permission_to_run,
+            num_trials=optuna_trials_num,
+        )
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/signature_opt_typed.py` & `dspy-ai-2.4.3/dspy/teleprompt/signature_opt_typed.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,17 +268,19 @@
                 new_signature = generator().proposed_signature
                 candidates[name].append(new_signature)
 
     if strategy == "last":
         pass
     elif strategy == "best":
         i = scores.index(max(scores))
+        if verbose:
+            print(f"Best signature: {i} with score: {scores[i]}")
         for name, p in named_predictors:
             p.signature = candidates[name][i].to_signature()
     else:
         raise ValueError(f"Invalid strategy: {strategy}")
 
     return OptimizerResult(
         program=module,
-        signatures=[{name: sigs[i].to_signature()} for name, sigs in candidates.items() for i in range(n_iterations)],
+        signatures=[{name: sigs[i].to_signature() for name, sigs in candidates.items()} for i in range(n_iterations)],
         scores=scores,
     )
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/teleprompt_optuna.py` & `dspy-ai-2.4.3/dspy/teleprompt/teleprompt_optuna.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,24 @@
 from dspy.evaluate.evaluate import Evaluate
 from dspy.teleprompt.teleprompt import Teleprompter
 
 from .bootstrap import BootstrapFewShot
 
 
 class BootstrapFewShotWithOptuna(Teleprompter):
-    def __init__(self, metric, teacher_settings={}, max_bootstrapped_demos=4, max_labeled_demos=16, max_rounds=1, num_candidate_programs=16, num_threads=6):
+    def __init__(
+        self,
+        metric,
+        teacher_settings={},
+        max_bootstrapped_demos=4,
+        max_labeled_demos=16,
+        max_rounds=1,
+        num_candidate_programs=16,
+        num_threads=6,
+    ):
         self.metric = metric
         self.teacher_settings = teacher_settings
         self.max_rounds = max_rounds
 
         self.num_threads = num_threads
 
         self.min_num_samples = 1
@@ -25,35 +34,46 @@
 
         print("Going to sample between", self.min_num_samples, "and", self.max_num_samples, "traces per predictor.")
         # print("Going to sample", self.max_num_traces, "traces in total.")
         print("Will attempt to train", self.num_candidate_sets, "candidate sets.")
 
     def objective(self, trial):
         program2 = self.student.reset_copy()
-        for (name, compiled_predictor), (_, program2_predictor) in zip(self.compiled_teleprompter.named_predictors(), program2.named_predictors()):
+        for (name, compiled_predictor), (_, program2_predictor) in zip(
+            self.compiled_teleprompter.named_predictors(), program2.named_predictors(),
+        ):
             all_demos = compiled_predictor.demos
             demo_index = trial.suggest_int(f"demo_index_for_{name}", 0, len(all_demos) - 1)
             selected_demo = dict(all_demos[demo_index])
             program2_predictor.demos = [selected_demo]
-        evaluate = Evaluate(devset=self.valset, metric=self.metric, num_threads=self.num_threads,
-                            display_table=False, display_progress=True)
+        evaluate = Evaluate(
+            devset=self.valset,
+            metric=self.metric,
+            num_threads=self.num_threads,
+            display_table=False,
+            display_progress=True,
+        )
         score, _ = evaluate(program2, return_all_scores=True)
         trial.set_user_attr("program", program2)
         return score
 
-
     def compile(self, student, *, teacher=None, max_demos, trainset, valset=None):
         self.trainset = trainset
         self.valset = valset or trainset
         self.student = student.reset_copy()
         self.teacher = teacher.deepcopy() if teacher is not None else student.reset_copy()
-        teleprompter_optimize = BootstrapFewShot(metric=self.metric, max_bootstrapped_demos=max_demos,
-                                        max_labeled_demos=self.max_labeled_demos,
-                                        teacher_settings=self.teacher_settings,
-                                        max_rounds=self.max_rounds)
-        self.compiled_teleprompter = teleprompter_optimize.compile(self.student, teacher=self.teacher, trainset=self.trainset)
-        study = optuna.create_study(direction='maximize')
+        teleprompter_optimize = BootstrapFewShot(
+            metric=self.metric,
+            max_bootstrapped_demos=max_demos,
+            max_labeled_demos=self.max_labeled_demos,
+            teacher_settings=self.teacher_settings,
+            max_rounds=self.max_rounds,
+        )
+        self.compiled_teleprompter = teleprompter_optimize.compile(
+            self.student, teacher=self.teacher, trainset=self.trainset,
+        )
+        study = optuna.create_study(direction="maximize")
         study.optimize(self.objective, n_trials=self.num_candidate_sets)
         best_program = study.trials[study.best_trial.number].user_attrs["program"]
-        print('Best score:', study.best_value)
-        print('Best program:', best_program)
-        return best_program
+        print("Best score:", study.best_value)
+        print("Best program:", best_program)
+        return best_program
```

### Comparing `dspy-ai-2.4.0/dspy/teleprompt/vanilla.py` & `dspy-ai-2.4.3/dspy/teleprompt/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
         rng = random.Random(0)
 
         for predictor in self.student.predictors():
             if sample:
                 predictor.demos = rng.sample(self.trainset, min(self.k, len(self.trainset)))
             else:
-                predictor.demos = self.trainset[:min(self.k, len(self.trainset))]
+                predictor.demos = self.trainset[: min(self.k, len(self.trainset))]
 
         return self.student
-    
+
+
 # NOTE: I believe templatev2 keeps rdemos as long as they have the last field.
 # This may change later, especially with the introduction of required vs optional fields.
 # NOTE: Since we're relying on downstream code to handle the demos, this sampling may be sub-sampled.
```

### Comparing `dspy-ai-2.4.0/dspy/utils/dummies.py` & `dspy-ai-2.4.3/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.0/dspy_ai.egg-info/PKG-INFO` & `dspy-ai-2.4.3/dspy_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.0
+Version: 2.4.3
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,15 @@
 Provides-Extra: chromadb
 Provides-Extra: qdrant
 Provides-Extra: marqo
 Provides-Extra: mongodb
 Provides-Extra: pinecone
 Provides-Extra: weaviate
 Provides-Extra: faiss-cpu
+Provides-Extra: anthropic
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
@@ -57,15 +58,16 @@
 
 If you need help thinking about your task, we recently created a [Discord server](https://discord.gg/VzS6RHHK6F) for the community.
 
 1. **[Installation](#1-installation)**
 1. **[Tutorials & Documentation](#2-documentation)**
 1. **[Framework Syntax](#3-syntax-youre-in-charge-of-the-workflowits-free-form-python-code)**
 1. **[Compiling: Two Powerful Concepts](#4-two-powerful-concepts-signatures--teleprompters)**
-1. **[FAQ: Is DSPy right for me?](#5-faq-is-dspy-right-for-me)**
+1. **[Pydantic Types](#5-pydantic-types)** 
+1. **[FAQ: Is DSPy right for me?](#6-faq-is-dspy-right-for-me)**
 
 
 
 ### Analogy to Neural Networks
 
 When we build neural networks, we don't write manual _for-loops_ over lists of _hand-tuned_ floats. Instead, you might use a framework like [PyTorch](https://pytorch.org/) to compose declarative layers (e.g., `Convolution` or `Dropout`) and then use optimizers (e.g., SGD or Adam) to learn the parameters of the network.
 
@@ -120,14 +122,15 @@
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
 - Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
+- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
```

### Comparing `dspy-ai-2.4.0/dspy_ai.egg-info/SOURCES.txt` & `dspy-ai-2.4.3/dspy_ai.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 README.md
 pyproject.toml
 setup.py
 dsp/__init__.py
 dsp/evaluation/__init__.py
 dsp/evaluation/utils.py
 dsp/modules/__init__.py
+dsp/modules/anthropic.py
 dsp/modules/aws_lm.py
 dsp/modules/azure_openai.py
 dsp/modules/azurecognitivesearch.py
 dsp/modules/bedrock.py
 dsp/modules/cache_utils.py
 dsp/modules/clarifai.py
 dsp/modules/cohere.py
 dsp/modules/colbertv2.py
 dsp/modules/databricks.py
 dsp/modules/google.py
 dsp/modules/gpt3.py
+dsp/modules/groq_client.py
 dsp/modules/hf.py
 dsp/modules/hf_client.py
 dsp/modules/hf_server.py
 dsp/modules/lm.py
+dsp/modules/mistral.py
 dsp/modules/ollama.py
 dsp/modules/pyserini.py
 dsp/modules/sbert.py
 dsp/modules/sentence_vectorizer.py
 dsp/modules/finetuning/__init__.py
 dsp/modules/finetuning/finetune_hf.py
 dsp/primitives/__init__.py
@@ -58,16 +61,21 @@
 dspy/datasets/gsm8k.py
 dspy/datasets/hotpotqa.py
 dspy/evaluate/__init__.py
 dspy/evaluate/auto_evaluation.py
 dspy/evaluate/evaluate.py
 dspy/evaluate/metrics.py
 dspy/experimental/__init__.py
-dspy/experimental/synthesizer.py
 dspy/experimental/synthetic_data.py
+dspy/experimental/synthesizer/__init__.py
+dspy/experimental/synthesizer/config.py
+dspy/experimental/synthesizer/instruction_suffixes.py
+dspy/experimental/synthesizer/signatures.py
+dspy/experimental/synthesizer/synthesizer.py
+dspy/experimental/synthesizer/utils.py
 dspy/functional/__init__.py
 dspy/functional/functional.py
 dspy/predict/__init__.py
 dspy/predict/aggregation.py
 dspy/predict/chain_of_thought.py
 dspy/predict/chain_of_thought_with_hint.py
 dspy/predict/knn.py
@@ -83,24 +91,27 @@
 dspy/primitives/box.py
 dspy/primitives/example.py
 dspy/primitives/module.py
 dspy/primitives/prediction.py
 dspy/primitives/program.py
 dspy/primitives/python_interpreter.py
 dspy/retrieve/__init__.py
+dspy/retrieve/azureaisearch_rm.py
 dspy/retrieve/chromadb_rm.py
 dspy/retrieve/clarifai_rm.py
 dspy/retrieve/databricks_rm.py
 dspy/retrieve/deeplake_rm.py
 dspy/retrieve/faiss_rm.py
 dspy/retrieve/marqo_rm.py
 dspy/retrieve/mongodb_atlas_rm.py
+dspy/retrieve/neo4j_rm.py
 dspy/retrieve/pgvector_rm.py
 dspy/retrieve/pinecone_rm.py
 dspy/retrieve/qdrant_rm.py
+dspy/retrieve/ragatouille_rm.py
 dspy/retrieve/retrieve.py
 dspy/retrieve/vectara_rm.py
 dspy/retrieve/weaviate_rm.py
 dspy/retrieve/weaviate_rm_test.py
 dspy/retrieve/you_rm.py
 dspy/signatures/__init__.py
 dspy/signatures/field.py
@@ -117,12 +128,13 @@
 dspy/teleprompt/signature_opt_bayesian.py
 dspy/teleprompt/signature_opt_typed.py
 dspy/teleprompt/teleprompt.py
 dspy/teleprompt/teleprompt_optuna.py
 dspy/teleprompt/vanilla.py
 dspy/utils/__init__.py
 dspy/utils/dummies.py
+dspy/utils/logging.py
 dspy_ai.egg-info/PKG-INFO
 dspy_ai.egg-info/SOURCES.txt
 dspy_ai.egg-info/dependency_links.txt
 dspy_ai.egg-info/requires.txt
 dspy_ai.egg-info/top_level.txt
```

### Comparing `dspy-ai-2.4.0/dspy_ai.egg-info/requires.txt` & `dspy-ai-2.4.3/dspy_ai.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 pandas
 regex
 ujson
 tqdm
 datasets<3.0.0,~=2.14.6
 requests
 optuna
-pydantic==2.5.0
+pydantic<=2.7,>=2.5.0
+
+[anthropic]
+anthropic~=0.18.0
 
 [chromadb]
 chromadb~=0.4.14
 
 [dev]
 pytest>=6.2.5
 
@@ -42,12 +45,13 @@
 
 [pinecone]
 pinecone-client~=2.2.4
 
 [qdrant]
 qdrant-client
 fastembed
-qdrant-client~=1.6.2
-fastembed~=0.1.0
+qdrant-client>=1.6.2
+fastembed>=0.1.0
 
 [weaviate]
 weaviate-client~=3.26.1
+weaviate-client~=4.5.4
```

### Comparing `dspy-ai-2.4.0/pyproject.toml` & `dspy-ai-2.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.4.0"
+version = "2.4.3"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.12"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",    # removed 3.8
     "Programming Language :: Python :: 3.9",
 ]
+
 # We have both project and tool.poetry.dependencies. Should we remove one?
+# tool.poetry.dependencies is a convenience thing for poetry users.
+# project dependencies function similarly to requirements.txt,
+# `pip install .` will pull from pyproject.toml dependencies
+
 dependencies = [
     "backoff~=2.2.1",
     "joblib~=1.3.2",
     "openai>=0.28.1,<2.0.0",
     "pandas",
     "regex",
     "ujson",
     "tqdm",
     "datasets~=2.14.6,<3.0.0",
     "requests",
     "optuna",
-    "pydantic==2.5.0",
+    "pydantic>=2.5.0,<=2.7",
 ]
 
 [project.optional-dependencies]
+anthropic = ["anthropic~=0.18.0"]
 chromadb = ["chromadb~=0.4.14"]
-qdrant = ["qdrant-client~=1.6.2", "fastembed~=0.1.0"]
+qdrant = ["qdrant-client>=1.6.2", "fastembed>=0.1.0"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client~=2.2.4"]
-weaviate = ["weaviate-client~=3.26.1"]
+weaviate = ["weaviate-client~=4.5.4"]
 docs = [
     "sphinx>=4.3.0",
     "furo>=2023.3.27",
     "docutils<0.17",
     "m2r2",
     "myst-parser",
     "myst-nb",
     "sphinx-autobuild",
     "sphinx_rtd_theme",
     "autodoc_pydantic",
     "sphinx-reredirects>=0.1.2",
     "sphinx-automodapi==0.16.0",
+    
 ]
 dev = ["pytest>=6.2.5"]
 
 [project.urls]
 homepage = "https://github.com/stanfordnlp/dspy"
 
 [tool.poetry]
@@ -69,55 +76,66 @@
 # documentation = "https://dspy-ai.readthedocs.io"
 keywords = ["dspy", "ai", "language models", "llm", "openai"]
 # may be a bit much
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = "2.5.0"
+pydantic = ">=2.5.0,<=2.7"
 backoff = "^2.2.1"
 joblib = "^1.3.2"
-openai = "^0.28.1"
+openai = ">=0.28.1,<2.0.0"
 pandas = "^2.1.1"
 regex = "^2023.10.3"
 ujson = "^5.8.0"
 tqdm = "^4.66.1"
 datasets = "^2.14.6"
 requests = "^2.31.0"
 optuna = "^3.4.0"
+anthropic = { version = "^0.18.0", optional = true }
 chromadb = { version = "^0.4.14", optional = true }
 fastembed = { version = "^0.1.0", optional = true }
 marqo = { version = "*", optional = true }
 qdrant-client = { version = "^1.6.2", optional = true }
 pinecone-client = { version = "^2.2.4", optional = true }
-weaviate-client = { version = "^3.26.1", optional = true }
+weaviate-client = { version = "^4.5.4", optional = true }
 sphinx = { version = ">=4.3.0", optional = true }
 furo = { version = ">=2023.3.27", optional = true }
 docutils = { version = "<0.17", optional = true }
 m2r2 = { version = "*", optional = true }
 myst-parser = { version = "*", optional = true }
 myst-nb = { version = "*", optional = true }
 sphinx-autobuild = { version = "*", optional = true }
 sphinx_rtd_theme = { version = "*", optional = true }
 autodoc_pydantic = { version = "*", optional = true }
 sphinx-reredirects = { version = "^0.1.2", optional = true }
 sphinx-automodapi = { version = "0.16.0", optional = true }
+groq = {version = "^0.4.2", optional = true }
+rich = "^13.7.1"
+psycopg2 = {version = "^2.9.9", optional = true}
+pgvector = {version = "^0.2.5", optional = true}
+structlog = "^24.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
+transformers = "^4.38.2"
+torch = "^2.2.1"
+pytest-mock = "^3.12.0"
 ruff = "^0.3.0"
-
+black = "^24.2.0"
+pre-commit = "^3.7.0"
 
 [tool.poetry.extras]
 chromadb = ["chromadb"]
 qdrant = ["qdrant-client", "fastembed"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client"]
 weaviate = ["weaviate-client"]
+postgres = ["psycopg2", "pgvector"]
 docs = [
     "sphinx",
     "furo",
     "docutils",
     "m2r2",
     "myst-parser",
     "myst-nb",
```

### Comparing `dspy-ai-2.4.0/setup.py` & `dspy-ai-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file	
 with open('requirements.txt', encoding='utf-8') as f:	
     requirements = f.read().splitlines()	
 
 setup(	
     name="dspy-ai",	
-    version="2.4.0",	
+    version="2.4.3",	
     description="DSPy",	
     long_description=long_description,	
     long_description_content_type='text/markdown',	
     url="https://github.com/stanfordnlp/dsp",	
     author="Omar Khattab",	
     author_email="okhattab@stanford.edu",	
     license="MIT License",
```

