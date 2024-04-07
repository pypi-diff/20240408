# Comparing `tmp/athina-1.2.7.tar.gz` & `tmp/athina-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina-1.2.7.tar", max compression
+gzip compressed data, was "athina-1.2.8.tar", max compression
```

## Comparing `athina-1.2.7.tar` & `athina-1.2.8.tar`

### file list

```diff
@@ -1,131 +1,133 @@
--rw-r--r--   0        0        0     8595 2024-03-19 22:27:57.176555 athina-1.2.7/README.md
--rw-r--r--   0        0        0      135 2024-03-31 08:08:53.507635 athina-1.2.7/athina/__init__.py
--rw-r--r--   0        0        0     2938 2024-03-19 22:27:57.176822 athina-1.2.7/athina/benchmark/eval_performance_calculator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.2.7/athina/cli/__init__.py
--rw-r--r--   0        0        0     5390 2024-03-31 07:49:47.783450 athina-1.2.7/athina/cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.2.7/athina/constants/__init__.py
--rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.2.7/athina/constants/messages.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177320 athina-1.2.7/athina/datasets/__init__.py
--rw-r--r--   0        0        0   218970 2024-03-19 22:27:57.177712 athina-1.2.7/athina/datasets/conversations.json
--rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.2.7/athina/datasets/summarization_sample.py
--rw-r--r--   0        0        0     2675 2024-03-19 22:27:57.177915 athina-1.2.7/athina/datasets/yc_query_mini.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.2.7/athina/errors/__init__.py
--rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.2.7/athina/errors/exceptions.py
--rw-r--r--   0        0        0     4069 2024-03-31 07:49:47.783585 athina-1.2.7/athina/evals/__init__.py
--rw-r--r--   0        0        0     7508 2024-03-27 06:24:44.855919 athina-1.2.7/athina/evals/base_evaluator.py
--rw-r--r--   0        0        0     4253 2024-03-20 00:06:17.768963 athina-1.2.7/athina/evals/conversation/conversation_coherence/evaluator.py
--rw-r--r--   0        0        0     1198 2024-03-19 22:27:57.178641 athina-1.2.7/athina/evals/conversation/conversation_coherence/prompt.py
--rw-r--r--   0        0        0     4408 2024-03-19 22:27:57.178765 athina-1.2.7/athina/evals/conversation/conversation_resolution/evaluator.py
--rw-r--r--   0        0        0     1104 2024-03-19 22:27:57.178845 athina-1.2.7/athina/evals/conversation/conversation_resolution/prompt.py
--rw-r--r--   0        0        0     2467 2024-03-31 07:49:47.783990 athina-1.2.7/athina/evals/eval_type.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.2.7/athina/evals/function/__init__.py
--rw-r--r--   0        0        0     3599 2024-03-27 06:24:44.856062 athina-1.2.7/athina/evals/function/function_evaluator.py
--rw-r--r--   0        0        0    18806 2024-03-27 11:54:50.117642 athina-1.2.7/athina/evals/function/functions.py
--rw-r--r--   0        0        0    10216 2024-03-27 09:12:43.212033 athina-1.2.7/athina/evals/function/wrapper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.2.7/athina/evals/grounded/__init__.py
--rw-r--r--   0        0        0     3879 2024-03-20 16:40:39.753015 athina-1.2.7/athina/evals/grounded/grounded_evaluator.py
--rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.2.7/athina/evals/grounded/similarity.py
--rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.2.7/athina/evals/grounded/wrapper.py
--rw-r--r--   0        0        0     2961 2024-03-31 07:59:33.939857 athina-1.2.7/athina/evals/guardrails/gibberish_text/evaluator.py
--rw-r--r--   0        0        0     3727 2024-03-31 07:59:40.366940 athina-1.2.7/athina/evals/guardrails/sensitive_topics/evaluator.py
--rw-r--r--   0        0        0     2885 2024-03-31 07:49:47.784487 athina-1.2.7/athina/evals/guardrails/sfw/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.2.7/athina/evals/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.2.7/athina/evals/llm/context_contains_enough_information/__init__.py
--rw-r--r--   0        0        0     2671 2024-03-27 03:09:24.346838 athina-1.2.7/athina/evals/llm/context_contains_enough_information/evaluator.py
--rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.2.7/athina/evals/llm/context_contains_enough_information/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.2.7/athina/evals/llm/custom_prompt/__init__.py
--rw-r--r--   0        0        0     2362 2024-03-27 06:24:44.857102 athina-1.2.7/athina/evals/llm/custom_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.2.7/athina/evals/llm/does_response_answer_query/__init__.py
--rw-r--r--   0        0        0     2632 2024-03-19 22:27:57.180901 athina-1.2.7/athina/evals/llm/does_response_answer_query/evaluator.py
--rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.2.7/athina/evals/llm/does_response_answer_query/examples.py
--rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.2.7/athina/evals/llm/example.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.2.7/athina/evals/llm/faithfulness/__init__.py
--rw-r--r--   0        0        0     2599 2024-03-19 22:27:57.181215 athina-1.2.7/athina/evals/llm/faithfulness/evaluator.py
--rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.2.7/athina/evals/llm/faithfulness/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.2.7/athina/evals/llm/grading_criteria/__init__.py
--rw-r--r--   0        0        0     2080 2024-03-30 01:06:22.852872 athina-1.2.7/athina/evals/llm/grading_criteria/evaluator.py
--rw-r--r--   0        0        0     5821 2024-03-20 00:37:57.522908 athina-1.2.7/athina/evals/llm/groundedness/evaluator.py
--rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.2.7/athina/evals/llm/groundedness/prompt.py
--rw-r--r--   0        0        0     4982 2024-03-19 22:27:57.181767 athina-1.2.7/athina/evals/llm/llm_evaluator.py
--rw-r--r--   0        0        0    10915 2024-03-20 02:27:27.436310 athina-1.2.7/athina/evals/llm/summary_accuracy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.2.7/athina/evals/ragas/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.2.7/athina/evals/ragas/answer_correctness/__init__.py
--rw-r--r--   0        0        0     2383 2024-03-19 22:27:57.182414 athina-1.2.7/athina/evals/ragas/answer_correctness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.2.7/athina/evals/ragas/answer_relevancy/__init__.py
--rw-r--r--   0        0        0     2441 2024-03-19 22:27:57.182610 athina-1.2.7/athina/evals/ragas/answer_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.2.7/athina/evals/ragas/answer_semantic_similarity/__init__.py
--rw-r--r--   0        0        0     2440 2024-03-19 22:27:57.182849 athina-1.2.7/athina/evals/ragas/answer_semantic_similarity/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.2.7/athina/evals/ragas/coherence/__init__.py
--rw-r--r--   0        0        0     2329 2024-03-19 22:27:57.183089 athina-1.2.7/athina/evals/ragas/coherence/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.2.7/athina/evals/ragas/conciseness/__init__.py
--rw-r--r--   0        0        0     2364 2024-03-19 22:27:57.183287 athina-1.2.7/athina/evals/ragas/conciseness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.2.7/athina/evals/ragas/context_precision/__init__.py
--rw-r--r--   0        0        0     2516 2024-03-19 22:27:57.183483 athina-1.2.7/athina/evals/ragas/context_precision/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.2.7/athina/evals/ragas/context_recall/__init__.py
--rw-r--r--   0        0        0     2316 2024-03-19 22:27:57.183641 athina-1.2.7/athina/evals/ragas/context_recall/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.2.7/athina/evals/ragas/context_relevancy/__init__.py
--rw-r--r--   0        0        0     2159 2024-03-19 22:27:57.183804 athina-1.2.7/athina/evals/ragas/context_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.2.7/athina/evals/ragas/faithfulness/__init__.py
--rw-r--r--   0        0        0     2370 2024-03-19 22:27:57.183971 athina-1.2.7/athina/evals/ragas/faithfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.2.7/athina/evals/ragas/harmfulness/__init__.py
--rw-r--r--   0        0        0     2306 2024-03-19 22:27:57.184158 athina-1.2.7/athina/evals/ragas/harmfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.2.7/athina/evals/ragas/maliciousness/__init__.py
--rw-r--r--   0        0        0     2268 2024-03-19 22:27:57.184345 athina-1.2.7/athina/evals/ragas/maliciousness/evaluator.py
--rw-r--r--   0        0        0     3298 2024-03-19 22:27:57.184435 athina-1.2.7/athina/evals/ragas/ragas_evaluator.py
--rw-r--r--   0        0        0     5154 2024-03-31 07:49:47.784643 athina-1.2.7/athina/evals/safety/content_moderation/evaluator.py
--rw-r--r--   0        0        0     3299 2024-03-27 06:24:44.857314 athina-1.2.7/athina/evals/safety/pii_detection/evaluator.py
--rw-r--r--   0        0        0     4370 2024-03-27 06:24:44.857479 athina-1.2.7/athina/evals/safety/prompt_injection/evaluator.py
--rw-r--r--   0        0        0      106 2024-03-27 06:24:44.857663 athina-1.2.7/athina/guard/exception.py
--rw-r--r--   0        0        0     1404 2024-03-31 07:49:47.784768 athina-1.2.7/athina/guard/guard.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.2.7/athina/helpers/__init__.py
--rw-r--r--   0        0        0     4446 2024-03-19 22:27:57.184591 athina-1.2.7/athina/helpers/athina_logging_helper.py
--rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.2.7/athina/helpers/config.py
--rw-r--r--   0        0        0      122 2024-03-19 22:27:57.184730 athina-1.2.7/athina/helpers/constants.py
--rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.2.7/athina/helpers/eval_helper.py
--rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.2.7/athina/helpers/function_eval_util.py
--rw-r--r--   0        0        0     4405 2024-03-31 07:49:47.785243 athina-1.2.7/athina/helpers/get_evaluator.py
--rw-r--r--   0        0        0     1190 2024-03-19 22:27:57.185041 athina-1.2.7/athina/helpers/json.py
--rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.2.7/athina/helpers/kwparser.py
--rw-r--r--   0        0        0      894 2024-03-31 07:49:47.785808 athina-1.2.7/athina/helpers/loader_helper.py
--rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.2.7/athina/helpers/logger.py
--rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.2.7/athina/helpers/package_helper.py
--rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.2.7/athina/helpers/run_helper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.2.7/athina/interfaces/__init__.py
--rw-r--r--   0        0        0     3905 2024-03-19 22:27:57.185587 athina-1.2.7/athina/interfaces/athina.py
--rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.2.7/athina/interfaces/data.py
--rw-r--r--   0        0        0     1238 2024-03-27 06:24:44.857991 athina-1.2.7/athina/interfaces/model.py
--rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.2.7/athina/interfaces/openai.py
--rw-r--r--   0        0        0     2944 2024-03-27 06:24:44.858163 athina-1.2.7/athina/interfaces/result.py
--rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.2.7/athina/keys/__init__.py
--rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.2.7/athina/keys/athina_api_key.py
--rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.2.7/athina/keys/openai_api_key.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.2.7/athina/llms/__init__.py
--rw-r--r--   0        0        0     1398 2024-03-19 22:27:57.186244 athina-1.2.7/athina/llms/abstract_llm_service.py
--rw-r--r--   0        0        0     3342 2024-03-19 22:27:57.186314 athina-1.2.7/athina/llms/openai_service.py
--rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.2.7/athina/llms/question_answerer.py
--rw-r--r--   0        0        0     2874 2024-03-19 22:27:57.186451 athina-1.2.7/athina/llms/question_answerer_bulk.py
--rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.2.7/athina/llms/question_answerer_cot.py
--rw-r--r--   0        0        0     6674 2024-03-20 01:02:59.337117 athina-1.2.7/athina/llms/question_answerer_with_retrieval.py
--rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.2.7/athina/llms/question_generator.py
--rw-r--r--   0        0        0      323 2024-03-27 06:24:44.858328 athina-1.2.7/athina/loaders/__init__.py
--rw-r--r--   0        0        0     2126 2024-03-19 22:27:57.186849 athina-1.2.7/athina/loaders/base_loader.py
--rw-r--r--   0        0        0     2173 2024-03-19 22:27:57.186916 athina-1.2.7/athina/loaders/conversation_loader.py
--rw-r--r--   0        0        0     4355 2024-03-20 04:43:24.983837 athina-1.2.7/athina/loaders/loader.py
--rw-r--r--   0        0        0     3501 2024-03-19 22:27:57.187089 athina-1.2.7/athina/loaders/response_loader.py
--rw-r--r--   0        0        0     2970 2024-03-19 22:27:57.187156 athina-1.2.7/athina/loaders/summary_loader.py
--rw-r--r--   0        0        0     2380 2024-03-27 06:24:44.858458 athina-1.2.7/athina/loaders/text_loader.py
--rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.2.7/athina/metrics/agreement_score.py
--rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.2.7/athina/metrics/contradiction_score.py
--rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.2.7/athina/metrics/groundedness.py
--rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.2.7/athina/metrics/hallucination_score.py
--rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.2.7/athina/metrics/metric.py
--rw-r--r--   0        0        0     3000 2024-03-20 00:48:19.997400 athina-1.2.7/athina/metrics/metric_type.py
--rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.2.7/athina/metrics/passed.py
--rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.2.7/athina/metrics/ragas_metric.py
--rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.2.7/athina/metrics/similarity_score.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.2.7/athina/runner/__init__.py
--rw-r--r--   0        0        0     5637 2024-03-19 22:27:57.188050 athina-1.2.7/athina/runner/run.py
--rw-r--r--   0        0        0     1262 2024-03-31 07:49:47.785926 athina-1.2.7/athina/scripts/guardrails.py
--rw-r--r--   0        0        0     9818 2024-03-30 01:03:46.851886 athina-1.2.7/athina/services/athina_api_service.py
--rw-r--r--   0        0        0      935 2024-03-31 07:50:04.639249 athina-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     9634 1970-01-01 00:00:00.000000 athina-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     8595 2024-03-19 22:27:57.176555 athina-1.2.8/README.md
+-rw-r--r--   0        0        0      169 2024-04-07 23:05:49.900916 athina-1.2.8/athina/__init__.py
+-rw-r--r--   0        0        0     2938 2024-03-19 22:27:57.176822 athina-1.2.8/athina/benchmark/eval_performance_calculator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.2.8/athina/cli/__init__.py
+-rw-r--r--   0        0        0     5390 2024-04-01 04:55:21.103552 athina-1.2.8/athina/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.2.8/athina/constants/__init__.py
+-rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.2.8/athina/constants/messages.py
+-rw-r--r--   0        0        0       72 2024-04-07 23:05:49.901344 athina-1.2.8/athina/datasets/__init__.py
+-rw-r--r--   0        0        0   218970 2024-03-19 22:27:57.177712 athina-1.2.8/athina/datasets/conversations.json
+-rw-r--r--   0        0        0     2971 2024-04-07 23:05:49.901583 athina-1.2.8/athina/datasets/dataset.py
+-rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.2.8/athina/datasets/summarization_sample.py
+-rw-r--r--   0        0        0     2675 2024-03-19 22:27:57.177915 athina-1.2.8/athina/datasets/yc_query_mini.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.2.8/athina/errors/__init__.py
+-rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.2.8/athina/errors/exceptions.py
+-rw-r--r--   0        0        0     4069 2024-04-02 05:23:54.521662 athina-1.2.8/athina/evals/__init__.py
+-rw-r--r--   0        0        0     7508 2024-03-27 06:24:44.855919 athina-1.2.8/athina/evals/base_evaluator.py
+-rw-r--r--   0        0        0     4253 2024-03-20 00:06:17.768963 athina-1.2.8/athina/evals/conversation/conversation_coherence/evaluator.py
+-rw-r--r--   0        0        0     1198 2024-03-19 22:27:57.178641 athina-1.2.8/athina/evals/conversation/conversation_coherence/prompt.py
+-rw-r--r--   0        0        0     4408 2024-03-19 22:27:57.178765 athina-1.2.8/athina/evals/conversation/conversation_resolution/evaluator.py
+-rw-r--r--   0        0        0     1104 2024-03-19 22:27:57.178845 athina-1.2.8/athina/evals/conversation/conversation_resolution/prompt.py
+-rw-r--r--   0        0        0     2470 2024-04-07 23:05:49.901880 athina-1.2.8/athina/evals/eval_type.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.2.8/athina/evals/function/__init__.py
+-rw-r--r--   0        0        0     3599 2024-03-27 06:24:44.856062 athina-1.2.8/athina/evals/function/function_evaluator.py
+-rw-r--r--   0        0        0    18806 2024-03-27 11:54:50.117642 athina-1.2.8/athina/evals/function/functions.py
+-rw-r--r--   0        0        0    10216 2024-03-27 09:12:43.212033 athina-1.2.8/athina/evals/function/wrapper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.2.8/athina/evals/grounded/__init__.py
+-rw-r--r--   0        0        0     3879 2024-03-20 16:40:39.753015 athina-1.2.8/athina/evals/grounded/grounded_evaluator.py
+-rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.2.8/athina/evals/grounded/similarity.py
+-rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.2.8/athina/evals/grounded/wrapper.py
+-rw-r--r--   0        0        0     2961 2024-04-02 05:23:01.185679 athina-1.2.8/athina/evals/guardrails/gibberish_text/evaluator.py
+-rw-r--r--   0        0        0     3727 2024-04-02 05:23:01.186096 athina-1.2.8/athina/evals/guardrails/sensitive_topics/evaluator.py
+-rw-r--r--   0        0        0     2885 2024-04-02 05:23:01.186344 athina-1.2.8/athina/evals/guardrails/sfw/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.2.8/athina/evals/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.2.8/athina/evals/llm/context_contains_enough_information/__init__.py
+-rw-r--r--   0        0        0     2671 2024-03-27 03:09:24.346838 athina-1.2.8/athina/evals/llm/context_contains_enough_information/evaluator.py
+-rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.2.8/athina/evals/llm/context_contains_enough_information/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.2.8/athina/evals/llm/custom_prompt/__init__.py
+-rw-r--r--   0        0        0     2362 2024-03-27 06:24:44.857102 athina-1.2.8/athina/evals/llm/custom_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.2.8/athina/evals/llm/does_response_answer_query/__init__.py
+-rw-r--r--   0        0        0     2632 2024-03-19 22:27:57.180901 athina-1.2.8/athina/evals/llm/does_response_answer_query/evaluator.py
+-rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.2.8/athina/evals/llm/does_response_answer_query/examples.py
+-rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.2.8/athina/evals/llm/example.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.2.8/athina/evals/llm/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2599 2024-03-19 22:27:57.181215 athina-1.2.8/athina/evals/llm/faithfulness/evaluator.py
+-rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.2.8/athina/evals/llm/faithfulness/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.2.8/athina/evals/llm/grading_criteria/__init__.py
+-rw-r--r--   0        0        0     2080 2024-04-01 04:53:12.884603 athina-1.2.8/athina/evals/llm/grading_criteria/evaluator.py
+-rw-r--r--   0        0        0     5821 2024-03-20 00:37:57.522908 athina-1.2.8/athina/evals/llm/groundedness/evaluator.py
+-rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.2.8/athina/evals/llm/groundedness/prompt.py
+-rw-r--r--   0        0        0     4982 2024-03-19 22:27:57.181767 athina-1.2.8/athina/evals/llm/llm_evaluator.py
+-rw-r--r--   0        0        0    10915 2024-03-20 02:27:27.436310 athina-1.2.8/athina/evals/llm/summary_accuracy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.2.8/athina/evals/ragas/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.2.8/athina/evals/ragas/answer_correctness/__init__.py
+-rw-r--r--   0        0        0     2383 2024-03-19 22:27:57.182414 athina-1.2.8/athina/evals/ragas/answer_correctness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.2.8/athina/evals/ragas/answer_relevancy/__init__.py
+-rw-r--r--   0        0        0     2441 2024-03-19 22:27:57.182610 athina-1.2.8/athina/evals/ragas/answer_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.2.8/athina/evals/ragas/answer_semantic_similarity/__init__.py
+-rw-r--r--   0        0        0     2440 2024-03-19 22:27:57.182849 athina-1.2.8/athina/evals/ragas/answer_semantic_similarity/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.2.8/athina/evals/ragas/coherence/__init__.py
+-rw-r--r--   0        0        0     2329 2024-03-19 22:27:57.183089 athina-1.2.8/athina/evals/ragas/coherence/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.2.8/athina/evals/ragas/conciseness/__init__.py
+-rw-r--r--   0        0        0     2364 2024-03-19 22:27:57.183287 athina-1.2.8/athina/evals/ragas/conciseness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.2.8/athina/evals/ragas/context_precision/__init__.py
+-rw-r--r--   0        0        0     2516 2024-03-19 22:27:57.183483 athina-1.2.8/athina/evals/ragas/context_precision/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.2.8/athina/evals/ragas/context_recall/__init__.py
+-rw-r--r--   0        0        0     2316 2024-03-19 22:27:57.183641 athina-1.2.8/athina/evals/ragas/context_recall/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.2.8/athina/evals/ragas/context_relevancy/__init__.py
+-rw-r--r--   0        0        0     2159 2024-03-19 22:27:57.183804 athina-1.2.8/athina/evals/ragas/context_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.2.8/athina/evals/ragas/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2370 2024-03-19 22:27:57.183971 athina-1.2.8/athina/evals/ragas/faithfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.2.8/athina/evals/ragas/harmfulness/__init__.py
+-rw-r--r--   0        0        0     2306 2024-03-19 22:27:57.184158 athina-1.2.8/athina/evals/ragas/harmfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.2.8/athina/evals/ragas/maliciousness/__init__.py
+-rw-r--r--   0        0        0     2268 2024-03-19 22:27:57.184345 athina-1.2.8/athina/evals/ragas/maliciousness/evaluator.py
+-rw-r--r--   0        0        0     3298 2024-03-19 22:27:57.184435 athina-1.2.8/athina/evals/ragas/ragas_evaluator.py
+-rw-r--r--   0        0        0     5154 2024-04-02 05:28:57.223435 athina-1.2.8/athina/evals/safety/content_moderation/evaluator.py
+-rw-r--r--   0        0        0     3299 2024-03-27 06:24:44.857314 athina-1.2.8/athina/evals/safety/pii_detection/evaluator.py
+-rw-r--r--   0        0        0     4370 2024-03-27 06:24:44.857479 athina-1.2.8/athina/evals/safety/prompt_injection/evaluator.py
+-rw-r--r--   0        0        0      106 2024-03-27 06:24:44.857663 athina-1.2.8/athina/guard/exception.py
+-rw-r--r--   0        0        0     1404 2024-04-01 04:53:12.917663 athina-1.2.8/athina/guard/guard.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.2.8/athina/helpers/__init__.py
+-rw-r--r--   0        0        0     4446 2024-03-19 22:27:57.184591 athina-1.2.8/athina/helpers/athina_logging_helper.py
+-rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.2.8/athina/helpers/config.py
+-rw-r--r--   0        0        0      122 2024-03-19 22:27:57.184730 athina-1.2.8/athina/helpers/constants.py
+-rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.2.8/athina/helpers/eval_helper.py
+-rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.2.8/athina/helpers/function_eval_util.py
+-rw-r--r--   0        0        0     4405 2024-04-01 04:53:12.911568 athina-1.2.8/athina/helpers/get_evaluator.py
+-rw-r--r--   0        0        0     1190 2024-03-19 22:27:57.185041 athina-1.2.8/athina/helpers/json.py
+-rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.2.8/athina/helpers/kwparser.py
+-rw-r--r--   0        0        0      894 2024-04-01 04:55:21.103741 athina-1.2.8/athina/helpers/loader_helper.py
+-rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.2.8/athina/helpers/logger.py
+-rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.2.8/athina/helpers/package_helper.py
+-rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.2.8/athina/helpers/run_helper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.2.8/athina/interfaces/__init__.py
+-rw-r--r--   0        0        0     3905 2024-03-19 22:27:57.185587 athina-1.2.8/athina/interfaces/athina.py
+-rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.2.8/athina/interfaces/data.py
+-rw-r--r--   0        0        0     1238 2024-03-27 06:24:44.857991 athina-1.2.8/athina/interfaces/model.py
+-rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.2.8/athina/interfaces/openai.py
+-rw-r--r--   0        0        0     2944 2024-03-27 06:24:44.858163 athina-1.2.8/athina/interfaces/result.py
+-rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.2.8/athina/keys/__init__.py
+-rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.2.8/athina/keys/athina_api_key.py
+-rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.2.8/athina/keys/openai_api_key.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.2.8/athina/llms/__init__.py
+-rw-r--r--   0        0        0     1398 2024-03-19 22:27:57.186244 athina-1.2.8/athina/llms/abstract_llm_service.py
+-rw-r--r--   0        0        0     3342 2024-03-19 22:27:57.186314 athina-1.2.8/athina/llms/openai_service.py
+-rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.2.8/athina/llms/question_answerer.py
+-rw-r--r--   0        0        0     2874 2024-03-19 22:27:57.186451 athina-1.2.8/athina/llms/question_answerer_bulk.py
+-rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.2.8/athina/llms/question_answerer_cot.py
+-rw-r--r--   0        0        0     6674 2024-03-20 01:02:59.337117 athina-1.2.8/athina/llms/question_answerer_with_retrieval.py
+-rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.2.8/athina/llms/question_generator.py
+-rw-r--r--   0        0        0      323 2024-03-27 06:24:44.858328 athina-1.2.8/athina/loaders/__init__.py
+-rw-r--r--   0        0        0     2126 2024-03-19 22:27:57.186849 athina-1.2.8/athina/loaders/base_loader.py
+-rw-r--r--   0        0        0     2173 2024-03-19 22:27:57.186916 athina-1.2.8/athina/loaders/conversation_loader.py
+-rw-r--r--   0        0        0     4355 2024-03-20 04:43:24.983837 athina-1.2.8/athina/loaders/loader.py
+-rw-r--r--   0        0        0     3501 2024-03-19 22:27:57.187089 athina-1.2.8/athina/loaders/response_loader.py
+-rw-r--r--   0        0        0     2970 2024-03-19 22:27:57.187156 athina-1.2.8/athina/loaders/summary_loader.py
+-rw-r--r--   0        0        0     2380 2024-03-27 06:24:44.858458 athina-1.2.8/athina/loaders/text_loader.py
+-rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.2.8/athina/metrics/agreement_score.py
+-rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.2.8/athina/metrics/contradiction_score.py
+-rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.2.8/athina/metrics/groundedness.py
+-rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.2.8/athina/metrics/hallucination_score.py
+-rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.2.8/athina/metrics/metric.py
+-rw-r--r--   0        0        0     3000 2024-03-20 00:48:19.997400 athina-1.2.8/athina/metrics/metric_type.py
+-rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.2.8/athina/metrics/passed.py
+-rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.2.8/athina/metrics/ragas_metric.py
+-rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.2.8/athina/metrics/similarity_score.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.2.8/athina/runner/__init__.py
+-rw-r--r--   0        0        0     5637 2024-03-19 22:27:57.188050 athina-1.2.8/athina/runner/run.py
+-rw-r--r--   0        0        0      341 2024-04-07 23:05:49.902009 athina-1.2.8/athina/runner/run_wrapper.py
+-rw-r--r--   0        0        0     1262 2024-04-02 05:23:08.938087 athina-1.2.8/athina/scripts/guardrails.py
+-rw-r--r--   0        0        0    12648 2024-04-07 23:05:49.902313 athina-1.2.8/athina/services/athina_api_service.py
+-rw-r--r--   0        0        0      935 2024-04-07 23:06:11.149532 athina-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     9634 1970-01-01 00:00:00.000000 athina-1.2.8/PKG-INFO
```

### Comparing `athina-1.2.7/README.md` & `athina-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/benchmark/eval_performance_calculator.py` & `athina-1.2.8/athina/benchmark/eval_performance_calculator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/cli/cli.py` & `athina-1.2.8/athina/cli/cli.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/constants/messages.py` & `athina-1.2.8/athina/constants/messages.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/datasets/conversations.json` & `athina-1.2.8/athina/datasets/conversations.json`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/datasets/summarization_sample.py` & `athina-1.2.8/athina/datasets/summarization_sample.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/datasets/yc_query_mini.py` & `athina-1.2.8/athina/datasets/yc_query_mini.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/errors/exceptions.py` & `athina-1.2.8/athina/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/__init__.py` & `athina-1.2.8/athina/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/base_evaluator.py` & `athina-1.2.8/athina/evals/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/conversation/conversation_coherence/evaluator.py` & `athina-1.2.8/athina/evals/conversation/conversation_coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/conversation/conversation_coherence/prompt.py` & `athina-1.2.8/athina/evals/conversation/conversation_coherence/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/conversation/conversation_resolution/evaluator.py` & `athina-1.2.8/athina/evals/conversation/conversation_resolution/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/conversation/conversation_resolution/prompt.py` & `athina-1.2.8/athina/evals/conversation/conversation_resolution/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/eval_type.py` & `athina-1.2.8/athina/evals/eval_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     LENGTH_LESS_THAN = "LengthLessThan"
     LENGTH_GREATER_THAN = "LengthGreaterThan"
     API_CALL = "ApiCall"
     SAFE_FOR_WORK_TEXT = "SafeForWorkText"
     NOT_GIBBERISH_TEXT = "NotGibberishText"
     CONTAINS_NO_SENSITIVE_TOPICS = "ContainsNoSensitiveTopics"
     OPENAI_CONTENT_MODERATION = "OpenAiContentModeration"
-
-
+    
 class GroundedEvalTypeId(Enum):
     ANSWER_SIMILARITY = "AnswerSimilarity"
     CONTEXT_SIMILARITY = "ContextSimilarity"
 
 def is_llm_eval(evaluator_type: str) -> bool:
     return any(evaluator_type == member.value for member in LlmEvalTypeId)
```

### Comparing `athina-1.2.7/athina/evals/function/function_evaluator.py` & `athina-1.2.8/athina/evals/function/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/function/functions.py` & `athina-1.2.8/athina/evals/function/functions.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/function/wrapper.py` & `athina-1.2.8/athina/evals/function/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/grounded/grounded_evaluator.py` & `athina-1.2.8/athina/evals/grounded/grounded_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/grounded/similarity.py` & `athina-1.2.8/athina/evals/grounded/similarity.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/grounded/wrapper.py` & `athina-1.2.8/athina/evals/grounded/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/guardrails/gibberish_text/evaluator.py` & `athina-1.2.8/athina/evals/guardrails/gibberish_text/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/guardrails/sensitive_topics/evaluator.py` & `athina-1.2.8/athina/evals/guardrails/sensitive_topics/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/guardrails/sfw/evaluator.py` & `athina-1.2.8/athina/evals/guardrails/sfw/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/context_contains_enough_information/evaluator.py` & `athina-1.2.8/athina/evals/llm/context_contains_enough_information/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/context_contains_enough_information/examples.py` & `athina-1.2.8/athina/evals/llm/context_contains_enough_information/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/custom_prompt/evaluator.py` & `athina-1.2.8/athina/evals/llm/custom_prompt/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/does_response_answer_query/evaluator.py` & `athina-1.2.8/athina/evals/llm/does_response_answer_query/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/does_response_answer_query/examples.py` & `athina-1.2.8/athina/evals/llm/does_response_answer_query/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/example.py` & `athina-1.2.8/athina/evals/llm/example.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/faithfulness/evaluator.py` & `athina-1.2.8/athina/evals/llm/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/faithfulness/examples.py` & `athina-1.2.8/athina/evals/llm/faithfulness/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/grading_criteria/evaluator.py` & `athina-1.2.8/athina/evals/llm/grading_criteria/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/groundedness/evaluator.py` & `athina-1.2.8/athina/evals/llm/groundedness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/groundedness/prompt.py` & `athina-1.2.8/athina/evals/llm/groundedness/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/llm_evaluator.py` & `athina-1.2.8/athina/evals/llm/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/llm/summary_accuracy/evaluator.py` & `athina-1.2.8/athina/evals/llm/summary_accuracy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/answer_correctness/evaluator.py` & `athina-1.2.8/athina/evals/ragas/answer_correctness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/answer_relevancy/evaluator.py` & `athina-1.2.8/athina/evals/ragas/answer_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/answer_semantic_similarity/evaluator.py` & `athina-1.2.8/athina/evals/ragas/answer_semantic_similarity/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/coherence/evaluator.py` & `athina-1.2.8/athina/evals/ragas/coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/conciseness/evaluator.py` & `athina-1.2.8/athina/evals/ragas/conciseness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/context_precision/evaluator.py` & `athina-1.2.8/athina/evals/ragas/context_precision/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/context_recall/evaluator.py` & `athina-1.2.8/athina/evals/ragas/context_recall/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/context_relevancy/evaluator.py` & `athina-1.2.8/athina/evals/ragas/context_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/faithfulness/evaluator.py` & `athina-1.2.8/athina/evals/ragas/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/harmfulness/evaluator.py` & `athina-1.2.8/athina/evals/ragas/harmfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/maliciousness/evaluator.py` & `athina-1.2.8/athina/evals/ragas/maliciousness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/ragas/ragas_evaluator.py` & `athina-1.2.8/athina/evals/ragas/ragas_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/safety/content_moderation/evaluator.py` & `athina-1.2.8/athina/evals/safety/content_moderation/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/safety/pii_detection/evaluator.py` & `athina-1.2.8/athina/evals/safety/pii_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/evals/safety/prompt_injection/evaluator.py` & `athina-1.2.8/athina/evals/safety/prompt_injection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/guard/guard.py` & `athina-1.2.8/athina/guard/guard.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/athina_logging_helper.py` & `athina-1.2.8/athina/helpers/athina_logging_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/config.py` & `athina-1.2.8/athina/helpers/config.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/function_eval_util.py` & `athina-1.2.8/athina/helpers/function_eval_util.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/get_evaluator.py` & `athina-1.2.8/athina/helpers/get_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/json.py` & `athina-1.2.8/athina/helpers/json.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/loader_helper.py` & `athina-1.2.8/athina/helpers/loader_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/logger.py` & `athina-1.2.8/athina/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/helpers/run_helper.py` & `athina-1.2.8/athina/helpers/run_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/interfaces/athina.py` & `athina-1.2.8/athina/interfaces/athina.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/interfaces/model.py` & `athina-1.2.8/athina/interfaces/model.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/interfaces/result.py` & `athina-1.2.8/athina/interfaces/result.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/llms/abstract_llm_service.py` & `athina-1.2.8/athina/llms/abstract_llm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/llms/openai_service.py` & `athina-1.2.8/athina/llms/openai_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/llms/question_answerer_bulk.py` & `athina-1.2.8/athina/llms/question_answerer_bulk.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/llms/question_answerer_cot.py` & `athina-1.2.8/athina/llms/question_answerer_cot.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/llms/question_answerer_with_retrieval.py` & `athina-1.2.8/athina/llms/question_answerer_with_retrieval.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/llms/question_generator.py` & `athina-1.2.8/athina/llms/question_generator.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/loaders/base_loader.py` & `athina-1.2.8/athina/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/loaders/conversation_loader.py` & `athina-1.2.8/athina/loaders/conversation_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/loaders/loader.py` & `athina-1.2.8/athina/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/loaders/response_loader.py` & `athina-1.2.8/athina/loaders/response_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/loaders/summary_loader.py` & `athina-1.2.8/athina/loaders/summary_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/loaders/text_loader.py` & `athina-1.2.8/athina/loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/metrics/agreement_score.py` & `athina-1.2.8/athina/metrics/agreement_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/metrics/contradiction_score.py` & `athina-1.2.8/athina/metrics/contradiction_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/metrics/groundedness.py` & `athina-1.2.8/athina/metrics/groundedness.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/metrics/hallucination_score.py` & `athina-1.2.8/athina/metrics/hallucination_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/metrics/metric_type.py` & `athina-1.2.8/athina/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/runner/run.py` & `athina-1.2.8/athina/runner/run.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/scripts/guardrails.py` & `athina-1.2.8/athina/scripts/guardrails.py`

 * *Files identical despite different names*

### Comparing `athina-1.2.7/athina/services/athina_api_service.py` & `athina-1.2.8/athina/services/athina_api_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pkg_resources
 import requests
+from dataclasses import asdict
 from retrying import retry
-from typing import List, Optional
+from typing import List, Optional, Dict
 from athina.errors.exceptions import NoAthinaApiKeyException
 from athina.interfaces.athina import (
     AthinaFilters,
     AthinaInference,
     AthinaEvalRequestCreateRequest,
     AthinaEvalResultCreateRequest,
     AthinaExperiment,
@@ -115,14 +116,79 @@
             return response.json()
         except Exception as e:
             print(
                 f"An error occurred while posting eval results",
                 str(e),
             )
             raise
+    
+    @staticmethod
+    def create_dataset(
+        dataset: Dict
+    ):
+        """
+        Creates a dataset by calling the Athina API
+        """
+        try:
+            endpoint = f"{API_BASE_URL}/api/v1/dataset"
+            response = requests.post(
+                endpoint,
+                headers=AthinaApiService._headers(),
+                json=dataset,
+            )
+            if response.status_code == 401:
+                response_json = response.json()
+                error_message = response_json.get('error', 'Unknown Error')
+                details_message = 'please check your athina api key and try again'
+                raise CustomException(error_message, details_message)
+            elif response.status_code != 200 and response.status_code != 201:
+                response_json = response.json()
+                error_message = response_json.get('error', 'Unknown Error')
+                details_message = response_json.get(
+                    'details', {}).get('message', 'No Details')
+                raise CustomException(error_message, details_message)
+            return response.json()['data']['dataset']
+        except Exception as e:
+            raise
+    
+    @staticmethod
+    def add_dataset_rows(dataset_id: str, rows: List[Dict]):
+        """
+        Adds rows to a dataset by calling the Athina API.
+
+        Parameters:
+        - dataset_id (str): The ID of the dataset to which rows are added.
+        - rows (List[Dict]): A list of rows to add to the dataset, where each row is represented as a dictionary.
+
+        Returns:
+        The API response data for the dataset after adding the rows.
+
+        Raises:
+        - CustomException: If the API call fails or returns an error.
+        """
+        try:
+            endpoint = f"{API_BASE_URL}/api/v1/dataset/{dataset_id}/add-rows"
+            response = requests.post(
+                endpoint,
+                headers=AthinaApiService._headers(),
+                json={"dataset_rows": rows},
+            )
+            if response.status_code == 401:
+                response_json = response.json()
+                error_message = response_json.get('error', 'Unknown Error')
+                details_message = 'please check your athina api key and try again'
+                raise CustomException(error_message, details_message)
+            elif response.status_code != 200 and response.status_code != 201:
+                response_json = response.json()
+                error_message = response_json.get('error', 'Unknown Error')
+                details_message = response_json.get('details', {}).get('message', 'No Details')
+                raise CustomException(error_message, details_message)
+            return response.json()['data']
+        except Exception as e:
+            raise
 
     @staticmethod
     def create_eval_request(
         athina_eval_request_create_request: AthinaEvalRequestCreateRequest,
     ):
         """
         Create eval request
```

### Comparing `athina-1.2.7/pyproject.toml` & `athina-1.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athina"
-version = "1.2.7"
+version = "1.2.8"
 description = "Python SDK to configure and run evaluations for your LLM-based application"
 authors = ["Shiv Sakhuja <shiv@athina.ai>", "Akshat Gupta <akshat@athina.ai>", "Vivek Aditya <vivek@athina.ai>", "Akhil Bisht <akhil@athina.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 retrying = "^1.3.4"
```

### Comparing `athina-1.2.7/PKG-INFO` & `athina-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athina
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python SDK to configure and run evaluations for your LLM-based application
 Author: Shiv Sakhuja
 Author-email: shiv@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

