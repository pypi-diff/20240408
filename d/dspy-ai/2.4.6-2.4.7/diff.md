# Comparing `tmp/dspy-ai-2.4.6.tar.gz` & `tmp/dspy-ai-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dspy-ai-2.4.6.tar", last modified: Mon Apr  8 19:45:44 2024, max compression
+gzip compressed data, was "dist/dspy-ai-2.4.7.tar", last modified: Mon Apr  8 20:57:43 2024, max compression
```

## Comparing `dspy-ai-2.4.6.tar` & `dspy-ai-2.4.7.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/
--rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.6/LICENSE
--rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)    34442 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/README.md
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/
--rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/evaluation/
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/evaluation/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/evaluation/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/modules/
--rw-r--r--   0 okhattab (19845) future   (20099)      446 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4547 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dsp/modules/anthropic.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/aws_lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/azure_openai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/azurecognitivesearch.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3102 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/bedrock.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1022 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dsp/modules/cache_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/clarifai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/cohere.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/colbertv2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/databricks.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/modules/finetuning/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/finetuning/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/finetuning/finetune_hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/google.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/gpt3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/hf_client.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/hf_server.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3258 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/modules/lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/ollama.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/pyserini.py
--rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/sbert.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/modules/sentence_vectorizer.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/primitives/compiler.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/primitives/demonstrate.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/primitives/inspect.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7948 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dsp/primitives/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/primitives/primitives.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dsp/primitives/search.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/templates/
--rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/templates/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/templates/template_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/templates/template_v3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/templates/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dsp/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/utils/ann_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/utils/dpr.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/utils/metrics.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3287 2024-04-08 17:29:25.000000 dspy-ai-2.4.6/dsp/utils/settings.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/utils/settings_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dsp/utils/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/
--rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/adapters/
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/adapters/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/adapters/basic_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/adapters/chatml_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/adapters/vicuna_adapter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/datasets/
--rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/datasets/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/datasets/colors.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/datasets/dataloader.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/datasets/dataset.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/datasets/gsm8k.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/datasets/hotpotqa.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/evaluate/
--rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/evaluate/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/evaluate/evaluate.py
--rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/evaluate/metrics.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/experimental/
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/experimental/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/config.py
--rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9542 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/experimental/synthetic_data.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/functional/
--rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/functional/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15805 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/functional/functional.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/predict/
--rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/aggregation.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/chain_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/knn.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/langchain.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/parameter.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/predict/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/predict/program_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/predict/react.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/predict/retry.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/assertions.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/box.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/example.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/primitives/module.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/prediction.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/program.py
--rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/primitives/python_interpreter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/retrieve/
--rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4793 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/databricks_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0 okhattab (19845) future   (20099)     6530 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/faiss_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/retrieve/marqo_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/retrieve.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/vectara_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/retrieve/you_rm.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/signatures/
--rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/signatures/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/signatures/field.py
--rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/signatures/signature.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/teleprompt/
--rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/teleprompt/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/bootstrap.py
--rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/ensemble.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/finetune.py
--rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/random_search.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/signature_opt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/teleprompt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 19:45:10.000000 dspy-ai-2.4.6/dspy/teleprompt/vanilla.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-04-08 17:11:57.000000 dspy-ai-2.4.6/dspy/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.6/dspy/utils/dummies.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/dspy_ai.egg-info/
--rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 19:45:43.000000 dspy-ai-2.4.6/dspy_ai.egg-info/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)     3752 2024-04-08 19:45:43.000000 dspy-ai-2.4.6/dspy_ai.egg-info/SOURCES.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 19:45:43.000000 dspy-ai-2.4.6/dspy_ai.egg-info/dependency_links.txt
--rw-r--r--   0 okhattab (19845) future   (20099)      635 2024-04-08 19:45:43.000000 dspy-ai-2.4.6/dspy_ai.egg-info/requires.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 19:45:43.000000 dspy-ai-2.4.6/dspy_ai.egg-info/top_level.txt
--rw-r--r--   0 okhattab (19845) future   (20099)     6888 2024-04-08 19:45:37.000000 dspy-ai-2.4.6/pyproject.toml
--rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 19:45:44.000000 dspy-ai-2.4.6/setup.cfg
--rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 19:45:28.000000 dspy-ai-2.4.6/setup.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.7/LICENSE
+-rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)    34442 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/README.md
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/evaluation/
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/evaluation/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/evaluation/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/modules/
+-rw-r--r--   0 okhattab (19845) future   (20099)      446 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4547 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dsp/modules/anthropic.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/aws_lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/azure_openai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/azurecognitivesearch.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3102 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/bedrock.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      964 2024-04-08 20:57:18.000000 dspy-ai-2.4.7/dsp/modules/cache_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/clarifai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/cohere.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/colbertv2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/databricks.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/modules/finetuning/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/finetuning/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/finetuning/finetune_hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/google.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/gpt3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/hf_client.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/hf_server.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3258 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/ollama.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/pyserini.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/sbert.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/sentence_vectorizer.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/compiler.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/demonstrate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/inspect.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7948 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dsp/primitives/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/primitives.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/primitives/search.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/templates/
+-rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/template_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/template_v3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/ann_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/dpr.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/metrics.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3287 2024-04-08 17:29:25.000000 dspy-ai-2.4.7/dsp/utils/settings.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/settings_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/
+-rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/adapters/
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/basic_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/chatml_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/llamachat_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/vicuna_adapter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/datasets/
+-rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/colors.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/datasets/dataloader.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/dataset.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/gsm8k.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/hotpotqa.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/evaluate/
+-rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/evaluate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/metrics.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/experimental/
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/experimental/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9542 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/experimental/synthetic_data.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/functional/
+-rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/functional/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15805 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/functional/functional.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/predict/
+-rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/aggregation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/chain_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/knn.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/langchain.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/parameter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/predict/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/predict/program_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/react.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/predict/retry.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/assertions.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/box.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/example.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/primitives/module.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/prediction.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/program.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/python_interpreter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/retrieve/
+-rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4793 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0 okhattab (19845) future   (20099)     6530 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/retrieve.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/you_rm.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/signatures/
+-rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/signatures/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/signatures/field.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/signatures/signature.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/teleprompt/
+-rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/teleprompt/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/ensemble.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/finetune.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/random_search.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/vanilla.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/utils/dummies.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy_ai.egg-info/
+-rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)     3752 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)      635 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/requires.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/top_level.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)     6888 2024-04-08 20:57:27.000000 dspy-ai-2.4.7/pyproject.toml
+-rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/setup.cfg
+-rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 20:57:37.000000 dspy-ai-2.4.7/setup.py
```

### Comparing `dspy-ai-2.4.6/LICENSE` & `dspy-ai-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/PKG-INFO` & `dspy-ai-2.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.6
+Version: 2.4.7
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dspy-ai-2.4.6/README.md` & `dspy-ai-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/__init__.py` & `dspy-ai-2.4.7/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/evaluation/utils.py` & `dspy-ai-2.4.7/dsp/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/anthropic.py` & `dspy-ai-2.4.7/dsp/modules/anthropic.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/aws_lm.py` & `dspy-ai-2.4.7/dsp/modules/aws_lm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/azure_openai.py` & `dspy-ai-2.4.7/dsp/modules/azure_openai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/azurecognitivesearch.py` & `dspy-ai-2.4.7/dsp/modules/azurecognitivesearch.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/bedrock.py` & `dspy-ai-2.4.7/dsp/modules/bedrock.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/cache_utils.py` & `dspy-ai-2.4.7/dsp/modules/cache_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import wraps
 from pathlib import Path
 
 from joblib import Memory
 
 from dsp.utils import dotdict
 
-cache_turn_on = not os.environ.get('DSP_CACHEBOOL', 'True').lower() == 'false'
+cache_turn_on = True
 
 
 def noop_decorator(arg=None, *noop_args, **noop_kwargs):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
```

### Comparing `dspy-ai-2.4.6/dsp/modules/clarifai.py` & `dspy-ai-2.4.7/dsp/modules/clarifai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/cohere.py` & `dspy-ai-2.4.7/dsp/modules/cohere.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/colbertv2.py` & `dspy-ai-2.4.7/dsp/modules/colbertv2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/databricks.py` & `dspy-ai-2.4.7/dsp/modules/databricks.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/finetuning/finetune_hf.py` & `dspy-ai-2.4.7/dsp/modules/finetuning/finetune_hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/google.py` & `dspy-ai-2.4.7/dsp/modules/google.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/gpt3.py` & `dspy-ai-2.4.7/dsp/modules/gpt3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/hf.py` & `dspy-ai-2.4.7/dsp/modules/hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/hf_client.py` & `dspy-ai-2.4.7/dsp/modules/hf_client.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/hf_server.py` & `dspy-ai-2.4.7/dsp/modules/hf_server.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/lm.py` & `dspy-ai-2.4.7/dsp/modules/lm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/ollama.py` & `dspy-ai-2.4.7/dsp/modules/ollama.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/pyserini.py` & `dspy-ai-2.4.7/dsp/modules/pyserini.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/sbert.py` & `dspy-ai-2.4.7/dsp/modules/sbert.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/modules/sentence_vectorizer.py` & `dspy-ai-2.4.7/dsp/modules/sentence_vectorizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/primitives/compiler.py` & `dspy-ai-2.4.7/dsp/primitives/compiler.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/primitives/demonstrate.py` & `dspy-ai-2.4.7/dsp/primitives/demonstrate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/primitives/inspect.py` & `dspy-ai-2.4.7/dsp/primitives/inspect.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/primitives/predict.py` & `dspy-ai-2.4.7/dsp/primitives/predict.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/primitives/primitives.py` & `dspy-ai-2.4.7/dsp/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/primitives/search.py` & `dspy-ai-2.4.7/dsp/primitives/search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/templates/template_v2.py` & `dspy-ai-2.4.7/dsp/templates/template_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/templates/template_v3.py` & `dspy-ai-2.4.7/dsp/templates/template_v3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/templates/utils.py` & `dspy-ai-2.4.7/dsp/templates/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/utils/ann_utils.py` & `dspy-ai-2.4.7/dsp/utils/ann_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/utils/dpr.py` & `dspy-ai-2.4.7/dsp/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/utils/metrics.py` & `dspy-ai-2.4.7/dsp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/utils/settings.py` & `dspy-ai-2.4.7/dsp/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/utils/settings_v2.py` & `dspy-ai-2.4.7/dsp/utils/settings_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dsp/utils/utils.py` & `dspy-ai-2.4.7/dsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/__init__.py` & `dspy-ai-2.4.7/dspy/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/datasets/colors.py` & `dspy-ai-2.4.7/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/datasets/dataloader.py` & `dspy-ai-2.4.7/dspy/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/datasets/dataset.py` & `dspy-ai-2.4.7/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/datasets/gsm8k.py` & `dspy-ai-2.4.7/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/datasets/hotpotqa.py` & `dspy-ai-2.4.7/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/evaluate/auto_evaluation.py` & `dspy-ai-2.4.7/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/evaluate/evaluate.py` & `dspy-ai-2.4.7/dspy/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/evaluate/metrics.py` & `dspy-ai-2.4.7/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/experimental/synthesizer/config.py` & `dspy-ai-2.4.7/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy-ai-2.4.7/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/experimental/synthesizer/signatures.py` & `dspy-ai-2.4.7/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/experimental/synthesizer/synthesizer.py` & `dspy-ai-2.4.7/dspy/experimental/synthesizer/synthesizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/experimental/synthesizer/utils.py` & `dspy-ai-2.4.7/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/experimental/synthetic_data.py` & `dspy-ai-2.4.7/dspy/experimental/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/functional/functional.py` & `dspy-ai-2.4.7/dspy/functional/functional.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/aggregation.py` & `dspy-ai-2.4.7/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/chain_of_thought.py` & `dspy-ai-2.4.7/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/chain_of_thought_with_hint.py` & `dspy-ai-2.4.7/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/knn.py` & `dspy-ai-2.4.7/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/langchain.py` & `dspy-ai-2.4.7/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/multi_chain_comparison.py` & `dspy-ai-2.4.7/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/predict.py` & `dspy-ai-2.4.7/dspy/predict/predict.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/program_of_thought.py` & `dspy-ai-2.4.7/dspy/predict/program_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/react.py` & `dspy-ai-2.4.7/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/predict/retry.py` & `dspy-ai-2.4.7/dspy/predict/retry.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/assertions.py` & `dspy-ai-2.4.7/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/box.py` & `dspy-ai-2.4.7/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/example.py` & `dspy-ai-2.4.7/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/module.py` & `dspy-ai-2.4.7/dspy/primitives/module.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/prediction.py` & `dspy-ai-2.4.7/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/program.py` & `dspy-ai-2.4.7/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/primitives/python_interpreter.py` & `dspy-ai-2.4.7/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/chromadb_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/chromadb_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/clarifai_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/clarifai_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/databricks_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/deeplake_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/deeplake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/faiss_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/faiss_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/marqo_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/mongodb_atlas_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/neo4j_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/pgvector_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/pgvector_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/pinecone_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/qdrant_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/qdrant_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/retrieve.py` & `dspy-ai-2.4.7/dspy/retrieve/retrieve.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/vectara_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/weaviate_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/weaviate_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/retrieve/you_rm.py` & `dspy-ai-2.4.7/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/signatures/field.py` & `dspy-ai-2.4.7/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/signatures/signature.py` & `dspy-ai-2.4.7/dspy/signatures/signature.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/bootstrap.py` & `dspy-ai-2.4.7/dspy/teleprompt/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/copro_optimizer.py` & `dspy-ai-2.4.7/dspy/teleprompt/copro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/ensemble.py` & `dspy-ai-2.4.7/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/finetune.py` & `dspy-ai-2.4.7/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/knn_fewshot.py` & `dspy-ai-2.4.7/dspy/teleprompt/knn_fewshot.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/mipro_optimizer.py` & `dspy-ai-2.4.7/dspy/teleprompt/mipro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/random_search.py` & `dspy-ai-2.4.7/dspy/teleprompt/random_search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/signature_opt.py` & `dspy-ai-2.4.7/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/signature_opt_bayesian.py` & `dspy-ai-2.4.7/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/signature_opt_typed.py` & `dspy-ai-2.4.7/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/teleprompt_optuna.py` & `dspy-ai-2.4.7/dspy/teleprompt/teleprompt_optuna.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/teleprompt/vanilla.py` & `dspy-ai-2.4.7/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy/utils/dummies.py` & `dspy-ai-2.4.7/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy_ai.egg-info/PKG-INFO` & `dspy-ai-2.4.7/dspy_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.6
+Version: 2.4.7
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dspy-ai-2.4.6/dspy_ai.egg-info/SOURCES.txt` & `dspy-ai-2.4.7/dspy_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/dspy_ai.egg-info/requires.txt` & `dspy-ai-2.4.7/dspy_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.6/pyproject.toml` & `dspy-ai-2.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.4.6"
+version = "2.4.7"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.12"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `dspy-ai-2.4.6/setup.py` & `dspy-ai-2.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file	
 with open('requirements.txt', encoding='utf-8') as f:	
     requirements = f.read().splitlines()	
 
 setup(	
     name="dspy-ai",	
-    version="2.4.6",	
+    version="2.4.7",	
     description="DSPy",	
     long_description=long_description,	
     long_description_content_type='text/markdown',	
     url="https://github.com/stanfordnlp/dsp",	
     author="Omar Khattab",	
     author_email="okhattab@stanford.edu",	
     license="MIT License",
```

