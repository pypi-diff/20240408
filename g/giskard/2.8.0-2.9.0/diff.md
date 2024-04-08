# Comparing `tmp/giskard-2.8.0.tar.gz` & `tmp/giskard-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.8.0.tar", last modified: Mon Mar 25 13:05:32 2024, max compression
+gzip compressed data, was "giskard-2.9.0.tar", last modified: Mon Apr  8 14:07:36 2024, max compression
```

## Comparing `giskard-2.8.0.tar` & `giskard-2.9.0.tar`

### file list

```diff
@@ -1,337 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.577326 giskard-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-03-25 13:04:47.000000 giskard-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-03-25 13:05:32.577326 giskard-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-03-25 13:04:47.000000 giskard-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.537326 giskard-2.8.0/giskard/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.537326 giskard-2.8.0/giskard/client/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/client/dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/client/giskard_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/client/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/client/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/client/python_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    18884 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/commands/cli_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/commands/cli_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/dataset_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/kwargs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/savable.py
--rw-r--r--   0 runner    (1001) docker     (127)    36940 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/core/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/datasets/base/
--rw-r--r--   0 runner    (1001) docker     (127)    31942 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/datasets/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/datasets/metadata/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/demo/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/demo/llm_ipcc_climate_change.py
--rw-r--r--   0 runner    (1001) docker     (127)    60302 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/demo/titanic.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/demo/titanic_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.541326 giskard-2.8.0/giskard/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/exceptions/IllegalArgumentError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/exceptions/giskard_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/functions/slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/functions/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/avid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/mlflow/evaluation_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/mlflow/giskard_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/mlflow/giskard_evaluator_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/integrations/wandb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/integrations/wandb/wandb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/llm/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/client/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/client/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/llm/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/coherency.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/plausibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/evaluators/string_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.545326 giskard-2.8.0/giskard/llm/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/generators/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/generators/implausible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/generators/sycophancy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.549326 giskard-2.8.0/giskard/llm/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/loaders/prompt_injections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.549326 giskard-2.8.0/giskard/ml_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.549326 giskard-2.8.0/giskard/ml_worker/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/bridge/service_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.549326 giskard-2.8.0/giskard/ml_worker/stomp/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/stomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/stomp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/stomp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/stomp/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/stomp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.549326 giskard-2.8.0/giskard/ml_worker/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/utils/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.549326 giskard-2.8.0/giskard/ml_worker/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/websocket/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/websocket/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/ml_worker/websocket/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/_precooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/automodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/models/base/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26183 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/base/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/base/model_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/base/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/models/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/catboost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/model_explanation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/shap_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/path_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/push/
--rw-r--r--   0 runner    (1001) docker     (127)    18662 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/push/contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/push/perturbation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/push/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/push/push_test_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/push/push_test_catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/push/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/knowledge_base_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.553326 giskard-2.8.0/giskard/rag/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/metrics/correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/metrics/ragas_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.557326 giskard-2.8.0/giskard/rag/question_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/complex_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/conversational_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/distracting_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/double_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/question_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/simple_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/situational_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/question_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/testset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/rag/testset_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.557326 giskard-2.8.0/giskard/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/decorators_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/giskard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/slicing_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/transformation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.557326 giskard-2.8.0/giskard/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.557326 giskard-2.8.0/giskard/scanner/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.561326 giskard-2.8.0/giskard/scanner/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/common/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/common/loss_based_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.561326 giskard-2.8.0/giskard/scanner/correlation/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/correlation/spurious_correlation_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.561326 giskard-2.8.0/giskard/scanner/data_leakage/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/data_leakage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.561326 giskard-2.8.0/giskard/scanner/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_basic_sycophancy_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_chars_injection_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_faithfulness_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_harmful_content_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_implausible_output_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_information_disclosure_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_output_formatting_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_prompt_injection_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/llm/llm_stereotypes_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.561326 giskard-2.8.0/giskard/scanner/performance/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/performance/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.565326 giskard-2.8.0/giskard/scanner/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)   497222 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.565326 giskard-2.8.0/giskard/scanner/stochasticity/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/stochasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.533326 giskard-2.8.0/giskard/scanner/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.565326 giskard-2.8.0/giskard/scanner/templates/static/
--rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/templates/static/external.js
--rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/scanner/templates/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.565326 giskard-2.8.0/giskard/slicing/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/category_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/opt_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/slice_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/stop_words.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/text_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/tree_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/slicing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.565326 giskard-2.8.0/giskard/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/debug_slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/drift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/testing/tests/llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/llm/correctness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/llm/ground_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/llm/hallucination.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/llm/injections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/llm/output_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    33910 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/utils/stat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/testing/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/analytics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/environment_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/utils/worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/custom_jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.537326 giskard-2.8.0/giskard/visualization/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/visualization/templates/rag_report/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/rag_report/rag_report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.569326 giskard-2.8.0/giskard/visualization/templates/rag_report/static/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/rag_report/static/internal.js
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/rag_report/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.537326 giskard-2.8.0/giskard/visualization/templates/scan_report/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.573326 giskard-2.8.0/giskard/visualization/templates/scan_report/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/_code_snippet.html
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/_issue.html
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/_issues_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/_main_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/_tab_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/full.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.573326 giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/
--rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/external.js
--rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/internal.js
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.573326 giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/github.md
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/huggingface.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/summary.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.573326 giskard-2.8.0/giskard/visualization/templates/suite_results/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/suite_results/_suite_results_cards.html
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/suite_results/_suite_results_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/templates/suite_results/suite_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-25 13:04:47.000000 giskard-2.8.0/giskard/visualization/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.577326 giskard-2.8.0/giskard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-03-25 13:05:32.000000 giskard-2.8.0/giskard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-03-25 13:05:32.000000 giskard-2.8.0/giskard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:05:32.000000 giskard-2.8.0/giskard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-25 13:05:32.000000 giskard-2.8.0/giskard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-25 13:05:32.000000 giskard-2.8.0/giskard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 13:05:32.000000 giskard-2.8.0/giskard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-25 13:05:02.000000 giskard-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:05:32.577326 giskard-2.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:05:32.577326 giskard-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_artifact_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_data_processing_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_import_giskard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_metamorphic_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_metamorphic_invariance.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_programmatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_project_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_push.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_statistical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-03-25 13:04:47.000000 giskard-2.8.0/tests/test_worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.594685 giskard-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-08 14:07:05.000000 giskard-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-08 14:07:36.594685 giskard-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-08 14:07:05.000000 giskard-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19627 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/giskard_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/client/python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/commands/cli_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/commands/cli_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/dataset_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/kwargs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/savable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/core/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.554685 giskard-2.9.0/giskard/datasets/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    31942 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/datasets/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/llm_ipcc_climate_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60302 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/demo/titanic_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/exceptions/giskard_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/functions/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/functions/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/avid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/evaluation_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/integrations/wandb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/integrations/wandb/wandb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.558686 giskard-2.9.0/giskard/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/client/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/plausibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/evaluators/string_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/implausible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/generators/sycophancy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/llm/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/loaders/prompt_injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/bridge/service_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/stomp/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/stomp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.562686 giskard-2.9.0/giskard/ml_worker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/utils/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/ml_worker/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30302 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/ml_worker/websocket/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/_precooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/automodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/model_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/models/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/catboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/model_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/shap_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/path_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.566686 giskard-2.9.0/giskard/push/
+-rw-r--r--   0 runner    (1001) docker     (127)    18662 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/contribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/perturbation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/push/push_test_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/push_test_catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/push/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/knowledge_base_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/rag/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/metrics/ragas_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.570685 giskard-2.9.0/giskard/rag/question_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/complex_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/conversational_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/distracting_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/double_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/oos_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/question_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/simple_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/situational_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/question_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/testset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/rag/testset_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/decorators_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/giskard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/slicing_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/transformation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/common/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/common/loss_based_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/correlation/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/correlation/spurious_correlation_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.574685 giskard-2.9.0/giskard/scanner/data_leakage/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/data_leakage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_basic_sycophancy_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_chars_injection_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_faithfulness_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_harmful_content_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_implausible_output_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_information_disclosure_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_output_formatting_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_prompt_injection_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/llm/llm_stereotypes_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   497222 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/stochasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/stochasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.550686 giskard-2.9.0/giskard/scanner/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.578685 giskard-2.9.0/giskard/scanner/templates/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/scanner/templates/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/slicing/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/category_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/slice_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/stop_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/text_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/slicing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/debug_slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/drift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/tests/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/correctness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/hallucination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/llm/output_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33910 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.582685 giskard-2.9.0/giskard/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/utils/stat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/testing/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/analytics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/environment_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/utils/worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/custom_jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.550686 giskard-2.9.0/giskard/visualization/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/rag_report/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/rag_report/rag_report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/rag_report/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/rag_report/static/internal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/rag_report/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.550686 giskard-2.9.0/giskard/visualization/templates/scan_report/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/scan_report/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_code_snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_issue.html
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_issues_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_main_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/_tab_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/full.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/external.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65083 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/internal.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/github.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/huggingface.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/summary.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.586686 giskard-2.9.0/giskard/visualization/templates/suite_results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_cards.html
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/templates/suite_results/suite_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-08 14:07:05.000000 giskard-2.9.0/giskard/visualization/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.590685 giskard-2.9.0/giskard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 14:07:36.000000 giskard-2.9.0/giskard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-08 14:07:17.000000 giskard-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:07:36.594685 giskard-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:07:36.590685 giskard-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_artifact_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_import_giskard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_metamorphic_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15728 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_programmatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_project_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_statistical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-08 14:07:05.000000 giskard-2.9.0/tests/test_worker_pool.py
```

### Comparing `giskard-2.8.0/LICENSE` & `giskard-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/PKG-INFO` & `giskard-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.8.0
+Version: 2.9.0
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
@@ -65,15 +65,14 @@
 Requires-Dist: psutil>=5.4.6; extra == "hub"
 Requires-Dist: click>=7.0; extra == "hub"
 Requires-Dist: docker>=6.0.0; extra == "hub"
 Requires-Dist: shap>=0.41.0; extra == "hub"
 Requires-Dist: llvmlite>=0.40.0; extra == "hub"
 Requires-Dist: numba>=0.50.0; extra == "hub"
 Requires-Dist: lockfile>=0.12.2; extra == "hub"
-Requires-Dist: python-daemon<3,>=2.2.2; extra == "hub"
 Requires-Dist: pycryptodome>=3.6.1; extra == "hub"
 Requires-Dist: pyngrok>=6.0.0; extra == "hub"
 
 <p align="center">
   <img alt="giskardlogo" src="https://raw.githubusercontent.com/giskard-ai/giskard/main/readme/giskard_logo.png#gh-light-mode-only">
   <img alt="giskardlogo" src="https://raw.githubusercontent.com/giskard-ai/giskard/main/readme/giskard_logo_green.png#gh-dark-mode-only">
 </p>
```

### Comparing `giskard-2.8.0/README.md` & `giskard-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/__init__.py` & `giskard-2.9.0/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/cli.py` & `giskard-2.9.0/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/client/dtos.py` & `giskard-2.9.0/giskard/client/dtos.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/client/io_utils.py` & `giskard-2.9.0/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/client/project.py` & `giskard-2.9.0/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/commands/cli_hub.py` & `giskard-2.9.0/giskard/commands/cli_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,21 +26,20 @@
 giskard_settings_path = settings.home_dir / "server-settings.yml"
 IMAGE_NAME = "docker.io/giskardai/giskard"
 
 
 def create_docker_client() -> DockerClient:
     try:
         return docker.from_env()
-    except DockerException as e:
+    except DockerException:
         logger.exception(
             """Failed to connect to Docker. Giskard requires Docker to be installed. If Docker is installed, please run it. Otherwise, please install it.
 For an easy installation of Docker you can execute:
 - sudo curl -fsSL https://get.docker.com -o get-docker.sh
 - sudo sh get-docker.sh""",
-            e,
         )
         exit(1)
 
 
 @click.group("hub", help="Giskard UI management", context_settings={"show_default": True})
 def hub() -> None:
     """
```

### Comparing `giskard-2.8.0/giskard/commands/cli_worker.py` & `giskard-2.9.0/giskard/commands/cli_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from typing import Optional
 
 import functools
 import logging
 import os
 import platform
 import sys
+from pathlib import Path
 
 import click
 import lockfile
 import psutil
 from click import INT, STRING
 from lockfile.pidlockfile import PIDLockFile, read_pid_from_pidfile, remove_existing_pidfile
 from pydantic import AnyHttpUrl
 
 from giskard.cli_utils import (
     common_options,
     create_pid_file_path,
     follow_file,
     get_log_path,
     remove_stale_pid_file,
-    run_daemon,
     tail,
     validate_url,
 )
+from giskard.client.giskard_client import GiskardClient
 from giskard.path_utils import run_dir
 from giskard.settings import settings
 from giskard.utils.analytics_collector import analytics, anonymize
 
 logger = logging.getLogger(__name__)
 
 
@@ -43,245 +44,258 @@
         "-u",
         type=STRING,
         default="http://localhost:19000",
         help="Remote Giskard hub url",
         callback=validate_url,
     )
     @click.option(
+        "--name",
+        "worker_name",
+        default="external_worker",
+        help="Name/id of the worker starting",
+    )
+    @click.option(
+        "--key",
+        "-k",
+        "api_key",
+        envvar="GSK_API_KEY",
+        help="Giskard hub API key",
+    )
+    @click.option(
+        "--hf-token",
+        "hf_token",
+        envvar="GSK_HF_TOKEN",
+        help="Access token for Giskard hosted in a private Hugging Face Spaces",
+    )
+    @click.option(
         "--server",
         "-s",
         "is_server",
         is_flag=True,
         default=False,
-        help="Server mode. Used by Giskard embedded ML Worker",
+        help="Server mode. Used to control Giskard managed ML Worker",
+    )
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def start_options(func):
+    @click.option(
+        "--parallelism",
+        "nb_workers",
+        default=None,
+        help="Number of processes to use for parallelism (None for number of cpu)",
+    )
+    @click.option(
+        "--log-level",
+        "log_level",
+        default=logging.getLevelName(logging.INFO),
+        type=click.Choice(
+            [
+                logging.getLevelName(logging.DEBUG),
+                logging.getLevelName(logging.INFO),
+                logging.getLevelName(logging.WARNING),
+                logging.getLevelName(logging.ERROR),
+            ]
+        ),
+        help="Global log level",
     )
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
 
 
 @worker.command("start")
 @common_options
 @start_stop_options
-@click.option(
-    "--key",
-    "-k",
-    "api_key",
-    envvar="GSK_API_KEY",
-    help="Giskard hub API key",
-)
-@click.option(
-    "--daemon",
-    "-d",
-    "is_daemon",
-    is_flag=True,
-    default=False,
-    help="Should ML Worker be started as a Daemon in a background",
-)
-@click.option(
-    "--hf-token",
-    "hf_token",
-    envvar="GSK_HF_TOKEN",
-    help="Access token for Giskard hosted in a private Hugging Face Spaces",
-)
-@click.option(
-    "--parallelism",
-    "nb_workers",
-    default=None,
-    help="Number of processes to use for parallelism (None for number of cpu)",
-)
-@click.option(
-    "--log-level",
-    "log_level",
-    default=logging.getLevelName(logging.INFO),
-    type=click.Choice(
-        [
-            logging.getLevelName(logging.DEBUG),
-            logging.getLevelName(logging.INFO),
-            logging.getLevelName(logging.WARNING),
-            logging.getLevelName(logging.ERROR),
-        ]
-    ),
-    help="Global log level",
-)
-def start_command(url: AnyHttpUrl, is_server, api_key, is_daemon, hf_token, nb_workers, log_level):
+@start_options
+def start_command(url: AnyHttpUrl, is_server, api_key, hf_token, nb_workers, worker_name, log_level):
     """\b
     Start ML Worker.
 
     ML Worker can be started in 2 modes:
 
-    - server: used by default by an ML Worker shipped by Giskard. ML Worker acts as a server that Giskard connects to.
+    - server: Giskard starts an ML Worker managed by itself on the server.
 
     - client: ML Worker acts as a client and should connect to a running Giskard instance
         by specifying this instance's host and port.
     """
     analytics.track(
         "giskard-worker:start",
-        {"is_server": is_server, "url": anonymize(url), "is_daemon": is_daemon, "log_level": log_level},
+        {"url": anonymize(url), "log_level": log_level},
     )
 
     logging.root.setLevel(logging.getLevelName(log_level))
 
-    api_key = initialize_api_key(api_key, is_server)
-    hf_token = initialize_hf_token(hf_token, is_server)
-    _start_command(is_server, url, api_key, is_daemon, hf_token, int(nb_workers) if nb_workers is not None else None)
+    api_key = initialize_api_key(api_key)
+    hf_token = initialize_hf_token(hf_token)
+    if is_server:
+        # Create a Giskard client and request to start an ML worker with given name
+        _start_server_command(worker_name, url, api_key, hf_token)
+    else:
+        _start_command(worker_name, url, api_key, hf_token, int(nb_workers) if nb_workers is not None else None)
 
 
-def initialize_api_key(api_key, is_server):
-    if is_server:
-        return None
+def initialize_api_key(api_key):
     if not api_key:
         api_key = click.prompt("Enter Giskard hub API key", type=str)
     if "GSK_API_KEY" in os.environ:
         # delete API key environment variable so that it doesn't get leaked when the test code is executed
         del os.environ["GSK_API_KEY"]
     return api_key
 
 
-def initialize_hf_token(hf_token, is_server):
-    if is_server:
-        return None
+def initialize_hf_token(hf_token):
     # HF token is not mandantory unless connection error
     if "GSK_HF_TOKEN" in os.environ:
         # delete HF token environment variable so that it doesn't get leaked when the test code is executed
         del os.environ["GSK_HF_TOKEN"]
     return hf_token
 
 
-def _start_command(is_server, url: AnyHttpUrl, api_key, is_daemon, hf_token=None, nb_workers=None):
+def _start_server_command(worker_name, url: AnyHttpUrl, api_key, hf_token=None):
+    client: GiskardClient = GiskardClient(str(url), api_key, hf_token)
+    client.start_managed_worker(worker_name)
+
+
+def _start_command(worker_name, url: AnyHttpUrl, api_key, hf_token=None, nb_workers=None):
     from giskard.ml_worker.ml_worker import MLWorker
 
     os.environ["TQDM_DISABLE"] = "1"
-    start_msg = "Starting ML Worker"
-    start_msg += " server" if is_server else " client"
-    if is_daemon:
-        start_msg += " daemon"
-    logger.info(start_msg)
-    logger.info(f"Python: {sys.executable} ({platform.python_version()})")
-    logger.info(f"Giskard Home: {settings.home_dir}")
-    pid_file_path = create_pid_file_path(is_server, url)
+    logger.info("Starting ML Worker %s", worker_name)
+    logger.info("Python: %s (%s)", sys.executable, platform.python_version())
+    logger.info("Giskard Home: %s", settings.home_dir)
+
+    pid_file_path = create_pid_file_path(worker_name, url)
+    logger.info("Creating pid file : %s", pid_file_path)
+
     pid_file = PIDLockFile(pid_file_path)
     remove_stale_pid_file(pid_file)
 
     ml_worker: Optional[MLWorker] = None
     try:
         pid_file.acquire()
-        if is_daemon:
-            # Releasing the lock because it will be re-acquired by a daemon process
-            pid_file.release()
-            # If on windows, throw error and exit
-            if sys.platform == "win32":
-                logger.error("Daemon mode is not supported on Windows.")
-                return
-
-            run_daemon(is_server, url, api_key, hf_token)
+        if settings.force_asyncio_event_loop or sys.platform == "win32":
+            logger.info("Using asyncio to run jobs")
+            from asyncio import run
         else:
-            if settings.force_asyncio_event_loop or sys.platform == "win32":
-                logger.info("Using asyncio to run jobs")
-                from asyncio import run
-            else:
-                logger.info("Using uvloop to run jobs")
-                from uvloop import run
-            run(_start_worker(is_server, url, api_key, hf_token, nb_workers))
+            logger.info("Using uvloop to run jobs")
+            from uvloop import run
+        run(_start_worker(worker_name, url, api_key, hf_token, nb_workers))
     except KeyboardInterrupt:
         logger.info("Exiting")
         if ml_worker:
             ml_worker.stop()
     except lockfile.AlreadyLocked:
         existing_pid = read_pid_from_pidfile(pid_file_path)
+        # TODO(Bazire) : update the info to include worker_name
         logger.warning(
-            f"Another ML Worker {_ml_worker_description(is_server, url)} "
+            f"Another ML Worker {_ml_worker_description(worker_name, url)} "
             f"is already running with PID: {existing_pid}. "
             "Not starting a new one. "
             'To stop a running worker for this instance execute: "giskard worker stop" or '
             '"giskard worker stop -a" to stop all running workers'
         )
     finally:
         if pid_file.i_am_locking():
             pid_file.release()
 
 
-def _ml_worker_description(is_server, url):
-    return "server" if is_server else f"client for {url}"
+def _ml_worker_description(worker_name: str, url: AnyHttpUrl):
+    return f"named {worker_name} for {url}"
 
 
-async def _start_worker(is_server, url, api_key, hf_token, nb_workers):
+async def _start_worker(worker_name, url, api_key, hf_token, nb_workers):
     from giskard.ml_worker.ml_worker import MLWorker
 
-    ml_worker = MLWorker(is_server, url, api_key, hf_token)
-    await ml_worker.start(nb_workers, restart=True)
+    ml_worker = MLWorker(worker_name, url, api_key, hf_token)
+    await ml_worker.start(restart=True, nb_workers=nb_workers)
+
+
+def _stop_server_command(worker_name, url: AnyHttpUrl, api_key, hf_token=None):
+    client: GiskardClient = GiskardClient(str(url), api_key, hf_token)
+    return client.stop_managed_worker(worker_name)
 
 
 @worker.command("stop", help="Stop running ML Workers")
 @common_options
 @start_stop_options
 @click.option("--all", "-a", "stop_all", is_flag=True, default=False, help="Stop all running ML Workers")
-def stop_command(is_server, url, stop_all):
+def stop_command(worker_name, stop_all, is_server, url: AnyHttpUrl, api_key, hf_token=None):
     import re
 
     analytics.track(
         "giskard-worker:stop",
-        {"is_server": is_server, "url": anonymize(url), "stop_all": stop_all},
+        {"url": anonymize(url), "stop_all": stop_all},
     )
     if stop_all:
-        for pid_fname in os.listdir(run_dir):
-            if not re.match(r"^ml-worker-.*\.pid$", pid_fname):
+        if is_server:
+            logger.fatal("Stopping all workers on the server is not yet supported.")
+            return
+        for pid_path in run_dir.iterdir():
+            if not re.match(r"^ml-worker-.*\.pid$", pid_path.name):
                 continue
-            _stop_pid_fname(pid_fname)
+            _stop_pid_fname(pid_path)
     else:
-        _find_and_stop(is_server, url)
+        if is_server:
+            api_key = initialize_api_key(api_key)
+            hf_token = initialize_hf_token(hf_token)
+            _stop_server_command(worker_name, url, api_key, hf_token)
+        else:
+            _find_and_stop(worker_name, url)
+
+
+def _restart_server_command(worker_name, url: AnyHttpUrl, api_key, hf_token=None):
+    client: GiskardClient = GiskardClient(url, api_key, hf_token)
+    client.stop_managed_worker(worker_name)
+    client.start_managed_worker(worker_name)
 
 
 @worker.command("restart", help="Restart ML Worker")
 @common_options
 @start_stop_options
-@click.option("--api-key", "-k", "api_key", help="Giskard hub API key")
-@click.option(
-    "--hf-token",
-    "hf_token",
-    help="Access token for Giskard hosted in a private Hugging Face Spaces",
-)
-def restart_command(is_server, url, api_key, hf_token):
+@start_options
+def restart_command(url: AnyHttpUrl, is_server, api_key, hf_token, nb_workers, worker_name, log_level):
     analytics.track(
         "giskard-worker:restart",
-        {"is_server": is_server, "url": anonymize(url)},
+        {"url": anonymize(url)},
     )
-    api_key = initialize_api_key(api_key, is_server)
+    logging.root.setLevel(logging.getLevelName(log_level))
 
-    _find_and_stop(is_server, url)
-    _start_command(is_server, url, api_key, is_daemon=True, hf_token=hf_token)
+    if is_server:
+        _restart_server_command(worker_name, url, api_key, hf_token)
+        return
 
+    # Restart the local worker
+    _find_and_stop(worker_name, url)
+    _start_command(worker_name, url, api_key, hf_token=hf_token, nb_workers=nb_workers)
 
-def _stop_pid_fname(pid_fname):
-    pid_file_path = str(run_dir / pid_fname)
-    remove_stale_pid_file(PIDLockFile(pid_file_path))
-    pid = read_pid_from_pidfile(pid_file_path)
-    if pid:
-        worker_process = psutil.Process(pid)
-        worker_process.terminate()
-        logger.info(f"Stopped ML Worker Daemon by PID: {pid}")
-    remove_existing_pidfile(pid_file_path)
 
-
-def _find_and_stop(is_server, url):
-    pid_file_path = str(create_pid_file_path(is_server, url))
-    remove_stale_pid_file(PIDLockFile(pid_file_path))
-    pid = read_pid_from_pidfile(pid_file_path)
-    logger.info("Stopping ML Worker Daemon")
+def _stop_pid_fname(pid_path: Path):
+    pid_file_path = str(pid_path)
+    remove_stale_pid_file(PIDLockFile(pid_path))
+    pid = read_pid_from_pidfile(pid_path)
     if pid:
         worker_process = psutil.Process(pid)
         worker_process.terminate()
-        logger.info(f"Stopped ML Worker {_ml_worker_description(is_server, url)}")
+        logger.info("Stopped ML Worker by PID: %s", pid)
     else:
-        logger.info(f"ML Worker {_ml_worker_description(is_server, url)} is not running")
+        logger.info("ML Worker (PID %s, path %s) is not running", pid, pid_path)
     remove_existing_pidfile(pid_file_path)
 
 
+def _find_and_stop(worker_name: str, url: AnyHttpUrl):
+    return _stop_pid_fname(create_pid_file_path(worker_name, url))
+
+
 @worker.command("logs")
 @common_options
 @click.option(
     "--lines",
     "-n",
     type=INT,
     default=10,
```

### Comparing `giskard-2.8.0/giskard/core/core.py` & `giskard-2.9.0/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/core/dataset_validation.py` & `giskard-2.9.0/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/core/errors.py` & `giskard-2.9.0/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/core/kwargs_utils.py` & `giskard-2.9.0/giskard/core/kwargs_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/core/model_validation.py` & `giskard-2.9.0/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/core/savable.py` & `giskard-2.9.0/giskard/core/savable.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,39 +49,25 @@
         return SavableMeta
 
     @classmethod
     def _get_name(cls) -> str:
         return f"{cls.__class__.__name__.lower()}s"
 
     @classmethod
-    def _get_meta_endpoint(cls, uuid: str, project_key: Optional[str]) -> str:
-        if project_key is None:
-            return posixpath.join(cls._get_name(), uuid)
-        else:
-            return posixpath.join("project", project_key, cls._get_name(), uuid)
+    def _get_meta_endpoint(cls, uuid: str, project_key: str) -> str:
+        return posixpath.join("project", project_key, cls._get_name(), uuid)
 
     def _save_meta_locally(self, local_dir):
         with open(Path(local_dir) / "meta.yaml", "w") as f:
             yaml.dump(self.meta, f)
 
-    @classmethod
-    def _load_meta_locally(cls, local_dir, uuid: str) -> Optional[SMT]:
-        file = Path(local_dir) / "meta.yaml"
-        if not file.exists():
-            return None
-
-        with open(file, "r") as f:
-            # PyYAML prohibits the arbitary execution so our class cannot be loaded safely,
-            # see: https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation
-            return yaml.load(f, Loader=yaml.UnsafeLoader)
-
     def upload(
         self,
         client: GiskardClient,
-        project_key: Optional[str] = None,
+        project_key: str,
         uploaded_dependencies: Optional[Set["Artifact"]] = None,
     ) -> str:
         """
         Uploads the slicing function and its metadata to the Giskard hub.
 
         Args:
             client (GiskardClient): The Giskard client instance used for communication with the hub.
@@ -110,40 +96,35 @@
 
         client.log_artifacts(local_dir, posixpath.join(self._get_name(), self.meta.uuid))
         self.meta = client.save_meta(self._get_meta_endpoint(self.meta.uuid, project_key), self.meta)
 
         return self.meta.uuid
 
     @classmethod
-    def download(cls, uuid: str, client: Optional[GiskardClient], project_key: Optional[str]) -> "Artifact":
+    def download(cls, uuid: str, client: GiskardClient, project_key: str) -> "Artifact":
         """
         Downloads the artifact from the Giskard hub or retrieves it from the local cache.
 
         Args:
             uuid (str): The UUID of the artifact to download.
-            client (Optional[GiskardClient]): The Giskard client instance used for communication with the hub. If None,
-                the artifact will be retrieved from the local cache if available. Defaults to None.
+            client (GiskardClient): The Giskard client instance used for communication with the hub.
             project_key (Optional[str]): The project key where the artifact is located. If None, the artifact will be
                 retrieved from the global scope. Defaults to None.
 
         Returns:
             Artifact: The downloaded artifact.
 
         Raises:
             AssertionError: If the artifact metadata cannot be retrieved.
             AssertionError: If the artifact is not found in the cache and the Giskard client is None.
         """
         name = cls._get_name()
 
         local_dir = settings.home_dir / settings.cache_dir / name / uuid
-
-        if client is None:
-            meta = cls._load_meta_locally(local_dir, uuid)
-        else:
-            meta = client.load_meta(cls._get_meta_endpoint(uuid, project_key), cls._get_meta_class())
+        meta = client.load_meta(cls._get_meta_endpoint(uuid, project_key), cls._get_meta_class())
 
         assert meta is not None, "Could not retrieve test meta"
 
         # check cache first
         data = cls.load(local_dir, uuid, meta)
 
         if data is None:
```

### Comparing `giskard-2.8.0/giskard/core/suite.py` & `giskard-2.9.0/giskard/core/suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
             if pname not in self.giskard_test.meta.args
         ]
         if len(kwargs_params) > 0:
             params["kwargs"] = TestInputDTO(name="kwargs", value="\n".join(kwargs_params), type="Kwargs")
 
         return SuiteTestDTO(
             id=self.suite_test_id,
-            testUuid=self.giskard_test.upload(client),
+            testUuid=self.giskard_test.upload(client, project_key),
             functionInputs=params,
             displayName=self.display_name,
         )
 
 
 def single_binary_result(test_results: List):
     return all(res.passed for res in test_results)
@@ -931,15 +931,15 @@
         suite_dto: SuiteInfo = client.get_suite(client.get_project(project_key).project_id, suite_id)
 
         suite = Suite(name=suite_dto.name)
         suite.id = suite_id
         suite.project_key = project_key
 
         for test_json in suite_dto.tests:
-            test = GiskardTest.download(test_json.testUuid, client, None)
+            test = GiskardTest.download(test_json.testUuid, client, project_key)
             test_arguments = parse_function_arguments(client, project_key, test_json.functionInputs.values())
             suite.add_test(test(**test_arguments), suite_test_id=test_json.id)
 
         return suite
 
 
 def contains_tag(func: TestFunctionMeta, tag: str):
```

### Comparing `giskard-2.8.0/giskard/core/test_result.py` & `giskard-2.9.0/giskard/core/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/core/validation.py` & `giskard-2.9.0/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/datasets/__init__.py` & `giskard-2.9.0/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/datasets/base/__init__.py` & `giskard-2.9.0/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/datasets/metadata/indexing.py` & `giskard-2.9.0/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/datasets/metadata/registry.py` & `giskard-2.9.0/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.9.0/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/demo/__init__.py` & `giskard-2.9.0/giskard/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/demo/linear_regression.py` & `giskard-2.9.0/giskard/demo/linear_regression.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/demo/llm_ipcc_climate_change.py` & `giskard-2.9.0/giskard/demo/llm_ipcc_climate_change.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/demo/titanic.csv` & `giskard-2.9.0/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/demo/titanic_classification.py` & `giskard-2.9.0/giskard/demo/titanic_classification.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/exceptions/giskard_exception.py` & `giskard-2.9.0/giskard/exceptions/giskard_exception.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/functions/slicing.py` & `giskard-2.9.0/giskard/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/functions/transformation.py` & `giskard-2.9.0/giskard/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/integrations/avid.py` & `giskard-2.9.0/giskard/integrations/avid.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/integrations/mlflow/evaluation_artifacts.py` & `giskard-2.9.0/giskard/integrations/mlflow/evaluation_artifacts.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/integrations/mlflow/giskard_evaluator.py` & `giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/integrations/mlflow/giskard_evaluator_utils.py` & `giskard-2.9.0/giskard/integrations/mlflow/giskard_evaluator_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/integrations/wandb/wandb_utils.py` & `giskard-2.9.0/giskard/integrations/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/client/__init__.py` & `giskard-2.9.0/giskard/llm/client/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/client/base.py` & `giskard-2.9.0/giskard/llm/client/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/client/logger.py` & `giskard-2.9.0/giskard/llm/client/logger.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/client/openai.py` & `giskard-2.9.0/giskard/llm/client/openai.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/evaluators/base.py` & `giskard-2.9.0/giskard/llm/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/evaluators/coherency.py` & `giskard-2.9.0/giskard/llm/evaluators/coherency.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/evaluators/correctness.py` & `giskard-2.9.0/giskard/llm/evaluators/correctness.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/evaluators/plausibility.py` & `giskard-2.9.0/giskard/llm/evaluators/plausibility.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/evaluators/requirements.py` & `giskard-2.9.0/giskard/llm/evaluators/requirements.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/evaluators/string_matcher.py` & `giskard-2.9.0/giskard/llm/evaluators/string_matcher.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/generators/adversarial.py` & `giskard-2.9.0/giskard/llm/generators/adversarial.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/generators/base.py` & `giskard-2.9.0/giskard/llm/generators/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/generators/implausible.py` & `giskard-2.9.0/giskard/llm/generators/implausible.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/generators/sycophancy.py` & `giskard-2.9.0/giskard/llm/generators/sycophancy.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/loaders/prompt_injections.py` & `giskard-2.9.0/giskard/llm/loaders/prompt_injections.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/testcase.py` & `giskard-2.9.0/giskard/llm/testcase.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/llm/utils.py` & `giskard-2.9.0/giskard/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.9.0/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/ml_worker.py` & `giskard-2.9.0/giskard/ml_worker/ml_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Optional, Union
 
 import logging
 import math
-import secrets
 from uuid import UUID
 
 from pydantic import AnyHttpUrl
 from websockets.client import WebSocketClientProtocol
 
 from giskard.cli_utils import validate_url
 from giskard.core.validation import ConfiguredBaseModel
@@ -19,50 +18,39 @@
 from giskard.registry.registry import load_plugins
 from giskard.settings import settings
 from giskard.utils import shutdown_pool, start_pool
 from giskard.utils.analytics_collector import analytics
 
 LOGGER = logging.getLogger(__name__)
 
-INTERNAL_WORKER_ID = "INTERNAL"
-EXTERNAL_WORKER_ID = "EXTERNAL"
 MAX_STOMP_ML_WORKER_REPLY_SIZE = 1500
 
 
 class FragmentedPayload(ConfiguredBaseModel):
     id: UUID
     action: str
     payload: str
     f_index: int
     f_count: int
 
 
 class MLWorker(StompWSClient):
     def __init__(
         self,
-        is_server=False,
+        worker_name,
         backend_url: AnyHttpUrl = None,
         api_key: Optional[str] = None,
         hf_token: Optional[str] = None,
     ) -> None:
         headers = {}
         connect_headers = {"COOKIE": f"spaces-jwt={hf_token};"} if hf_token is not None else None
 
-        if is_server:
-            # Retrieve from settings for internal ML Worker
-            self._worker_type = INTERNAL_WORKER_ID
-            backend_url = validate_url(None, None, f"http://{settings.host}:{settings.ws_port}{settings.ws_path}")
-            internal_ml_worker_token = secrets.token_hex(16)
-            headers["token"] = internal_ml_worker_token
-            with open(f"{settings.home_dir / 'run' / 'internal-ml-worker'}", "w") as f:
-                f.write(internal_ml_worker_token)
-        else:
-            # External ML worker: URL should be provided
-            self._worker_type = EXTERNAL_WORKER_ID
-            headers["api-key"] = api_key
+        # External ML worker: URL should be provided
+        self._worker_name = worker_name
+        headers["api-key"] = api_key
 
         # Use the URL path component provided by settings
         if backend_url.port is not None:
             port = backend_url.port
         elif backend_url.scheme == "https":
             port = 443
         else:
@@ -71,40 +59,34 @@
         ws_str = f"{'ws' if backend_url.scheme == 'http' else 'wss'}://{backend_url.host}:{port}{settings.ws_path}"
 
         super().__init__(ws_str, headers, connect_headers)
         self._backend_url = f"{backend_url.scheme}://{backend_url.host}:{port}"
         self._ws_max_reply_payload_size = MAX_STOMP_ML_WORKER_REPLY_SIZE
         self._api_key = api_key
         self._hf_token = hf_token
-        self._worker_info = MLWorkerInfo(id=self._worker_type, is_remote=self.is_remote_worker())
-
-    def is_remote_worker(self):
-        return self._worker_type is not INTERNAL_WORKER_ID
+        # TODO(Bazire): Cleanup this
+        self._worker_info = MLWorkerInfo(id=self._worker_name)
 
     async def config_handler(self, frame: Frame) -> List[Frame]:
         payload = ConfigPayload.parse_raw(frame.body)
         self._ws_max_reply_payload_size = max(MAX_STOMP_ML_WORKER_REPLY_SIZE, payload.value)
         LOGGER.info("MAX_STOMP_ML_WORKER_REPLY_SIZE set to %s", self._ws_max_reply_payload_size)
 
         return []
 
     async def action_handler(self, frame: Frame) -> List[Frame]:
         data = ActionPayload.parse_raw(frame.body)
-        logging.info(f"Running job {data.id}: {data.action.name}")
+        logging.info("Running job %s: %s", data.id, data.action.name)
 
         # Dispatch the action
-        client_params = (
-            {
-                "url": self._backend_url,
-                "key": self._api_key,
-                "hf_token": self._hf_token,
-            }
-            if self.is_remote_worker()
-            else None
-        )
+        client_params = {
+            "url": self._backend_url,
+            "key": self._api_key,
+            "hf_token": self._hf_token,
+        }
         if data.action == MLWorkerAction.stopWorker:
             LOGGER.info("Marking worker as stopping...")
             self.stop()
 
         payload: Optional[Union[str, Frame]] = await WEBSOCKET_ACTORS[data.action.name](
             data, client_params, self._worker_info
         )
@@ -128,15 +110,15 @@
                 "reply_len": len(payload),
             },
         )
 
         return [
             StompFrame.SEND.build_frame(
                 headers={
-                    HeaderType.DESTINATION: f"/app/ml-worker/{self._worker_type}/reply",
+                    HeaderType.DESTINATION: f"/app/ml-worker/{self._worker_name}/reply",
                 },
                 body=FragmentedPayload(
                     id=data.id,
                     action=data.action.name,
                     payload=fragment_message(payload, frag_i, self._ws_max_reply_payload_size),
                     f_index=frag_i,
                     f_count=frag_count,
@@ -145,27 +127,31 @@
             for frag_i in range(frag_count)
         ]
 
     async def setup(self, websocket: WebSocketClientProtocol):
         LOGGER.info("Subscribing for action...")
         await self.subscribe(
             websocket,
-            f"/ml-worker/{self._worker_type}/action",
-            f"ws-worker-{self._worker_type}-action",
+            f"/ml-worker/{self._worker_name}/action",
+            f"ws-worker-{self._worker_name}-action",
             self.action_handler,
         )
         LOGGER.info("Subscribing for config...")
         await self.subscribe(
             websocket,
-            f"/ml-worker/{self._worker_type}/config",
-            f"ws-worker-{self._worker_type}-config",
+            f"/ml-worker/{self._worker_name}/config",
+            f"ws-worker-{self._worker_name}-config",
             self.config_handler,
         )
 
-    async def start(self, nb_workers: Optional[int] = None, restart: bool = False):
+    async def start(
+        self,
+        restart: bool = False,
+        nb_workers: Optional[int] = None,
+    ):
         load_plugins()
         start_pool(nb_workers)
         await super().start(restart=restart)
 
     def stop(self):
         super().stop()
         shutdown_pool()
```

### Comparing `giskard-2.8.0/giskard/ml_worker/stomp/client.py` & `giskard-2.9.0/giskard/ml_worker/stomp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
                 for frame in frames:
                     await self._sender_queue.put(frame)
             # Handle disconnect frame
             if self._is_stopping:
                 await self._sender_queue.put(StompFrame.DISCONNECT.build_frame({}))
 
     async def _process_frame(self, frame: Frame) -> List[Frame]:
+        if HeaderType.SUBSCRIPTION not in frame.headers:
+            raise StompClientError(f"Missing subscription header, got frame ({frame})")
         subscription = frame.headers[HeaderType.SUBSCRIPTION]
         if subscription not in self._subscriptions:
             raise StompClientError(f"Unknown subscription {subscription}")
         result = await self._subscriptions[subscription](frame)
         return result
 
     @abstractmethod
```

### Comparing `giskard-2.8.0/giskard/ml_worker/stomp/constants.py` & `giskard-2.9.0/giskard/ml_worker/stomp/constants.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/stomp/parsing.py` & `giskard-2.9.0/giskard/ml_worker/stomp/parsing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/stomp/utils.py` & `giskard-2.9.0/giskard/ml_worker/stomp/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/utils/cache.py` & `giskard-2.9.0/giskard/ml_worker/utils/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/utils/network.py` & `giskard-2.9.0/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/ml_worker/websocket/__init__.py` & `giskard-2.9.0/giskard/ml_worker/websocket/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,16 +225,15 @@
 
 
 class GetInfo(WorkerReply):
     platform: Platform
     interpreter: str
     interpreterVersion: str
     installedPackages: Dict[str, str]
-    mlWorkerId: str
-    isRemote: bool
+    kernelName: str
     pid: int
     processStartTime: int
     giskardClientVersion: str
 
 
 class GetInfoParam(ConfiguredBaseModel):
     list_packages: bool
```

### Comparing `giskard-2.8.0/giskard/ml_worker/websocket/action.py` & `giskard-2.9.0/giskard/ml_worker/websocket/action.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     getCatalog = "getCatalog"
     generateQueryBasedSlicingFunction = "generateQueryBasedSlicingFunction"
     getPush = "getPush"
     createSubDataset = "createSubDataset"
     abort = "abort"
     getLogs = "getLogs"
     createDataset = "createDataset"
+    devJob = "devTask"
 
     @classmethod
     def __get_validators__(cls):
         if IS_PYDANTIC_V2:
             yield cls.validate
         else:
             yield cls.validate_v1
```

### Comparing `giskard-2.8.0/giskard/ml_worker/websocket/listener.py` & `giskard-2.9.0/giskard/ml_worker/websocket/listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from giskard.ml_worker.websocket import CallToActionKind, GetInfoParam, PushKind
 from giskard.ml_worker.websocket.action import ActionPayload, MLWorkerAction
 from giskard.ml_worker.websocket.utils import (
     do_create_dataset,
     do_create_sub_dataset,
     do_run_adhoc_test,
     function_argument_to_ws,
-    log_artifact_local,
     map_dataset_process_function_meta_ws,
     map_function_meta_ws,
     map_result_to_single_test_result_ws,
     parse_action_param,
     parse_function_arguments,
 )
 from giskard.models.base import BaseModel
@@ -61,15 +60,14 @@
 logger = logging.getLogger(__name__)
 MAX_STOMP_ML_WORKER_REPLY_SIZE = 1500
 
 
 @dataclass
 class MLWorkerInfo:
     id: str
-    is_remote: bool
 
 
 def websocket_log_actor(ml_worker: MLWorkerInfo, req: ActionPayload, *args, **kwargs):
     logger.info("ML Worker %s performing %s params: %s", {ml_worker.id}, {req.action}, {req.param})
 
 
 WEBSOCKET_ACTORS = dict((action.name, websocket_log_actor) for action in MLWorkerAction)
@@ -131,20 +129,20 @@
 
 def parse_and_execute(
     *,
     callback: Callable,
     action: MLWorkerAction,
     params,
     ml_worker: MLWorkerInfo,
-    client_params: Optional[Dict[str, str]],
+    client_params: Dict[str, str],
 ) -> websocket.WorkerReply:
     action_params = parse_action_param(action, params)
     return callback(
         ml_worker=ml_worker,
-        client=GiskardClient(**client_params) if client_params is not None else None,
+        client=GiskardClient(**client_params),
         action=action.name,
         params=action_params,
     )
 
 
 async def dispatch_action(
     callback: Callable,
@@ -244,16 +242,15 @@
         ),
         giskardClientVersion=giskard.__version__,
         pid=os.getpid(),
         processStartTime=int(current_process.create_time()),
         interpreter=sys.executable,
         interpreterVersion=platform.python_version(),
         installedPackages=installed_packages,
-        mlWorkerId=ml_worker.id,
-        isRemote=ml_worker.is_remote,
+        kernelName=ml_worker.id,
     )
 
 
 @websocket_actor(MLWorkerAction.stopWorker, execute_in_pool=False)
 def on_ml_worker_stop_worker(*args, **kwargs) -> None:
     # Stop the server properly after sending disconnect
     logger.info("Stopping ML Worker")
@@ -312,15 +309,15 @@
         )
     else:
         calculated = pd.concat([preds_serie], axis=1)
     return results, calculated
 
 
 @websocket_actor(MLWorkerAction.runModel)
-def run_model(client: Optional[GiskardClient], params: websocket.RunModelParam, *args, **kwargs) -> websocket.Empty:
+def run_model(client: GiskardClient, params: websocket.RunModelParam, *args, **kwargs) -> websocket.Empty:
     try:
         model = BaseModel.download(client, params.model.project_key, params.model.id)
         dataset = Dataset.download(
             client,
             params.dataset.project_key,
             params.dataset.id,
             sample=params.dataset.sample,
@@ -347,43 +344,31 @@
     else:
         results, calculated = run_other_model(dataset, prediction_results, model.is_text_generation)
 
     with tempfile.TemporaryDirectory(prefix="giskard-") as f:
         tmp_dir = Path(f)
         predictions_csv = get_file_name("predictions", "csv", params.dataset.sample)
         results.to_csv(index=False, path_or_buf=tmp_dir / predictions_csv)
-        if client:
-            client.log_artifact(
-                tmp_dir / predictions_csv,
-                f"models/inspections/{params.inspectionId}",
-            )
-        else:
-            log_artifact_local(
-                tmp_dir / predictions_csv,
-                f"models/inspections/{params.inspectionId}",
-            )
+        client.log_artifact(
+            tmp_dir / predictions_csv,
+            f"models/inspections/{params.inspectionId}",
+        )
 
         calculated_csv = get_file_name("calculated", "csv", params.dataset.sample)
         calculated.to_csv(index=False, path_or_buf=tmp_dir / calculated_csv)
-        if client:
-            client.log_artifact(
-                tmp_dir / calculated_csv,
-                f"models/inspections/{params.inspectionId}",
-            )
-        else:
-            log_artifact_local(
-                tmp_dir / calculated_csv,
-                f"models/inspections/{params.inspectionId}",
-            )
+        client.log_artifact(
+            tmp_dir / calculated_csv,
+            f"models/inspections/{params.inspectionId}",
+        )
     return websocket.Empty()
 
 
 @websocket_actor(MLWorkerAction.runModelForDataFrame)
 def run_model_for_data_frame(
-    client: Optional[GiskardClient], params: websocket.RunModelForDataFrameParam, *args, **kwargs
+    client: GiskardClient, params: websocket.RunModelForDataFrameParam, *args, **kwargs
 ) -> websocket.RunModelForDataFrame:
     model = BaseModel.download(client, params.model.project_key, params.model.id)
     df = pd.DataFrame.from_records([r.columns for r in params.dataframe.rows])
     ds = Dataset(
         model.prepare_dataframe(df, column_dtypes=params.column_dtypes),
         target=None,
         column_types=params.column_types,
@@ -405,27 +390,36 @@
         return websocket.RunModelForDataFrame(
             prediction=list(predictions.prediction.astype(str)),
             raw_prediction=list(predictions.prediction),
         )
 
 
 @websocket_actor(MLWorkerAction.explain)
-def explain_ws(client: Optional[GiskardClient], params: websocket.ExplainParam, *args, **kwargs) -> websocket.Explain:
+def explain_ws(client: GiskardClient, params: websocket.ExplainParam, *args, **kwargs) -> websocket.Explain:
     model = BaseModel.download(client, params.model.project_key, params.model.id)
     dataset = Dataset.download(client, params.dataset.project_key, params.dataset.id, params.dataset.sample)
     explanations = explain(model, dataset, params.columns)
 
     return websocket.Explain(
         explanations={str(k): websocket.Explanation(per_feature=v) for k, v in explanations["explanations"].items()}
     )
 
 
+@websocket_actor(MLWorkerAction.devJob)
+def dev_job(client: GiskardClient, params: websocket.Empty, *args, **kwargs) -> websocket.Empty:
+    for i in range(10000):
+        time.sleep(1)
+        logger.info(f"Sleeping for 100ms {i}")
+
+    return websocket.Empty()
+
+
 @websocket_actor(MLWorkerAction.explainText)
 def explain_text_ws(
-    client: Optional[GiskardClient], params: websocket.ExplainTextParam, *args, **kwargs
+    client: GiskardClient, params: websocket.ExplainTextParam, *args, **kwargs
 ) -> websocket.ExplainText:
     model = BaseModel.download(client, params.model.project_key, params.model.id)
     text_column = params.feature_name
 
     if params.column_types[text_column] != "text":
         raise ValueError(f"Column {text_column} is not of type text")
     text_document = params.columns[text_column]
@@ -458,15 +452,15 @@
         slices=map_dataset_process_function_meta_ws("SLICE"),
         transformations=map_dataset_process_function_meta_ws("TRANSFORMATION"),
     )
 
 
 @websocket_actor(MLWorkerAction.datasetProcessing)
 def dataset_processing(
-    client: Optional[GiskardClient], params: websocket.DatasetProcessingParam, *args, **kwargs
+    client: GiskardClient, params: websocket.DatasetProcessingParam, *args, **kwargs
 ) -> websocket.DatasetProcessing:
     dataset = Dataset.download(client, params.dataset.project_key, params.dataset.id, params.dataset.sample)
 
     for function in params.functions:
         arguments = parse_function_arguments(client, function.arguments)
         if function.slicingFunction:
             dataset.add_slicing_function(
@@ -498,15 +492,15 @@
             for row in modified_rows.iterrows()
         ],
     )
 
 
 @websocket_actor(MLWorkerAction.runAdHocTest)
 def run_ad_hoc_test(
-    client: Optional[GiskardClient], params: websocket.RunAdHocTestParam, *args, **kwargs
+    client: GiskardClient, params: websocket.RunAdHocTestParam, *args, **kwargs
 ) -> websocket.RunAdHocTest:
     test: GiskardTest = GiskardTest.download(params.testUuid, client, params.projectKey)
 
     arguments = parse_function_arguments(client, params.arguments)
     if params.debug:
         arguments.update({"debug": True})
     if "kwargs" in arguments:
@@ -523,17 +517,15 @@
                 result=map_result_to_single_test_result_ws(test_result, datasets, client, params.projectKey),
             )
         ]
     )
 
 
 @websocket_actor(MLWorkerAction.runTestSuite)
-def run_test_suite(
-    client: Optional[GiskardClient], params: websocket.TestSuiteParam, *args, **kwargs
-) -> websocket.TestSuite:
+def run_test_suite(client: GiskardClient, params: websocket.TestSuiteParam, *args, **kwargs) -> websocket.TestSuite:
     loaded_artifacts = defaultdict(dict)
 
     try:
         tests = [
             {
                 "test": GiskardTest.download(t.testUuid, client, params.projectKey),
                 "arguments": parse_function_arguments(client, t.arguments, loaded_artifacts),
@@ -592,15 +584,15 @@
 
 @websocket_actor(MLWorkerAction.echo, execute_in_pool=False)
 def echo(params: websocket.EchoMsg, *args, **kwargs) -> websocket.EchoResponse:
     return websocket.EchoResponse(msg=params.msg, job_ids=list_pool_job_ids())
 
 
 def handle_cta(
-    client: Optional[GiskardClient],
+    client: GiskardClient,
     params: websocket.GetPushParam,
     push: Optional[Push],
     push_kind: PushKind,
     cta_kind: CallToActionKind,
 ):
     if push is None:
         push = get_push_objects(client, params)
@@ -633,17 +625,15 @@
 
     if object_uuid:
         logger.info("Uploaded object for CTA with uuid: %s", object_uuid)
         return websocket.PushAction(object_uuid=object_uuid, arguments=function_argument_to_ws(object_params))
 
 
 @websocket_actor(MLWorkerAction.getPush, timeout=30, ignore_timeout=True)
-def get_push(
-    client: Optional[GiskardClient], params: websocket.GetPushParam, *args, **kwargs
-) -> websocket.GetPushResponse:
+def get_push(client: GiskardClient, params: websocket.GetPushParam, *args, **kwargs) -> websocket.GetPushResponse:
     # Save cta_kind and push_kind and remove it from params
     cta_kind = params.cta_kind
     push_kind = params.push_kind
     params.cta_kind = None
     params.push_kind = None
 
     kinds = (
@@ -688,15 +678,15 @@
     )
 
 
 def push_to_ws(push: Push):
     return push.to_ws() if push is not None else None
 
 
-def get_push_objects(client: Optional[GiskardClient], params: websocket.GetPushParam):
+def get_push_objects(client: GiskardClient, params: websocket.GetPushParam):
     try:
         model = BaseModel.download(client, params.model.project_key, params.model.id)
         dataset = Dataset.download(client, params.dataset.project_key, params.dataset.id)
 
         df = pd.DataFrame.from_records([r.columns for r in params.dataframe.rows])
         if params.column_dtypes:
             for missing_column in [
@@ -733,15 +723,15 @@
     }
 
     return push_functions[params.push_kind](model, dataset, df)
 
 
 @websocket_actor(MLWorkerAction.createSubDataset)
 def create_sub_dataset(
-    client: Optional[GiskardClient], params: websocket.CreateSubDatasetParam, *arg, **kwargs
+    client: GiskardClient, params: websocket.CreateSubDatasetParam, *arg, **kwargs
 ) -> websocket.CreateSubDataset:
     datasets = {
         dateset_id: Dataset.download(
             client=client, project_key=params.projectKey, dataset_id=dateset_id, sample=params.sample
         )
         for dateset_id in params.copiedRows.keys()
     }
@@ -749,15 +739,15 @@
     sub_dataset = do_create_sub_dataset(datasets, params.name, params.copiedRows)
 
     return websocket.CreateSubDataset(datasetUuid=sub_dataset.upload(client=client, project_key=params.projectKey))
 
 
 @websocket_actor(MLWorkerAction.createDataset)
 def create_dataset(
-    client: Optional[GiskardClient], params: websocket.CreateDatasetParam, *arg, **kwargs
+    client: GiskardClient, params: websocket.CreateDatasetParam, *arg, **kwargs
 ) -> websocket.CreateSubDataset:
     dataset = do_create_dataset(params.name, params.headers, params.rows)
 
     return websocket.CreateSubDataset(datasetUuid=dataset.upload(client=client, project_key=params.projectKey))
 
 
 def tail_file(file_path: Path, n_lines: int):
@@ -778,8 +768,14 @@
 
 
 @websocket_actor(MLWorkerAction.getLogs, execute_in_pool=False)
 def get_logs(params: websocket.GetLogsParams, *arg, **kwargs):
     job_id = params.job_id
     assert job_id, "Job ID is required"
 
-    return websocket.GetLogs(logs=tail_file(job_logs_path(job_id), params.nb_last_lines))
+    try:
+        logs = tail_file(job_logs_path(job_id), params.nb_last_lines)
+    except Exception as e:
+        logger.exception(f"Failed to get logs for job {job_id}: {e}")
+        logs = str(e)
+
+    return websocket.GetLogs(logs=logs)
```

### Comparing `giskard-2.8.0/giskard/ml_worker/websocket/utils.py` & `giskard-2.9.0/giskard/ml_worker/websocket/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import logging
-import os
-import shutil
 import uuid
 from collections import defaultdict
 
 import pandas as pd
-from mlflow.store.artifact.artifact_repo import verify_artifact_path
 
 from giskard.client.giskard_client import GiskardClient
 from giskard.core.suite import DatasetInput, ModelInput, SuiteInput
 from giskard.core.test_result import TestMessageLevel, TestResult
 from giskard.datasets.base import Dataset
 from giskard.exceptions.IllegalArgumentError import IllegalArgumentError
 from giskard.ml_worker import websocket
@@ -30,15 +27,14 @@
     RunAdHocTestParam,
     RunModelForDataFrameParam,
     RunModelParam,
     TestSuiteParam,
 )
 from giskard.ml_worker.websocket.action import MLWorkerAction
 from giskard.models.base import BaseModel
-from giskard.path_utils import artifacts_dir
 from giskard.registry.registry import tests_registry
 from giskard.registry.slicing_function import SlicingFunction
 from giskard.registry.transformation_function import TransformationFunction
 
 logger = logging.getLogger(__name__)
 
 
@@ -122,29 +118,14 @@
             debugDescription=test.debug_description,
         )
         for test in tests_registry.get_all().values()
         if test.type == callable_type and "giskard" in test.tags
     }
 
 
-def log_artifact_local(local_file, artifact_path=None):
-    # Log artifact locally from an internal worker
-    verify_artifact_path(artifact_path)
-
-    file_name = os.path.basename(local_file)
-
-    if artifact_path:
-        artifact_file = artifacts_dir / artifact_path / file_name
-    else:
-        artifact_file = artifacts_dir / file_name
-    artifact_file.parent.mkdir(parents=True, exist_ok=True)
-
-    shutil.copy(local_file, artifact_file)
-
-
 def map_dataset_process_function_meta_ws(callable_type):
     return {
         test.uuid: websocket.DatasetProcessFunctionMeta(
             uuid=test.uuid,
             name=test.name,
             displayName=test.display_name,
             module=test.module,
@@ -178,15 +159,15 @@
     if uuid not in loaded_artifacts[type]:
         loaded_artifacts[type][uuid] = load_fn()
 
     return loaded_artifacts[type][uuid]
 
 
 def parse_function_arguments(
-    client: Optional[GiskardClient],
+    client: GiskardClient,
     request_arguments: List[websocket.FuncArgument],
     loaded_artifacts: Optional[Dict[str, Dict[str, Any]]] = None,
 ):
     if loaded_artifacts is None:
         loaded_artifacts = defaultdict(dict)
 
     arguments = dict()
@@ -241,15 +222,15 @@
             raise IllegalArgumentError("Unknown argument type")
     return arguments
 
 
 def map_result_to_single_test_result_ws(
     result,
     datasets: Dict[uuid.UUID, Dataset],
-    client: Optional[GiskardClient] = None,
+    client: GiskardClient,
     project_key: Optional[str] = None,
 ) -> websocket.SingleTestResult:
     if isinstance(result, TestResult):
         result.output_ds = result.output_ds or []
 
         if result.output_df is not None:
             _upload_generated_output_df(client, datasets, project_key, result)
@@ -298,17 +279,14 @@
         """
     Your using legacy test debugging though `output_df`. This feature will be removed in the future.
     Please migrate to `output_ds`.
     """
     )
 
     if result.output_df.original_id not in datasets.keys():
-        if not client:
-            raise RuntimeError("Legacy test debugging using `output_df` is not supported internal ML worker")
-
         if not project_key:
             raise ValueError("Unable to upload debug dataset due to missing `project_key`")
 
         result.output_df.upload(client, project_key)
 
     datasets[result.output_df.original_id] = result.output_df
     result.output_ds.append(result.output_df)
```

### Comparing `giskard-2.8.0/giskard/models/__init__.py` & `giskard-2.9.0/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/_precooked.py` & `giskard-2.9.0/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/automodel.py` & `giskard-2.9.0/giskard/models/automodel.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/base/model.py` & `giskard-2.9.0/giskard/models/base/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 
             if client is not None:
                 client.log_artifacts(f, posixpath.join("models", str(self.id)))
                 client.save_model_meta(project_key, self.id, self.meta, platform.python_version(), get_size(f))
         return str(self.id)
 
     @classmethod
-    def download(cls, client: Optional[GiskardClient], project_key, model_id, *_args, **_kwargs):
+    def download(cls, client: GiskardClient, project_key, model_id, *_args, **_kwargs):
         """
         Downloads the specified model from the Giskard hub and loads it into memory.
 
         Args:
             client (GiskardClient): The client instance that will connect to the Giskard hub.
             project_key (str): The key for the project that the model belongs to.
             model_id (str): The ID of the model to download.
@@ -476,37 +476,32 @@
         Returns:
             An instance of the class calling the method, with the specified model loaded into memory.
 
         Raises:
             AssertionError: If the local directory where the model should be saved does not exist.
         """
         local_dir = settings.home_dir / settings.cache_dir / "models" / model_id
-        if client is None:
-            # internal worker case, no token based http client [deprecated, to be removed]
-            assert local_dir.exists(), f"Cannot find existing model {project_key}.{model_id} in {local_dir}"
-            meta_response, meta = cls.read_meta_from_local_dir(local_dir)
-        else:
-            client.load_artifact(local_dir, posixpath.join("models", model_id))
-            meta_response: ModelMetaInfo = client.load_model_meta(project_key, model_id)
-            # internal worker case, no token based http client
-            if not local_dir.exists():
-                raise RuntimeError(f"Cannot find existing model {project_key}.{model_id} in {local_dir}")
-            with (Path(local_dir) / META_FILENAME).open(encoding="utf-8") as f:
-                file_meta = yaml.load(f, Loader=yaml.Loader)
-                classification_labels = cls.cast_labels(meta_response)
-                meta = ModelMeta(
-                    name=meta_response.name,
-                    description=meta_response.description,
-                    model_type=SupportedModelTypes[meta_response.modelType],
-                    feature_names=meta_response.featureNames,
-                    classification_labels=classification_labels,
-                    classification_threshold=meta_response.threshold,
-                    loader_module=file_meta["loader_module"],
-                    loader_class=file_meta["loader_class"],
-                )
+        client.load_artifact(local_dir, posixpath.join("models", model_id))
+        meta_response: ModelMetaInfo = client.load_model_meta(project_key, model_id)
+        # internal worker case, no token based http client
+        if not local_dir.exists():
+            raise RuntimeError(f"Cannot find existing model {project_key}.{model_id} in {local_dir}")
+        with (Path(local_dir) / META_FILENAME).open(encoding="utf-8") as f:
+            file_meta = yaml.load(f, Loader=yaml.Loader)
+            classification_labels = cls.cast_labels(meta_response)
+            meta = ModelMeta(
+                name=meta_response.name,
+                description=meta_response.description,
+                model_type=SupportedModelTypes[meta_response.modelType],
+                feature_names=meta_response.featureNames,
+                classification_labels=classification_labels,
+                classification_threshold=meta_response.threshold,
+                loader_module=file_meta["loader_module"],
+                loader_class=file_meta["loader_class"],
+            )
 
         model_py_ver = (
             tuple(meta_response.languageVersion.split(".")) if "PYTHON" == meta_response.language.upper() else None
         )
 
         clazz = cls.determine_model_class(meta, local_dir, model_py_ver=model_py_ver)
```

### Comparing `giskard-2.8.0/giskard/models/base/model_prediction.py` & `giskard-2.9.0/giskard/models/base/model_prediction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/base/serialization.py` & `giskard-2.9.0/giskard/models/base/serialization.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/base/wrapper.py` & `giskard-2.9.0/giskard/models/base/wrapper.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/cache/__init__.py` & `giskard-2.9.0/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/cache/cache.py` & `giskard-2.9.0/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/catboost.py` & `giskard-2.9.0/giskard/models/catboost.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/function.py` & `giskard-2.9.0/giskard/models/function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/huggingface.py` & `giskard-2.9.0/giskard/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/langchain.py` & `giskard-2.9.0/giskard/models/langchain.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/model_explanation.py` & `giskard-2.9.0/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/pytorch.py` & `giskard-2.9.0/giskard/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/shap_result.py` & `giskard-2.9.0/giskard/models/shap_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/sklearn.py` & `giskard-2.9.0/giskard/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/tensorflow.py` & `giskard-2.9.0/giskard/models/tensorflow.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/models/utils.py` & `giskard-2.9.0/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/push/__init__.py` & `giskard-2.9.0/giskard/push/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/push/contribution.py` & `giskard-2.9.0/giskard/push/contribution.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/push/perturbation.py` & `giskard-2.9.0/giskard/push/perturbation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/push/prediction.py` & `giskard-2.9.0/giskard/push/prediction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/push/push_test_catalog/catalog.py` & `giskard-2.9.0/giskard/push/push_test_catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/push/utils.py` & `giskard-2.9.0/giskard/push/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/evaluate.py` & `giskard-2.9.0/giskard/rag/evaluate.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/knowledge_base.py` & `giskard-2.9.0/giskard/rag/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/knowledge_base_plots.py` & `giskard-2.9.0/giskard/rag/knowledge_base_plots.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/metrics/base.py` & `giskard-2.9.0/giskard/rag/metrics/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/metrics/correctness.py` & `giskard-2.9.0/giskard/rag/metrics/correctness.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/metrics/ragas_metrics.py` & `giskard-2.9.0/giskard/rag/metrics/ragas_metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/__init__.py` & `giskard-2.9.0/giskard/rag/question_generators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .base import QuestionGenerator
 from .complex_questions import ComplexQuestionsGenerator, complex_questions
 from .conversational_questions import ConversationalQuestionsGenerator, conversational_questions
 from .distracting_questions import DistractingQuestionsGenerator, distracting_questions
 from .double_questions import DoubleQuestionsGenerator, double_questions
+from .oos_questions import OutOfScopeGenerator, oos_questions
 from .question_types import COMPONENT_DESCRIPTIONS, QUESTION_ATTRIBUTION, RAGComponents
 from .simple_questions import SimpleQuestionsGenerator, simple_questions
 from .situational_questions import SituationalQuestionsGenerator, situational_questions
 
 __all__ = [
     "RAGComponents",
     "QuestionGenerator",
@@ -14,14 +15,16 @@
     "COMPONENT_DESCRIPTIONS",
     "SimpleQuestionsGenerator",
     "ComplexQuestionsGenerator",
     "ConversationalQuestionsGenerator",
     "DistractingQuestionsGenerator",
     "SituationalQuestionsGenerator",
     "DoubleQuestionsGenerator",
+    "OutOfScopeGenerator",
     "simple_questions",
     "complex_questions",
     "conversational_questions",
     "distracting_questions",
     "situational_questions",
     "double_questions",
+    "oos_questions",
 ]
```

### Comparing `giskard-2.8.0/giskard/rag/question_generators/base.py` & `giskard-2.9.0/giskard/rag/question_generators/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/complex_questions.py` & `giskard-2.9.0/giskard/rag/question_generators/complex_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/conversational_questions.py` & `giskard-2.9.0/giskard/rag/question_generators/conversational_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/distracting_questions.py` & `giskard-2.9.0/giskard/rag/question_generators/distracting_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/double_questions.py` & `giskard-2.9.0/giskard/rag/question_generators/double_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/prompt.py` & `giskard-2.9.0/giskard/rag/question_generators/prompt.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/question_types.py` & `giskard-2.9.0/giskard/rag/question_generators/question_types.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/simple_questions.py` & `giskard-2.9.0/giskard/rag/question_generators/simple_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/question_generators/situational_questions.py` & `giskard-2.9.0/giskard/rag/question_generators/situational_questions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/recommendation.py` & `giskard-2.9.0/giskard/rag/recommendation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/report.py` & `giskard-2.9.0/giskard/rag/report.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/testset.py` & `giskard-2.9.0/giskard/rag/testset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/rag/testset_generation.py` & `giskard-2.9.0/giskard/rag/testset_generation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/decorators.py` & `giskard-2.9.0/giskard/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/decorators_utils.py` & `giskard-2.9.0/giskard/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/giskard_test.py` & `giskard-2.9.0/giskard/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/registry.py` & `giskard-2.9.0/giskard/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/slicing_function.py` & `giskard-2.9.0/giskard/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/transformation_function.py` & `giskard-2.9.0/giskard/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/registry/utils.py` & `giskard-2.9.0/giskard/registry/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/__init__.py` & `giskard-2.9.0/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.9.0/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.9.0/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/common/examples.py` & `giskard-2.9.0/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/common/loss_based_detector.py` & `giskard-2.9.0/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/common/utils.py` & `giskard-2.9.0/giskard/scanner/common/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/correlation/spurious_correlation_detector.py` & `giskard-2.9.0/giskard/scanner/correlation/spurious_correlation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.9.0/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/decorators.py` & `giskard-2.9.0/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/issues.py` & `giskard-2.9.0/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/__init__.py` & `giskard-2.9.0/giskard/scanner/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/base.py` & `giskard-2.9.0/giskard/scanner/llm/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_basic_sycophancy_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_basic_sycophancy_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_chars_injection_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_chars_injection_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_faithfulness_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_faithfulness_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_harmful_content_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_harmful_content_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_implausible_output_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_implausible_output_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_information_disclosure_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_information_disclosure_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_output_formatting_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_output_formatting_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_prompt_injection_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_prompt_injection_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/llm/llm_stereotypes_detector.py` & `giskard-2.9.0/giskard/scanner/llm/llm_stereotypes_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/performance/__init__.py` & `giskard-2.9.0/giskard/scanner/performance/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/performance/metrics.py` & `giskard-2.9.0/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.9.0/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/registry.py` & `giskard-2.9.0/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/report.py` & `giskard-2.9.0/giskard/scanner/report.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/__init__.py` & `giskard-2.9.0/giskard/scanner/robustness/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/base_detector.py` & `giskard-2.9.0/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/entity_swap.py` & `giskard-2.9.0/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.9.0/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/nationalities.json` & `giskard-2.9.0/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.9.0/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/robustness/text_transformations.py` & `giskard-2.9.0/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/scanner.py` & `giskard-2.9.0/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.9.0/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/templates/static/external.js` & `giskard-2.9.0/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/templates/static/internal.js` & `giskard-2.9.0/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/scanner/templates/static/style.css` & `giskard-2.9.0/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/settings.py` & `giskard-2.9.0/giskard/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         current = os.path.expandvars(current)
     return current
 
 
 class Settings(BaseModel):
     home: str = "~/giskard-home"
     ws_port: int = 9000
-    ws_path: str = "/ml-worker"
+    ws_path: str = "/websocket"
     host: str = "localhost"
     max_workers: int = 10
     loglevel: str = "INFO"
     cache_dir: str = "cache"
     disable_analytics: bool = False
     force_asyncio_event_loop: bool = False
     min_workers: int = 2
```

### Comparing `giskard-2.8.0/giskard/slicing/base.py` & `giskard-2.9.0/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/bruteforce_slicer.py` & `giskard-2.9.0/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/category_slicer.py` & `giskard-2.9.0/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/multiscale_slicer.py` & `giskard-2.9.0/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/opt_slicer.py` & `giskard-2.9.0/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/slice.py` & `giskard-2.9.0/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/slice_finder.py` & `giskard-2.9.0/giskard/slicing/slice_finder.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/stop_words.py` & `giskard-2.9.0/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/text_slicer.py` & `giskard-2.9.0/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/tree_slicer.py` & `giskard-2.9.0/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/slicing/utils.py` & `giskard-2.9.0/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/__init__.py` & `giskard-2.9.0/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/calibration.py` & `giskard-2.9.0/giskard/testing/tests/calibration.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/data_quality.py` & `giskard-2.9.0/giskard/testing/tests/data_quality.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/debug_slicing_functions.py` & `giskard-2.9.0/giskard/testing/tests/debug_slicing_functions.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/drift.py` & `giskard-2.9.0/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/llm/__init__.py` & `giskard-2.9.0/giskard/testing/tests/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/llm/correctness.py` & `giskard-2.9.0/giskard/testing/tests/llm/correctness.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/llm/ground_truth.py` & `giskard-2.9.0/giskard/testing/tests/llm/ground_truth.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/llm/hallucination.py` & `giskard-2.9.0/giskard/testing/tests/llm/hallucination.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/llm/injections.py` & `giskard-2.9.0/giskard/testing/tests/llm/injections.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/llm/output_requirements.py` & `giskard-2.9.0/giskard/testing/tests/llm/output_requirements.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/metamorphic.py` & `giskard-2.9.0/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/performance.py` & `giskard-2.9.0/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/tests/statistic.py` & `giskard-2.9.0/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/utils/stat_utils.py` & `giskard-2.9.0/giskard/testing/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/testing/utils/utils.py` & `giskard-2.9.0/giskard/testing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/__init__.py` & `giskard-2.9.0/giskard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/analytics_collector.py` & `giskard-2.9.0/giskard/utils/analytics_collector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/artifacts.py` & `giskard-2.9.0/giskard/utils/artifacts.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/display.py` & `giskard-2.9.0/giskard/utils/display.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/environment_detector.py` & `giskard-2.9.0/giskard/utils/environment_detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -111,53 +111,67 @@
 ENV_DETECTED = enum(
     CLOUD="CLOUD",
     NON_CLOUD="NON_CLOUD",
     BOTH_CLOUD_AND_NON_CLOUD="BOTH_CLOUD_AND_NON_CLOUD",
 )
 
 
+DOCKER_DEV = "docker-dev-mode"
+DATABRICKS = "databricks"
+VSCODE = "vscode"
+AZURE = "azure"
+AZUREML = "azureml"
+KAGGLE = "kaggle"
+SAGEMAKER = "sagemaker"
+BINDER = "binder"
+COLAB = "colab"
+AZURESYNAPSE = "azuresynapse"
+IPYTHON = "ipython"
+IPYTHON_ZMQ = "ipython-zmq"
+
+
 def is_cloud_env(detected):
     non_cloud_env = [
-        "ipython-zmq",
-        "ipython",
-        "vscode",
+        IPYTHON_ZMQ,
+        IPYTHON,
+        VSCODE,
     ]
     cloud_env = [
-        "databricks",
-        "azure",
-        "azureml",
-        "kaggle",
-        "sagemaker",
-        "binder",
-        "colab",
-        "azuresynapse",
+        DATABRICKS,
+        AZURE,
+        AZUREML,
+        KAGGLE,
+        SAGEMAKER,
+        BINDER,
+        COLAB,
+        AZURESYNAPSE,
     ]
     if len(set(cloud_env).intersection(detected)) != 0 and len(set(non_cloud_env).intersection(detected)) == 0:
         return ENV_DETECTED.CLOUD
     elif len(set(cloud_env).intersection(detected)) != 0 and len(set(non_cloud_env).intersection(detected)) != 0:
         return ENV_DETECTED.BOTH_CLOUD_AND_NON_CLOUD
     else:
         return ENV_DETECTED.NON_CLOUD
 
 
 class EnvironmentDetector:
     def __init__(self):
         self.checks = {
-            "docker-dev-mode": _is_docker_development_mode,
-            "databricks": _detect_databricks,
-            "vscode": _detect_vscode,
-            "azure": _detect_azure_notebook,
-            "azureml": _detect_azureml,
-            "kaggle": _detect_kaggle,
-            "sagemaker": _detect_sagemaker,
-            "binder": _detect_binder,
-            "colab": _detect_colab,
-            "ipython-zmq": _detect_ipython_zmq,
-            "ipython": _detect_ipython,
-            "azuresynapse": _detect_azure_synapse,
+            DOCKER_DEV: _is_docker_development_mode,
+            DATABRICKS: _detect_databricks,
+            VSCODE: _detect_vscode,
+            AZURE: _detect_azure_notebook,
+            AZUREML: _detect_azureml,
+            KAGGLE: _detect_kaggle,
+            SAGEMAKER: _detect_sagemaker,
+            BINDER: _detect_binder,
+            COLAB: _detect_colab,
+            IPYTHON_ZMQ: _detect_ipython_zmq,
+            IPYTHON: _detect_ipython,
+            AZURESYNAPSE: _detect_azure_synapse,
         }
 
     def detect(self):
         envs = []
         for name, check in self.checks.items():
             try:
                 check_passed = check()
```

### Comparing `giskard-2.8.0/giskard/utils/logging_utils.py` & `giskard-2.9.0/giskard/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/sentry.py` & `giskard-2.9.0/giskard/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/utils/worker_pool.py` & `giskard-2.9.0/giskard/utils/worker_pool.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/custom_jinja.py` & `giskard-2.9.0/giskard/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/rag_report/rag_report.html` & `giskard-2.9.0/giskard/visualization/templates/rag_report/rag_report.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/rag_report/static/internal.js` & `giskard-2.9.0/giskard/visualization/templates/rag_report/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/rag_report/static/style.css` & `giskard-2.9.0/giskard/visualization/templates/rag_report/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/_code_snippet.html` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_code_snippet.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/_issue.html` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_issue.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/_main_content.html` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/_tab_header.html` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/full.html` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/full.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/external.js` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/internal.js` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/html/static/style.css` & `giskard-2.9.0/giskard/visualization/templates/scan_report/html/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/github.md` & `giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/github.md`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/huggingface.md` & `giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/huggingface.md`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/scan_report/markdown/summary.md` & `giskard-2.9.0/giskard/visualization/templates/scan_report/markdown/summary.md`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/suite_results/_suite_results_cards.html` & `giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_cards.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/suite_results/_suite_results_header.html` & `giskard-2.9.0/giskard/visualization/templates/suite_results/_suite_results_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/templates/suite_results/suite_results.html` & `giskard-2.9.0/giskard/visualization/templates/suite_results/suite_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard/visualization/widget.py` & `giskard-2.9.0/giskard/visualization/widget.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/giskard.egg-info/PKG-INFO` & `giskard-2.9.0/giskard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.8.0
+Version: 2.9.0
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
@@ -65,15 +65,14 @@
 Requires-Dist: psutil>=5.4.6; extra == "hub"
 Requires-Dist: click>=7.0; extra == "hub"
 Requires-Dist: docker>=6.0.0; extra == "hub"
 Requires-Dist: shap>=0.41.0; extra == "hub"
 Requires-Dist: llvmlite>=0.40.0; extra == "hub"
 Requires-Dist: numba>=0.50.0; extra == "hub"
 Requires-Dist: lockfile>=0.12.2; extra == "hub"
-Requires-Dist: python-daemon<3,>=2.2.2; extra == "hub"
 Requires-Dist: pycryptodome>=3.6.1; extra == "hub"
 Requires-Dist: pyngrok>=6.0.0; extra == "hub"
 
 <p align="center">
   <img alt="giskardlogo" src="https://raw.githubusercontent.com/giskard-ai/giskard/main/readme/giskard_logo.png#gh-light-mode-only">
   <img alt="giskardlogo" src="https://raw.githubusercontent.com/giskard-ai/giskard/main/readme/giskard_logo_green.png#gh-dark-mode-only">
 </p>
```

### Comparing `giskard-2.8.0/giskard.egg-info/SOURCES.txt` & `giskard-2.9.0/giskard.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 giskard/rag/metrics/ragas_metrics.py
 giskard/rag/question_generators/__init__.py
 giskard/rag/question_generators/base.py
 giskard/rag/question_generators/complex_questions.py
 giskard/rag/question_generators/conversational_questions.py
 giskard/rag/question_generators/distracting_questions.py
 giskard/rag/question_generators/double_questions.py
+giskard/rag/question_generators/oos_questions.py
 giskard/rag/question_generators/prompt.py
 giskard/rag/question_generators/question_types.py
 giskard/rag/question_generators/simple_questions.py
 giskard/rag/question_generators/situational_questions.py
 giskard/rag/question_generators/utils.py
 giskard/registry/__init__.py
 giskard/registry/decorators.py
```

### Comparing `giskard-2.8.0/giskard.egg-info/requires.txt` & `giskard-2.9.0/giskard.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 psutil>=5.4.6
 click>=7.0
 docker>=6.0.0
 shap>=0.41.0
 llvmlite>=0.40.0
 numba>=0.50.0
 lockfile>=0.12.2
-python-daemon<3,>=2.2.2
 pycryptodome>=3.6.1
 pyngrok>=6.0.0
 
 [hub:sys_platform != "win32"]
 uvloop>=0.18.0
 
 [llm]
```

### Comparing `giskard-2.8.0/pyproject.toml` & `giskard-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     "pytest>=7.1.2",
     "pytest-xdist>=3.3.1",
     "polyfactory",
     "pytest-env>=1.1.0",
     "openai>=1",
     "pytest-memray; sys_platform == 'linux' or sys_platform == 'darwin'",
     "pytest-reportlog>=0.4.0",
+    "shap<0.45",                                                          # Fixing this to avoid changed on insights
 ]
 doc = [
     "furo>=2023.5.20",
     "myst-parser>=1.0.0",
     "sphinx-autobuild>=2021.3.14",
     "sphinx>=6.1.3",
     "sphinxcontrib-napoleon>=0.7",
@@ -128,15 +129,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.8.0"
+version = "2.9.0"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [{ name = "Giskard AI", email = "hello@giskard.ai" }]
 keywords = ["Artificial Intelligence", "Machine Learning", "Quality", "MLOps"]
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -196,18 +197,17 @@
     "uvloop>=0.18.0; sys_platform != 'win32'",
     # Server deps
     "tenacity>=4.11.0",
     "psutil>=5.4.6",
     "click>=7.0",
     "docker>=6.0.0",
     "shap>=0.41.0",
-    "llvmlite>=0.40.0",        # Needed to be installable for Poetry
-    "numba>=0.50.0",           # Needed to be installable for Poetry
+    "llvmlite>=0.40.0",    # Needed to be installable for Poetry
+    "numba>=0.50.0",       # Needed to be installable for Poetry
     "lockfile>=0.12.2",
-    "python-daemon>=2.2.2,<3",
     "pycryptodome>=3.6.1",
     "pyngrok>=6.0.0",
 ]
 
 [tool.ruff]
 line-length = 120
 ignore = ["E501"]
```

### Comparing `giskard-2.8.0/tests/test_artifact_download.py` & `giskard-2.9.0/tests/test_artifact_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     is_url_requested,
     local_save_artifact_under_giskard_home_cache,
     register_uri_for_artifact_info,
     register_uri_for_artifact_meta_info,
 )
 
 BASE_CLIENT_URL = "http://giskard-host:12345/api/v2"
+PROJECT_KEY = "project_key"
 
 
 # Define a test function
 @test
 def my_custom_test(model, data):
     return GiskardTestResult(passed=True)
 
@@ -42,47 +43,14 @@
 
 # Define a transformation function
 @transformation_function()
 def do_nothing(row):
     return row
 
 
-def test_download_global_test_function_from_registry():
-    cf: Artifact = my_custom_test
-
-    # Load from registry using uuid without client
-    download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=None, project_key=None)
-
-    # Check the downloaded info
-    assert download_cf.__class__ is cf.__class__
-    assert download_cf.meta.uuid == cf.meta.uuid
-
-
-@pytest.mark.parametrize(
-    "cf",
-    [
-        my_custom_test,  # Test
-        head_slice,  # Slice
-        do_nothing,  # Transformation
-    ],
-)
-def test_download_global_test_function_from_local(cf):
-    with MockedProjectCacheDir():
-        cf.meta.uuid = str(uuid.uuid4())  # Regenerate a UUID to ensure not loading from registry
-
-        local_save_artifact_under_giskard_home_cache(cf)
-
-        # Load from registry using uuid without client
-        download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=None, project_key=None)
-
-        # Check the downloaded info
-        assert download_cf.__class__ is cf.__class__
-        assert download_cf.meta.uuid == cf.meta.uuid
-
-
 @pytest.mark.parametrize(
     "cf",
     [
         my_custom_test,  # Test
         head_slice,  # Slice
         do_nothing,  # Transformation
     ],
@@ -105,34 +73,34 @@
             meta_info = fixup_mocked_artifact_meta_version(cf.meta.to_json())
             # Fixup the name to avoid load from module
             meta_info.update(
                 {
                     "name": f"fake_{cf._get_name()}",
                 }
             )
-            url = get_url_for_artifact_meta_info(cf, project_key=None)
+            url = get_url_for_artifact_meta_info(cf, PROJECT_KEY)
             mr.register_uri(method=requests_mock.GET, url=url, json=meta_info)
             requested_urls.append(url)
 
             # Register for Artifact info
-            requested_urls.extend(register_uri_for_artifact_info(mr, cf, project_key=None))
+            requested_urls.extend(register_uri_for_artifact_info(mr, cf, PROJECT_KEY))
 
             # Register for Artifacts content
             artifacts_base_url = get_url_for_artifacts_base(cf)
             for file in [CALLABLE_FUNCTION_META_CACHE, CALLABLE_FUNCTION_PKL_CACHE]:
                 with open(tmpdir_path / file, "rb") as f:
                     mr.register_uri(
                         method=requests_mock.GET,
                         url=posixpath.join(artifacts_base_url, file),
                         content=f.read(),
                     )
                     requested_urls.append(posixpath.join(artifacts_base_url, file))
 
             # Download: should not call load_artifact to request and download
-            download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=None)
+            download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=PROJECT_KEY)
 
             for requested_url in requested_urls:
                 assert is_url_requested(mr.request_history, requested_url)
 
             # Check the downloaded info
             assert download_cf.__class__ is cf.__class__
             assert download_cf.meta.uuid == cf.meta.uuid
@@ -145,25 +113,25 @@
     "cf",
     [
         my_custom_test,  # Test
         head_slice,  # Slice
         do_nothing,  # Transformation
     ],
 )
-def test_download_global_callable_function_from_module(cf: Artifact):
+def test_download_callable_function_from_module(cf: Artifact):
     with MockedClient(mock_all=False) as (client, mr):
         cf.meta.uuid = str(uuid.uuid4())  # Regenerate a UUID to ensure not loading from registry
         cache_dir = get_local_cache_callable_artifact(artifact=cf)
 
         requested_urls = []
-        # Prepare global URL
-        requested_urls.extend(register_uri_for_artifact_meta_info(mr, cf, project_key=None))
+        # Prepare URL
+        requested_urls.extend(register_uri_for_artifact_meta_info(mr, cf, project_key=PROJECT_KEY))
 
         # Download: should not call load_artifact to request and download
-        download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=None)
+        download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=PROJECT_KEY)
 
         for requested_url in requested_urls:
             assert is_url_requested(mr.request_history, requested_url)
 
         # Check the downloaded info
         assert download_cf.__class__ is cf.__class__
         assert download_cf.meta.uuid == cf.meta.uuid
@@ -176,28 +144,28 @@
     "cf",
     [
         my_custom_test,  # Test
         head_slice,  # Slice
         do_nothing,  # Transformation
     ],
 )
-def test_download_global_callable_function_from_cache(cf: Artifact):
+def test_download_callable_function_from_cache(cf: Artifact):
     with MockedClient(mock_all=False) as (client, mr):
         cf.meta.uuid = str(uuid.uuid4())  # Regenerate a UUID
         cache_dir = get_local_cache_callable_artifact(artifact=cf)
 
         # Save to local cache
         local_save_artifact_under_giskard_home_cache(artifact=cf)
         assert (cache_dir / CALLABLE_FUNCTION_PKL_CACHE).exists()
         assert (cache_dir / CALLABLE_FUNCTION_META_CACHE).exists()
 
-        requested_urls = register_uri_for_artifact_meta_info(mr, cf, project_key=None)
+        requested_urls = register_uri_for_artifact_meta_info(mr, cf, project_key=PROJECT_KEY)
 
         # Download: should not call load_artifact to request and download
-        download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=None)
+        download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=PROJECT_KEY)
 
         for requested_url in requested_urls:
             assert is_url_requested(mr.request_history, requested_url)
 
         # Check the downloaded info
         assert download_cf.__class__ is cf.__class__
         assert download_cf.meta.uuid == cf.meta.uuid
@@ -277,15 +245,15 @@
 def test_download_callable_function_from_module_in_project(cf: Artifact):
     project_key = str(uuid.uuid4())
     with MockedClient(mock_all=False) as (client, mr), MockedProjectCacheDir():
         cf.meta.uuid = str(uuid.uuid4())  # Regenerate a UUID to ensure not loading from registry
         cache_dir = get_local_cache_callable_artifact(artifact=cf)
 
         requested_urls = []
-        # Prepare global URL
+        # Prepare URL
         requested_urls.extend(register_uri_for_artifact_meta_info(mr, cf, project_key))
 
         # Download: should not call load_artifact to request and download
         download_cf = cf.__class__.download(uuid=cf.meta.uuid, client=client, project_key=project_key)
 
         for requested_url in requested_urls:
             assert is_url_requested(mr.request_history, requested_url)
```

### Comparing `giskard-2.8.0/tests/test_custom_model.py` & `giskard-2.9.0/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_data_drift.py` & `giskard-2.9.0/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_data_processing_pipeline.py` & `giskard-2.9.0/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_dataset.py` & `giskard-2.9.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_import_giskard.py` & `giskard-2.9.0/tests/test_import_giskard.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_metamorphic_direction.py` & `giskard-2.9.0/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_metamorphic_invariance.py` & `giskard-2.9.0/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_performance.py` & `giskard-2.9.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_programmatic.py` & `giskard-2.9.0/tests/test_programmatic.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
                         "test": None,
                     }
                 ],
                 "id": 2,
                 "projectKey": "test_project",
             },
         )
-        register_uri_for_artifact_meta_info(mr, test_auc)
+        register_uri_for_artifact_meta_info(mr, test_auc, "test_project")
 
         mr.register_uri(requests_mock.GET, UPLOAD_RESULTS_URL, json={})
 
         suite = Suite.download(client, "test_project", 2)
         results = suite.run()
         results.upload(client)
```

### Comparing `giskard-2.8.0/tests/test_project_uploads.py` & `giskard-2.9.0/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_push.py` & `giskard-2.9.0/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_settings.py` & `giskard-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_statistical.py` & `giskard-2.9.0/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_suite.py` & `giskard-2.9.0/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.8.0/tests/test_upload.py` & `giskard-2.9.0/tests/test_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     MockedClient,
     get_local_cache_callable_artifact,
     match_model_id,
     match_url_patterns,
 )
 
 model_name = "uploaded model"
+PROJECT_KEY = "project_key"
 
 
 def test_upload_df(diabetes_dataset: Dataset, diabetes_dataset_with_target: Dataset):
     artifact_url_pattern = re.compile(
         r"http://giskard-host:12345/api/v2/artifacts/datasets/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/[data.csv.zst|giskard\-dataset\-meta.yaml]"
     )
     datasets_url_pattern = re.compile("http://giskard-host:12345/api/v2/project/test-project/datasets")
@@ -147,15 +148,15 @@
 def test_upload_callable_function(cf: Artifact):
     artifact_url_pattern = re.compile(
         "http://giskard-host:12345/api/v2/artifacts/"
         + cf._get_name()
         + "/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/.*"
     )
     with MockedClient() as (client, mr):
-        cf.upload(client=client, project_key=None)
+        cf.upload(client=client, project_key=PROJECT_KEY)
         # Check local cache
         cache_dir = get_local_cache_callable_artifact(artifact=cf)
         assert (cache_dir / CALLABLE_FUNCTION_PKL_CACHE).exists()
         assert (cache_dir / CALLABLE_FUNCTION_META_CACHE).exists()
         # Check requested URL
         match_url_patterns(mr.request_history, artifact_url_pattern)
```

### Comparing `giskard-2.8.0/tests/test_worker_pool.py` & `giskard-2.9.0/tests/test_worker_pool.py`

 * *Files identical despite different names*

