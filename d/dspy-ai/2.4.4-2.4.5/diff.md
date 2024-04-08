# Comparing `tmp/dspy-ai-2.4.4.tar.gz` & `tmp/dspy-ai-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dspy-ai-2.4.4.tar", last modified: Mon Apr  8 17:21:05 2024, max compression
+gzip compressed data, was "dist/dspy-ai-2.4.5.tar", last modified: Mon Apr  8 17:29:58 2024, max compression
```

## Comparing `dspy-ai-2.4.4.tar` & `dspy-ai-2.4.5.tar`

### file list

```diff
@@ -1,159 +1,153 @@
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/
--rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.4/LICENSE
--rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)    34442 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/README.md
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/
--rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/evaluation/
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/evaluation/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/evaluation/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/modules/
--rw-r--r--   0 okhattab (19845) future   (20099)      446 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4547 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/anthropic.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/aws_lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/azure_openai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/azurecognitivesearch.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3102 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/bedrock.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1022 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/cache_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/clarifai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/cohere.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/colbertv2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/databricks.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/modules/finetuning/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/finetuning/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/finetuning/finetune_hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/google.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/gpt3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/hf_client.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/hf_server.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3258 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/ollama.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/pyserini.py
--rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/sbert.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/sentence_vectorizer.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/compiler.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/demonstrate.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/inspect.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7948 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/primitives/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/primitives.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/primitives/search.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/templates/
--rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/template_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/template_v3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/ann_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/dpr.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/metrics.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3285 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/settings.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/settings_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/
--rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/adapters/
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/basic_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/chatml_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/vicuna_adapter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/datasets/
--rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/colors.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/datasets/dataloader.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/dataset.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/gsm8k.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/hotpotqa.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/evaluate/
--rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/evaluate.py
--rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/metrics.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/experimental/
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/config.py
--rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9542 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/experimental/synthetic_data.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/functional/
--rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/functional/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15805 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/functional/functional.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/predict/
--rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/aggregation.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/chain_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/knn.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/langchain.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/parameter.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/predict/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/predict/program_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/react.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/predict/retry.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/assertions.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/box.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/example.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/module.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/prediction.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/program.py
--rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/python_interpreter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/retrieve/
--rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4793 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/databricks_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0 okhattab (19845) future   (20099)     6530 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/faiss_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/marqo_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/retrieve.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/vectara_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/you_rm.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy/signatures/
--rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/signatures/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/signatures/field.py
--rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/signatures/signature.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy/teleprompt/
--rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/bootstrap.py
--rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/ensemble.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/finetune.py
--rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/random_search.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/signature_opt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/teleprompt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/vanilla.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/utils/dummies.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy_ai.egg-info/
--rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)     3752 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/SOURCES.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/dependency_links.txt
--rw-r--r--   0 okhattab (19845) future   (20099)      635 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/requires.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/top_level.txt
--rw-r--r--   0 okhattab (19845) future   (20099)     6888 2024-04-08 17:20:51.000000 dspy-ai-2.4.4/pyproject.toml
--rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/setup.cfg
--rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 17:13:24.000000 dspy-ai-2.4.4/setup.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.5/LICENSE
+-rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)    34442 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/README.md
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/evaluation/
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/evaluation/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/evaluation/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/modules/
+-rw-r--r--   0 okhattab (19845) future   (20099)      446 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4771 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dsp/modules/anthropic.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/aws_lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/azure_openai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/azurecognitivesearch.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3102 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/bedrock.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      964 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dsp/modules/cache_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/clarifai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/cohere.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/colbertv2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/databricks.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/modules/finetuning/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/finetuning/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/finetuning/finetune_hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/google.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/gpt3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/hf_client.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/hf_server.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3258 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/modules/lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/ollama.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/pyserini.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/sbert.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/modules/sentence_vectorizer.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/primitives/compiler.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/primitives/demonstrate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/primitives/inspect.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8432 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dsp/primitives/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/primitives/primitives.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dsp/primitives/search.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/templates/
+-rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/templates/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/templates/template_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/templates/template_v3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/templates/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dsp/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/utils/ann_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/utils/dpr.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/utils/metrics.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3287 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dsp/utils/settings.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/utils/settings_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dsp/utils/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/
+-rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/adapters/
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/adapters/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/adapters/basic_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/adapters/chatml_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/adapters/llamachat_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/adapters/vicuna_adapter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/datasets/
+-rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/datasets/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/datasets/colors.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/datasets/dataloader.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/datasets/dataset.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/datasets/gsm8k.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/datasets/hotpotqa.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/evaluate/
+-rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/evaluate/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/evaluate/evaluate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/evaluate/metrics.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/experimental/
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/experimental/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6845 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/experimental/synthesizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/experimental/synthetic_data.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/functional/
+-rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/functional/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    18631 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/functional/functional.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/predict/
+-rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/aggregation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/chain_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/knn.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/langchain.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/parameter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/predict/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/predict/program_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/predict/react.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/predict/retry.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/assertions.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/box.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/example.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2490 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/primitives/module.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/prediction.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/program.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/primitives/python_interpreter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/retrieve/
+-rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4793 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0 okhattab (19845) future   (20099)     6530 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3454 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/retrieve.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/retrieve/you_rm.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/signatures/
+-rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/signatures/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2556 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/signatures/field.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/signatures/signature.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/teleprompt/
+-rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/teleprompt/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9384 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    17283 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1385 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/ensemble.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6211 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/finetune.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      807 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    29365 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7923 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/random_search.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2578 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3401 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11790 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       60 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3097 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      950 2024-04-08 17:29:25.000000 dspy-ai-2.4.5/dspy/teleprompt/vanilla.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-04-08 17:11:57.000000 dspy-ai-2.4.5/dspy/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.5/dspy/utils/dummies.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy_ai.egg-info/
+-rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 17:29:57.000000 dspy-ai-2.4.5/dspy_ai.egg-info/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)     3521 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/dspy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 17:29:57.000000 dspy-ai-2.4.5/dspy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)      635 2024-04-08 17:29:57.000000 dspy-ai-2.4.5/dspy_ai.egg-info/requires.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 17:29:57.000000 dspy-ai-2.4.5/dspy_ai.egg-info/top_level.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)     6871 2024-04-08 17:29:34.000000 dspy-ai-2.4.5/pyproject.toml
+-rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 17:29:58.000000 dspy-ai-2.4.5/setup.cfg
+-rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 17:29:47.000000 dspy-ai-2.4.5/setup.py
```

### Comparing `dspy-ai-2.4.4/LICENSE` & `dspy-ai-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/PKG-INFO` & `dspy-ai-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.4
+Version: 2.4.5
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dspy-ai-2.4.4/README.md` & `dspy-ai-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/__init__.py` & `dspy-ai-2.4.5/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/evaluation/utils.py` & `dspy-ai-2.4.5/dsp/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/anthropic.py` & `dspy-ai-2.4.5/dsp/modules/anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 logger = logging.getLogger(__name__)
 
 BASE_URL = "https://api.anthropic.com/v1/messages"
 
 
 def backoff_hdlr(details):
-    """Handler from https://pypi.org/project/backoff/."""
+    """Handler from https://pypi.org/project/backoff/"""
     print(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with kwargs "
         "{kwargs}".format(**details),
     )
 
 
 def giveup_hdlr(details):
-    """Wrapper function that decides when to give up on retry."""
+    """wrapper function that decides when to give up on retry"""
     if "rate limits" in details.message:
         return False
     return True
 
 
 class Claude(LM):
     """Wrapper around anthropic's API. Supports both the Anthropic and Azure APIs."""
@@ -42,27 +42,27 @@
             api_key: Optional[str] = None,
             api_base: Optional[str] = None,
             **kwargs,
     ):
         super().__init__(model)
 
         try:
-            from anthropic import Anthropic
+            from anthropic import Anthropic, RateLimitError
         except ImportError as err:
             raise ImportError("Claude requires `pip install anthropic`.") from err
-
+        
         self.provider = "anthropic"
         self.api_key = api_key = os.environ.get("ANTHROPIC_API_KEY") if api_key is None else api_key
         self.api_base = BASE_URL if api_base is None else api_base
 
         self.kwargs = {
-            "temperature": kwargs.get("temperature", 0.0),
+            "temperature": 0.0 if "temperature" not in kwargs else kwargs["temperature"],
             "max_tokens": min(kwargs.get("max_tokens", 4096), 4096),
-            "top_p": kwargs.get("top_p", 1.0),
-            "top_k": kwargs.get("top_k", 1),
+            "top_p": 1.0 if "top_p" not in kwargs else kwargs["top_p"],
+            "top_k": 1 if "top_k" not in kwargs else kwargs["top_k"],
             "n": kwargs.pop("n", kwargs.pop("num_generations", 1)),
             **kwargs,
         }
         self.kwargs["model"] = model
         self.history: list[dict[str, Any]] = []
         self.client = Anthropic(api_key=api_key)
 
@@ -76,14 +76,15 @@
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
 
         kwargs = {**self.kwargs, **kwargs}
         # caching mechanism requires hashable kwargs
         kwargs["messages"] = [{"role": "user", "content": prompt}]
         kwargs.pop("n")
+        print(kwargs)
         response = self.client.messages.create(**kwargs)
 
         history = {
             "prompt": prompt,
             "response": response,
             "kwargs": kwargs,
             "raw_kwargs": raw_kwargs,
@@ -97,15 +98,15 @@
         (anthropic_rate_limit),
         max_time=1000,
         max_tries=8,
         on_backoff=backoff_hdlr,
         giveup=giveup_hdlr,
     )
     def request(self, prompt: str, **kwargs):
-        """Handles retrieval of completions from Anthropic whilst handling API errors."""
+        """Handles retrieval of completions from Anthropic whilst handling API errors"""
         return self.basic_request(prompt, **kwargs)
 
     def __call__(self, prompt, only_completed=True, return_sorted=False, **kwargs):
         """Retrieves completions from Anthropic.
 
         Args:
             prompt (str): prompt to send to Anthropic
@@ -115,23 +116,25 @@
         Returns:
             list[str]: list of completion choices
         """
 
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
 
-
+      
         # per eg here: https://docs.anthropic.com/claude/reference/messages-examples
         # max tokens can be used as a proxy to return smaller responses
         # so this cannot be a proper indicator for incomplete response unless it isnt the user-intent.
+        # if only_completed and response.stop_reason != "end_turn":
+        #     choices = []
 
         n = kwargs.pop("n", 1)
         completions = []
-        for _ in range(n):
+        for i in range(n):
             response = self.request(prompt, **kwargs)
             # TODO: Log llm usage instead of hardcoded openai usage
             # if dsp.settings.log_openai_usage:
             #     self.log_usage(response)
             if only_completed and response.stop_reason == "max_tokens":
                 continue
             completions = [c.text for c in response.content]
-        return completions
+        return completions
```

### Comparing `dspy-ai-2.4.4/dsp/modules/aws_lm.py` & `dspy-ai-2.4.5/dsp/modules/aws_lm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/azure_openai.py` & `dspy-ai-2.4.5/dsp/modules/azure_openai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/azurecognitivesearch.py` & `dspy-ai-2.4.5/dsp/modules/azurecognitivesearch.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/bedrock.py` & `dspy-ai-2.4.5/dsp/modules/bedrock.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/cache_utils.py` & `dspy-ai-2.4.5/dsp/modules/cache_utils.py`

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

### Comparing `dspy-ai-2.4.4/dsp/modules/clarifai.py` & `dspy-ai-2.4.5/dsp/modules/clarifai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/cohere.py` & `dspy-ai-2.4.5/dsp/modules/cohere.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/colbertv2.py` & `dspy-ai-2.4.5/dsp/modules/colbertv2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/databricks.py` & `dspy-ai-2.4.5/dsp/modules/databricks.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/finetuning/finetune_hf.py` & `dspy-ai-2.4.5/dsp/modules/finetuning/finetune_hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/google.py` & `dspy-ai-2.4.5/dsp/modules/google.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/gpt3.py` & `dspy-ai-2.4.5/dsp/modules/gpt3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/hf.py` & `dspy-ai-2.4.5/dsp/modules/hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/hf_client.py` & `dspy-ai-2.4.5/dsp/modules/hf_client.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/hf_server.py` & `dspy-ai-2.4.5/dsp/modules/hf_server.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/lm.py` & `dspy-ai-2.4.5/dsp/modules/lm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/ollama.py` & `dspy-ai-2.4.5/dsp/modules/ollama.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/pyserini.py` & `dspy-ai-2.4.5/dsp/modules/pyserini.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/sbert.py` & `dspy-ai-2.4.5/dsp/modules/sbert.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/modules/sentence_vectorizer.py` & `dspy-ai-2.4.5/dsp/modules/sentence_vectorizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/primitives/compiler.py` & `dspy-ai-2.4.5/dsp/primitives/compiler.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/primitives/demonstrate.py` & `dspy-ai-2.4.5/dsp/primitives/demonstrate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/primitives/inspect.py` & `dspy-ai-2.4.5/dsp/primitives/inspect.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/primitives/predict.py` & `dspy-ai-2.4.5/dsp/primitives/predict.py`

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

### Comparing `dspy-ai-2.4.4/dsp/primitives/primitives.py` & `dspy-ai-2.4.5/dsp/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/primitives/search.py` & `dspy-ai-2.4.5/dsp/primitives/search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/templates/template_v2.py` & `dspy-ai-2.4.5/dsp/templates/template_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/templates/template_v3.py` & `dspy-ai-2.4.5/dsp/templates/template_v3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/templates/utils.py` & `dspy-ai-2.4.5/dsp/templates/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/utils/ann_utils.py` & `dspy-ai-2.4.5/dsp/utils/ann_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/utils/dpr.py` & `dspy-ai-2.4.5/dsp/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/utils/metrics.py` & `dspy-ai-2.4.5/dsp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/utils/settings.py` & `dspy-ai-2.4.5/dsp/utils/settings.py`

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
-                trace=[],
+                trace=None,
                 release=0,
                 log_openai_usage=False,
                 bypass_assert=False,
                 bypass_suggest=False,
                 assert_failures=0,
                 suggest_failures=0,
                 langchain_history=[],
```

### Comparing `dspy-ai-2.4.4/dsp/utils/settings_v2.py` & `dspy-ai-2.4.5/dsp/utils/settings_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dsp/utils/utils.py` & `dspy-ai-2.4.5/dsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/__init__.py` & `dspy-ai-2.4.5/dspy/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/datasets/colors.py` & `dspy-ai-2.4.5/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/datasets/dataloader.py` & `dspy-ai-2.4.5/dspy/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/datasets/dataset.py` & `dspy-ai-2.4.5/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/datasets/gsm8k.py` & `dspy-ai-2.4.5/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/datasets/hotpotqa.py` & `dspy-ai-2.4.5/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/evaluate/auto_evaluation.py` & `dspy-ai-2.4.5/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/evaluate/evaluate.py` & `dspy-ai-2.4.5/dspy/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/evaluate/metrics.py` & `dspy-ai-2.4.5/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/experimental/synthetic_data.py` & `dspy-ai-2.4.5/dspy/experimental/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/functional/functional.py` & `dspy-ai-2.4.5/dspy/functional/functional.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import inspect
 import json
+import os
 import typing
 from typing import Annotated, List, Tuple  # noqa: UP035
 
+import openai
 import pydantic
 import ujson
 
 import dspy
 from dsp.templates import passages2text
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, make_signature
 
+# Some improvement ideas:
+# - Increase the temperature on error
+
 
 def predictor(func) -> dspy.Module:
     """Decorator that creates a predictor module based on the provided function."""
     signature = _func_to_signature(func)
     *_, output_key = signature.output_fields.keys()
     return _StripOutput(TypedPredictor(signature), output_key)
 
@@ -64,46 +69,32 @@
             ),
         ),
         max_retries=max_retries,
     )
 
 
 class TypedPredictor(dspy.Module):
-    def __init__(self, signature, max_retries=3, wrap_json=False):
-        """Like dspy.Predict, but enforces type annotations in the signature.
-
-        Args:
-            signature: The signature of the module. Can use type annotations.
-            max_retries: The number of times to retry the prediction if the output is invalid.
-            wrap_json: If True, json objects in the input will be wrapped in ```json ... ```
-        """
+    def __init__(self, signature, max_retries=3):
         super().__init__()
         self.signature = ensure_signature(signature)
         self.predictor = dspy.Predict(signature)
         self.max_retries = max_retries
-        self.wrap_json = wrap_json
 
     def copy(self) -> "TypedPredictor":
-        return TypedPredictor(self.signature, self.max_retries, self.wrap_json)
-
-    def __repr__(self):
-        """Return a string representation of the TypedPredictor object."""
-        return f"TypedPredictor({self.signature})"
+        return TypedPredictor(self.signature, self.max_retries)
 
-    def _make_example(self, type_) -> str:
+    @staticmethod
+    def _make_example(type_) -> str:
         # Note: DSPy will cache this call so we only pay the first time TypedPredictor is called.
-        schema = json.dumps(type_.model_json_schema())
-        if self.wrap_json:
-            schema = "```json\n" + schema + "\n```\n"
         json_object = dspy.Predict(
             make_signature(
                 "json_schema -> json_object",
                 "Make a very succinct json object that validates with the following schema",
             ),
-        )(json_schema=schema).json_object
+        )(json_schema=json.dumps(type_.model_json_schema())).json_object
         # We use the model_validate_json method to make sure the example is valid
         try:
             type_.model_validate_json(_unwrap_json(json_object))
         except (pydantic.ValidationError, ValueError):
             return ""  # Unable to make an example
         return json_object
         # TODO: Another fun idea is to only (but automatically) do this if the output fails.
@@ -115,30 +106,15 @@
     def _prepare_signature(self) -> dspy.Signature:
         """Add formats and parsers to the signature fields, based on the type annotations of the fields."""
         signature = self.signature
         for name, field in self.signature.fields.items():
             is_output = field.json_schema_extra["__dspy_field_type"] == "output"
             type_ = field.annotation
             if is_output:
-                if type_ is bool:
-
-                    def parse(x):
-                        x = x.strip().lower()
-                        if x not in ("true", "false"):
-                            raise ValueError("Respond with true or false")
-                        return x == "true"
-
-                    signature = signature.with_updated_fields(
-                        name,
-                        desc=field.json_schema_extra.get("desc", "")
-                        + (" (Respond with true or false)" if type_ != str else ""),
-                        format=lambda x: x if isinstance(x, str) else str(x),
-                        parser=parse,
-                    )
-                elif type_ in (str, int, float, bool):
+                if type_ in (str, int, float, bool):
                     signature = signature.with_updated_fields(
                         name,
                         desc=field.json_schema_extra.get("desc", "")
                         + (f" (Respond with a single {type_.__name__} value)" if type_ != str else ""),
                         format=lambda x: x if isinstance(x, str) else str(x),
                         parser=type_,
                     )
@@ -164,45 +140,37 @@
                         to_json = lambda x, type_=type_: type_(value=x).model_dump_json()
                         from_json = lambda x, type_=type_: type_.model_validate_json(x).value
                         schema = json.dumps(type_.model_json_schema())
                     else:
                         to_json = lambda x: x.model_dump_json()
                         from_json = lambda x, type_=type_: type_.model_validate_json(x)
                         schema = json.dumps(type_.model_json_schema())
-                    if self.wrap_json:
-                        to_json = lambda x, inner=to_json: "```json\n" + inner(x) + "\n```\n"
-                        schema = "```json\n" + schema + "\n```"
                     signature = signature.with_updated_fields(
                         name,
                         desc=field.json_schema_extra.get("desc", "")
                         + (". Respond with a single JSON object. JSON Schema: " + schema),
                         format=lambda x, to_json=to_json: (x if isinstance(x, str) else to_json(x)),
                         parser=lambda x, from_json=from_json: from_json(_unwrap_json(x)),
                         type_=type_,
                     )
             else:  # If input field
-                is_json = False
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
-                    is_json = True
                 elif inspect.isclass(type_) and issubclass(type_, pydantic.BaseModel):
                     format_ = lambda x: x if isinstance(x, str) else x.model_dump_json()
-                    is_json = True
-                if self.wrap_json and is_json:
-                    format_ = lambda x, inner=format_: x if isinstance(x, str) else "```json\n" + inner(x) + "\n```\n"
                 signature = signature.with_updated_fields(name, format=format_)
 
         return signature
 
     def forward(self, **kwargs) -> dspy.Prediction:
         modified_kwargs = kwargs.copy()
         # We have to re-prepare the signature on every forward call, because the base
@@ -240,31 +208,26 @@
                             )
                 # No reason trying to parse the general signature, or run more completions, if we already have errors
                 if errors:
                     break
                 # Instantiate the actual signature with the parsed values.
                 # This allow pydantic to validate the fields defined in the signature.
                 try:
-                    _ = self.signature(**kwargs, **parsed)
+                    _dummy = self.signature(**kwargs, **parsed)
                     parsed_results.append(parsed)
                 except pydantic.ValidationError as e:
                     errors["general"] = _format_error(e)
             if errors:
                 # Add new fields for each error
                 for name, error in errors.items():
                     modified_kwargs[f"error_{name}_{try_i}"] = error
-                    if name == "general":
-                        error_prefix = "General:"
-                    else:
-                        error_prefix = signature.output_fields[name].json_schema_extra["prefix"]
-                    number = "" if try_i == 0 else f" ({try_i+1})"
                     signature = signature.append(
                         f"error_{name}_{try_i}",
                         dspy.InputField(
-                            prefix=f"Past Error{number} in {error_prefix}",
+                            prefix="Past Error " + (f"({name}):" if try_i == 0 else f"({name}, {try_i+1}):"),
                             desc="An error to avoid in the future",
                         ),
                     )
             else:
                 # If there are no errors, we return the parsed results
                 return Prediction.from_completions(
                     {key: [r[key] for r in parsed_results] for key in signature.output_fields},
@@ -278,54 +241,188 @@
 def _format_error(error: Exception):
     if isinstance(error, pydantic.ValidationError):
         errors = []
         for e in error.errors():
             fields = ", ".join(map(str, e["loc"]))
             errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
         return "; ".join(errors)
-    return repr(error)
+    else:
+        return repr(error)
 
 
 def _func_to_signature(func):
     """Make a dspy.Signature based on a function definition."""
     sig = inspect.signature(func)
-    annotations = typing.get_type_hints(func, include_extras=True)
+    annotations = typing.get_type_hints(func)
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
-            desc = next((arg for arg in typing.get_args(annotation) if isinstance(arg, str)), None)
-            if desc is not None:
-                kwargs["desc"] = desc
+            annotation, kwargs["desc"] = typing.get_args(annotation)
         fields[param.name] = (annotation, dspy.InputField(**kwargs))
 
     # Output field
     kwargs = {}
     annotation = annotations.get("return", str)
     if typing.get_origin(annotation) is Annotated:
-        desc = next((arg for arg in typing.get_args(annotation) if isinstance(arg, str)), None)
-        if desc is not None:
-            kwargs["desc"] = desc
+        annotation, kwargs["desc"] = typing.get_args(annotation)
     fields[output_key] = (annotation, dspy.OutputField(**kwargs))
 
     return dspy.Signature(fields, instructions)
 
 
 def _unwrap_json(output):
     output = output.strip()
     if output.startswith("```"):
         if not output.startswith("```json"):
             raise ValueError("json output should start with ```json")
         if not output.endswith("```"):
-            raise ValueError("Don't write anything after the final json ```")
+            raise ValueError("json output should end with ```")
         output = output[7:-3].strip()
     if not output.startswith("{") or not output.endswith("}"):
         raise ValueError("json output should start and end with { and }")
     return ujson.dumps(ujson.loads(output))  # ujson is a bit more robust than the standard json
+
+
+################################################################################
+# Example usage
+################################################################################
+
+
+def main() -> None:
+    class Answer(pydantic.BaseModel):
+        value: float
+        certainty: float
+        comments: list[str] = pydantic.Field(description="At least two comments about the answer")
+
+    class QA(dspy.Module):
+        @predictor
+        def hard_question(self, topic: str) -> str:
+            """Think of a hard factual question about a topic. It should be answerable with a number."""
+
+        @cot
+        def answer(self, question: Annotated[str, "Question to answer"]) -> Answer:
+            pass
+
+        def forward(self, **kwargs):
+            question = self.hard_question(**kwargs)
+            return (question, self.answer(question=question))
+
+    openai.api_key = os.getenv("OPENAI_API_KEY")
+    lm = dspy.OpenAI(model="gpt-3.5-turbo", max_tokens=4000)
+    # lm = dspy.OpenAI(model="gpt-4", max_tokens=4000)
+    # lm = dspy.OpenAI(model="gpt-4-preview-1106", max_tokens=4000)
+    with dspy.context(lm=lm):
+        qa = QA()
+        question, answer = qa(topic="Physics")
+        # lm.inspect_history(n=5)
+
+        print("Question:", question)  # noqa: T201
+        print("Answer:", answer)  # noqa: T201
+
+
+################################################################################
+# HotpotQA example with SimpleBaleen
+################################################################################
+
+
+def validate_context_and_answer_and_hops(example, pred, trace=None) -> bool:
+    if not dspy.evaluate.answer_exact_match(example, pred):
+        return False
+    if not dspy.evaluate.answer_passage_match(example, pred):
+        return False
+
+    hops = [example.question] + [outputs.query for *_, outputs in trace if "query" in outputs]
+
+    if max([len(h) for h in hops]) > 100:
+        return False
+    if any(dspy.evaluate.answer_exact_match_str(hops[idx], hops[:idx], frac=0.8) for idx in range(2, len(hops))):
+        return False
+
+    return True
+
+
+def gold_passages_retrieved(example, pred, _trace=None) -> bool:
+    gold_titles = set(map(dspy.evaluate.normalize_text, example["gold_titles"]))
+    found_titles = set(map(dspy.evaluate.normalize_text, [c.split(" | ")[0] for c in pred.context]))
+
+    return gold_titles.issubset(found_titles)
+
+
+def hotpot() -> None:
+    import dspy.evaluate
+    from dsp.utils import deduplicate
+    from dspy.datasets import HotPotQA
+    from dspy.evaluate.evaluate import Evaluate
+    from dspy.teleprompt.bootstrap import BootstrapFewShot
+
+    print("Load the dataset.")  # noqa: T201
+    dataset = HotPotQA(train_seed=1, train_size=20, eval_seed=2023, dev_size=50, test_size=0)
+    trainset = [x.with_inputs("question") for x in dataset.train]
+    devset = [x.with_inputs("question") for x in dataset.dev]
+    print("Done")  # noqa: T201
+
+    class SimplifiedBaleen(FunctionalModule):
+        def __init__(self, passages_per_hop=3, max_hops=1):
+            super().__init__()
+            self.retrieve = dspy.Retrieve(k=passages_per_hop)
+            self.max_hops = max_hops
+
+        @cot
+        def generate_query(self, context: list[str], question) -> str:
+            """Write a simple search query that will help answer a complex question."""
+            pass
+
+        @cot
+        def generate_answer(self, context: list[str], question) -> str:
+            """Answer questions with short factoid answers."""
+            pass
+
+        def forward(self, question):
+            context = []
+
+            for _ in range(self.max_hops):
+                query = self.generate_query(context=context, question=question)
+                passages = self.retrieve(query).passages
+                context = deduplicate(context + passages)
+
+            answer = self.generate_answer(context=context, question=question)
+            return dspy.Prediction(context=context, answer=answer)
+
+    openai.api_key = os.getenv("OPENAI_API_KEY")
+    rm = dspy.ColBERTv2(url="http://20.102.90.50:2017/wiki17_abstracts")
+    lm = dspy.OpenAI(model="gpt-3.5-turbo", max_tokens=4000)
+    dspy.settings.configure(lm=lm, rm=rm, trace=[])
+
+    evaluate_on_hotpotqa = Evaluate(devset=devset, num_threads=10, display_progress=True, display_table=5)
+
+    # uncompiled (i.e., zero-shot) program
+    uncompiled_baleen = SimplifiedBaleen()
+    print(  # noqa: T201
+        "Uncompiled Baleen retrieval score:",
+        evaluate_on_hotpotqa(uncompiled_baleen, metric=gold_passages_retrieved),
+    )
+
+    # compiled (i.e., few-shot) program
+    compiled_baleen = BootstrapFewShot(metric=validate_context_and_answer_and_hops).compile(
+        SimplifiedBaleen(),
+        teacher=SimplifiedBaleen(passages_per_hop=2),
+        trainset=trainset,
+    )
+    print(  # noqa: T201
+        "Compiled Baleen retrieval score:",
+        evaluate_on_hotpotqa(compiled_baleen, metric=gold_passages_retrieved),
+    )
+    # lm.inspect_history(n=5)
+
+
+if __name__ == "__main__":
+    # main()
+    hotpot()
```

### Comparing `dspy-ai-2.4.4/dspy/predict/aggregation.py` & `dspy-ai-2.4.5/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/chain_of_thought.py` & `dspy-ai-2.4.5/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/chain_of_thought_with_hint.py` & `dspy-ai-2.4.5/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/knn.py` & `dspy-ai-2.4.5/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/langchain.py` & `dspy-ai-2.4.5/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/multi_chain_comparison.py` & `dspy-ai-2.4.5/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/predict.py` & `dspy-ai-2.4.5/dspy/predict/predict.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/program_of_thought.py` & `dspy-ai-2.4.5/dspy/predict/program_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/react.py` & `dspy-ai-2.4.5/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/predict/retry.py` & `dspy-ai-2.4.5/dspy/predict/retry.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/primitives/assertions.py` & `dspy-ai-2.4.5/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/primitives/box.py` & `dspy-ai-2.4.5/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/primitives/example.py` & `dspy-ai-2.4.5/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/primitives/prediction.py` & `dspy-ai-2.4.5/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/primitives/program.py` & `dspy-ai-2.4.5/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/primitives/python_interpreter.py` & `dspy-ai-2.4.5/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/chromadb_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/chromadb_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/clarifai_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/clarifai_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/databricks_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/deeplake_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/deeplake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/faiss_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/faiss_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/marqo_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/marqo_rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 from typing import List, Union
 
 import dspy
-from dsp.utils import dotdict
+from dspy import dotdict
 
 try:
     import marqo
 except ImportError:
     raise ImportError(
         "The 'marqo' extra is required to use MarqoRM. Install it with `pip install dspy-ai[marqo]`",
     )
```

### Comparing `dspy-ai-2.4.4/dspy/retrieve/mongodb_atlas_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/neo4j_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/pgvector_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/pgvector_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/pinecone_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/qdrant_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/qdrant_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/retrieve.py` & `dspy-ai-2.4.5/dspy/retrieve/retrieve.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/vectara_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/weaviate_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/weaviate_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/retrieve/you_rm.py` & `dspy-ai-2.4.5/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/signatures/field.py` & `dspy-ai-2.4.5/dspy/signatures/field.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,14 @@
     pydantic_kwargs = {}
     json_schema_extra = {}
     for k, v in kwargs.items():
         if k in DSPY_FIELD_ARG_NAMES:
             json_schema_extra[k] = v
         else:
             pydantic_kwargs[k] = v
-    # Also copy over the pydantic "description" if no dspy "desc" is given.
-    if "description" in kwargs and "desc" not in json_schema_extra:
-        json_schema_extra["desc"] = kwargs["description"]
     pydantic_kwargs["json_schema_extra"] = json_schema_extra
     return pydantic_kwargs
 
 
 def InputField(**kwargs):
     return pydantic.Field(**move_kwargs(**kwargs, __dspy_field_type="input"))
```

### Comparing `dspy-ai-2.4.4/dspy/signatures/signature.py` & `dspy-ai-2.4.5/dspy/signatures/signature.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/bootstrap.py` & `dspy-ai-2.4.5/dspy/teleprompt/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,23 @@
 # TODO: When this bootstraps for another teleprompter like finetune, we want all demos we gather.
 # But when it's for direct use we may want to sample ONE demo per predictor--example pair. This is important for "multi-use" modules.
 
 # TODO: Add baselines=[...]
 
 
 class BootstrapFewShot(Teleprompter):
-    def __init__(
-        self,
-        metric=None,
-        metric_threshold=None,
-        teacher_settings={},
-        max_bootstrapped_demos=4,
-        max_labeled_demos=16,
-        max_rounds=1,
-        max_errors=5,
-    ):
+    def __init__(self, metric=None, metric_threshold=None, teacher_settings={}, max_bootstrapped_demos=4, max_labeled_demos=16, max_rounds=1, max_errors=5):
         self.metric = metric
         self.metric_threshold = metric_threshold
         self.teacher_settings = teacher_settings
 
         self.max_bootstrapped_demos = max_bootstrapped_demos
         self.max_labeled_demos = max_labeled_demos
         self.max_rounds = max_rounds
-        self.max_errors = max_errors
+        self.max_errors= max_errors
         self.error_count = 0
         self.error_lock = threading.Lock()
 
     def compile(self, student, *, teacher=None, trainset, valset=None):
         self.trainset = trainset
         self.valset = valset
 
@@ -64,49 +55,45 @@
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
 
-        assert getattr(self.student, "_compiled", False) is False, "Student must be uncompiled."
+        assert getattr(self.student, '_compiled', False) is False, "Student must be uncompiled."
 
-        if self.max_labeled_demos and getattr(self.teacher, "_compiled", False) is False:
+        if self.max_labeled_demos and getattr(self.teacher, '_compiled', False) is False:
             teleprompter = LabeledFewShot(k=self.max_labeled_demos)
             self.teacher = teleprompter.compile(self.teacher.reset_copy(), trainset=self.trainset)
 
     def _prepare_predictor_mappings(self):
         name2predictor, predictor2name = {}, {}
         student, teacher = self.student, self.teacher
 
-        assert len(student.predictors()) == len(
-            teacher.predictors(),
-        ), "Student and teacher must have the same number of predictors."
+        assert len(student.predictors()) == len(teacher.predictors()), "Student and teacher must have the same number of predictors."
 
         for (name1, predictor1), (name2, predictor2) in zip(student.named_predictors(), teacher.named_predictors()):
             assert name1 == name2, "Student and teacher must have the same program structure."
-            assert predictor1.signature.equals(
-                predictor2.signature,
-            ), f"Student and teacher must have the same signatures. {type(predictor1.signature)} != {type(predictor2.signature)}"
+            assert predictor1.signature.equals(predictor2.signature), f"Student and teacher must have the same signatures. {type(predictor1.signature)} != {type(predictor2.signature)}"
             assert id(predictor1) != id(predictor2), "Student and teacher must be different objects."
 
-            name2predictor[name1] = None  # dict(student=predictor1, teacher=predictor2)
+            name2predictor[name1] = None # dict(student=predictor1, teacher=predictor2)
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
 
@@ -120,30 +107,30 @@
 
                 if example_idx not in bootstrapped:
                     success = self._bootstrap_one_example(example, round_idx)
 
                     if success:
                         bootstrapped[example_idx] = True
 
-        print(f"Bootstrapped {len(bootstrapped)} full traces after {example_idx+1} examples in round {round_idx}.")
-
+        print(f'Bootstrapped {len(bootstrapped)} full traces after {example_idx+1} examples in round {round_idx}.')
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
-        teacher = self.teacher  # .deepcopy()
+        teacher = self.teacher #.deepcopy()
         predictor_cache = {}
 
         try:
             with dsp.settings.context(trace=[], **self.teacher_settings):
                 lm = dsp.settings.lm
                 lm = lm.copy(temperature=0.7 + 0.001 * round_idx) if round_idx > 0 else lm
                 new_settings = dict(lm=lm) if round_idx > 0 else {}
@@ -154,15 +141,15 @@
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
@@ -171,56 +158,52 @@
         except Exception as e:
             success = False
             with self.error_lock:
                 self.error_count += 1
                 current_error_count = self.error_count
             if current_error_count >= self.max_errors:
                 raise e
-            print(f"Failed to run or to evaluate example {example} with {self.metric} due to {e}.")
-
+            print(f'Failed to run or to evaluate example {example} with {self.metric} due to {e}.')
+        
         if success:
             for step in trace:
                 predictor, inputs, outputs = step
 
-                if "dspy_uuid" in example:
+                if 'dspy_uuid' in example:
                     demo = Example(augmented=True, dspy_uuid=example.dspy_uuid, **inputs, **outputs)
                 else:
                     # TODO: FIXME: This is a hack. RandomSearch will complain for now in this edge case.
                     demo = Example(augmented=True, **inputs, **outputs)
 
                 try:
                     predictor_name = self.predictor2name[id(predictor)]
                 except KeyError as e:
-                    continue  # FIXME: !
+                    continue # FIXME: !
 
                     # TODO: Look closer into this. It's a bit tricky to reproduce.
-                    print(f"Failed to find predictor {predictor} in {self.predictor2name}.")
-                    print(
-                        "Are you doing this in a notebook (Jupyter)? This might be caused by redefining values by rerunning cells.",
-                    )
-                    print("Try restarting the notebook, or open an issue.")
-                    raise KeyError(
-                        f"Failed to find predictor {id(predictor)} {predictor} in {self.predictor2name}.",
-                    ) from e
+                    print(f'Failed to find predictor {predictor} in {self.predictor2name}.')
+                    print('Are you doing this in a notebook (Jupyter)? This might be caused by redefining values by rerunning cells.')
+                    print('Try restarting the notebook, or open an issue.')
+                    raise KeyError(f'Failed to find predictor {id(predictor)} {predictor} in {self.predictor2name}.') from e
 
                 name2traces[predictor_name].append(demo)
-
+        
         return success
 
     def _train(self):
         rng = random.Random(0)
         raw_demos = self.validation
 
         for name, predictor in self.student.named_predictors():
-            augmented_demos = self.name2traces[name][: self.max_bootstrapped_demos]
-
+            augmented_demos = self.name2traces[name][:self.max_bootstrapped_demos]
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

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/copro_optimizer.py` & `dspy-ai-2.4.5/dspy/teleprompt/copro_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,49 +27,32 @@
 * track_stats: Tells the method whether or not to track statistics about the optimization process.
                 If True, the method will track the following statistics:
                     * results_best: The min,max,avg,stddev of top 10 scores for each predictor at each depth.
                     * results_latest: The min,max,avg,stddev of newest prompt scores for each predictor at each depth.
                     * total_calls: The total number of calls to the task metric.
                 These statistics will be returned as attributes of the best program.
 """
-
-
 class BasicGenerateInstruction(Signature):
     """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
 
     basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
     proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(
-        desc="The string at the end of the prompt, which will help the model start solving the task",
-    )
-
+    proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class GenerateInstructionGivenAttempts(dspy.Signature):
-    """You are an instruction optimizer for large language models. I will give some task instructions I've tried, along with their corresponding validation scores. The instructions are arranged in increasing order based on their scores, where higher scores indicate better quality.
-
-    Your task is to propose a new instruction that will lead a good language model to perform the task even better. Don't be afraid to be creative."""
+        """You are an instruction optimizer for large language models. I will give some task instructions I've tried, along with their corresponding validation scores. The instructions are arranged in increasing order based on their scores, where higher scores indicate better quality.
 
-    attempted_instructions = dspy.InputField(format=dsp.passages2text)
-    proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(
-        desc="The string at the end of the prompt, which will help the model start solving the task",
-    )
+Your task is to propose a new instruction that will lead a good language model to perform the task even better. Don't be afraid to be creative."""
 
+        attempted_instructions = dspy.InputField(format=dsp.passages2text)
+        proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
+        proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class COPRO(Teleprompter):
-    def __init__(
-        self,
-        prompt_model=None,
-        metric=None,
-        breadth=10,
-        depth=3,
-        init_temperature=1.4,
-        verbose=False,
-        track_stats=False,
-    ):
+    def __init__(self, prompt_model=None, metric=None, breadth=10, depth=3, init_temperature=1.4, verbose=False, track_stats=False):
         if breadth <= 1:
             raise ValueError("Breadth must be greater than 1")
         self.metric = metric
         self.breadth = breadth
         self.depth = depth
         self.init_temperature = init_temperature
         self.prompt_model = prompt_model
@@ -88,276 +71,231 @@
 
     def _drop_duplicates(self, candidates):
         final_candidates = []
         last_batch = []
         last_batch_score = -1
         for c in candidates:
             repeat = False
-            if c["score"] == last_batch_score:
+            if c['score'] == last_batch_score:
                 for c2 in last_batch:
-                    if self._check_candidates_equal(c, c2):
+                    if (self._check_candidates_equal(c, c2)):
                         repeat = True
                         break
                 if not repeat:
                     last_batch.append(c)
             else:
                 last_batch = [c]
-                last_batch_score = c["score"]
+                last_batch_score = c['score']
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
-        if hasattr(predictor, "extended_signature"):
+        if (hasattr(predictor, 'extended_signature')):
             return predictor.extended_signature
-        elif hasattr(predictor, "signature"):
+        elif (hasattr(predictor, 'signature')):
             return predictor.signature
-
+    
     def _set_signature(self, predictor, updated_signature):
-        if hasattr(predictor, "extended_signature"):
+        if (hasattr(predictor, 'extended_signature')):
             predictor.extended_signature = updated_signature
-        elif hasattr(predictor, "signature"):
+        elif (hasattr(predictor, 'signature')):
             predictor.signature = updated_signature
 
+    
     def compile(self, student, *, trainset, eval_kwargs):
         """student is a program that needs to be optimized, note that it may be zero-shot or already pre-optimized for demos != []"""
         module = student.deepcopy()
         evaluate = Evaluate(devset=trainset, metric=self.metric, **eval_kwargs)
         total_calls = 0
-        results_best = {
-            id(p): {"depth": [], "max": [], "average": [], "min": [], "std": []} for p in module.predictors()
-        }
-        results_latest = {
-            id(p): {"depth": [], "max": [], "average": [], "min": [], "std": []} for p in module.predictors()
-        }
+        results_best = {id(p):{"depth": [], "max": [], "average": [], "min":[], "std": []} for p in module.predictors()}
+        results_latest = {id(p):{"depth": [], "max": [], "average": [], "min":[], "std": []} for p in module.predictors()}
 
         if self.track_stats:
             import numpy as np
 
+
         candidates = {}
         evaluated_candidates = defaultdict(dict)
 
         # Seed the prompt optimizer zero shot with just the instruction, generate BREADTH new prompts
         for predictor in module.predictors():
             basic_instruction = None
             basic_prefix = None
             *_, last_key = self._get_signature(predictor).fields.keys()
             basic_instruction = self._get_signature(predictor).instructions
-            basic_prefix = self._get_signature(predictor).fields[last_key].json_schema_extra["prefix"]
-            if self.prompt_model:
+            basic_prefix = self._get_signature(predictor).fields[last_key].json_schema_extra['prefix']
+            if self.prompt_model: 
                 with dspy.settings.context(lm=self.prompt_model):
-                    instruct = dspy.Predict(
-                        BasicGenerateInstruction,
-                        n=self.breadth - 1,
-                        temperature=self.init_temperature,
-                    )(basic_instruction=basic_instruction)
+                    instruct = dspy.Predict(BasicGenerateInstruction, n=self.breadth-1, temperature=self.init_temperature)(basic_instruction=basic_instruction)
             else:
-                instruct = dspy.Predict(
-                    BasicGenerateInstruction,
-                    n=self.breadth - 1,
-                    temperature=self.init_temperature,
-                )(basic_instruction=basic_instruction)
+                instruct = dspy.Predict(BasicGenerateInstruction, n=self.breadth-1, temperature=self.init_temperature)(basic_instruction=basic_instruction)
             # Add in our initial prompt as a candidate as well
             instruct.completions.proposed_instruction.append(basic_instruction)
             instruct.completions.proposed_prefix_for_output_field.append(basic_prefix)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
-
-        if self.verbose and self.prompt_model:
-            print(f"{self.prompt_model.inspect_history(n=1)}")
+        
+        if self.verbose and self.prompt_model: print(f"{self.prompt_model.inspect_history(n=1)}")
 
         latest_candidates = candidates
         all_candidates = candidates
-
+        
         module_clone = module.deepcopy()
 
         # For each iteration in depth...
-        for d in range(
-            self.depth,
-        ):  # TODO: fix this so that we eval the new batch of predictors with the new best followoing predictors
+        for d in range(self.depth): # TODO: fix this so that we eval the new batch of predictors with the new best followoing predictors
             print(f"Iteration Depth: {d+1}/{self.depth}.")
 
             latest_scores = []
-
+        
             # Go through our module's predictors
             for p_i, (p_old, p_new) in enumerate(zip(module.predictors(), module_clone.predictors())):
-                candidates_ = latest_candidates[id(p_old)]  # Use the most recently generated candidates for evaluation
+                candidates_ = latest_candidates[id(p_old)] # Use the most recently generated candidates for evaluation 
                 if len(module.predictors()) > 1:
-                    candidates_ = all_candidates[
-                        id(p_old)
-                    ]  # Unless our program has multiple predictors, in which case we need to reevaluate all prompts with the new prompt(s) for the other predictor(s)
+                    candidates_ = all_candidates[id(p_old)] # Unless our program has multiple predictors, in which case we need to reevaluate all prompts with the new prompt(s) for the other predictor(s)   
 
                 # For each candidate
-                for c_i, c in enumerate(candidates_):
-                    # Get the candidate instruction and prefix
-                    instruction, prefix = (
-                        c.proposed_instruction.strip('"').strip(),
-                        c.proposed_prefix_for_output_field.strip('"').strip(),
-                    )
+                for c_i, c in enumerate(candidates_):                    
+                    # Get the candidate instruction and prefix 
+                    instruction, prefix = c.proposed_instruction.strip('"').strip(), c.proposed_prefix_for_output_field.strip('"').strip()
 
-                    # Set this new module with our instruction / prefix
+                    # Set this new module with our instruction / prefix 
                     *_, last_key = self._get_signature(p_new).fields.keys()
-                    updated_signature = (
-                        self._get_signature(p_new)
-                        .with_instructions(instruction)
+                    updated_signature = self._get_signature(p_new) \
+                        .with_instructions(instruction) \
                         .with_updated_fields(last_key, prefix=prefix)
-                    )
                     self._set_signature(p_new, updated_signature)
 
-                    # Score the instruction / prefix
-                    if self.verbose:
-                        print("----------------")
-                    for i, predictor in enumerate(module_clone.predictors()):
-                        if self.verbose:
-                            print(f"Predictor {i+1}")
+                    # Score the instruction / prefix 
+                    if self.verbose: print("----------------")
+                    for i,predictor in enumerate(module_clone.predictors()):
+                        if self.verbose: print(f"Predictor {i+1}")
                         self._print_signature(predictor)
-                    print(
-                        f"At Depth {d+1}/{self.depth}, Evaluating Prompt Candidate #{c_i+1}/{len(candidates_)} for Predictor {p_i+1} of {len(module.predictors())}.",
-                    )
+                    print(f"At Depth {d+1}/{self.depth}, Evaluating Prompt Candidate #{c_i+1}/{len(candidates_)} for Predictor {p_i+1} of {len(module.predictors())}.")
                     score = evaluate(module_clone, devset=trainset, **eval_kwargs)
-                    if self.verbose and self.prompt_model:
-                        print(f"prompt_model.inspect_history(n=1) {self.prompt_model.inspect_history(n=1)}")
+                    if self.verbose and self.prompt_model: print(f"prompt_model.inspect_history(n=1) {self.prompt_model.inspect_history(n=1)}")
                     total_calls += 1
-                    if self.verbose:
-                        print("----------------")
+                    if self.verbose: print("----------------")
 
                     replace_entry = True
-                    if self.verbose:
-                        print(f"(instruction, prefix) {(instruction, prefix)}")
+                    if self.verbose: print(f"(instruction, prefix) {(instruction, prefix)}")
                     # if verbose: print(f"evaluated_candidates[id(p_old)] {evaluated_candidates[id(p_old)]}")
-                    if (instruction, prefix) in evaluated_candidates[id(p_old)]:
+                    if ((instruction, prefix) in evaluated_candidates[id(p_old)]):
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
-                    if len(candidates_) - self.breadth <= c_i:
+                    
+                    if (len(candidates_)-self.breadth <= c_i):
                         latest_scores.append(score)
 
                 if self.track_stats:
                     results_latest[id(p_old)]["depth"].append(d)
                     results_latest[id(p_old)]["max"].append(max(latest_scores))
-                    results_latest[id(p_old)]["average"].append(sum(latest_scores) / len(latest_scores))
+                    results_latest[id(p_old)]["average"].append(sum(latest_scores)/len(latest_scores))
                     results_latest[id(p_old)]["min"].append(min(latest_scores))
                     results_latest[id(p_old)]["std"].append(np.std(latest_scores))
-
+                
                 # Now that we've evaluated the candidates, set this predictor to the best performing version
                 # to ensure the next round of scores reflect the best possible version
-                best_candidate = max(evaluated_candidates[id(p_old)].values(), key=lambda candidate: candidate["score"])
+                best_candidate = max(evaluated_candidates[id(p_old)].values(), key=lambda candidate: candidate['score'])
                 *_, last_key = self._get_signature(p_old).fields.keys()
-                updated_signature = (
-                    self._get_signature(p_new)
-                    .with_instructions(best_candidate["instruction"])
+                updated_signature = self._get_signature(p_new) \
+                    .with_instructions(best_candidate["instruction"]) \
                     .with_updated_fields(last_key, prefix=best_candidate["prefix"])
-                )
                 self._set_signature(p_new, updated_signature)
-                if self.verbose:
-                    print(
-                        f"Updating Predictor {id(p_old)} to:\ni: {best_candidate['instruction']}\np: {best_candidate['prefix']}",
-                    )
-                if self.verbose:
-                    print("Full predictor with update: ")
-                for i, predictor in enumerate(module_clone.predictors()):
-                    if self.verbose:
-                        print(f"Predictor {i}")
+                if self.verbose: print(f"Updating Predictor {id(p_old)} to:\ni: {best_candidate['instruction']}\np: {best_candidate['prefix']}")
+                if self.verbose: print("Full predictor with update: ")
+                for i,predictor in enumerate(module_clone.predictors()):
+                    if self.verbose: print(f"Predictor {i}")
                     self._print_signature(predictor)
 
-            if d == self.depth - 1:
+            if d == self.depth-1:
                 break
 
+            
             new_candidates = {}
             for p_base in module.predictors():
                 # Build Few-Shot Example of Optimized Prompts
                 attempts = []
                 shortest_len = self.breadth
-                shortest_len = min(len(evaluated_candidates[id(p_base)]), shortest_len)
+                shortest_len = min(len(evaluated_candidates[id(p_base)]),shortest_len)
                 best_predictors = list(evaluated_candidates[id(p_base)].values())
 
                 # best_predictors = evaluated_candidates[id(p_base)].values()[:]
-                best_predictors.sort(key=lambda x: x["score"], reverse=True)
+                best_predictors.sort(key=lambda x: x['score'], reverse=True)
 
                 if self.track_stats:
-                    scores = [x["score"] for x in best_predictors][:10]
+                    scores = [x['score'] for x in best_predictors][:10]
                     results_best[id(p_base)]["depth"].append(d)
                     results_best[id(p_base)]["max"].append(max(scores))
-                    results_best[id(p_base)]["average"].append(sum(scores) / len(scores))
+                    results_best[id(p_base)]["average"].append(sum(scores)/len(scores))
                     results_best[id(p_base)]["min"].append(min(scores))
                     results_best[id(p_base)]["std"].append(np.std(scores))
-
-                for i in range(shortest_len - 1, -1, -1):
+                
+                for i in range(shortest_len-1,-1,-1):
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
-                        instr = dspy.Predict(
-                            GenerateInstructionGivenAttempts,
-                            n=self.breadth,
-                            temperature=self.init_temperature,
-                        )(attempted_instructions=attempts)
+                        instr = dspy.Predict(GenerateInstructionGivenAttempts, n=self.breadth, temperature=self.init_temperature)(attempted_instructions=attempts)
                 else:
-                    instr = dspy.Predict(
-                        GenerateInstructionGivenAttempts,
-                        n=self.breadth,
-                        temperature=self.init_temperature,
-                    )(attempted_instructions=attempts)
+                    instr = dspy.Predict(GenerateInstructionGivenAttempts, n=self.breadth, temperature=self.init_temperature)(attempted_instructions=attempts)
 
-                if self.verbose and self.prompt_model:
-                    print(f"{self.prompt_model.inspect_history(n=1)}")
+                if self.verbose and self.prompt_model: print(f"{self.prompt_model.inspect_history(n=1)}")
                 # Get candidates for each predictor
                 new_candidates[id(p_base)] = instr.completions
                 all_candidates[id(p_base)].proposed_instruction.extend(instr.completions.proposed_instruction)
-                all_candidates[id(p_base)].proposed_prefix_for_output_field.extend(
-                    instr.completions.proposed_prefix_for_output_field,
-                )
+                all_candidates[id(p_base)].proposed_prefix_for_output_field.extend(instr.completions.proposed_prefix_for_output_field)
 
-            if self.verbose and self.prompt_model:
-                print(f"{self.prompt_model.inspect_history(n=1)}")
+            if self.verbose and self.prompt_model: print(f"{self.prompt_model.inspect_history(n=1)}")
             latest_candidates = new_candidates
-
+        
         candidates = []
         for predictor in module.predictors():
             candidates.extend(list(evaluated_candidates[id(predictor)].values()))
 
             if self.track_stats:
                 best_predictors = list(evaluated_candidates[id(predictor)].values())
-                best_predictors.sort(key=lambda x: x["score"], reverse=True)
+                best_predictors.sort(key=lambda x: x['score'], reverse=True)
 
-                scores = [x["score"] for x in best_predictors][:10]
+                scores = [x['score'] for x in best_predictors][:10]
                 results_best[id(predictor)]["depth"].append(d)
                 results_best[id(predictor)]["max"].append(max(scores))
-                results_best[id(predictor)]["average"].append(sum(scores) / len(scores))
+                results_best[id(predictor)]["average"].append(sum(scores)/len(scores))
                 results_best[id(predictor)]["min"].append(min(scores))
                 results_best[id(predictor)]["std"].append(np.std(scores))
 
         # if verbose: print(f"candidates: {candidates}")
-        candidates.sort(key=lambda x: x["score"], reverse=True)
+        candidates.sort(key=lambda x: x['score'], reverse=True)
 
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

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/ensemble.py` & `dspy-ai-2.4.5/dspy/teleprompt/ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,34 @@
 
 from dspy.teleprompt.teleprompt import Teleprompter
 
 """
 TODO: The EnsembledProgram should actually imitate the structure of the individual programs (IF they are all compatible). This allows compiling with an ensemble program as a (singular) teacher. Basically the top majority-compatible trace will end up being used, if dspy.majority is the reduce_fn.
 """
 
-
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
-
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

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/finetune.py` & `dspy-ai-2.4.5/dspy/teleprompt/finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from .teleprompt import Teleprompter
 
 # from .vanilla import LabeledFewShot
 
 # from dspy.evaluate.evaluate import Evaluate
 
 
-if os.environ.get("DSP_NOTEBOOK_CACHEDIR"):
-    training_data_directory = os.path.join(os.environ.get("DSP_NOTEBOOK_CACHEDIR"), "compiler")
+if os.environ.get('DSP_NOTEBOOK_CACHEDIR'):
+    training_data_directory = os.path.join(os.environ.get('DSP_NOTEBOOK_CACHEDIR'), 'compiler')
     print(training_data_directory)
 else:
-    training_data_directory = "local_cache/compiler"
+    training_data_directory = 'local_cache/compiler'
 
 if not os.path.exists(training_data_directory):
     os.makedirs(training_data_directory)
 
 
 """
 TODO: Reduce and document the dependencies.
@@ -50,56 +50,40 @@
 class BootstrapFinetune(Teleprompter):
     def __init__(self, metric=None, teacher_settings={}, multitask=True):
         self.metric = metric
         self.teacher_settings = teacher_settings
         self.multitask = multitask
 
         metric = metric or (lambda *args: True)
-        self.teleprompter = BootstrapFewShot(
-            metric=metric,
-            max_bootstrapped_demos=999999,
-            max_labeled_demos=0,  # FIXME: TODO: Make this zero? or param, with default as 16 or 0?
-            teacher_settings=teacher_settings,
-        )
-
-    def compile(
-        self,
-        student,
-        *,
-        teacher=None,
-        trainset,
-        valset=None,
-        target="t5-large",
-        bsize=12,
-        accumsteps=1,
-        lr=5e-5,
-        epochs=1,
-        bf16=False,
-        int8=False,
-        peft=False,
-        path_prefix=None,
-    ):
+        self.teleprompter = BootstrapFewShot(metric=metric,
+                                             max_bootstrapped_demos=999999,
+                                             max_labeled_demos=0,  # FIXME: TODO: Make this zero? or param, with default as 16 or 0?
+                                             teacher_settings=teacher_settings)
+        
+
+    def compile(self, student, *, teacher=None, trainset, valset=None,
+                target='t5-large', bsize=12, accumsteps=1, lr=5e-5, epochs=1, bf16=False, int8=False, peft=False, path_prefix=None):
+
         # It's usually better to supply a few-shot teacher, rather than uncompiled module (the student).
         if teacher is None:
-            print(
-                "WARNING: Using a vanilla teacher. "
-                "Are you sure you want to use BootstrapFinetune without a compiled teacher?",
-            )
+            print("WARNING: Using a vanilla teacher. "
+                  "Are you sure you want to use BootstrapFinetune without a compiled teacher?")
+
 
         teachers = teacher if isinstance(teacher, list) else [teacher]
         finetune_data = {}
 
         for teacher in teachers:
             # Dummy compilation to get bootstraps.
             compiled = self.teleprompter.compile(student, teacher=teacher, trainset=trainset)
             multitask = self.multitask
 
             # Prepare finetune <prompt, completion> pairs.
             for name, predictor in compiled.named_predictors():
-                name_ = "all" if multitask else name
+                name_ = 'all' if multitask else name
                 finetune_data[name_] = [] if name_ not in finetune_data else finetune_data[name_]
 
                 for demo in predictor.demos:
                     demo = dict(demo)
 
                     # TODO: FIXME: generalize.
                     template = signature_to_template(predictor.signature)
@@ -108,82 +92,79 @@
 
                     finetune_data[name_].append(dict(prompt=prompt, completion=completion))
 
         for name_ in finetune_data:
             random.Random(0).shuffle(finetune_data[name_])
             print(name_, len(finetune_data[name_]))
 
+
         #
         # Dump as files.
-        #
+        # 
         finetune_paths = {}
 
         for name in finetune_data:
             data = finetune_data[name]
-            hashed_name = name + "." + Hasher.hash(data)
-            output_path = os.path.join(training_data_directory, f"{hashed_name}.jsonl")
+            hashed_name = name + '.' + Hasher.hash(data)
+            output_path = os.path.join(training_data_directory, f'{hashed_name}.jsonl')
             print(output_path)
 
-            with open(output_path, "w") as f:
+            with open(output_path, 'w') as f:
                 for line in data:
-                    f.write(ujson.dumps(line) + "\n")
-
+                    f.write(ujson.dumps(line) + '\n')
+            
             finetune_paths[name] = output_path
+        
 
         #
         # Train!
         #
         import string
-
         compiler_config = {
-            "save": "".join(
-                random.Random(time.time()).choices(string.ascii_uppercase + string.digits, k=13),
-            ),  # https://stackoverflow.com/a/2257449/1493011
-            "peft": peft,
-            "fp16": False,
-            "bf16": bf16,
-            "int8": int8,
-            "fid": False,
-            "rationale": False,
-            "batch_size": bsize,
-            "epochs": epochs,
-            "gradient_accumulation_steps": accumsteps,  # 2,
-            "lr": lr,
+            'save': ''.join(random.Random(time.time()).choices(string.ascii_uppercase + string.digits, k=13)), # https://stackoverflow.com/a/2257449/1493011
+            'peft': peft,
+            'fp16': False,
+            'bf16': bf16,
+            'int8': int8,
+            'fid': False,
+            'rationale': False,
+            'batch_size': bsize,
+            'epochs': epochs,
+            'gradient_accumulation_steps': accumsteps, # 2,
+            'lr': lr,
         }
 
-        compiler_config["save"] = (
-            os.path.join(path_prefix, compiler_config["save"]) if path_prefix else compiler_config["save"]
-        )
+        compiler_config['save'] = os.path.join(path_prefix, compiler_config['save']) if path_prefix else compiler_config['save']
 
         from dsp.modules.finetuning import finetune_hf
 
         target = target
         finetune_models = {}
 
         for name in finetune_data:
             training_data_path = finetune_paths[name]
             compiler_config_ = dict(compiler_config)
-            compiler_config_["save"] = compiler_config["save"] + "." + name
+            compiler_config_['save'] = compiler_config['save'] + '.' + name
             best_ckpt_path = finetune_hf(training_data_path, target, compiler_config_)
 
             print(f"#> Best checkpoint path: {best_ckpt_path} for {name}")
-            finetune_models[name] = dsp.HFModel(model=target, checkpoint=best_ckpt_path)  # best_ckpt_path
+            finetune_models[name] = dsp.HFModel(model=target, checkpoint=best_ckpt_path) # best_ckpt_path
 
         #
         # Set the LMs to the finetuned ones, per module
         #
         compiled2 = compiled.reset_copy()
 
         assert len(compiled.named_predictors()) == len(compiled2.named_predictors())
 
         for (name, predictor), (name2, predictor2) in zip(compiled.named_predictors(), compiled2.named_predictors()):
             assert name == name2
-            name = "all" if multitask else name
+            name = 'all' if multitask else name
 
             # TODO: FIXME: When we assign .lm, the Predict.forward will also set only_query=True.
             # This is correct for here but we may want to make it more explicitly restricted to finetuned models.
             print(f"Assigning the LM of predictor {name}.")
 
             predictor2.lm = finetune_models[name]
             assert predictor2.demos == []
-
+        
         return compiled2
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/knn_fewshot.py` & `dspy-ai-2.4.5/dspy/teleprompt/knn_fewshot.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,12 @@
 
     def compile(self, student, *, teacher=None, trainset, valset=None):
         student_copy = student.reset_copy()
 
         def forward_pass(*args, **kwargs):
             knn_trainset = self.KNN(**kwargs)
             few_shot_bootstrap = BootstrapFewShot()
-            compiled_program = few_shot_bootstrap.compile(
-                student,
-                teacher=teacher,
-                trainset=knn_trainset,
-                valset=valset,
-            )
+            compiled_program = few_shot_bootstrap.compile(student, teacher=teacher, trainset=knn_trainset, valset=valset)
             return compiled_program(**kwargs)
-
+        
         student_copy.forward = types.MethodType(forward_pass, student_copy)
-        return student_copy
+        return student_copy
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/mipro_optimizer.py` & `dspy-ai-2.4.5/dspy/teleprompt/mipro_optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
 import random
 import sys
 import textwrap
 from collections import defaultdict
-from typing import Any
 
 import optuna
 
 import dsp
 import dspy
 from dspy.evaluate.evaluate import Evaluate
 from dspy.signatures import Signature
@@ -40,168 +39,123 @@
                 and a value containing a dict with the following keys:
                     * program: the program being evaluated at a given trial
                     * score: the last average evaluated score for the program
                     * pruned: whether or not this program was pruned
                 This information will be returned as attributes of the best program.
 """
 
-
 class BasicGenerateInstruction(Signature):
     """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
 
     basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
     proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(
-        desc="The string at the end of the prompt, which will help the model start solving the task",
-    )
-
+    proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class BasicGenerateInstructionWithDataObservations(Signature):
     """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English.  I will also give you some ``observations`` I have made about the dataset and task. Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
 
     basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
     observations = dspy.InputField(desc="Observations about the dataset and task")
     proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(
-        desc="The string at the end of the prompt, which will help the model start solving the task",
-    )
-
+    proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class BasicGenerateInstructionWithExamples(dspy.Signature):
-    """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will also provide you with the current ``basic instruction`` that is being used for this task. I will also provide you with some ``examples`` of the expected inputs and outputs.
-
-    Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative."""
-
-    # attempted_instructions = dspy.InputField(format=str, desc="Previously attempted task instructions, along with their resulting validation score, and an example of the instruction in use on a sample from our dataset.")
-    basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
-    # examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
-    examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
-    proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(
-        desc="The string at the end of the prompt, which will help the model start solving the task",
-    )
+        ("""You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will also provide you with the current ``basic instruction`` that is being used for this task. I will also provide you with some ``examples`` of the expected inputs and outputs.
 
+Your task is to propose an instruction that will lead a good language model to perform the task well. Don't be afraid to be creative.""")
+        # attempted_instructions = dspy.InputField(format=str, desc="Previously attempted task instructions, along with their resulting validation score, and an example of the instruction in use on a sample from our dataset.")
+        basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
+        # examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
+        examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
+        proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
+        proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class BasicGenerateInstructionWithExamplesAndDataObservations(dspy.Signature):
-    """You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will give you some ``observations`` I have made about the dataset and task, along with some ``examples`` of the expected inputs and outputs. I will also provide you with the current ``basic instruction`` that is being used for this task.
-
-    Your task is to propose a new improved instruction and prefix for the output field that will lead a good language model to perform the task well. Don't be afraid to be creative."""
-
-    observations = dspy.InputField(desc="Observations about the dataset and task")
-    examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
-    basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
-    proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
-    proposed_prefix_for_output_field = dspy.OutputField(
-        desc="The string at the end of the prompt, which will help the model start solving the task",
-    )
+        ("""You are an instruction optimizer for large language models. I will give you a ``signature`` of fields (inputs and outputs) in English. Specifically, I will give you some ``observations`` I have made about the dataset and task, along with some ``examples`` of the expected inputs and outputs. I will also provide you with the current ``basic instruction`` that is being used for this task.
 
+Your task is to propose a new improved instruction and prefix for the output field that will lead a good language model to perform the task well. Don't be afraid to be creative.""")
+        observations = dspy.InputField(desc="Observations about the dataset and task")
+        examples = dspy.InputField(format=dsp.passages2text, desc="Example(s) of the task")
+        basic_instruction = dspy.InputField(desc="The initial instructions before optimization")
+        proposed_instruction = dspy.OutputField(desc="The improved instructions for the language model")
+        proposed_prefix_for_output_field = dspy.OutputField(desc="The string at the end of the prompt, which will help the model start solving the task")
 
 class ObservationSummarizer(dspy.Signature):
-    """Given a series of observations I have made about my dataset, please summarize them into a brief 2-3 sentence summary which highlights only the most important details."""
-
+    ("""Given a series of observations I have made about my dataset, please summarize them into a brief 2-3 sentence summary which highlights only the most important details.""")
     observations = dspy.InputField(desc="Observations I have made about my dataset")
-    summary = dspy.OutputField(
-        desc="Two to Three sentence summary of only the most significant highlights of my observations",
-    )
-
+    summary = dspy.OutputField(desc="Two to Three sentence summary of only the most significant highlights of my observations")
 
 class DatasetDescriptor(dspy.Signature):
-    (
-        """Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
-        """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
-        """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative"""
-    )
-
+    ("""Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
+    """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
+    """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative""")
+    
     examples = dspy.InputField(desc="Sample data points from the dataset")
     observations = dspy.OutputField(desc="Somethings that holds true for most or all of the data you observed")
 
-
 class DatasetDescriptorWithPriorObservations(dspy.Signature):
-    (
-        """Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
-        """I will also provide you with a few observations I have already made.  Please add your own observations or if you feel the observations are comprehensive say 'COMPLETE' """
-        """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
-        """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative"""
-    )
-
+    ("""Given several examples from a dataset please write observations about trends that hold for most or all of the samples. """
+    """I will also provide you with a few observations I have already made.  Please add your own observations or if you feel the observations are comprehensive say 'COMPLETE' """
+    """Some areas you may consider in your observations: topics, content, syntax, conciceness, etc. """
+    """It will be useful to make an educated guess as to the nature of the task this dataset will enable. Don't be afraid to be creative""")
+    
     examples = dspy.InputField(desc="Sample data points from the dataset")
     prior_observations = dspy.InputField(desc="Some prior observations I made about the data")
-    observations = dspy.OutputField(
-        desc="Somethings that holds true for most or all of the data you observed or COMPLETE if you have nothing to add",
-    )
-
+    observations = dspy.OutputField(desc="Somethings that holds true for most or all of the data you observed or COMPLETE if you have nothing to add")
 
 class MIPRO(Teleprompter):
-    def __init__(
-        self,
-        metric,
-        prompt_model=None,
-        task_model=None,
-        teacher_settings={},
-        num_candidates=10,
-        init_temperature=1.0,
-        verbose=False,
-        track_stats=True,
-        view_data_batch_size=10,
-    ):
+    def __init__(self, metric, prompt_model=None, task_model=None, teacher_settings={}, num_candidates=10, init_temperature=1.0, verbose=False, track_stats=True, view_data_batch_size=10):
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
-        for i, predictor in enumerate(program.predictors()):
-            if self.verbose:
-                print(f"Predictor {i}")
-            if self.verbose:
-                print(f"i: {self._get_signature(predictor).instructions}")
+        for i,predictor in enumerate(program.predictors()):
+            if self.verbose: print(f"Predictor {i}")
+            if self.verbose: print(f"i: {self._get_signature(predictor).instructions}")
             *_, last_field = self._get_signature(predictor).fields.values()
-            if self.verbose:
-                print(f"p: {last_field.json_schema_extra['prefix']}")
-            if self.verbose:
-                print("\n")
-
+            if self.verbose: print(f"p: {last_field.json_schema_extra['prefix']}")
+            if self.verbose: print("\n")
+    
     def _print_model_history(self, model, n=1):
-        if self.verbose:
-            print(f"Model ({model}) History:")
+        if self.verbose: print(f"Model ({model}) History:")
         model.inspect_history(n=n)
 
     def _observe_data(self, trainset, max_iterations=10):
         upper_lim = min(len(trainset), self.view_data_batch_size)
         observation = dspy.Predict(DatasetDescriptor, n=1, temperature=1.0)(examples=(trainset[0:upper_lim].__repr__()))
         observations = observation["observations"]
 
         skips = 0
         iterations = 0
         for b in range(self.view_data_batch_size, len(trainset), self.view_data_batch_size):
-            upper_lim = min(len(trainset), b + self.view_data_batch_size)
-            output = dspy.Predict(DatasetDescriptorWithPriorObservations, n=1, temperature=1.0)(
-                prior_observations=observations,
-                examples=(trainset[b:upper_lim].__repr__()),
-            )
+            upper_lim = min(len(trainset), b+self.view_data_batch_size)
+            output = dspy.Predict(DatasetDescriptorWithPriorObservations, n=1, temperature=1.0)(prior_observations=observations, examples=(trainset[b:upper_lim].__repr__()))
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
+    
     def _create_example_string(self, fields, example):
+
         # Building the output string
         output = []
         for field in fields:
             name = field.name
             separator = field.separator
             input_variable = field.input_variable
 
@@ -209,79 +163,71 @@
             value = example.get(input_variable)
 
             # Construct the string for the current field
             field_str = f"{name}{separator}{value}"
             output.append(field_str)
 
         # Joining all the field strings
-        return "\n".join(output)
+        return '\n'.join(output)
 
     def _get_signature(self, predictor):
-        if hasattr(predictor, "extended_signature"):
+        if (hasattr(predictor, 'extended_signature')):
             return predictor.extended_signature
-        elif hasattr(predictor, "signature"):
+        elif (hasattr(predictor, 'signature')):
             return predictor.signature
-        return None
-
+    
     def _set_signature(self, predictor, updated_signature):
-        if hasattr(predictor, "extended_signature"):
+        if (hasattr(predictor, 'extended_signature')):
             predictor.extended_signature = updated_signature
-        elif hasattr(predictor, "signature"):
+        elif (hasattr(predictor, 'signature')):
             predictor.signature = updated_signature
-
-    def _generate_first_N_candidates(  # noqa: N802
-        self,
-        module: dspy.Module,
-        N: int,  # noqa: N803
-        view_data: bool,
-        view_examples: bool,
-        demo_candidates: dict,
-        devset,
-    ) -> tuple[dict, dict]:
+    
+    def _generate_first_N_candidates(self, module, N, view_data, view_examples, demo_candidates, devset):
         candidates = {}
         evaluated_candidates = defaultdict(dict)
 
         if view_data:
             # Create data observations
             self.observations = None
             with dspy.settings.context(lm=self.prompt_model):
-                self.observations = self._observe_data(devset).replace("Observations:", "").replace("Summary:", "")
-
+                self.observations = self._observe_data(devset).replace("Observations:","").replace("Summary:","")
+            
         if view_examples:
             example_sets = {}
             for predictor in module.predictors():
                 # Get all augmented examples
                 example_set = {}
-                all_sets_of_examples = demo_candidates[id(predictor)]  # Get all generated sets of examples
+                all_sets_of_examples = demo_candidates[id(predictor)] # Get all generated sets of examples
                 for example_set_i, set_of_examples in enumerate(all_sets_of_examples):
-                    if example_set_i != 0:  # Skip the no examples case
-                        for example in set_of_examples:  # Get each individual example in the set
-                            if "augmented" in example and example["augmented"]:
-                                if example_set_i not in example_set:
-                                    example_set[example_set_i] = []
-                                fields_to_use = signature_to_template(predictor.signature).fields
-                                _input_variable_names = list(self._get_signature(predictor).input_fields.keys())
-                                example_string = self._create_example_string(fields_to_use, example)
-                                example_set[example_set_i].append(example_string)
-                        example_sets[id(predictor)] = example_set
+                    if example_set_i != 0: # Skip the no examples case
+                        for example in set_of_examples: # Get each individual example in the set
+                            if "augmented" in example.keys():
+                                if example["augmented"]:
+                                    if example_set_i not in example_set:
+                                        example_set[example_set_i] = []
+                                    fields_to_use = signature_to_template(predictor.signature).fields
+                                    input_variable_names = list(self._get_signature(predictor).input_fields.keys())
+                                    example_string = self._create_example_string(fields_to_use, example)
+                                    example_set[example_set_i].append(example_string)
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
-                    if 1 not in example_sets[id(predictor)]:
+                    if 1 not in example_sets[id(predictor)].keys():
                         raise ValueError("No examples found for the given predictor")
                     instruct = None
                     for i in range(1, self.num_candidates):
                         new_instruct = dspy.Predict(
                             BasicGenerateInstructionWithExamplesAndDataObservations,
                             n=1,
                             temperature=self.init_temperature,
@@ -289,91 +235,61 @@
                             basic_instruction=basic_instruction,
                             observations=self.observations,
                             examples=example_sets[id(predictor)][i],
                         )
                         if not instruct:
                             instruct = new_instruct
                         else:
-                            instruct.completions.proposed_instruction.extend(
-                                new_instruct.completions.proposed_instruction,
-                            )
-                            instruct.completions.proposed_prefix_for_output_field.extend(
-                                new_instruct.completions.proposed_prefix_for_output_field,
-                            )
+                            instruct.completions.proposed_instruction.extend(new_instruct.completions.proposed_instruction)
+                            instruct.completions.proposed_prefix_for_output_field.extend(new_instruct.completions.proposed_prefix_for_output_field)
                 # Just data
-                elif view_data:
-                    instruct = dspy.Predict(
-                        BasicGenerateInstructionWithDataObservations,
-                        n=N - 1,
-                        temperature=self.init_temperature,
-                    )(basic_instruction=basic_instruction, observations=self.observations)
+                elif view_data: 
+                    instruct = dspy.Predict(BasicGenerateInstructionWithDataObservations, n=N-1, temperature=self.init_temperature)(basic_instruction=basic_instruction, observations=self.observations)
                 # Just examples
-                elif view_examples:
+                elif view_examples: 
                     instruct = None
-                    for i in range(1, self.num_candidates):  # Note: skip over the first example set which is empty
+                    for i in range(1,self.num_candidates): # Note: skip over the first example set which is empty
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
-                            instruct.completions.proposed_instruction.extend(
-                                new_instruct.completions.proposed_instruction,
-                            )
-                            instruct.completions.proposed_prefix_for_output_field.extend(
-                                new_instruct.completions.proposed_prefix_for_output_field,
-                            )
+                            instruct.completions.proposed_instruction.extend(new_instruct.completions.proposed_instruction)
+                            instruct.completions.proposed_prefix_for_output_field.extend(new_instruct.completions.proposed_prefix_for_output_field)
                 # Neither
-                else:
-                    instruct = dspy.Predict(BasicGenerateInstruction, n=N - 1, temperature=self.init_temperature)(
-                        basic_instruction=basic_instruction,
-                    )
-
+                else: 
+                    instruct = dspy.Predict(BasicGenerateInstruction, n=N-1, temperature=self.init_temperature)(basic_instruction=basic_instruction)
+            
             # Add in our initial prompt as a candidate as well
             instruct.completions.proposed_instruction.insert(0, basic_instruction)
             instruct.completions.proposed_prefix_for_output_field.insert(0, basic_prefix)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
-
-        if self.verbose:
-            self._print_model_history(self.prompt_model)
-
+        
+        if self.verbose: self._print_model_history(self.prompt_model)
+        
         return candidates, evaluated_candidates
 
-    def compile(
-        self,
-        student: dspy.Program,
-        *,
-        trainset: list[dspy.Example],
-        num_trials: int,
-        max_bootstrapped_demos: int,
-        max_labeled_demos: int,
-        eval_kwargs: dict[str, Any],
-        seed=42,
-        view_data=True,
-        view_examples=True,
-        requires_permission_to_run=True,
-    ) -> dspy.Program:
+    def compile(self, student, *, trainset, num_trials, max_bootstrapped_demos, max_labeled_demos, eval_kwargs, seed=42, view_data=True, view_examples=True, requires_permission_to_run=True):
         # Define ANSI escape codes for colors
-        YELLOW = "\033[93m"
-        BLUE = "\033[94m"
-        BOLD = "\033[1m"
-        ENDC = "\033[0m"  # Resets the color to default
+        YELLOW = '\033[93m'
+        BLUE = '\033[94m'
+        BOLD = '\033[1m'
+        ENDC = '\033[0m'  # Resets the color to default
 
         random.seed(seed)
-
+        
         estimated_task_model_calls_wo_module_calls = len(trainset) * num_trials  # M * T * P
-        estimated_prompt_model_calls = 10 + self.num_candidates * len(
-            student.predictors(),
-        )  # num data summary calls + N * P
+        estimated_prompt_model_calls = 10 + self.num_candidates * len(student.predictors()) # num data summary calls + N * P
 
         user_message = textwrap.dedent(f"""\
             {YELLOW}{BOLD}WARNING: Projected Language Model (LM) Calls{ENDC}
 
             Please be advised that based on the parameters you have set, the maximum number of LM calls is projected as follows:
 
             {YELLOW}- Task Model: {BLUE}{BOLD}{len(trainset)}{ENDC}{YELLOW} examples in dev set * {BLUE}{BOLD}{num_trials}{ENDC}{YELLOW} trials * {BLUE}{BOLD}# of LM calls in your program{ENDC}{YELLOW} = ({BLUE}{BOLD}{estimated_task_model_calls_wo_module_calls} * # of LM calls in your program{ENDC}{YELLOW}) task model calls{ENDC}
@@ -385,212 +301,177 @@
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
+        
         sys.stdout.flush()  # Flush the output buffer to force the message to print
 
-        run = True
+
+        run=True
         if requires_permission_to_run:
             print(user_confirmation_message)
             user_input = input("Do you wish to continue? (y/n): ").strip().lower()
-            if user_input != "y":
+            if user_input != 'y':
                 print("Compilation aborted by the user.")
-                run = False
+                run=False
 
         if run:
             # Set up program and evaluation function
             module = student.deepcopy()
             evaluate = Evaluate(devset=trainset, metric=self.metric, **eval_kwargs)
-
+            
             # In the case where the bootstrapped and labeled demos are set to 0, we'll stil bootstrap examples to use in our meta prompt
-            if (
-                max_bootstrapped_demos == 0 and max_labeled_demos == 0
-            ):  # TODO: address case when max_bootstrapped alone is 0
-                max_bootstrapped_demos_for_candidate_gen = 1
-                max_labeled_demos_for_candidate_gen = 1  # TODO: this might only need to be 0
+            if max_bootstrapped_demos==0 and max_labeled_demos==0: #TODO: address case when max_bootstrapped alone is 0
+                max_bootstrapped_demos_for_candidate_gen = 1 
+                max_labeled_demos_for_candidate_gen = 1 #TODO: this might only need to be 0
             else:
-                max_bootstrapped_demos_for_candidate_gen = max_bootstrapped_demos
+                max_bootstrapped_demos_for_candidate_gen = max_bootstrapped_demos 
                 max_labeled_demos_for_candidate_gen = max_labeled_demos
 
             # Generate N few shot example sets
             demo_candidates = {}
             for i in range(self.num_candidates):
-                if i == 0:  # Story empty set of demos as default for index 0
+                if i == 0: # Story empty set of demos as default for index 0
                     for module_p in module.predictors():
                         if id(module_p) not in demo_candidates:
                             demo_candidates[id(module_p)] = []
                         demo_candidates[id(module_p)].append([])
                 else:
-                    if self.verbose:
-                        print(f"Creating basic bootstrap: {i}/{self.num_candidates-1}")
+                    if self.verbose: print(f"Creating basic bootstrap: {i}/{self.num_candidates-1}")
 
                     # Create a new basic bootstrap few - shot program .
                     rng = random.Random(i)
                     shuffled_trainset = trainset[:]  # Create a copy of devset
                     rng.shuffle(shuffled_trainset)  # Shuffle the copy
-                    tp = BootstrapFewShot(
-                        metric=self.metric,
-                        max_bootstrapped_demos=max_bootstrapped_demos_for_candidate_gen,
-                        max_labeled_demos=max_labeled_demos_for_candidate_gen,
-                        teacher_settings=self.teacher_settings,
-                    )
+                    tp = BootstrapFewShot(metric = self.metric, max_bootstrapped_demos=max_bootstrapped_demos_for_candidate_gen, max_labeled_demos=max_labeled_demos_for_candidate_gen, teacher_settings=self.teacher_settings)
                     candidate_program = tp.compile(student=module.deepcopy(), trainset=shuffled_trainset)
 
                     # Store the candidate demos
                     for module_p, candidate_p in zip(module.predictors(), candidate_program.predictors()):
                         if id(module_p) not in demo_candidates:
                             demo_candidates[id(module_p)] = []
                         demo_candidates[id(module_p)].append(candidate_p.demos)
-
+                
             # Generate N candidate prompts
-            instruction_candidates, _ = self._generate_first_N_candidates(
-                module,
-                self.num_candidates,
-                view_data,
-                view_examples,
-                demo_candidates,
-                trainset,
-            )
+            instruction_candidates, _ = self._generate_first_N_candidates(module, self.num_candidates, view_data, view_examples, demo_candidates, trainset)
 
             # Reset demo_candidates to None for our optimization if the user asked for no fewshot examples
-            if max_bootstrapped_demos == 0 and max_labeled_demos == 0:
+            if max_bootstrapped_demos==0 and max_labeled_demos==0:
                 demo_candidates = None
 
             # Initialize variables to store the best program and its score
-            best_score = float("-inf")
+            best_score = float('-inf')
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
+
                         # Get instruction candidates for our given predictor
                         p_instruction_candidates = instruction_candidates[id(p_old)]
-                        if demo_candidates:
-                            p_demo_candidates = demo_candidates[id(p_old)]
+                        if demo_candidates: p_demo_candidates = demo_candidates[id(p_old)]
 
                         # Suggest the index of the instruction candidate to use in our trial
-                        instruction_idx = trial.suggest_categorical(
-                            f"{id(p_old)}_predictor_instruction",
-                            range(len(p_instruction_candidates)),
-                        )
-                        if demo_candidates:
-                            demos_idx = trial.suggest_categorical(
-                                f"{id(p_old)}_predictor_demos",
-                                range(len(p_demo_candidates)),
-                            )
+                        instruction_idx = trial.suggest_categorical(f"{id(p_old)}_predictor_instruction",range(len(p_instruction_candidates)))
+                        if demo_candidates: demos_idx = trial.suggest_categorical(f"{id(p_old)}_predictor_demos",range(len(p_demo_candidates)))
                         trial_logs[trial_num][f"{id(p_old)}_predictor_instruction"] = instruction_idx
-                        if demo_candidates:
-                            trial_logs[trial_num][f"{id(p_old)}_predictor_demos"] = demos_idx
+                        if demo_candidates: trial_logs[trial_num][f"{id(p_old)}_predictor_demos"] = demos_idx
 
-                        # Get the selected instruction candidate
+                        # Get the selected instruction candidate 
                         selected_candidate = p_instruction_candidates[instruction_idx]
                         selected_instruction = selected_candidate.proposed_instruction.strip('"').strip()
                         selected_prefix = selected_candidate.proposed_prefix_for_output_field.strip('"').strip()
 
                         # Use this candidates in our program
                         *_, last_field = self._get_signature(p_new).fields.keys()
-                        updated_signature = (
-                            self._get_signature(p_new)
-                            .with_instructions(selected_instruction)
-                            .with_updated_fields(last_field, prefix=selected_prefix)
-                        )
+                        updated_signature = self._get_signature(p_new).with_instructions(selected_instruction).with_updated_fields(last_field, prefix=selected_prefix)
                         self._set_signature(p_new, updated_signature)
 
                         # Get the selected demos
-                        if demo_candidates:
-                            selected_demos = p_demo_candidates[demos_idx]
+                        if demo_candidates: selected_demos = p_demo_candidates[demos_idx]
 
                         # Use these demos in our program
-                        if demo_candidates:
-                            p_new.demos = selected_demos
-
-                    if self.verbose:
-                        print("Evaling the following program:")
-                    if self.verbose:
-                        self._print_full_program(candidate_program)
+                        if demo_candidates: p_new.demos = selected_demos
+                        
+                    if self.verbose: print("Evaling the following program:")
+                    if self.verbose: self._print_full_program(candidate_program)
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
-                        if self.verbose:
-                            print(f"{i}st split score: {split_score}")
+                        if self.verbose: print(f"{i}st split score: {split_score}")
 
                         total_score += split_score * len(split_trainset)
-                        curr_weighted_avg_score = total_score / min((i + 1) * 100, len(trainset))
-                        if self.verbose:
-                            print(f"curr average score: {curr_weighted_avg_score}")
+                        curr_weighted_avg_score = total_score / min((i+1)*100,len(trainset))
+                        if self.verbose: print(f"curr average score: {curr_weighted_avg_score}")
 
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
-                    if self.verbose:
-                        print(f"Fully evaled score: {curr_weighted_avg_score}")
-                    if self.verbose:
-                        self._print_model_history(self.task_model, n=1)
+                    
+                    if self.verbose: print(f"Fully evaled score: {curr_weighted_avg_score}")
+                    if self.verbose: self._print_model_history(self.task_model, n=1)
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
-            _score = study.optimize(objective_function, n_trials=num_trials)
+            score = study.optimize(objective_function, n_trials=num_trials)
 
             if best_program is not None and self.track_stats:
                 best_program.trial_logs = trial_logs
 
             print(f"Returning {best_program} from continue_program")
-            return best_program
-        return None
+            return best_program
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/random_search.py` & `dspy-ai-2.4.5/dspy/teleprompt/random_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,15 @@
 # Progressive elimination sounds about right: after 50 examples, drop bottom third, after 100, another third, etc.
 # until only 3--5 are left for the end. Could also be systematic and add (earlier) stopping based on error bounds.
 # In general, though, the early filtering is just saying: either there are some really bad ones, or some really really
 # good ones, or most things are pretty close. In all of these cases, dropping the bottom third is not going to hurt.
 
 
 class BootstrapFewShotWithRandomSearch(Teleprompter):
-    def __init__(
-        self,
-        metric,
-        teacher_settings={},
-        max_bootstrapped_demos=4,
-        max_labeled_demos=16,
-        max_rounds=1,
-        num_candidate_programs=16,
-        num_threads=6,
-        max_errors=10,
-        stop_at_score=None,
-        metric_threshold=None,
-    ):
+    def __init__(self, metric, teacher_settings={}, max_bootstrapped_demos=4, max_labeled_demos=16, max_rounds=1, num_candidate_programs=16, num_threads=6, max_errors=10, stop_at_score=None, metric_threshold=None):
         self.metric = metric
         self.teacher_settings = teacher_settings
         self.max_rounds = max_rounds
 
         self.num_threads = num_threads
         self.stop_at_score = stop_at_score
         self.metric_threshold = metric_threshold
@@ -72,105 +60,92 @@
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
-                program = BootstrapFewShot(
-                    metric=self.metric,
-                    metric_threshold=self.metric_threshold,
-                    max_bootstrapped_demos=self.max_num_samples,
-                    max_labeled_demos=self.max_labeled_demos,
-                    teacher_settings=self.teacher_settings,
-                    max_rounds=self.max_rounds,
-                )
+                program = BootstrapFewShot(metric=self.metric, metric_threshold=self.metric_threshold, max_bootstrapped_demos=self.max_num_samples,
+                                           max_labeled_demos=self.max_labeled_demos,
+                                           teacher_settings=self.teacher_settings, max_rounds=self.max_rounds)
                 program2 = program.compile(student, teacher=teacher, trainset=trainset2)
 
             else:
                 assert seed >= 0, seed
 
                 random.Random(seed).shuffle(trainset2)
                 size = random.Random(seed).randint(self.min_num_samples, self.max_num_samples)
 
-                teleprompter = BootstrapFewShot(
-                    metric=self.metric,
-                    metric_threshold=self.metric_threshold,
-                    max_bootstrapped_demos=size,
-                    max_labeled_demos=self.max_labeled_demos,
-                    teacher_settings=self.teacher_settings,
-                    max_rounds=self.max_rounds,
-                )
+                teleprompter = BootstrapFewShot(metric=self.metric, metric_threshold=self.metric_threshold, max_bootstrapped_demos=size,
+                                                max_labeled_demos=self.max_labeled_demos,
+                                                teacher_settings=self.teacher_settings,
+                                                max_rounds=self.max_rounds)
 
                 program2 = teleprompter.compile(student, teacher=teacher, trainset=trainset2)
 
-            evaluate = Evaluate(
-                devset=self.valset,
-                metric=self.metric,
-                num_threads=self.num_threads,
-                max_errors=self.max_errors,
-                display_table=False,
-                display_progress=True,
-            )
+            evaluate = Evaluate(devset=self.valset, metric=self.metric, num_threads=self.num_threads,
+                                max_errors=self.max_errors, display_table=False, display_progress=True)
 
             score, subscores = evaluate(program2, return_all_scores=True)
 
             all_subscores.append(subscores)
 
             ############ Assertion-aware Optimization ############
-            if hasattr(program2, "_suggest_failures"):
+            if hasattr(program2, '_suggest_failures'):
                 score = score - program2._suggest_failures * 0.2
-            if hasattr(program2, "_assert_failures"):
+            if hasattr(program2, '_assert_failures'):
                 score = 0 if program2._assert_failures > 0 else score
             ######################################################
 
-            print("Score:", score, "for set:", [len(predictor.demos) for predictor in program2.predictors()])
+            print('Score:', score, 'for set:', [len(predictor.demos) for predictor in program2.predictors()])
 
             if len(scores) == 0 or score > max(scores):
-                print("New best score:", score, "for seed", seed)
+                print('New best score:', score, 'for seed', seed)
                 best_program = program2
 
             scores.append(score)
             print(f"Scores so far: {scores}")
 
-            print("Best score:", max(scores))
+            print('Best score:', max(scores))
 
             score_data.append((score, subscores, seed, program2))
 
             if len(score_data) > 2:  # We check if there are at least 3 scores to consider
                 for k in [1, 2, 3, 5, 8, 9999]:
                     top_3_scores = sorted(score_data, key=lambda x: x[0], reverse=True)[:k]
 
                     # Transpose the subscores to get max per entry and then calculate their average
                     transposed_subscores = zip(*[subscores for _, subscores, *_ in top_3_scores if subscores])
                     avg_of_max_per_entry = sum(max(entry) for entry in transposed_subscores) / len(top_3_scores[0][1])
 
-                    print(f"Average of max per entry across top {k} scores: {avg_of_max_per_entry}")
-
+                    print(f'Average of max per entry across top {k} scores: {avg_of_max_per_entry}')
+            
             if self.stop_at_score is not None and score >= self.stop_at_score:
                 print(f"Stopping early because score {score} is >= stop_at_score {self.stop_at_score}")
                 break
 
         # To best program, attach all program candidates in decreasing average score
         best_program.candidate_programs = score_data
         best_program.candidate_programs = sorted(best_program.candidate_programs, key=lambda x: x[0], reverse=True)
 
         print(len(best_program.candidate_programs), "candidate programs found.")
 
         return best_program
 
 
+
+
 # sample between 4 and 10 examples from traces
 # TODO: FIXME: The max number of demos should be determined in part by the LM's tokenizer + max_length.
 # This does require executing the program, or at least the predictor.
 # # # # # # (Actually we can just combine the token counts of the traces, when formatted via signature/adapter).
 # Alternatively, we can keep track of the (zero-shot) number of tokens when we bootstrap.
 # As another option, we can just try a wide range and handle failures as penalties on the score.
 # The number "24" of traces to collect can also be affected. If we only need 3x10, some overlap is ok.
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/signature_opt.py` & `dspy-ai-2.4.5/dspy/teleprompt/signature_opt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from .copro_optimizer import COPRO
 
 """
 ===============================================================
 DEPRECATED!!!
 PLEASE USE COPRO INSTEAD.
 ===============================================================
@@ -27,26 +28,14 @@
                 If True, the method will track the following statistics:
                     * results_best: The min,max,avg,stddev of top 10 scores for each predictor at each depth.
                     * results_latest: The min,max,avg,stddev of newest prompt scores for each predictor at each depth.
                     * total_calls: The total number of calls to the task metric.
                 These statistics will be returned as attributes of the best program.
 """
 
-
 class SignatureOptimizer(COPRO):
-    def __init__(
-        self,
-        prompt_model=None,
-        metric=None,
-        breadth=10,
-        depth=3,
-        init_temperature=1.4,
-        verbose=False,
-        track_stats=False,
-    ):
-        print(
-            "\u001b[31m[WARNING] SignatureOptimizer has been deprecated and replaced with COPRO.  SignatureOptimizer will be removed in a future release. \u001b[31m",
-        )
+    def __init__(self, prompt_model=None, metric=None, breadth=10, depth=3, init_temperature=1.4, verbose=False, track_stats=False):
+        print("\u001b[31m[WARNING] SignatureOptimizer has been deprecated and replaced with COPRO.  SignatureOptimizer will be removed in a future release. \u001b[31m")
         super().__init__(prompt_model, metric, breadth, depth, init_temperature, verbose, track_stats)
 
     def compile(self, student, *, devset, eval_kwargs):
-        return super().compile(student, trainset=devset, eval_kwargs=eval_kwargs)
+        return super().compile(student, trainset=devset, eval_kwargs=eval_kwargs)
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/signature_opt_bayesian.py` & `dspy-ai-2.4.5/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from dspy.teleprompt.mipro_optimizer import MIPRO
 
 """
 ===============================================================
 DEPRECATED!!!
 PLEASE USE MIPRO INSTEAD.
 ===============================================================
@@ -30,64 +31,15 @@
                 and a value containing a dict with the following keys:
                     * program: the program being evaluated at a given trial
                     * score: the last average evaluated score for the program
                     * pruned: whether or not this program was pruned
                 This information will be returned as attributes of the best program.
 """
 
-
 class BayesianSignatureOptimizer(MIPRO):
-    def __init__(
-        self,
-        prompt_model=None,
-        task_model=None,
-        teacher_settings={},
-        n=10,
-        metric=None,
-        init_temperature=1.0,
-        verbose=False,
-        track_stats=True,
-        view_data_batch_size=10,
-    ):
-        print(
-            "\u001b[31m[WARNING] BayesianSignatureOptimizer has been deprecated and replaced with MIPRO.  BayesianSignatureOptimizer will be removed in a future release. \u001b[31m",
-        )
-
-        super().__init__(
-            metric=metric,
-            prompt_model=prompt_model,
-            task_model=task_model,
-            teacher_settings=teacher_settings,
-            num_candidates=n,
-            init_temperature=init_temperature,
-            verbose=verbose,
-            track_stats=track_stats,
-            view_data_batch_size=view_data_batch_size,
-        )
-
-    def compile(
-        self,
-        student,
-        *,
-        devset,
-        max_bootstrapped_demos,
-        max_labeled_demos,
-        eval_kwargs,
-        seed=42,
-        optuna_trials_num,
-        view_data=True,
-        view_examples=True,
-        requires_permission_to_run=False,
-        num_trials=None,
-    ):
-        return super().compile(
-            student,
-            trainset=devset,
-            max_bootstrapped_demos=max_bootstrapped_demos,
-            max_labeled_demos=max_labeled_demos,
-            eval_kwargs=eval_kwargs,
-            seed=seed,
-            view_data=view_data,
-            view_examples=view_examples,
-            requires_permission_to_run=requires_permission_to_run,
-            num_trials=optuna_trials_num,
-        )
+    def __init__(self, prompt_model=None, task_model=None, teacher_settings={}, n=10, metric=None, init_temperature=1.0, verbose=False, track_stats=True, view_data_batch_size=10):
+        print("\u001b[31m[WARNING] BayesianSignatureOptimizer has been deprecated and replaced with MIPRO.  BayesianSignatureOptimizer will be removed in a future release. \u001b[31m")
+
+        super().__init__(metric=metric,prompt_model=prompt_model, task_model=task_model, teacher_settings=teacher_settings,num_candidates=n,init_temperature=init_temperature,verbose=verbose,track_stats=track_stats,view_data_batch_size=view_data_batch_size)
+
+    def compile(self, student, *, devset, max_bootstrapped_demos, max_labeled_demos, eval_kwargs, seed=42, optuna_trials_num, view_data=True, view_examples=True, requires_permission_to_run=False, num_trials=None):
+        return super().compile(student, trainset=devset, max_bootstrapped_demos=max_bootstrapped_demos, max_labeled_demos=max_labeled_demos, eval_kwargs=eval_kwargs, seed=seed, view_data=view_data, view_examples=view_examples, requires_permission_to_run=requires_permission_to_run, num_trials=optuna_trials_num)
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/signature_opt_typed.py` & `dspy-ai-2.4.5/dspy/teleprompt/signature_opt_typed.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,19 +268,17 @@
                 new_signature = generator().proposed_signature
                 candidates[name].append(new_signature)
 
     if strategy == "last":
         pass
     elif strategy == "best":
         i = scores.index(max(scores))
-        if verbose:
-            print(f"Best signature: {i} with score: {scores[i]}")
         for name, p in named_predictors:
             p.signature = candidates[name][i].to_signature()
     else:
         raise ValueError(f"Invalid strategy: {strategy}")
 
     return OptimizerResult(
         program=module,
-        signatures=[{name: sigs[i].to_signature() for name, sigs in candidates.items()} for i in range(n_iterations)],
+        signatures=[{name: sigs[i].to_signature()} for name, sigs in candidates.items() for i in range(n_iterations)],
         scores=scores,
     )
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/teleprompt_optuna.py` & `dspy-ai-2.4.5/dspy/teleprompt/teleprompt_optuna.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,15 @@
 from dspy.evaluate.evaluate import Evaluate
 from dspy.teleprompt.teleprompt import Teleprompter
 
 from .bootstrap import BootstrapFewShot
 
 
 class BootstrapFewShotWithOptuna(Teleprompter):
-    def __init__(
-        self,
-        metric,
-        teacher_settings={},
-        max_bootstrapped_demos=4,
-        max_labeled_demos=16,
-        max_rounds=1,
-        num_candidate_programs=16,
-        num_threads=6,
-    ):
+    def __init__(self, metric, teacher_settings={}, max_bootstrapped_demos=4, max_labeled_demos=16, max_rounds=1, num_candidate_programs=16, num_threads=6):
         self.metric = metric
         self.teacher_settings = teacher_settings
         self.max_rounds = max_rounds
 
         self.num_threads = num_threads
 
         self.min_num_samples = 1
@@ -34,46 +25,35 @@
 
         print("Going to sample between", self.min_num_samples, "and", self.max_num_samples, "traces per predictor.")
         # print("Going to sample", self.max_num_traces, "traces in total.")
         print("Will attempt to train", self.num_candidate_sets, "candidate sets.")
 
     def objective(self, trial):
         program2 = self.student.reset_copy()
-        for (name, compiled_predictor), (_, program2_predictor) in zip(
-            self.compiled_teleprompter.named_predictors(), program2.named_predictors(),
-        ):
+        for (name, compiled_predictor), (_, program2_predictor) in zip(self.compiled_teleprompter.named_predictors(), program2.named_predictors()):
             all_demos = compiled_predictor.demos
             demo_index = trial.suggest_int(f"demo_index_for_{name}", 0, len(all_demos) - 1)
             selected_demo = dict(all_demos[demo_index])
             program2_predictor.demos = [selected_demo]
-        evaluate = Evaluate(
-            devset=self.valset,
-            metric=self.metric,
-            num_threads=self.num_threads,
-            display_table=False,
-            display_progress=True,
-        )
+        evaluate = Evaluate(devset=self.valset, metric=self.metric, num_threads=self.num_threads,
+                            display_table=False, display_progress=True)
         score, _ = evaluate(program2, return_all_scores=True)
         trial.set_user_attr("program", program2)
         return score
 
+
     def compile(self, student, *, teacher=None, max_demos, trainset, valset=None):
         self.trainset = trainset
         self.valset = valset or trainset
         self.student = student.reset_copy()
         self.teacher = teacher.deepcopy() if teacher is not None else student.reset_copy()
-        teleprompter_optimize = BootstrapFewShot(
-            metric=self.metric,
-            max_bootstrapped_demos=max_demos,
-            max_labeled_demos=self.max_labeled_demos,
-            teacher_settings=self.teacher_settings,
-            max_rounds=self.max_rounds,
-        )
-        self.compiled_teleprompter = teleprompter_optimize.compile(
-            self.student, teacher=self.teacher, trainset=self.trainset,
-        )
-        study = optuna.create_study(direction="maximize")
+        teleprompter_optimize = BootstrapFewShot(metric=self.metric, max_bootstrapped_demos=max_demos,
+                                        max_labeled_demos=self.max_labeled_demos,
+                                        teacher_settings=self.teacher_settings,
+                                        max_rounds=self.max_rounds)
+        self.compiled_teleprompter = teleprompter_optimize.compile(self.student, teacher=self.teacher, trainset=self.trainset)
+        study = optuna.create_study(direction='maximize')
         study.optimize(self.objective, n_trials=self.num_candidate_sets)
         best_program = study.trials[study.best_trial.number].user_attrs["program"]
-        print("Best score:", study.best_value)
-        print("Best program:", best_program)
-        return best_program
+        print('Best score:', study.best_value)
+        print('Best program:', best_program)
+        return best_program
```

### Comparing `dspy-ai-2.4.4/dspy/teleprompt/vanilla.py` & `dspy-ai-2.4.5/dspy/teleprompt/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
         rng = random.Random(0)
 
         for predictor in self.student.predictors():
             if sample:
                 predictor.demos = rng.sample(self.trainset, min(self.k, len(self.trainset)))
             else:
-                predictor.demos = self.trainset[: min(self.k, len(self.trainset))]
+                predictor.demos = self.trainset[:min(self.k, len(self.trainset))]
 
         return self.student
-
-
+    
 # NOTE: I believe templatev2 keeps rdemos as long as they have the last field.
 # This may change later, especially with the introduction of required vs optional fields.
 # NOTE: Since we're relying on downstream code to handle the demos, this sampling may be sub-sampled.
```

### Comparing `dspy-ai-2.4.4/dspy/utils/dummies.py` & `dspy-ai-2.4.5/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/dspy_ai.egg-info/PKG-INFO` & `dspy-ai-2.4.5/dspy_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.4
+Version: 2.4.5
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dspy-ai-2.4.4/dspy_ai.egg-info/SOURCES.txt` & `dspy-ai-2.4.5/dspy_ai.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -59,21 +59,16 @@
 dspy/datasets/gsm8k.py
 dspy/datasets/hotpotqa.py
 dspy/evaluate/__init__.py
 dspy/evaluate/auto_evaluation.py
 dspy/evaluate/evaluate.py
 dspy/evaluate/metrics.py
 dspy/experimental/__init__.py
+dspy/experimental/synthesizer.py
 dspy/experimental/synthetic_data.py
-dspy/experimental/synthesizer/__init__.py
-dspy/experimental/synthesizer/config.py
-dspy/experimental/synthesizer/instruction_suffixes.py
-dspy/experimental/synthesizer/signatures.py
-dspy/experimental/synthesizer/synthesizer.py
-dspy/experimental/synthesizer/utils.py
 dspy/functional/__init__.py
 dspy/functional/functional.py
 dspy/predict/__init__.py
 dspy/predict/aggregation.py
 dspy/predict/chain_of_thought.py
 dspy/predict/chain_of_thought_with_hint.py
 dspy/predict/knn.py
```

### Comparing `dspy-ai-2.4.4/dspy_ai.egg-info/requires.txt` & `dspy-ai-2.4.5/dspy_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.4/pyproject.toml` & `dspy-ai-2.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.4.4"
+version = "2.4.5"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.12"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -104,15 +104,14 @@
 myst-parser = { version = "*", optional = true }
 myst-nb = { version = "*", optional = true }
 sphinx-autobuild = { version = "*", optional = true }
 sphinx_rtd_theme = { version = "*", optional = true }
 autodoc_pydantic = { version = "*", optional = true }
 sphinx-reredirects = { version = "^0.1.2", optional = true }
 sphinx-automodapi = { version = "0.16.0", optional = true }
-rich = "^13.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 transformers = "^4.38.2"
 torch = "^2.2.1"
 pytest-mock = "^3.12.0"
```

### Comparing `dspy-ai-2.4.4/setup.py` & `dspy-ai-2.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file	
 with open('requirements.txt', encoding='utf-8') as f:	
     requirements = f.read().splitlines()	
 
 setup(	
     name="dspy-ai",	
-    version="2.4.4",	
+    version="2.4.5",	
     description="DSPy",	
     long_description=long_description,	
     long_description_content_type='text/markdown',	
     url="https://github.com/stanfordnlp/dsp",	
     author="Omar Khattab",	
     author_email="okhattab@stanford.edu",	
     license="MIT License",
```

