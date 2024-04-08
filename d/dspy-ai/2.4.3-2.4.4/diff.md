# Comparing `tmp/dspy-ai-2.4.3.tar.gz` & `tmp/dspy-ai-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dspy-ai-2.4.3.tar", last modified: Mon Apr  8 16:49:27 2024, max compression
+gzip compressed data, was "dist/dspy-ai-2.4.4.tar", last modified: Mon Apr  8 17:21:05 2024, max compression
```

## Comparing `dspy-ai-2.4.3.tar` & `dspy-ai-2.4.4.tar`

### file list

```diff
@@ -1,164 +1,159 @@
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/
--rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.3/LICENSE
--rw-r--r--   0 okhattab (19845) future   (20099)    35537 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)    34661 2024-04-08 16:37:16.000000 dspy-ai-2.4.3/README.md
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/
--rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/evaluation/
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/evaluation/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/evaluation/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/modules/
--rw-r--r--   0 okhattab (19845) future   (20099)      497 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4516 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/anthropic.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6803 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/aws_lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9539 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/azure_openai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3135 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/azurecognitivesearch.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3195 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/bedrock.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1018 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/cache_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/clarifai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3214 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/cohere.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/colbertv2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5278 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/databricks.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/modules/finetuning/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/finetuning/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/finetuning/finetune_hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/google.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8610 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/gpt3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5023 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/groq_client.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15430 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/hf_client.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/hf_server.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3601 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3655 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/mistral.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/ollama.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/pyserini.py
--rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/sbert.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/modules/sentence_vectorizer.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/compiler.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/demonstrate.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/inspect.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8432 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/primitives.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2727 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/primitives/search.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/templates/
--rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/template_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/template_v3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/templates/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dsp/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/ann_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/dpr.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/metrics.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3285 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/settings.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/settings_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dsp/utils/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/
--rw-r--r--   0 okhattab (19845) future   (20099)      891 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/adapters/
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/basic_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/chatml_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/adapters/vicuna_adapter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/datasets/
--rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/colors.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4949 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/dataloader.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/dataset.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/gsm8k.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/datasets/hotpotqa.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/evaluate/
--rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/evaluate.py
--rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/evaluate/metrics.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/experimental/
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/config.py
--rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9723 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4237 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/experimental/synthetic_data.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/functional/
--rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/functional/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    18768 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/functional/functional.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/predict/
--rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/aggregation.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/chain_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/knn.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/langchain.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/parameter.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5583 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7603 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/program_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/react.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2827 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/predict/retry.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/assertions.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/box.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/example.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/module.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/prediction.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/program.py
--rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/primitives/python_interpreter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/retrieve/
--rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9126 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/azureaisearch_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4812 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3275 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/databricks_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3897 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0 okhattab (19845) future   (20099)     6548 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/faiss_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/marqo_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5930 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3264 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2425 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/ragatouille_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1442 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/retrieve.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/vectara_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4491 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/retrieve/you_rm.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/signatures/
--rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/signatures/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/signatures/field.py
--rw-r--r--   0 okhattab (19845) future   (20099)    14464 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/signatures/signature.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/teleprompt/
--rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/bootstrap.py
--rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/ensemble.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/finetune.py
--rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/random_search.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/signature_opt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/teleprompt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/teleprompt/vanilla.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/utils/dummies.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3378 2024-04-08 16:37:23.000000 dspy-ai-2.4.3/dspy/utils/logging.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/dspy_ai.egg-info/
--rw-r--r--   0 okhattab (19845) future   (20099)    35537 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)     3890 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/SOURCES.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/dependency_links.txt
--rw-r--r--   0 okhattab (19845) future   (20099)      664 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/requires.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 16:49:26.000000 dspy-ai-2.4.3/dspy_ai.egg-info/top_level.txt
--rw-r--r--   0 okhattab (19845) future   (20099)     7129 2024-04-08 16:38:10.000000 dspy-ai-2.4.3/pyproject.toml
--rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 16:49:27.000000 dspy-ai-2.4.3/setup.cfg
--rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 16:38:10.000000 dspy-ai-2.4.3/setup.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.4/LICENSE
+-rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)    34442 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/README.md
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/
+-rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/evaluation/
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/evaluation/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/evaluation/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/modules/
+-rw-r--r--   0 okhattab (19845) future   (20099)      446 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4547 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/anthropic.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/aws_lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/azure_openai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/azurecognitivesearch.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3102 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/bedrock.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1022 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/cache_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/clarifai.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/cohere.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/colbertv2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/databricks.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/modules/finetuning/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/finetuning/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/finetuning/finetune_hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/google.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/gpt3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/hf.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/hf_client.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/hf_server.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3258 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/modules/lm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/ollama.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/pyserini.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/sbert.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/modules/sentence_vectorizer.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/compiler.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/demonstrate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/inspect.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7948 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/primitives/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/primitives/primitives.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dsp/primitives/search.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/templates/
+-rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/template_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/template_v3.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/templates/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dsp/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/ann_utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/dpr.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/metrics.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3285 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/settings.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/settings_v2.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dsp/utils/utils.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/
+-rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/adapters/
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/basic_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/chatml_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/llamachat_adapter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/adapters/vicuna_adapter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/datasets/
+-rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/colors.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/datasets/dataloader.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/dataset.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/gsm8k.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/datasets/hotpotqa.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/evaluate/
+-rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/evaluate.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/evaluate/metrics.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/experimental/
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/__init__.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/
+-rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9542 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/experimental/synthetic_data.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/functional/
+-rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/functional/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    15805 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/functional/functional.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/predict/
+-rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/aggregation.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/chain_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/knn.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/langchain.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/parameter.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/predict/predict.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/predict/program_of_thought.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/predict/react.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/predict/retry.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/primitives/
+-rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/assertions.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/box.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/example.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/module.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/prediction.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/program.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/primitives/python_interpreter.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy/retrieve/
+-rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4793 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0 okhattab (19845) future   (20099)     6530 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/retrieve.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/retrieve/you_rm.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy/signatures/
+-rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/signatures/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/signatures/field.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/signatures/signature.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy/teleprompt/
+-rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/ensemble.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/finetune.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/random_search.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/teleprompt/vanilla.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy/utils/
+-rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-04-08 17:11:57.000000 dspy-ai-2.4.4/dspy/utils/__init__.py
+-rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.4/dspy/utils/dummies.py
+drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/dspy_ai.egg-info/
+-rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/PKG-INFO
+-rw-r--r--   0 okhattab (19845) future   (20099)     3752 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)      635 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/requires.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 17:21:04.000000 dspy-ai-2.4.4/dspy_ai.egg-info/top_level.txt
+-rw-r--r--   0 okhattab (19845) future   (20099)     6888 2024-04-08 17:20:51.000000 dspy-ai-2.4.4/pyproject.toml
+-rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 17:21:05.000000 dspy-ai-2.4.4/setup.cfg
+-rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 17:13:24.000000 dspy-ai-2.4.4/setup.py
```

### Comparing `dspy-ai-2.4.3/LICENSE` & `dspy-ai-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/PKG-INFO` & `dspy-ai-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.3
+Version: 2.4.4
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
@@ -122,15 +122,14 @@
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
 - Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
-- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
```

### Comparing `dspy-ai-2.4.3/README.md` & `dspy-ai-2.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
 - Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
-- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
```

### Comparing `dspy-ai-2.4.3/dsp/__init__.py` & `dspy-ai-2.4.4/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/evaluation/utils.py` & `dspy-ai-2.4.4/dsp/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/anthropic.py` & `dspy-ai-2.4.4/dsp/modules/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,49 +8,56 @@
 
 try:
     import anthropic
     anthropic_rate_limit = anthropic.RateLimitError
 except ImportError:
     anthropic_rate_limit = Exception
 
+
 logger = logging.getLogger(__name__)
+
 BASE_URL = "https://api.anthropic.com/v1/messages"
 
+
 def backoff_hdlr(details):
     """Handler from https://pypi.org/project/backoff/."""
     print(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with kwargs "
         "{kwargs}".format(**details),
     )
 
+
 def giveup_hdlr(details):
     """Wrapper function that decides when to give up on retry."""
     if "rate limits" in details.message:
         return False
     return True
 
+
 class Claude(LM):
     """Wrapper around anthropic's API. Supports both the Anthropic and Azure APIs."""
     def __init__(
-        self,
-        model: str = "claude-3-opus-20240229",
-        api_key: Optional[str] = None,
-        api_base: Optional[str] = None,
-        **kwargs,
+            self,
+            model: str = "claude-instant-1.2",
+            api_key: Optional[str] = None,
+            api_base: Optional[str] = None,
+            **kwargs,
     ):
         super().__init__(model)
+
         try:
             from anthropic import Anthropic
         except ImportError as err:
             raise ImportError("Claude requires `pip install anthropic`.") from err
 
         self.provider = "anthropic"
         self.api_key = api_key = os.environ.get("ANTHROPIC_API_KEY") if api_key is None else api_key
         self.api_base = BASE_URL if api_base is None else api_base
+
         self.kwargs = {
             "temperature": kwargs.get("temperature", 0.0),
             "max_tokens": min(kwargs.get("max_tokens", 4096), 4096),
             "top_p": kwargs.get("top_p", 1.0),
             "top_k": kwargs.get("top_k", 1),
             "n": kwargs.pop("n", kwargs.pop("num_generations", 1)),
             **kwargs,
@@ -64,26 +71,29 @@
         usage_data = response.usage
         if usage_data:
             total_tokens = usage_data.input_tokens + usage_data.output_tokens
             logger.info(f'{total_tokens}')
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
+
         kwargs = {**self.kwargs, **kwargs}
         # caching mechanism requires hashable kwargs
         kwargs["messages"] = [{"role": "user", "content": prompt}]
         kwargs.pop("n")
         response = self.client.messages.create(**kwargs)
+
         history = {
             "prompt": prompt,
             "response": response,
             "kwargs": kwargs,
             "raw_kwargs": raw_kwargs,
         }
         self.history.append(history)
+
         return response
 
     @backoff.on_exception(
         backoff.expo,
         (anthropic_rate_limit),
         max_time=1000,
         max_tries=8,
@@ -101,23 +111,27 @@
             prompt (str): prompt to send to Anthropic
             only_completed (bool, optional): return only completed responses and ignores completion due to length. Defaults to True.
             return_sorted (bool, optional): sort the completion choices using the returned probabilities. Defaults to False.
 
         Returns:
             list[str]: list of completion choices
         """
+
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
+
+
         # per eg here: https://docs.anthropic.com/claude/reference/messages-examples
         # max tokens can be used as a proxy to return smaller responses
         # so this cannot be a proper indicator for incomplete response unless it isnt the user-intent.
+
         n = kwargs.pop("n", 1)
         completions = []
         for _ in range(n):
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

### Comparing `dspy-ai-2.4.3/dsp/modules/aws_lm.py` & `dspy-ai-2.4.4/dsp/modules/aws_lm.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 import json
 import logging
 from abc import abstractmethod
-from typing import Any, Literal, Optional
+from typing import Any, Literal
 
 from dsp.modules.lm import LM
 
 # Heuristic translating number of chars to tokens
 # ~4 chars = 1 token
 CHARS2TOKENS: int = 4
 
@@ -23,15 +23,14 @@
 
     def __init__(
         self,
         model: str,
         region_name: str,
         service_name: str,
         max_new_tokens: int,
-        profile_name: Optional[str] = None,
         truncate_long_prompts: bool = False,
         input_output_ratio: int = 3,
         batch_n: bool = True,
     ) -> None:
         """_summary_
 
         Args:
@@ -52,20 +51,15 @@
         self._max_new_tokens: int = max_new_tokens
         self._model_name: str = model
         self._truncate_long_prompt_prompts: bool = truncate_long_prompts
         self._batch_n: bool = batch_n
 
         import boto3
 
-        if profile_name is None:
-            self.predictor = boto3.client(service_name, region_name=region_name)
-        else:
-            self.predictor = boto3.Session(profile_name=profile_name).client(
-                service_name, region_name=region_name,
-            )
+        self.predictor = boto3.client(service_name, region_name=region_name)
 
     @abstractmethod
     def _create_body(self, prompt: str, **kwargs):
         pass
 
     def _sanitize_kwargs(self, query_kwargs: dict[str, Any]) -> dict[str, Any]:
         """Ensure that input kwargs can be used by Bedrock or Sagemaker."""
```

### Comparing `dspy-ai-2.4.3/dsp/modules/azure_openai.py` & `dspy-ai-2.4.4/dsp/modules/azure_openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+import logging
+
+# Configure logging
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(message)s",
+    handlers=[logging.FileHandler("azure_openai_usage.log")],
+)
+
 import functools
 import json
-import logging
 from typing import Any, Literal, Optional, cast
 
 import backoff
 import openai
 
 import dsp
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
@@ -104,18 +112,14 @@
             "top_p": 1,
             "frequency_penalty": 0,
             "presence_penalty": 0,
             "n": 1,
             **kwargs,
         }  # TODO: add kwargs above for </s>
 
-        self.api_base = api_base
-        self.api_version = api_version
-        self.api_key = api_key
-
         self.history: list[dict[str, Any]] = []
 
     def _openai_client(self):
         if OPENAI_LEGACY:
             return openai
 
         return self.client
@@ -219,27 +223,14 @@
                 avglog = sum(logprobs) / len(logprobs)
                 scored_completions.append((avglog, self._get_choice_text(c)))
 
             scored_completions = sorted(scored_completions, reverse=True)
             completions = [c for _, c in scored_completions]
 
         return completions
-    
-    def copy(self, **kwargs):
-        """Returns a copy of the language model with the same parameters."""
-        kwargs = {**self.kwargs, **kwargs}
-        model = kwargs.pop("model")
-
-        return self.__class__(
-            model=model, 
-            api_key=self.api_key, 
-            api_version=self.api_version, 
-            api_base=self.api_base, 
-            **kwargs,
-        )
 
 
 @CacheMemory.cache
 def cached_gpt3_request_v2(**kwargs):
     return openai.Completion.create(**kwargs)
```

### Comparing `dspy-ai-2.4.3/dsp/modules/azurecognitivesearch.py` & `dspy-ai-2.4.4/dsp/modules/azurecognitivesearch.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     from azure.search.documents._paging import SearchItemPaged
 except ImportError:
     raise ImportError(
         "You need to install azure-search-documents library"
         "Please use the command: pip install azure-search-documents",
     )
 
-# Deprecated: This module is scheduled for removal in future releases.
-# Please use the AzureAISearchRM class from dspy.retrieve.azureaisearch_rm instead.
-# For more information, refer to the updated documentation.
-
 class AzureCognitiveSearch:
     """Wrapper for the Azure Cognitive Search Retrieval."""
 
     def __init__(
         self,
         search_service_name: str,
         search_api_key: str,
@@ -37,20 +33,17 @@
         # Create a client
         self.credential = AzureKeyCredential(self.search_api_key)
         self.client = SearchClient(endpoint=self.endpoint,
                         index_name=self.search_index_name,
                         credential=self.credential)
 
     def __call__(self, query: str, k: int = 10) -> Union[list[str], list[dotdict]]:
-        print("""# Deprecated: This module is scheduled for removal in future releases.
-                Please use the AzureAISearchRM class from dspy.retrieve.azureaisearch_rm instead.
-                For more information, refer to the updated documentation.""")
-
+        
         topk: list[dict[str, Any]] = azure_search_request(self.field_text, self.field_score, self.client, query, k)
-        topk = [{**d, "long_text": d["text"]} for d in topk]
+        topk = [{**d, "long_text": d["text"]} for d in topk]            
 
         return [dotdict(psg) for psg in topk]
 
 def azure_search_request(key_content: str, key_score: str,  client: SearchClient, query: str, top: int =1):
     '''
     Search in Azure Cognitive Search Index
     '''
@@ -68,10 +61,10 @@
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

### Comparing `dspy-ai-2.4.3/dsp/modules/bedrock.py` & `dspy-ai-2.4.4/dsp/modules/bedrock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import json
-from typing import Any, Optional
+from typing import Any
 
 from dsp.modules.aws_lm import AWSLM
 
 
 class Bedrock(AWSLM):
     def __init__(
         self,
         region_name: str,
         model: str,
-        profile_name: Optional[str] = None,
         input_output_ratio: int = 3,
         max_new_tokens: int = 1500,
     ) -> None:
         """Use an AWS Bedrock language model.
         NOTE: You must first configure your AWS credentials with the AWS CLI before using this model!
 
         Args:
@@ -25,15 +24,14 @@
             input_output_ratio (int, optional): The rough size of the number of input tokens to output tokens in the worst case. Defaults to 3.
             max_new_tokens (int, optional): The maximum number of tokens to be sampled from the LM.
         """
         super().__init__(
             model=model,
             service_name="bedrock-runtime",
             region_name=region_name,
-            profile_name=profile_name,
             truncate_long_prompts=False,
             input_output_ratio=input_output_ratio,
             max_new_tokens=max_new_tokens,
             batch_n=True,  # Bedrock does not support the `n` parameter
         )
         self._validate_model(model)
         self.provider = "claude" if "claude" in model.lower() else "bedrock"
```

### Comparing `dspy-ai-2.4.3/dsp/modules/cache_utils.py` & `dspy-ai-2.4.4/dsp/modules/cache_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import wraps
 from pathlib import Path
 
 from joblib import Memory
 
 from dsp.utils import dotdict
 
-cache_turn_on = os.environ.get('DSP_CACHEBOOL', 'True').lower() != 'false'
+cache_turn_on = not os.environ.get('DSP_CACHEBOOL', 'True').lower() == 'false'
 
 
 def noop_decorator(arg=None, *noop_args, **noop_kwargs):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
```

### Comparing `dspy-ai-2.4.3/dsp/modules/clarifai.py` & `dspy-ai-2.4.4/dsp/modules/clarifai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/colbertv2.py` & `dspy-ai-2.4.4/dsp/modules/colbertv2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/databricks.py` & `dspy-ai-2.4.4/dsp/modules/databricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+import logging
+
+# Configure logging
+logging.basicConfig(
+    level=logging.INFO,
+    format='%(message)s',
+    handlers=[
+        logging.FileHandler('openai_usage.log'),
+    ],
+)
+
 import functools
 import json
 from typing import Literal, Optional
 
 import openai
 
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
```

### Comparing `dspy-ai-2.4.3/dsp/modules/finetuning/finetune_hf.py` & `dspy-ai-2.4.4/dsp/modules/finetuning/finetune_hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/google.py` & `dspy-ai-2.4.4/dsp/modules/google.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/gpt3.py` & `dspy-ai-2.4.4/dsp/modules/gpt3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+import logging
+
+# Configure logging
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(message)s",
+    handlers=[logging.FileHandler("openai_usage.log")],
+)
+
 import functools
 import json
-import logging
 from typing import Any, Literal, Optional, cast
 
 import backoff
 import openai
 
 import dsp
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
@@ -50,23 +58,20 @@
     def __init__(
         self,
         model: str = "gpt-3.5-turbo-instruct",
         api_key: Optional[str] = None,
         api_provider: Literal["openai"] = "openai",
         api_base: Optional[str] = None,
         model_type: Literal["chat", "text"] = None,
-        system_prompt: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(model)
         self.provider = "openai"
         openai.api_type = api_provider
 
-        self.system_prompt = system_prompt
-
         assert (
             api_provider != "azure"
         ), "Azure functionality with base OpenAI has been deprecated, please use dspy.AzureOpenAI instead."
 
         default_model_type = (
             "chat"
             if ("gpt-3.5" in model or "turbo" in model or "gpt-4" in model)
@@ -109,18 +114,15 @@
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
 
         kwargs = {**self.kwargs, **kwargs}
         if self.model_type == "chat":
             # caching mechanism requires hashable kwargs
-            messages = [{"role": "user", "content": prompt}]
-            if self.system_prompt:
-                messages.insert(0, {"role": "system", "content": self.system_prompt})
-            kwargs["messages"] = messages
+            kwargs["messages"] = [{"role": "user", "content": prompt}]
             kwargs = {"stringify_request": json.dumps(kwargs)}
             response = chat_request(**kwargs)
 
         else:
             kwargs["prompt"] = prompt
             response = completions_request(**kwargs)
```

### Comparing `dspy-ai-2.4.3/dsp/modules/groq_client.py` & `dspy-ai-2.4.4/dsp/modules/cohere.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,169 +1,145 @@
-import logging
-from typing import Any
+import math
+from typing import Any, Optional
 
 import backoff
 
-try:
-    import groq
-    from groq import Groq
-    groq_api_error = (groq.APIError, groq.RateLimitError)
-except ImportError:
-    groq_api_error = (Exception)
-
-
-import dsp
 from dsp.modules.lm import LM
 
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[logging.FileHandler("groq_usage.log")],
-)
-
+try:
+    import cohere
+    cohere_api_error = cohere.CohereAPIError
+except ImportError:
+    cohere_api_error = Exception
+    # print("Not loading Cohere because it is not installed.")
 
 
 def backoff_hdlr(details):
     """Handler from https://pypi.org/project/backoff/"""
     print(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with kwargs "
         "{kwargs}".format(**details),
     )
 
 
-class GroqLM(LM):
-    """Wrapper around groq's API.
+def giveup_hdlr(details):
+    """wrapper function that decides when to give up on retry"""
+    if "rate limits" in details.message:
+        return False
+    return True
+
+
+class Cohere(LM):
+    """Wrapper around Cohere's API.
 
-    Args:
-        model (str, optional): groq supported LLM model to use. Defaults to "mixtral-8x7b-32768".
-        api_key (Optional[str], optional): API provider Authentication token. use Defaults to None.
-        **kwargs: Additional arguments to pass to the API provider.
+    Currently supported models include `command`, `command-nightly`, `command-light`, `command-light-nightly`.
     """
 
     def __init__(
         self,
-        api_key: str,
-        model: str = "mixtral-8x7b-32768",
+        model: str = "command-nightly",
+        api_key: Optional[str] = None,
+        stop_sequences: list[str] = [],
         **kwargs,
     ):
+        """
+        Parameters
+        ----------
+        model : str
+            Which pre-trained model from Cohere to use?
+            Choices are [`command`, `command-nightly`, `command-light`, `command-light-nightly`]
+        api_key : str
+            The API key for Cohere.
+            It can be obtained from https://dashboard.cohere.ai/register.
+        stop_sequences : list of str
+            Additional stop tokens to end generation.
+        **kwargs: dict
+            Additional arguments to pass to the API provider.
+        """
         super().__init__(model)
-        self.provider = "groq"
-        if api_key:
-            self.api_key = api_key
-            self.client = Groq(api_key = api_key)
-        else:
-            raise ValueError("api_key is required for groq")
-            
-
+        self.co = cohere.Client(api_key)
+        self.provider = "cohere"
         self.kwargs = {
+            "model": model,
             "temperature": 0.0,
             "max_tokens": 150,
-            "top_p": 1,
+            "p": 1,
             "frequency_penalty": 0,
             "presence_penalty": 0,
-            "n": 1,
+            "num_generations": 1,
             **kwargs,
-        }  
-        models = self.client.models.list().data
-        if models is not None:
-            if model in [m.id for m in models]: 
-                self.kwargs["model"] = model
-        self.history: list[dict[str, Any]] = []
-
+        }
+        self.stop_sequences = stop_sequences
+        self.max_num_generations = 5
 
-    def log_usage(self, response):
-        """Log the total tokens from the Groq API response."""
-        usage_data = response.get("usage")
-        if usage_data:
-            total_tokens = usage_data.get("total_tokens")
-            logging.info(f"{total_tokens}")
+        self.history: list[dict[str, Any]] = []
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
-
-        kwargs = {**self.kwargs, **kwargs}
-
-        kwargs["messages"] = [{"role": "user", "content": prompt}]
-        response = self.chat_request(**kwargs)
+        kwargs = {
+            **self.kwargs,
+            "stop_sequences": self.stop_sequences,
+            "prompt": prompt,
+            **kwargs,
+        }
+        response = self.co.generate(**kwargs)
 
         history = {
             "prompt": prompt,
-            "response": response.choices[0].message.content,
+            "response": response,
             "kwargs": kwargs,
             "raw_kwargs": raw_kwargs,
         }
-
         self.history.append(history)
 
         return response
 
     @backoff.on_exception(
         backoff.expo,
-        groq_api_error,
+        (cohere_api_error),
         max_time=1000,
         on_backoff=backoff_hdlr,
+        giveup=giveup_hdlr,
     )
     def request(self, prompt: str, **kwargs):
-        """Handles retreival of model completions whilst handling rate limiting and caching."""
-        if "model_type" in kwargs:
-            del kwargs["model_type"]
-
+        """Handles retrieval of completions from Cohere whilst handling API errors"""
         return self.basic_request(prompt, **kwargs)
 
-    def _get_choice_text(self, choice) -> str:
-        return choice.message.content
-
-    def chat_request(self, **kwargs):
-        """Handles retreival of model completions whilst handling rate limiting and caching."""
-        response = self.client.chat.completions.create(**kwargs)
-        return response
-    
     def __call__(
         self,
         prompt: str,
         only_completed: bool = True,
         return_sorted: bool = False,
         **kwargs,
-    ) -> list[dict[str, Any]]:
-        """Retrieves completions from model.
-
-        Args:
-            prompt (str): prompt to send to model
-            only_completed (bool, optional): return only completed responses and ignores completion due to length. Defaults to True.
-            return_sorted (bool, optional): sort the completion choices using the returned probabilities. Defaults to False.
-
-        Returns:
-            list[dict[str, Any]]: list of completion choices
-        """
-
+    ):
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
-        response = self.request(prompt, **kwargs)
 
-        if dsp.settings.log_openai_usage:
-            self.log_usage(response)
+        # Cohere uses 'num_generations' whereas dsp.generate() uses 'n'
+        n = kwargs.pop("n", 1)
 
-        choices = response.choices
+        # Cohere can generate upto self.max_num_generations completions at a time
+        choices = []
+        num_iters = math.ceil(n / self.max_num_generations)
+        remainder = n % self.max_num_generations
+        for i in range(num_iters):
+            if i == (num_iters - 1):
+                kwargs["num_generations"] = (
+                    remainder if remainder != 0 else self.max_num_generations
+                )
+            else:
+                kwargs["num_generations"] = self.max_num_generations
+            response = self.request(prompt, **kwargs)
+            choices.extend(response.generations)
+        completions = [c.text for c in choices]
 
-        completions = [self._get_choice_text(c) for c in choices]
-        if return_sorted and kwargs.get("n", 1) > 1:
+        if return_sorted and kwargs.get("num_generations", 1) > 1:
             scored_completions = []
 
             for c in choices:
-                tokens, logprobs = (
-                    c["logprobs"]["tokens"],
-                    c["logprobs"]["token_logprobs"],
-                )
-
-                if "<|endoftext|>" in tokens:
-                    index = tokens.index("<|endoftext|>") + 1
-                    tokens, logprobs = tokens[:index], logprobs[:index]
-
-                avglog = sum(logprobs) / len(logprobs)
-                scored_completions.append((avglog, self._get_choice_text(c)))
+                scored_completions.append((c.likelihood, c.text))
 
             scored_completions = sorted(scored_completions, reverse=True)
             completions = [c for _, c in scored_completions]
 
-        return completions
+        return completions
```

### Comparing `dspy-ai-2.4.3/dsp/modules/hf.py` & `dspy-ai-2.4.4/dsp/modules/hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/hf_client.py` & `dspy-ai-2.4.4/dsp/modules/hf_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,44 +112,29 @@
 def send_hftgi_request_v00(arg, **kwargs):
     return requests.post(arg, **kwargs)
 
 
 class HFClientVLLM(HFModel):
     def __init__(self, model, port, url="http://localhost", **kwargs):
         super().__init__(model=model, is_client=True)
-
-        if isinstance(url, list):
-            self.urls = url
-        
-        elif isinstance(url, str):
-            self.urls = [f'{url}:{port}']
-        
-        else:
-            raise ValueError(f"The url provided to `HFClientVLLM` is neither a string nor a list of strings. It is of type {type(url)}.")
-        
+        self.url = f"{url}:{port}"
         self.headers = {"Content-Type": "application/json"}
-        self.kwargs |= kwargs
-
 
     def _generate(self, prompt, **kwargs):
         kwargs = {**self.kwargs, **kwargs}
 
         payload = {
-            "model": self.kwargs["model"],
+            "model": kwargs["model"],
             "prompt": prompt,
-            **kwargs,
+            "max_tokens": kwargs["max_tokens"],
+            "temperature": kwargs["temperature"],
         }
 
-        
-        # Round robin the urls.
-        url = self.urls.pop(0)
-        self.urls.append(url)
-
         response = send_hfvllm_request_v00(
-            f"{url}/v1/completions",
+            f"{self.url}/v1/completions",
             json=payload,
             headers=self.headers,
         )
 
         try:
             json_response = response.json()
             completions = json_response["choices"]
@@ -431,8 +416,8 @@
         except Exception:
             print("Failed to parse JSON response:", response.text)
             raise Exception("Received invalid JSON response from server")
 
 
 @CacheMemory.cache
 def send_hfsglang_request_v00(arg, **kwargs):
-    return requests.post(arg, **kwargs)
+    return requests.post(arg, **kwargs)
```

### Comparing `dspy-ai-2.4.3/dsp/modules/hf_server.py` & `dspy-ai-2.4.4/dsp/modules/hf_server.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/lm.py` & `dspy-ai-2.4.4/dsp/modules/lm.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,89 +22,83 @@
     def basic_request(self, prompt, **kwargs):
         pass
 
     def request(self, prompt, **kwargs):
         return self.basic_request(prompt, **kwargs)
 
     def print_green(self, text: str, end: str = "\n"):
-        return "\x1b[32m" + str(text) + "\x1b[0m" + end
+        print("\x1b[32m" + str(text) + "\x1b[0m", end=end)
 
     def print_red(self, text: str, end: str = "\n"):
-        return "\x1b[31m" + str(text) + "\x1b[0m" + end
+        print("\x1b[31m" + str(text) + "\x1b[0m", end=end)
 
     def inspect_history(self, n: int = 1, skip: int = 0):
         """Prints the last n prompts and their completions.
-
-        TODO: print the valid choice that contains filled output field instead of the first.
+        TODO: print the valid choice that contains filled output field instead of the first
         """
         provider: str = self.provider
 
         last_prompt = None
         printed = []
         n = n + skip
 
         for x in reversed(self.history[-100:]):
             prompt = x["prompt"]
 
             if prompt != last_prompt:
-                if provider == "clarifai" or provider == "google":
-                    printed.append((prompt, x["response"]))
-                elif provider == "anthropic":
-                    blocks = [{"text": block.text} for block in x["response"].content if block.type == "text"]
-                    printed.append((prompt, blocks))
-                elif provider == "cohere":
-                    printed.append((prompt, x["response"].text))
-                elif provider == "mistral":
-                    printed.append((prompt, x['response'].choices))
+
+                if provider == "clarifai" or provider == "google" or provider == "claude":
+                    printed.append(
+                        (
+                            prompt,
+                            x['response'],
+                        ),
+                    )
                 else:
-                    printed.append((prompt, x["response"]["choices"]))
+                    printed.append(
+                        (
+                            prompt,
+                            x["response"].generations
+                            if provider == "cohere"
+                            else x["response"]["choices"],
+                        ),
+                    )
 
             last_prompt = prompt
 
             if len(printed) >= n:
                 break
 
         for idx, (prompt, choices) in enumerate(reversed(printed)):
-            printing_value = ""
-
             # skip the first `skip` prompts
             if (n - idx - 1) < skip:
                 continue
 
-            printing_value += "\n\n\n"
-            printing_value += prompt
-
+            print("\n\n\n")
+            print(prompt, end="")
             text = ""
             if provider == "cohere":
-                text = choices
+                text = choices[0].text
             elif provider == "openai" or provider == "ollama":
                 text = ' ' + self._get_choice_text(choices[0]).strip()
             elif provider == "clarifai" or provider == "claude" :
                 text=choices
-            elif provider == "groq":
-                text = ' ' + choices
             elif provider == "google":
                 text = choices[0].parts[0].text
-            elif provider == "mistral":
-                text = choices[0].message.content
             else:
                 text = choices[0]["text"]
-            printing_value += self.print_green(text, end="")
+            self.print_green(text, end="")
 
             if len(choices) > 1:
-                printing_value += self.print_red(f" \t (and {len(choices)-1} other completions)", end="")
-
-            printing_value += "\n\n\n"
-
-        print(printing_value)
-        return printing_value
+                self.print_red(f" \t (and {len(choices)-1} other completions)", end="")
+            print("\n\n\n")
 
     @abstractmethod
     def __call__(self, prompt, only_completed=True, return_sorted=False, **kwargs):
         pass
 
     def copy(self, **kwargs):
         """Returns a copy of the language model with the same parameters."""
         kwargs = {**self.kwargs, **kwargs}
-        model = kwargs.pop("model")
+        model = kwargs.pop('model')
 
         return self.__class__(model=model, **kwargs)
```

### Comparing `dspy-ai-2.4.3/dsp/modules/ollama.py` & `dspy-ai-2.4.4/dsp/modules/ollama.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/pyserini.py` & `dspy-ai-2.4.4/dsp/modules/pyserini.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/sbert.py` & `dspy-ai-2.4.4/dsp/modules/sbert.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/modules/sentence_vectorizer.py` & `dspy-ai-2.4.4/dsp/modules/sentence_vectorizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/primitives/compiler.py` & `dspy-ai-2.4.4/dsp/primitives/compiler.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/primitives/demonstrate.py` & `dspy-ai-2.4.4/dsp/primitives/demonstrate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/primitives/inspect.py` & `dspy-ai-2.4.4/dsp/primitives/inspect.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/primitives/predict.py` & `dspy-ai-2.4.4/dsp/primitives/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,28 +94,19 @@
         # If none of the completions is completed (i.e., none has the final field set).
         if last_field_idx < len(field_names):
             # Pick the first completion that has gone farthest.
             completion = completions[0]
             completion[field_names[last_field_idx]] = ""
 
             # Recurse with greedy decoding and a shorter length.
-            max_tokens = (kwargs.get("max_tokens") or 
-                        kwargs.get("max_output_tokens") or
-                        dsp.settings.lm.kwargs.get("max_tokens") or 
-                        dsp.settings.lm.kwargs.get('max_output_tokens'))
-
-
-            if max_tokens is None:
-                raise ValueError("Required 'max_tokens' or 'max_output_tokens' not specified in settings.")
+            max_tokens = kwargs.get("max_tokens", dsp.settings.lm.kwargs["max_tokens"])
             max_tokens = min(max(75, max_tokens // 2), max_tokens)
-            keys = list(kwargs.keys()) + list(dsp.settings.lm.kwargs.keys()) 
-            max_tokens_key = "max_tokens" if "max_tokens" in keys else "max_output_tokens"
             new_kwargs = {
                 **kwargs,
-                max_tokens_key: max_tokens,
+                "max_tokens": max_tokens,
                 "n": 1,
                 "temperature": 0.0,
             }
 
             assert max_depth > 0
             return generate(template, **new_kwargs)(
                 completion,
```

### Comparing `dspy-ai-2.4.3/dsp/primitives/primitives.py` & `dspy-ai-2.4.4/dsp/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/primitives/search.py` & `dspy-ai-2.4.4/dsp/primitives/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,49 +20,49 @@
         passages_cs_scores = dsp.settings.reranker(query, passages)
         passages_cs_scores_sorted = np.argsort(passages_cs_scores)[::-1]
         passages = [passages[idx] for idx in passages_cs_scores_sorted]
 
     return passages
 
 
-def retrieveRerankEnsemble(queries: list[str], k: int,**kwargs) -> list[str]:
+def retrieveRerankEnsemble(queries: list[str], k: int) -> list[str]:
     if not (dsp.settings.rm and dsp.settings.reranker):
         raise AssertionError("Both RM and Reranker are needed to retrieve & re-rank.")
     queries = [q for q in queries if q]
     passages = {}
     for query in queries:
-        retrieved_passages = dsp.settings.rm(query, k=k*3,**kwargs)
+        retrieved_passages = dsp.settings.rm(query, k=k*3)
         passages_cs_scores = dsp.settings.reranker(query, [psg.long_text for psg in retrieved_passages])
         for idx in np.argsort(passages_cs_scores)[::-1]:
             psg = retrieved_passages[idx]
             passages[psg.long_text] = passages.get(psg.long_text, []) + [
                 passages_cs_scores[idx],
             ]
 
     passages = [(np.average(score), text) for text, score in passages.items()]
     return [text for _, text in sorted(passages, reverse=True)[:k]]
 
 
-def retrieveEnsemble(queries: list[str], k: int, by_prob: bool = True,**kwargs) -> list[str]:
+def retrieveEnsemble(queries: list[str], k: int, by_prob: bool = True) -> list[str]:
     """Retrieves passages from the RM for each query in queries and returns the top k passages
     based on the probability or score.
     """
     if not dsp.settings.rm:
         raise AssertionError("No RM is loaded.")
     if dsp.settings.reranker:
         return retrieveRerankEnsemble(queries, k)
     
     queries = [q for q in queries if q]
 
     if len(queries) == 1:
-        return retrieve(queries[0], k, **kwargs)
+        return retrieve(queries[0], k)
 
     passages = {}
     for q in queries:
-        for psg in dsp.settings.rm(q, k=k * 3,**kwargs):
+        for psg in dsp.settings.rm(q, k=k * 3):
             if by_prob:
                 passages[psg.long_text] = passages.get(psg.long_text, 0.0) + psg.prob
             else:
                 passages[psg.long_text] = passages.get(psg.long_text, 0.0) + psg.score
 
     passages = [(score, text) for text, score in passages.items()]
     passages = sorted(passages, reverse=True)[:k]
```

### Comparing `dspy-ai-2.4.3/dsp/templates/template_v2.py` & `dspy-ai-2.4.4/dsp/templates/template_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/templates/template_v3.py` & `dspy-ai-2.4.4/dsp/templates/template_v3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/templates/utils.py` & `dspy-ai-2.4.4/dsp/templates/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/utils/ann_utils.py` & `dspy-ai-2.4.4/dsp/utils/ann_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/utils/dpr.py` & `dspy-ai-2.4.4/dsp/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/utils/metrics.py` & `dspy-ai-2.4.4/dsp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/utils/settings.py` & `dspy-ai-2.4.4/dsp/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/utils/settings_v2.py` & `dspy-ai-2.4.4/dsp/utils/settings_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dsp/utils/utils.py` & `dspy-ai-2.4.4/dsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/__init__.py` & `dspy-ai-2.4.4/dspy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 from .predict import *
 from .primitives import *
 from .retrieve import *
 from .signatures import *
 
 # Functional must be imported after primitives, predict and signatures
 from .functional import * # isort: skip
-from .utils.logging import logger, set_log_level, set_log_output
 
 settings = dsp.settings
 
 AzureOpenAI = dsp.AzureOpenAI
 OpenAI = dsp.GPT3
-Mistral = dsp.Mistral
 Databricks = dsp.Databricks
 Cohere = dsp.Cohere
 ColBERTv2 = dsp.ColBERTv2
 Pyserini = dsp.PyseriniRetriever
 Clarifai = dsp.ClarifaiLLM
 Google = dsp.Google
-GROQ = dsp.GroqLM
 
 HFClientTGI = dsp.HFClientTGI
 HFClientVLLM = HFClientVLLM
 
 Anyscale = dsp.Anyscale
 Together = dsp.Together
 HFModel = dsp.HFModel
```

### Comparing `dspy-ai-2.4.3/dspy/datasets/colors.py` & `dspy-ai-2.4.4/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/datasets/dataloader.py` & `dspy-ai-2.4.4/dspy/datasets/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,21 +58,14 @@
         dataset = load_dataset("json", data_files=file_path)["train"]
         
         if not fields:
             fields = list(dataset.features)
         
         return [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
 
-    def from_parquet(self, file_path: str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
-        dataset = load_dataset("parquet", data_files=file_path)["train"]
-
-        if not fields:
-            fields = list(dataset.features)
-
-        return [dspy.Example({field: row[field] for field in fields}).with_inputs(input_keys) for row in dataset]
 
     def sample(
         self,
         dataset: List[dspy.Example],
         n: int,
         *args,
         **kwargs,
```

### Comparing `dspy-ai-2.4.3/dspy/datasets/dataset.py` & `dspy-ai-2.4.4/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/datasets/gsm8k.py` & `dspy-ai-2.4.4/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/datasets/hotpotqa.py` & `dspy-ai-2.4.4/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/evaluate/auto_evaluation.py` & `dspy-ai-2.4.4/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/evaluate/evaluate.py` & `dspy-ai-2.4.4/dspy/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/evaluate/metrics.py` & `dspy-ai-2.4.4/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/experimental/synthesizer/config.py` & `dspy-ai-2.4.4/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy-ai-2.4.4/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/experimental/synthesizer/signatures.py` & `dspy-ai-2.4.4/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/experimental/synthesizer/synthesizer.py` & `dspy-ai-2.4.4/dspy/experimental/synthesizer/synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,17 +198,15 @@
             kwargs = {
                 "task_description": task_description,
                 "knowledge_seed": iter_seed,
                 "config": dict(temperature=iter_temperature, n=batch_size),
             }
 
             if self.config.num_example_for_optim:
-                if not isinstance(ground_source, list):
-                    raise ValueError("Ground source must be a list of examples when `num_example_for_optim` is provided.")
-                kwargs["ground_source"] = random.sample(ground_source, k=self.config.num_example_for_optim)
+                kwargs["ground_source"] = random.sample(ground_source, self.config.num_example_for_optim)
             
             with dspy.context(lm=self.input_lm):
                 inputs = self.input_predictor(**kwargs)
 
             input_kwargs = [{
                 key: getattr(completions, key)
                 for key in input_keys
```

### Comparing `dspy-ai-2.4.3/dspy/experimental/synthesizer/utils.py` & `dspy-ai-2.4.4/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/experimental/synthetic_data.py` & `dspy-ai-2.4.4/dspy/experimental/synthetic_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,63 @@
-import logging
 import random
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 import dspy
 
 
-class DescriptionSignature(dspy.Signature):
-    field_name = dspy.InputField(desc="name of a field")
-    example = dspy.InputField(desc="an example value for the field")
-    description = dspy.OutputField(desc="a short text only description of what the field contains")
-
+class descriptionSignature(dspy.Signature):
+  field_name = dspy.InputField(desc="name of a field")
+  example = dspy.InputField(desc="an example value for the field")
+  description = dspy.OutputField(desc="a short text only description of what the field contains")
 
 class SyntheticDataGenerator:
     def __init__(self, schema_class: Optional[BaseModel] = None, examples: Optional[List[dspy.Example]] = None):
         self.schema_class = schema_class
         self.examples = examples
 
     def generate(self, sample_size: int) -> List[dspy.Example]:
-        """Generate synthetic examples.
-
-        Args:
-            sample_size (int): number of examples to generate
-        Raises:
-            ValueError: either a schema_class or examples should be provided
-        Returns:
-            List[dspy.Example]: list of synthetic examples generated
-        """
         if not self.schema_class and not self.examples:
             raise ValueError("Either a schema_class or examples must be provided.")
         if self.examples and len(self.examples) >= sample_size:
-            logging.info("No additional data generation needed.")
+            print("No additional data generation needed.")
             return self.examples[:sample_size]
 
         additional_samples_needed = sample_size - (len(self.examples) if self.examples else 0)
         generated_examples = self._generate_additional_examples(additional_samples_needed)
 
         return self.examples + generated_examples if self.examples else generated_examples
 
     def _define_or_infer_fields(self):
-        """Define fields to generate if a schema class is provided.
-        Infer fields to generate if an inital sample of examples is provided.
-
-        Returns:
-            dict: dictionary of fields to generate
-        """  # noqa: D205
         if self.schema_class:
             data_schema = self.schema_class.model_json_schema()
             properties = data_schema['properties']
         elif self.examples:
             inferred_schema = self.examples[0].__dict__['_store']
-            descriptor = dspy.Predict(DescriptionSignature)
+            descriptor = dspy.Predict(descriptionSignature)
             properties = {field: {'description': str((descriptor(field_name=field, example=str(inferred_schema[field]))).description)}
                           for field in inferred_schema.keys()}
         else:
             properties = {}
         return properties
 
     def _generate_additional_examples(self, additional_samples_needed: int) -> List[dspy.Example]:
-        """Generate additional examples if needed.
-
-        Args:
-            additional_samples_needed (int): the difference between the desired
-            number of examples and the current number of examples
-        Returns:
-            List[dspy.Example]: list of synthetic examples
-        """
         properties = self._define_or_infer_fields()
         class_name = f"{self.schema_class.__name__ if self.schema_class else 'Inferred'}Signature"
         fields = self._prepare_fields(properties)
 
         signature_class = type(class_name, (dspy.Signature,), fields)
         generator = dspy.Predict(signature_class, n=additional_samples_needed)
         response = generator(sindex=str(random.randint(1, additional_samples_needed)))
 
         return [dspy.Example({field_name: getattr(completion, field_name) for field_name in properties.keys()})
                 for completion in response.completions]
 
     def _prepare_fields(self, properties) -> dict:
-        """Prepare fields to generate in an appropriate format."""
         return {
             '__doc__': f"Generates the following outputs: {{{', '.join(properties.keys())}}}.",
             'sindex': dspy.InputField(desc="a random string"),
             **{field_name: dspy.OutputField(desc=properties[field_name].get('description', 'No description'))
                for field_name in properties.keys()},
         }
```

### Comparing `dspy-ai-2.4.3/dspy/functional/functional.py` & `dspy-ai-2.4.4/dspy/functional/functional.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import inspect
 import json
-import textwrap
 import typing
-from typing import Annotated, List, Tuple, Union  # noqa: UP035
+from typing import Annotated, List, Tuple  # noqa: UP035
 
 import pydantic
 import ujson
-from pydantic.fields import FieldInfo
 
 import dspy
 from dsp.templates import passages2text
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, make_signature
 
 
@@ -49,53 +47,47 @@
         super().__init__()
         for name in dir(self):
             attr = getattr(self, name)
             if isinstance(attr, dspy.Module):
                 self.__dict__[name] = attr.copy()
 
 
-def TypedChainOfThought(signature, instructions=None, *, max_retries=3) -> dspy.Module:  # noqa: N802
+def TypedChainOfThought(signature, max_retries=3) -> dspy.Module:  # noqa: N802
     """Just like TypedPredictor, but adds a ChainOfThought OutputField."""
-    signature = ensure_signature(signature, instructions)
+    signature = ensure_signature(signature)
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
-    def __init__(self, signature, instructions=None, *, max_retries=3, wrap_json=False, explain_errors=False):
+    def __init__(self, signature, max_retries=3, wrap_json=False):
         """Like dspy.Predict, but enforces type annotations in the signature.
 
         Args:
             signature: The signature of the module. Can use type annotations.
             max_retries: The number of times to retry the prediction if the output is invalid.
             wrap_json: If True, json objects in the input will be wrapped in ```json ... ```
         """
         super().__init__()
-        self.signature = ensure_signature(signature, instructions)
+        self.signature = ensure_signature(signature)
         self.predictor = dspy.Predict(signature)
         self.max_retries = max_retries
         self.wrap_json = wrap_json
-        self.explain_errors = explain_errors
 
     def copy(self) -> "TypedPredictor":
-        return TypedPredictor(
-            self.signature,
-            max_retries=self.max_retries,
-            wrap_json=self.wrap_json,
-            explain_errors=self.explain_errors,
-        )
+        return TypedPredictor(self.signature, self.max_retries, self.wrap_json)
 
     def __repr__(self):
         """Return a string representation of the TypedPredictor object."""
         return f"TypedPredictor({self.signature})"
 
     def _make_example(self, type_) -> str:
         # Note: DSPy will cache this call so we only pay the first time TypedPredictor is called.
@@ -116,71 +108,14 @@
         return json_object
         # TODO: Another fun idea is to only (but automatically) do this if the output fails.
         # We could also have a more general "suggest solution" prompt that tries to fix the output
         # More directly.
         # TODO: Instead of using a language model to create the example, we can also just use a
         # library like https://pypi.org/project/polyfactory/ that's made exactly to do this.
 
-    def _format_error(
-        self,
-        error: Exception,
-        task_description: Union[str, FieldInfo],
-        model_output: str,
-        lm_explain: bool,
-    ) -> str:
-        if isinstance(error, pydantic.ValidationError):
-            errors = []
-            for e in error.errors():
-                fields = ", ".join(map(str, e["loc"]))
-                errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
-            error_text = "; ".join(errors)
-        else:
-            error_text = repr(error)
-
-        if self.explain_errors and lm_explain:
-            if isinstance(task_description, FieldInfo):
-                args = task_description.json_schema_extra
-                task_description = args["prefix"] + " " + args["desc"]
-            return (
-                error_text
-                + "\n"
-                + self._make_explanation(
-                    task_description=task_description,
-                    model_output=model_output,
-                    error=error_text,
-                )
-            )
-
-        return error_text
-
-    def _make_explanation(self, task_description: str, model_output: str, error: str) -> str:
-        class Signature(dspy.Signature):
-            __doc__ = textwrap.dedent(
-                """
-                I gave my language model a task, but it failed. Figure out what went wrong,
-                and write instructions to help it avoid the error next time.""",
-            )
-
-            task_description: str = dspy.InputField(desc="What I asked the model to do")
-            language_model_output: str = dspy.InputField(desc="The output of the model")
-            error: str = dspy.InputField(desc="The validation error trigged by the models output")
-            explanation: str = dspy.OutputField(desc="Explain what the model did wrong")
-            advice: str = dspy.OutputField(
-                desc="Instructions for the model to do better next time. A single paragraph.",
-            )
-
-        # TODO: We could also try repair the output here. For example, if the output is a float, but the
-        # model returned a "float + explanation", the repair could be to remove the explanation.
-
-        return dspy.Predict(Signature)(
-            task_description=task_description,
-            language_model_output=model_output,
-            error=error,
-        ).advice
-
     def _prepare_signature(self) -> dspy.Signature:
         """Add formats and parsers to the signature fields, based on the type annotations of the fields."""
         signature = self.signature
         for name, field in self.signature.fields.items():
             is_output = field.json_schema_extra["__dspy_field_type"] == "output"
             type_ = field.annotation
             if is_output:
@@ -282,21 +217,15 @@
                 parsed = {}
                 for name, field in signature.output_fields.items():
                     try:
                         value = completion[name]
                         parser = field.json_schema_extra.get("parser", lambda x: x)
                         parsed[name] = parser(value)
                     except (pydantic.ValidationError, ValueError) as e:
-                        errors[name] = self._format_error(
-                            e,
-                            signature.fields[name],
-                            value,
-                            lm_explain=try_i + 1 < self.max_retries,
-                        )
-
+                        errors[name] = _format_error(e)
                         # If we can, we add an example to the error message
                         current_desc = field.json_schema_extra.get("desc", "")
                         i = current_desc.find("JSON Schema: ")
                         if i == -1:
                             continue  # Only add examples to JSON objects
                         suffix, current_desc = current_desc[i:], current_desc[:i]
                         prefix = "You MUST use this format: "
@@ -314,23 +243,15 @@
                     break
                 # Instantiate the actual signature with the parsed values.
                 # This allow pydantic to validate the fields defined in the signature.
                 try:
                     _ = self.signature(**kwargs, **parsed)
                     parsed_results.append(parsed)
                 except pydantic.ValidationError as e:
-                    errors["general"] = self._format_error(
-                        e,
-                        signature.instructions,
-                        "\n\n".join(
-                            "> " + field.json_schema_extra["prefix"] + " " + completion[name]
-                            for name, field in signature.output_fields.items()
-                        ),
-                        lm_explain=try_i + 1 < self.max_retries,
-                    )
+                    errors["general"] = _format_error(e)
             if errors:
                 # Add new fields for each error
                 for name, error in errors.items():
                     modified_kwargs[f"error_{name}_{try_i}"] = error
                     if name == "general":
                         error_prefix = "General:"
                     else:
@@ -350,14 +271,24 @@
                 )
         raise ValueError(
             "Too many retries trying to get the correct output format. " + "Try simplifying the requirements.",
             errors,
         )
 
 
+def _format_error(error: Exception):
+    if isinstance(error, pydantic.ValidationError):
+        errors = []
+        for e in error.errors():
+            fields = ", ".join(map(str, e["loc"]))
+            errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
+        return "; ".join(errors)
+    return repr(error)
+
+
 def _func_to_signature(func):
     """Make a dspy.Signature based on a function definition."""
     sig = inspect.signature(func)
     annotations = typing.get_type_hints(func, include_extras=True)
     output_key = func.__name__
     instructions = func.__doc__
     fields = {}
```

### Comparing `dspy-ai-2.4.3/dspy/predict/aggregation.py` & `dspy-ai-2.4.4/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/chain_of_thought.py` & `dspy-ai-2.4.4/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/chain_of_thought_with_hint.py` & `dspy-ai-2.4.4/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/knn.py` & `dspy-ai-2.4.4/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/langchain.py` & `dspy-ai-2.4.4/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/multi_chain_comparison.py` & `dspy-ai-2.4.4/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/predict.py` & `dspy-ai-2.4.4/dspy/predict/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import random
 
-from pydantic import BaseModel
-
 import dsp
 from dspy.predict.parameter import Parameter
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, signature_to_template
 
 
 class Predict(Parameter):
@@ -18,27 +16,17 @@
     def reset(self):
         self.lm = None
         self.traces = []
         self.train = []
         self.demos = []
 
     def dump_state(self):
-        state_keys = ["lm", "traces", "train"]
+        state_keys = ["lm", "traces", "train", "demos"]
         state = {k: getattr(self, k) for k in state_keys}
 
-        state["demos"] = []
-        for demo in self.demos:
-            demo = demo.copy()
-
-            for field in demo:
-                if isinstance(demo[field], BaseModel):
-                    demo[field] = demo[field].model_dump_json()
-
-            state["demos"].append(demo)
-
         # Cache the signature instructions and the last field's name.
         state["signature_instructions"] = self.signature.instructions
 
         *_, last_key = self.signature.fields.keys()
         state["signature_prefix"] = self.signature.fields[last_key].json_schema_extra["prefix"]
 
         return state
```

### Comparing `dspy-ai-2.4.3/dspy/predict/program_of_thought.py` & `dspy-ai-2.4.4/dspy/predict/program_of_thought.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 from dspy.signatures.signature import ensure_signature
 
 from ..primitives.program import Module
 from ..primitives.python_interpreter import CodePrompt, PythonInterpreter
 
 
 class ProgramOfThought(Module):
-    def __init__(self, signature, max_iters=3, import_white_list=None):
+    def __init__(self, signature, max_iters=3):
         super().__init__()
         self.signature = signature = ensure_signature(signature)
         self.max_iters = max_iters
-        self.import_white_list = import_white_list
 
         self.input_fields = signature.input_fields
         self.output_fields = signature.output_fields
 
-        assert len(self.output_fields) == 1, "PoT only supports one output field."
-
-        self.output_field_name = next(iter(self.output_fields))
         inputs_ = ", ".join(
             [f"`{field_name}`" for field_name in self.input_fields.keys()],
         )
-        outputs_ = f"`{self.output_field_name}`"
+        outputs_ = ", ".join(
+            [f"`{field_name}`" for field_name in self.output_fields.keys()],
+        )
 
         assert len(self.output_fields) == 1, "PoT only supports one output field."
 
         instr = []
         instr.append(
             f"You will be given {inputs_} and you will respond with {outputs_}.",
         )
@@ -53,14 +51,15 @@
         )
         self.generate_answer = dspy.ChainOfThought(
             dspy.Signature(
                 self._generate_signature("answer").fields,
                 self._generate_instruction("answer"),
             ),
         )
+
     def _generate_signature(self, mode):
         signature_dict = dict(self.input_fields)
         fields_for_mode = {
             "generate": {
                 "generated_code": dspy.OutputField(
                     prefix="Code:",
                     desc="python code that answers the question",
@@ -89,47 +88,51 @@
                     desc="python code that answers the question",
                     format=str,
                 ),
                 "code_output": dspy.InputField(
                     prefix="Code Output:",
                     desc="output of previously-generated python code",
                 ),
-                self.output_field_name: self.signature.fields[self.output_field_name],
+                "answer": self.signature.fields["answer"],
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
-        mode_outputs = f"`{self.output_field_name}`"
+        mode_outputs = ", ".join(
+            [
+                f"`{field_name}`"
+                for field_name in self._generate_signature(mode).output_fields
+            ],
+        )
         if mode == "generate":
             instr = [
                 f"You will be given {mode_inputs} and you will respond with {mode_outputs}.",
                 f"Generating executable Python code that programmatically computes the correct {mode_outputs}.",
                 f"After you're done with the computation, make sure the last line in your code evaluates to the correct value for {mode_outputs}.",
             ]
         elif mode == "regenerate":
             instr = [
                 f"You are given {mode_inputs} due to an error in previous code.",
-                "Your task is to correct the error and provide the new `generated_code`.",
+                f"Your task is to correct the error and provide the new {mode_outputs}.",
             ]
         else:  # mode == 'answer'
             instr = [
                 f"Given the final code {mode_inputs}, provide the final {mode_outputs}.",
             ]
 
         return "\n".join(instr)
 
-
     def parse_code(self, code_data):
         code = (
             code_data.get("generated_code", "").split("---", 1)[0].split("\n\n\n", 1)[0]
         )
         code_match = re.search(r"```python[ \n](.*?)[ \n]```?", code, re.DOTALL)
         code_block = (code_match.group(1) if code_match else code).replace("\\n", "\n")
         if not code_block:
@@ -149,37 +152,36 @@
             )
         return code_block, None
 
     def execute_code(self, code):
         if not code:
             return code, None, "Error: Empty code before execution."
         code_prompt = CodePrompt(code, code_type="python")
-        interpreter = PythonInterpreter(action_space={"print": print}, import_white_list=self.import_white_list)
+        interpreter = PythonInterpreter(action_space={"print": print})
         try:
             output = str(code_prompt.execute(interpreter=interpreter)[0])
-            print
             return code, output, None
         except Exception as e:
             return code, None, str(e)
+
     def forward(self, **kwargs):
-        input_kwargs = {
-            field_name: kwargs[field_name] for field_name in self.input_fields
-        }
-        code_data = self.code_generate(**input_kwargs)
+        code_data = self.code_generate(question=kwargs["question"])
         parsed_code, error = self.parse_code(code_data)
         # FIXME: Don't try to execute the code if it didn't parse
         code, output, error = self.execute_code(parsed_code)
         hop = 0
         while hop < self.max_iters and error:
             print("Error in code execution")
-            input_kwargs.update({"previous_code": code, "error": error})
-            code_data = self.code_regenerate(**input_kwargs)
+            code_data = self.code_regenerate(
+                question=kwargs["question"], previous_code=code, error=error,
+            )
             parsed_code, error = self.parse_code(code_data)
             # FIXME: Don't try to execute the code if it didn't parse
             code, output, error = self.execute_code(parsed_code)
             hop += 1
             if hop == self.max_iters:
                 print("Max hops reached. Error persists.")
                 return None
-        input_kwargs.update({"final_generated_code": code, "code_output": output})
-        answer_gen_result = self.generate_answer(**input_kwargs)
-        return answer_gen_result
+        answer_gen_result = self.generate_answer(
+            question=kwargs["question"], final_generated_code=code, code_output=output,
+        )
+        return answer_gen_result
```

### Comparing `dspy-ai-2.4.3/dspy/predict/react.py` & `dspy-ai-2.4.4/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/predict/retry.py` & `dspy-ai-2.4.4/dspy/predict/retry.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,31 +28,25 @@
             desc="Some instructions you must satisfy",
             format=str,
         ))
 
         return signature
 
     def forward(self, *, past_outputs, **kwargs):
-        # Take into account the possible new signature, as in TypedPredictor
-        new_signature = kwargs.pop("new_signature", None)
-        if new_signature:
-            self.original_signature = new_signature
-            self.new_signature = self._create_new_signature(self.original_signature)
-
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
@@ -61,14 +55,14 @@
             pred = self.forward(**kwargs)
         else:
             pred = self.module(**kwargs)
 
         # now pop multiple reserved keys
         # NOTE(shangyin) past_outputs seems not useful to include in demos,
         # therefore dropped
-        for key in ["_trace", "demos", "signature", "new_signature", "config", "lm", "past_outputs"]:
+        for key in ["_trace", "demos", "signature", "config", "lm", "past_outputs"]:
             kwargs.pop(key, None)
 
         if dsp.settings.trace is not None:
             trace = dsp.settings.trace
             trace.append((self, {**kwargs}, pred))
         return pred
```

### Comparing `dspy-ai-2.4.3/dspy/primitives/assertions.py` & `dspy-ai-2.4.4/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/primitives/box.py` & `dspy-ai-2.4.4/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/primitives/example.py` & `dspy-ai-2.4.4/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/primitives/module.py` & `dspy-ai-2.4.4/dspy/primitives/module.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/primitives/prediction.py` & `dspy-ai-2.4.4/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/primitives/program.py` & `dspy-ai-2.4.4/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/primitives/python_interpreter.py` & `dspy-ai-2.4.4/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/chromadb_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/chromadb_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         Returns:
             List[List[float]]: List of embeddings corresponding to each query.
         """
         return self.ef(queries)
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,
     ) -> dspy.Prediction:
         """Search with db for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
@@ -138,15 +138,15 @@
             else query_or_queries
         )
         queries = [q for q in queries if q]  # Filter empty queries
         embeddings = self._get_embeddings(queries)
 
         k = self.k if k is None else k
         results = self._chromadb_collection.query(
-            query_embeddings=embeddings, n_results=k,**kwargs,
+            query_embeddings=embeddings, n_results=k,
         )
 
         zipped_results = zip(
             results["ids"][0], 
             results["distances"][0], 
             results["documents"][0], 
             results["metadatas"][0])
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/clarifai_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/clarifai_rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         header = {"Authorization": f"Key {self.pat}"}
         request = requests.get(hits.input.data.text.url, headers=header)
         request.encoding = request.apparent_encoding
         requested_text = request.text
         return requested_text
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,
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
-            search_response = self.clarifai_search.query(ranks=[{"text_raw": query}],**kwargs)
+            search_response = self.clarifai_search.query(ranks=[{"text_raw": query}])
 
             # Retrieve hits
             hits = [hit for data in search_response for hit in data.hits]
             with ThreadPoolExecutor(max_workers=10) as executor:
                 results = list(executor.map(self.retrieve_hits, hits))
             passages.extend(dotdict({"long_text": d}) for d in results)
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/databricks_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/deeplake_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/deeplake_rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         texts = [t.replace("\n", " ") for t in texts]
         return [
             data["embedding"]
             for data in openai.Embedding.create(input=texts, model=model)["data"]
         ]
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int],**kwargs,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int],
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
-            ).search(query, k=k,**kwargs)
+            ).search(query, k=k)
 
             for score,text in zip(results.get('score',0.0),results.get('text',"")):
                 passages[text] += score
 
         sorted_passages = sorted(
             passages.items(), key=lambda x: x[1], reverse=True)[:k]
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/faiss_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/faiss_rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             indices = index_list[i]
             distances = distance_list[i]
             logging.debug(f"Query: {queries[i]}")
             for j in range(len(indices)):
                 logging.debug(f"    Hit {j} = {indices[j]}/{distances[j]}: {self._document_chunks[indices[j]]}")
         return
 
-    def forward(self, query_or_queries: Union[str, list[str]], k: Optional[int] = None,**kwargs) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, list[str]], k: Optional[int] = None) -> dspy.Prediction:
         """Search the faiss index for k or self.k top passages for query.
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -123,15 +123,15 @@
         # For single query, just look up the top k passages
         if len(queries) == 1:
             distance_list, index_list = self._faiss_index.search(emb_npa, k or self.k)
             # self._dump_raw_results(queries, index_list, distance_list)
             passages = [(self._document_chunks[ind], ind) for ind in index_list[0]]
             return [dotdict({"long_text": passage[0], "index": passage[1]}) for passage in passages]
 
-        distance_list, index_list = self._faiss_index.search(emb_npa, (k or self.k) * 3,**kwargs)
+        distance_list, index_list = self._faiss_index.search(emb_npa, (k or self.k) * 3)
         # self._dump_raw_results(queries, index_list, distance_list)
         passage_scores = {}
         for emb in range(len(embeddings)):
             indices = index_list[emb]  # indices of neighbors for embeddings[emb] - this is an array of k*3 integers
             distances = distance_list[
                 emb
             ]  # distances of neighbors for embeddings[emb] - this is an array of k*3 floating point numbers
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/marqo_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/mongodb_atlas_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/neo4j_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/pinecone_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/qdrant_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/qdrant_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         k: int = 3,
     ):
         self._qdrant_collection_name = qdrant_collection_name
         self._qdrant_client = qdrant_client
 
         super().__init__(k=k)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int],**kwargs) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int]) -> dspy.Prediction:
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
-            self._qdrant_collection_name, query_texts=queries, limit=k,**kwargs)
+            self._qdrant_collection_name, query_texts=queries, limit=k)
 
         passages_scores = defaultdict(float)
         for batch in batch_results:
             for result in batch:
                 # If a passage is returned multiple times, the score is accumulated.
                 passages_scores[result.document] += result.score
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/retrieve.py` & `dspy-ai-2.4.4/dspy/retrieve/retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     def load_state(self, state):
         for name, value in state.items():
             setattr(self, name, value)
 
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs) -> Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None) -> Prediction:
         queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [query.strip().split('\n')[0].strip() for query in queries]
 
         # print(queries)
         # TODO: Consider removing any quote-like markers that surround the query too.
         k = k if k is not None else self.k
-        passages = dsp.retrieveEnsemble(queries, k=k,**kwargs)
+        passages = dsp.retrieveEnsemble(queries, k=k)
         return Prediction(passages=passages)
 
 # TODO: Consider doing Prediction.from_completions with the individual sets of passages (per query) too.
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/vectara_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/retrieve/weaviate_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/weaviate_rm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List, Optional, Union
 
 import dspy
 from dsp.utils import dotdict
 
 try:
     import weaviate
-    import weaviate.classes as wvc
-    from weaviate.collections.classes.grpc import HybridFusion
 except ImportError:
     raise ImportError(
         "The 'weaviate' extra is required to use WeaviateRM. Install it with `pip install dspy-ai[weaviate]`",
     )
 
 
 class WeaviateRM(dspy.Retrieve):
@@ -20,17 +18,14 @@
     Assumes that a Weaviate collection has been created and populated with the following payload:
         - content: The text of the passage
 
     Args:
         weaviate_collection_name (str): The name of the Weaviate collection.
         weaviate_client (WeaviateClient): An instance of the Weaviate client.
         k (int, optional): The default number of top passages to retrieve. Defaults to 3.
-        weaviate_collection_text_key (str, optional): The key in the collection with the content. Defaults to content.
-        weaviate_alpha (float, optional): The alpha value for the hybrid query. Defaults to 0.5.
-        weaviate_fusion_type (wvc.HybridFusion, optional): The fusion type for the query. Defaults to RELATIVE_SCORE.
 
     Examples:
         Below is a code snippet that shows how to use Weaviate as the default retriver:
         ```python
         import weaviate
 
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
@@ -45,28 +40,24 @@
         ```python
         self.retrieve = WeaviateRM("my_collection_name", weaviate_client=weaviate_client, k=num_passages)
         ```
     """
 
     def __init__(self, 
                  weaviate_collection_name: str, 
-                 weaviate_client: weaviate.WeaviateClient,
+                 weaviate_client: weaviate.Client, 
                  k: int = 3,
                  weaviate_collection_text_key: Optional[str] = "content",
-                 weaviate_alpha: Optional[float] = 0.5,
-                 weaviate_fusion_type: Optional[HybridFusion] = HybridFusion.RELATIVE_SCORE,
         ):
         self._weaviate_collection_name = weaviate_collection_name
         self._weaviate_client = weaviate_client
         self._weaviate_collection_text_key = weaviate_collection_text_key
-        self._weaviate_alpha = weaviate_alpha
-        self._weaviate_fusion_type = weaviate_fusion_type
         super().__init__(k=k)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int]) -> dspy.Prediction:
         """Search with Weaviate for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -77,22 +68,18 @@
             [query_or_queries]
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         queries = [q for q in queries if q]
         passages = []
         for query in queries:
-            collection = self._weaviate_client.collections.get(self._weaviate_collection_name)
-            results = collection.query.hybrid(query=query,
-                                              limit=k,
-                                              alpha=self._weaviate_alpha,
-                                              fusion_type=self._weaviate_fusion_type,
-                                              return_metadata=wvc.query.MetadataQuery(
-                                                  distance=True, score=True),
-                                              **kwargs,
-                                              )
+            results = self._weaviate_client.query\
+                .get(self._weaviate_collection_name, [self._weaviate_collection_text_key])\
+                .with_hybrid(query=query)\
+                .with_limit(k)\
+                .do()
 
-            parsed_results = [result.properties[self._weaviate_collection_text_key] for result in results.objects]
+            results = results["data"]["Get"][self._weaviate_collection_name]
+            parsed_results = [result[self._weaviate_collection_text_key] for result in results]
             passages.extend(dotdict({"long_text": d}) for d in parsed_results)
 
-        # Return type not changed, needs to be a Prediction object. But other code will break if we change it.
         return passages
```

### Comparing `dspy-ai-2.4.3/dspy/retrieve/you_rm.py` & `dspy-ai-2.4.4/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/signatures/field.py` & `dspy-ai-2.4.4/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/signatures/signature.py` & `dspy-ai-2.4.4/dspy/signatures/signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -202,21 +202,19 @@
     ""  # noqa: D419
 
     # Note: Don't put a docstring here, as it will become the default instructions
     # for any signature that doesn't define it's own instructions.
     pass
 
 
-def ensure_signature(signature: Union[str, Type[Signature]], instructions=None) -> Signature:
+def ensure_signature(signature: Union[str, Type[Signature]]) -> Signature:
     if signature is None:
         return None
     if isinstance(signature, str):
-        return Signature(signature, instructions)
-    if instructions is not None:
-        raise ValueError("Don't specify instructions when initializing with a Signature")
+        return Signature(signature)
     return signature
 
 
 def make_signature(
     signature: Union[str, Dict[str, Tuple[type, FieldInfo]]],
     instructions: str = None,
     signature_name: str = "StringSignature",
@@ -275,39 +273,44 @@
     )
 
 
 def _parse_signature(signature: str) -> Tuple[Type, Field]:
     if signature.count("->") != 1:
         raise ValueError(f"Invalid signature format: '{signature}', must contain exactly one '->'.")
 
-    inputs_str, outputs_str = signature.split("->")
-
     fields = {}
-    for name, type_ in _parse_arg_string(inputs_str):
+    inputs_str, outputs_str = map(str.strip, signature.split("->"))
+    inputs = [v.strip() for v in inputs_str.split(",") if v.strip()]
+    outputs = [v.strip() for v in outputs_str.split(",") if v.strip()]
+    for name_type in inputs:
+        name, type_ = _parse_named_type_node(name_type)
         fields[name] = (type_, InputField())
-    for name, type_ in _parse_arg_string(outputs_str):
+    for name_type in outputs:
+        name, type_ = _parse_named_type_node(name_type)
         fields[name] = (type_, OutputField())
 
     return fields
 
 
-def _parse_arg_string(string: str, names=None) -> Dict[str, str]:
-    args = ast.parse("def f(" + string + "): pass").body[0].args.args
-    names = [arg.arg for arg in args]
-    types = [str if arg.annotation is None else _parse_type_node(arg.annotation) for arg in args]
-    return zip(names, types)
+def _parse_named_type_node(node, names=None) -> Any:
+    parts = node.split(":")
+    if len(parts) == 1:
+        return parts[0], str
+    name, type_str = parts
+    type_ = _parse_type_node(ast.parse(type_str), names)
+    return name, type_
 
 
 def _parse_type_node(node, names=None) -> Any:
     """Recursively parse an AST node representing a type annotation.
 
     without using structural pattern matching introduced in Python 3.10.
     """
     if names is None:
-        names = typing.__dict__
+        names = {}
 
     if isinstance(node, ast.Module):
         body = node.body
         if len(body) != 1:
             raise ValueError(f"Code is not syntactically valid: {node}")
         return _parse_type_node(body[0], names)
 
@@ -318,31 +321,24 @@
     if isinstance(node, ast.Name):
         id_ = node.id
         if id_ in names:
             return names[id_]
         for type_ in [int, str, float, bool, list, tuple, dict]:
             if type_.__name__ == id_:
                 return type_
-        raise ValueError(f"Unknown name: {id_}")
 
-    if isinstance(node, ast.Subscript):
+    elif isinstance(node, ast.Subscript):
         base_type = _parse_type_node(node.value, names)
         arg_type = _parse_type_node(node.slice, names)
         return base_type[arg_type]
 
-    if isinstance(node, ast.Tuple):
+    elif isinstance(node, ast.Tuple):
         elts = node.elts
         return tuple(_parse_type_node(elt, names) for elt in elts)
 
-    if isinstance(node, ast.Call):
-        if node.func.id == "Field":
-            keys = [kw.arg for kw in node.keywords]
-            values = [kw.value.value for kw in node.keywords]
-            return Field(**dict(zip(keys, values)))
-
     raise ValueError(f"Code is not syntactically valid: {node}")
 
 
 def infer_prefix(attribute_name: str) -> str:
     """Infer a prefix from an attribute name."""
     # Convert camelCase to snake_case, but handle sequences of capital letters properly
     s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", attribute_name)
```

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/bootstrap.py` & `dspy-ai-2.4.4/dspy/teleprompt/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/copro_optimizer.py` & `dspy-ai-2.4.4/dspy/teleprompt/copro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/ensemble.py` & `dspy-ai-2.4.4/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/finetune.py` & `dspy-ai-2.4.4/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/knn_fewshot.py` & `dspy-ai-2.4.4/dspy/teleprompt/knn_fewshot.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/mipro_optimizer.py` & `dspy-ai-2.4.4/dspy/teleprompt/mipro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/random_search.py` & `dspy-ai-2.4.4/dspy/teleprompt/random_search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/signature_opt.py` & `dspy-ai-2.4.4/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/signature_opt_bayesian.py` & `dspy-ai-2.4.4/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/signature_opt_typed.py` & `dspy-ai-2.4.4/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/teleprompt_optuna.py` & `dspy-ai-2.4.4/dspy/teleprompt/teleprompt_optuna.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/teleprompt/vanilla.py` & `dspy-ai-2.4.4/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy/utils/dummies.py` & `dspy-ai-2.4.4/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.3/dspy_ai.egg-info/PKG-INFO` & `dspy-ai-2.4.4/dspy_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.3
+Version: 2.4.4
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
@@ -122,15 +122,14 @@
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
 - Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
-- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
```

### Comparing `dspy-ai-2.4.3/dspy_ai.egg-info/SOURCES.txt` & `dspy-ai-2.4.4/dspy_ai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 dsp/modules/cache_utils.py
 dsp/modules/clarifai.py
 dsp/modules/cohere.py
 dsp/modules/colbertv2.py
 dsp/modules/databricks.py
 dsp/modules/google.py
 dsp/modules/gpt3.py
-dsp/modules/groq_client.py
 dsp/modules/hf.py
 dsp/modules/hf_client.py
 dsp/modules/hf_server.py
 dsp/modules/lm.py
-dsp/modules/mistral.py
 dsp/modules/ollama.py
 dsp/modules/pyserini.py
 dsp/modules/sbert.py
 dsp/modules/sentence_vectorizer.py
 dsp/modules/finetuning/__init__.py
 dsp/modules/finetuning/finetune_hf.py
 dsp/primitives/__init__.py
@@ -91,27 +89,25 @@
 dspy/primitives/box.py
 dspy/primitives/example.py
 dspy/primitives/module.py
 dspy/primitives/prediction.py
 dspy/primitives/program.py
 dspy/primitives/python_interpreter.py
 dspy/retrieve/__init__.py
-dspy/retrieve/azureaisearch_rm.py
 dspy/retrieve/chromadb_rm.py
 dspy/retrieve/clarifai_rm.py
 dspy/retrieve/databricks_rm.py
 dspy/retrieve/deeplake_rm.py
 dspy/retrieve/faiss_rm.py
 dspy/retrieve/marqo_rm.py
 dspy/retrieve/mongodb_atlas_rm.py
 dspy/retrieve/neo4j_rm.py
 dspy/retrieve/pgvector_rm.py
 dspy/retrieve/pinecone_rm.py
 dspy/retrieve/qdrant_rm.py
-dspy/retrieve/ragatouille_rm.py
 dspy/retrieve/retrieve.py
 dspy/retrieve/vectara_rm.py
 dspy/retrieve/weaviate_rm.py
 dspy/retrieve/weaviate_rm_test.py
 dspy/retrieve/you_rm.py
 dspy/signatures/__init__.py
 dspy/signatures/field.py
@@ -128,13 +124,12 @@
 dspy/teleprompt/signature_opt_bayesian.py
 dspy/teleprompt/signature_opt_typed.py
 dspy/teleprompt/teleprompt.py
 dspy/teleprompt/teleprompt_optuna.py
 dspy/teleprompt/vanilla.py
 dspy/utils/__init__.py
 dspy/utils/dummies.py
-dspy/utils/logging.py
 dspy_ai.egg-info/PKG-INFO
 dspy_ai.egg-info/SOURCES.txt
 dspy_ai.egg-info/dependency_links.txt
 dspy_ai.egg-info/requires.txt
 dspy_ai.egg-info/top_level.txt
```

### Comparing `dspy-ai-2.4.3/dspy_ai.egg-info/requires.txt` & `dspy-ai-2.4.4/dspy_ai.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pandas
 regex
 ujson
 tqdm
 datasets<3.0.0,~=2.14.6
 requests
 optuna
-pydantic<=2.7,>=2.5.0
+pydantic==2.5.0
 
 [anthropic]
 anthropic~=0.18.0
 
 [chromadb]
 chromadb~=0.4.14
 
@@ -45,13 +45,12 @@
 
 [pinecone]
 pinecone-client~=2.2.4
 
 [qdrant]
 qdrant-client
 fastembed
-qdrant-client>=1.6.2
-fastembed>=0.1.0
+qdrant-client~=1.6.2
+fastembed~=0.1.0
 
 [weaviate]
 weaviate-client~=3.26.1
-weaviate-client~=4.5.4
```

### Comparing `dspy-ai-2.4.3/pyproject.toml` & `dspy-ai-2.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.4.3"
+version = "2.4.4"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.12"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -31,37 +31,36 @@
     "pandas",
     "regex",
     "ujson",
     "tqdm",
     "datasets~=2.14.6,<3.0.0",
     "requests",
     "optuna",
-    "pydantic>=2.5.0,<=2.7",
+    "pydantic==2.5.0",
 ]
 
 [project.optional-dependencies]
 anthropic = ["anthropic~=0.18.0"]
 chromadb = ["chromadb~=0.4.14"]
-qdrant = ["qdrant-client>=1.6.2", "fastembed>=0.1.0"]
+qdrant = ["qdrant-client~=1.6.2", "fastembed~=0.1.0"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client~=2.2.4"]
-weaviate = ["weaviate-client~=4.5.4"]
+weaviate = ["weaviate-client~=3.26.1"]
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
-    
 ]
 dev = ["pytest>=6.2.5"]
 
 [project.urls]
 homepage = "https://github.com/stanfordnlp/dspy"
 
 [tool.poetry]
@@ -76,15 +75,15 @@
 # documentation = "https://dspy-ai.readthedocs.io"
 keywords = ["dspy", "ai", "language models", "llm", "openai"]
 # may be a bit much
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = ">=2.5.0,<=2.7"
+pydantic = "2.5.0"
 backoff = "^2.2.1"
 joblib = "^1.3.2"
 openai = ">=0.28.1,<2.0.0"
 pandas = "^2.1.1"
 regex = "^2023.10.3"
 ujson = "^5.8.0"
 tqdm = "^4.66.1"
@@ -93,49 +92,43 @@
 optuna = "^3.4.0"
 anthropic = { version = "^0.18.0", optional = true }
 chromadb = { version = "^0.4.14", optional = true }
 fastembed = { version = "^0.1.0", optional = true }
 marqo = { version = "*", optional = true }
 qdrant-client = { version = "^1.6.2", optional = true }
 pinecone-client = { version = "^2.2.4", optional = true }
-weaviate-client = { version = "^4.5.4", optional = true }
+weaviate-client = { version = "^3.26.1", optional = true }
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
-groq = {version = "^0.4.2", optional = true }
 rich = "^13.7.1"
-psycopg2 = {version = "^2.9.9", optional = true}
-pgvector = {version = "^0.2.5", optional = true}
-structlog = "^24.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 transformers = "^4.38.2"
 torch = "^2.2.1"
 pytest-mock = "^3.12.0"
 ruff = "^0.3.0"
 black = "^24.2.0"
-pre-commit = "^3.7.0"
 
 [tool.poetry.extras]
 chromadb = ["chromadb"]
 qdrant = ["qdrant-client", "fastembed"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client"]
 weaviate = ["weaviate-client"]
-postgres = ["psycopg2", "pgvector"]
 docs = [
     "sphinx",
     "furo",
     "docutils",
     "m2r2",
     "myst-parser",
     "myst-nb",
```

### Comparing `dspy-ai-2.4.3/setup.py` & `dspy-ai-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file	
 with open('requirements.txt', encoding='utf-8') as f:	
     requirements = f.read().splitlines()	
 
 setup(	
     name="dspy-ai",	
-    version="2.4.3",	
+    version="2.4.4",	
     description="DSPy",	
     long_description=long_description,	
     long_description_content_type='text/markdown',	
     url="https://github.com/stanfordnlp/dsp",	
     author="Omar Khattab",	
     author_email="okhattab@stanford.edu",	
     license="MIT License",
```

