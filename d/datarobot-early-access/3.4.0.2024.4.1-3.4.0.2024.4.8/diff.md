# Comparing `tmp/datarobot_early_access-3.4.0.2024.4.1.tar.gz` & `tmp/datarobot_early_access-3.4.0.2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.4.0.2024.4.1.tar", last modified: Mon Apr  1 16:47:17 2024, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.4.0.2024.4.8.tar", last modified: Mon Apr  8 16:47:24 2024, max compression
```

## Comparing `datarobot_early_access-3.4.0.2024.4.1.tar` & `datarobot_early_access-3.4.0.2024.4.8.tar`

### file list

```diff
@@ -1,215 +1,216 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   221774 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2535 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25506 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/chunking_service.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/data_matching.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11572 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/enums.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5661 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23220 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5939 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13717 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1818 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_llm_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15666 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22662 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm_blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6886 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/playground.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/user_limits.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26323 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/vector_database.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/incremental_learning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    29350 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipe_operations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipes.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/config.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32947 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9262 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/base.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2698 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1409 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1622 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_preview.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4351 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32414 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    61948 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/challenger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/champion_model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57730 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/custom_metrics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_exports.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/sharing.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11232 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/key_values.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   305975 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/common.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/recommended_model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job_run.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/runtime_parameters.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7487 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   223607 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2535 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25506 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/chunking_service.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11628 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/enums.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5661 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24973 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5939 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13717 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1818 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15919 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22662 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7281 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6945 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/prompt_trace.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27868 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/incremental_learning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30661 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/config.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32946 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8744 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9262 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/base.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2698 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1409 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1622 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_preview.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4351 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34090 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    63934 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/challenger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/champion_model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57732 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/custom_metrics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_exports.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/sharing.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13141 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/key_values.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   305975 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/common.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/recommended_model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job_run.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/runtime_parameters.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4722 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8216 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2676 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7540 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/setup_weekly.py
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/CHANGES.rst` & `datarobot_early_access-3.4.0.2024.4.8/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #########
 Changelog
 #########
 3.4.0b0
 =======
 
-New Features
+New features
 ************
 
 - Extended the advanced options available when setting a target to include new
   parameter: 'incrementalLearningEarlyStoppingRounds'(part of the AdvancedOptions object).
   This parameter allows you to specify when to stop for incremental learning automation.
 - Added experimental support for Chunking Service:
     - :class:`DatasetChunkDefinition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition>` for defining how chunks are created from a data source.
@@ -79,15 +79,15 @@
   :meth:`CustomMetric.get <datarobot.models.deployment.custom_metrics.CustomMetric.get>` to retrieve a custom metric object by ID from a given deployment.
   :meth:`CustomMetric.list <datarobot.models.deployment.custom_metrics.CustomMetric.list>` to list all custom metrics from a given deployment.
   :meth:`CustomMetric.create <datarobot.models.deployment.custom_metrics.CustomMetric.create>` to create a new custom metric for a given deployment.
   :meth:`CustomMetric.update <datarobot.models.deployment.custom_metrics.CustomMetric.update>` to update a custom metric for a given deployment.
   :meth:`CustomMetric.delete <datarobot.models.deployment.custom_metrics.CustomMetric.delete>` to delete a custom metric for a given deployment.
   :meth:`CustomMetric.unset_baseline <datarobot.models.deployment.custom_metrics.CustomMetric.unset_baseline>` to remove baseline for a given custom metric.
   :meth:`CustomMetric.submit_values <datarobot.models.deployment.custom_metrics.CustomMetric.submit_values>` to submit aggregated custom metrics values from code. The provided data should be in the form of a dict or a Pandas DataFrame.
-  :meth:`CustomMetric.report_single_value <datarobot.models.deployment.custom_metrics.CustomMetric.report_single_value>` to submit a single custom metric value.
+  :meth:`CustomMetric.submit_single_value <datarobot.models.deployment.custom_metrics.CustomMetric.submit_single_value>` to submit a single custom metric value.
   :meth:`CustomMetric.submit_values_from_catalog <datarobot.models.deployment.custom_metrics.CustomMetric.submit_values_from_catalog>` to submit aggregated custom metrics values from a dataset via the AI Catalog.
   :meth:`CustomMetric.get_values_over_time <datarobot.models.deployment.custom_metrics.CustomMetric.get_values_over_time>` to retrieve values of a custom metric over a time period.
   :meth:`CustomMetric.get_summary <datarobot.models.deployment.custom_metrics.CustomMetric.get_summary>` to retrieve the summary of a custom metric over a time period.
   :meth:`CustomMetric.get_values_over_batch <datarobot.models.deployment.custom_metrics.CustomMetric.get_values_over_batch>` to retrieve values of a custom metric over batches.
   :meth:`CustomMetric.get_batch_summary <datarobot.models.deployment.custom_metrics.CustomMetric.get_batch_summary>` to retrieve the summary of a custom metric over batches.
 - Added :class:`CustomMetricValuesOverTime <datarobot.models.deployment.custom_metrics.CustomMetricValuesOverTime>` to retrieve custom metric over time information.
 - Added :class:`CustomMetricSummary <datarobot.models.deployment.custom_metrics.CustomMetricSummary>` to retrieve custom metric over time summary.
@@ -106,14 +106,19 @@
   :meth:`ActualsDataExport.create <datarobot.models.deployment.data_exports.ActualsDataExport.create>` to create a new actuals data export for a given deployment.
   :meth:`ActualsDataExport.fetch_data <datarobot.models.deployment.data_exports.ActualsDataExport.fetch_data>` to retrieve an actuals export data  as a DataRobot dataset.
 - Added a new class :class:`TrainingDataExport <datarobot.models.deployment.data_exports.TrainingDataExport>` for interacting with DataRobot deployment data export to support the following methods:
   :meth:`TrainingDataExport.get <datarobot.models.deployment.data_exports.TrainingDataExport.get>` to retrieve a training data export object by ID from a given deployment.
   :meth:`TrainingDataExport.list <datarobot.models.deployment.data_exports.TrainingDataExport.list>` to list all training data exports from a given deployment.
   :meth:`TrainingDataExport.create <datarobot.models.deployment.data_exports.TrainingDataExport.create>` to create a new training data export for a given deployment.
   :meth:`TrainingDataExport.fetch_data <datarobot.models.deployment.data_exports.TrainingDataExport.fetch_data>` to retrieve a training export data as a DataRobot dataset.
+- Added a new parameter `base_environment_version_id` to :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` for overriding the default environment version selection behavior.
+- Added a new parameter `base_environment_version_id` to :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` for overriding the default environment version selection behavior.
+- Added a new class :class:`PromptTrace <datarobot._experimental.models.genai.prompt_trace.PromptTrace>` for interacting with DataRobot prompt trace to support the following methods:
+  :meth:`PromptTrace.list <datarobot._experimental.models.genai.prompt_trace.PromptTrace.list>` to list all prompt traces from a given playground.
+  :meth:`PromptTrace.export_to_ai_catalog <datarobot._experimental.models.genai.prompt_trace.PromptTrace.export_to_ai_catalog>` to export prompt traces for the playground to AI catalog.
 
 Key Changes
   1.	Parameter Overrides: Users can now override most of the previously set configuration values directly through parameters when initializing the Client.
   2.	Exceptions: The endpoint and token values must be initiated from one source(client params, environment, or config file) and cannot be overridden individually for security and consistency reasons.
 
 Configuration Priority:
   1.	Client Params
@@ -146,32 +151,38 @@
 - Added two new parameters to :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` for filtering the job definitions:
     - `deployment_id`
     - `search_name`
 - Added new parameter to :meth:`Deployment.validate_replacement_model<datarobot.models.Deployment.validate_replacement_model>` to support replacement validation based on model package ID:
     - `new_registered_model_version_id`
 - Added support for Native Connectors to `Connector <datarobot.models.Connector>` for everything other than :meth:` Connector.create <datarobot.models.Connector.create>` and :meth:` Connector.update <datarobot.models.Connector.update>`
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Removed `Model.get_leaderboard_ui_permalink` and `Model.open_model_browser`
 - Deprecated :meth:`Project.get_models <datarobot.models.Project.get_models>` in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
 - :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` will no longer return all job definitions after version 3.6 is released.
   To preserve current behavior please pass limit=0.
 - `new_model_id` parameter in :meth:`Deployment.validate_replacement_model<datarobot.models.Deployment.validate_replacement_model>` will be removed after version 3.6 is released.
 - :meth:`Deployment.replace_model<datarobot.models.Deployment.replace_model>` will be removed after version 3.6 is released.
   Method :meth:`Deployment.perform_model_replace<datarobot.models.Deployment.perform_model_replace>` should be used instead.
-- Removed `CustomInferenceModel.assign_training_data`.
+- :meth:`CustomInferenceModel.assign_training_data <datarobot.CustomInferenceModel.assign_training_data>` was marked as deprecated in v3.2. The deprecation period has been extended, and the feature will now be removed in v3.5.
   Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
 
 Documentation changes
 *********************
 - Updated `genai_example.rst` to utilize latest genAI features and methods introduced most recently in the API client.
 
 Experimental changes
 *********************
+- Added new attributes, `feedback_result`, `metrics`, and `final_prompt` to :class:`ResultMetadata <datarobot._experimental.models.genai.chat_prompt.ResultMetadata>`.
+- Added `use_case_id` to :class:`CustomModelValidation <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation>`.
+- Added `llm_blueprints_count` and `user_name` to :class:`Playground <datarobot._experimental.models.genai.playground.Playground>`.
+- Added `custom_model_embedding_validations` to :class:`SupportedEmbeddings <datarobot._experimental.models.genai.vector_database.SupportedEmbeddings>`.
+- Added `embedding_validation_id` and `is_separator_regex` to :class:`VectorDatabase <datarobot._experimental.models.genai.vector_database.VectorDatabase>`.
+
 - Added optional parameters, `use_case`, `name`, and `model` to :meth:`CustomModelValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>`.
 - Added a method :meth:`CustomModelValidation.list <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.list>`, to list custom model validations available to a user with several optional parameters to filter the results.
 - Added a method :meth:`CustomModelValidation.update <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.update>`, to update a custom model validation.
 
 - Added an optional parameter, `use_case`, to :meth:`LLMDefinition.list <datarobot._experimental.models.genai.llm.LLMDefinition.list>`,
   to include in the returned LLMs the external LLMs available for the specified `use_case` as well.
 
@@ -222,19 +233,20 @@
 - Added a new method :meth:`Model.start_incremental_learning <datarobot._experimental.models.model.Model.start_incremental_learning>` that starts incremental learning for a model.
 
 Bugfixes
 ********
 - Fixed how async url is build in :meth:`Model.get_or_request_feature_impact <datarobot.models.Model.get_or_request_feature_impact>`
 - Fixed setting ssl_verify by env variables.
 - Resolved a problem related to tilde-based paths in the Client's 'config_path' attribute.
+- Changed the force_size default of :class:`ImageOptions <datarobot.helpers.image_utils.ImageOptions>` to apply the same transformations by default, which are applied when image archive datasets are uploaded to DataRobot.
 
 3.3.0
 =====
 
-New Features
+New features
 ************
 - Added support for Python 3.11.
 - Added new library "strenum" to add `StrEnum` support while maintaining backwards compatibility with Python 3.7-3.10. DataRobot does not use the native `StrEnum` class in Python 3.11.
 - Added a new class :class:`PredictionEnvironment <datarobot.models.PredictionEnvironment>` for interacting with DataRobot Prediction environments.
 - Extended the advanced options available when setting a target to include new
   parameters: 'modelGroupId', 'modelRegimeId', and 'modelBaselines' (part of the AdvancedOptions object). These parameters allow you to specify the user columns required to run time series models without feature derivation in OTV projects.
 - Added a new method :meth:`PredictionExplanations.create_on_training_data <datarobot.PredictionExplanations.create_on_training_data>`, for computing prediction explanation on training data.
@@ -282,21 +294,21 @@
 ********
 - Payload property `subset` renamed to `source` in :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>`
 - Fixed an issue where Context.trace_context was not being set from environment variables or DR config files.
 - :meth:`Project.refresh <datarobot.models.Project.refresh>` no longer sets ``Project.advanced_options`` to a dictionary.
 - Fixed :meth:`Dataset.modify <datarobot.models.Dataset.modify>` to clarify behavior of when to preserve or clear categories.
 - Fixed an issue with enums in f-strings resulting in the enum class and property being printed instead of the enum property's value in Python 3.11 environments.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - :meth:`Project.refresh <datarobot.models.Project.refresh>` will no longer set ``Project.advanced_options`` to a dictionary after version 3.5 is released.
    All interactions with ``Project.advanced_options`` should be expected to be through the :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` class.
 
 Experimental changes
-*********************
+********************
 - Added a new class, :class:`VectorDatabase <datarobot._experimental.models.genai.vector_database.VectorDatabase>`, for interacting with DataRobot vector databases.
   :meth:`VectorDatabase.get <datarobot._experimental.models.genai.vector_database.VectorDatabase.get>` retrieves a VectorDatabase object by ID.
   :meth:`VectorDatabase.list <datarobot._experimental.models.genai.vector_database.VectorDatabase.list>` lists all VectorDatabases available to the user.
   :meth:`VectorDatabase.create <datarobot._experimental.models.genai.vector_database.VectorDatabase.create>` creates a new VectorDatabase.
   :meth:`VectorDatabase.create <datarobot._experimental.models.genai.vector_database.VectorDatabase.create_from_custom_model>` allows you to use a validated deployment of a custom model as your own Vector Database.
   :meth:`VectorDatabase.update <datarobot._experimental.models.genai.vector_database.VectorDatabase.update>` updates the name of a VectorDatabase.
   :meth:`VectorDatabase.delete <datarobot._experimental.models.genai.vector_database.VectorDatabase.delete>` deletes a single VectorDatabase.
@@ -354,15 +366,15 @@
 - Added a new method, :meth:`CustomModelLLMValidation.delete <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.delete>`, to delete a custom model LLM validation record.
 
 - Added a new method, :meth:`LLMBlueprint.register_custom_model <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.register_custom_model>`, for registering a custom model from a generative AI LLM blueprint.
 
 3.2.0
 =====
 
-New Features
+New features
 ************
 - Added new methods to trigger batch monitoring jobs without providing a job definition.
   :meth:`BatchMonitoringJob.run <datarobot.models.BatchMonitoringJob.run>`
   :meth:`BatchMonitoringJob.get_status <datarobot.models.BatchMonitoringJob.get_status>`
   :meth:`BatchMonitoringJob.cancel <datarobot.models.BatchMonitoringJob.cancel>`
   :meth:`BatchMonitoringJob.download <datarobot.models.BatchMonitoringJob.download>`
 
@@ -507,20 +519,20 @@
 Bugfixes
 ********
 - Fixed incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
 - Fixed a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 - Fixed an issue where failed authentication when invoking `datarobot.client.Client()` raises a misleading error about client-server compatibility.
 - Fixed incompatibilities with Pandas 2.0 in :meth:`AccuracyOverTime.get_as_dataframe <datarobot.models.deployment.AccuracyOverTime.get_as_dataframe>`. The method will now throw a `ValueError` if an empty list is passed to the parameter `metrics`.
 
-API Changes
+API changes
 ***********
 - Added parameter ``unsupervised_type`` to the class :class:`DatetimePartitioning <datarobot.DatetimePartitioning>`.
 - The sliced insight API endpoint `GET: api/v2/insights/<insight_name>/` returns a paginated response. This means that it returns an empty response if no insights data is found, unlike `GET: api/v2/projects/<pid>/models/<lid>/<insight_name>/`, which returns 404 NOT FOUND in this case. To maintain backwards-compatibility, all methods that retrieve insights data raise 404 NOT FOUND if the insights API returns an empty response.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``Model.get_feature_fit_metadata`` has been removed.
   Use :meth:`Model.get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>` instead.
 - ``DatetimeModel.get_feature_fit_metadata`` has been removed.
   Use :meth:`DatetimeModel.get_feature_effect_metadata <datarobot.models.DatetimeModel.get_feature_effect_metadata>` instead.
 - ``Model.request_feature_fit`` has been removed.
   Use :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>` instead.
@@ -534,32 +546,32 @@
   Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
 - ``DatetimeModel.get_or_request_feature_fit`` has been removed.
   Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
 - Deprecated the use of :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` in favor of :class:`SharingRole <datarobot.models.sharing.SharingRole>` for sharing in the following classes:
   - :meth:`DataStore.share <datarobot.DataStore.share>`
 - Deprecated the following methods for retrieving :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` information.
   - :meth:`DataStore.get_access_list <datarobot.DataStore.get_access_list>`. Please use :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>` instead.
-- `CustomInferenceModel.assign_training_data` was marked as deprecated and will be removed in v3.4.
+- :meth:`CustomInferenceModel.assign_training_data <datarobot.CustomInferenceModel.assign_training_data>` was marked as deprecated and will be removed in v3.4.
   Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Deprecated parameter `user_agent_suffix` in `datarobot.Client`. `user_agent_suffix` will be removed in v3.4. Please use `trace_context` instead.
 
-Documentation Changes
+Documentation changes
 *********************
 - Fixed in-line documentation of `DataRobotClientConfig`.
 - Fixed documentation around client configuration from environment variables or config file.
 
 Experimental changes
-*********************
+********************
 - Added experimental support for data matching:
 
   - :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`
   - :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>`
 
 - Added new method :meth:`DataMatchingQuery.get_result <datarobot._experimental.models.data_matching.DataMatchingQuery.get_result>` for returning data matching query results as pandas dataframes to :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>` .
 - Changed behavior for returning results in the :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. Instead of saving the results as a file, a pandas dataframe will be returned in the following methods:
@@ -579,25 +591,22 @@
 
   - :class:`Recipe <datarobot._experimental.models.recipes.Recipe>`
 
 
 3.1.1
 =====
 
-Configuration Changes
+Configuration changes
 *********************
 - Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
 - Update `typing-extensions <https://pypi.org/project/typing-extensions/>`_ to be inclusive of versions from 4.3.0 to < 5.0.0.
 
 3.1.0
 =====
 
-New Features
-************
-
 Enhancements
 ************
 - Added new methods :meth:`BatchPredictionJob.apply_time_series_data_prep_and_score<datarobot.models.BatchPredictionJob.apply_time_series_data_prep_and_score>`
   and :meth:`BatchPredictionJob.apply_time_series_data_prep_and_score_to_file<datarobot.models.BatchPredictionJob.apply_time_series_data_prep_and_score_to_file>`
   that apply time series data prep to a file or dataset and make batch predictions with a deployment.
 - Added new methods :meth:`DataEngineQueryGenerator.prepare_prediction_dataset<datarobot.DataEngineQueryGenerator.prepare_prediction_dataset>`
   and :meth:`DataEngineQueryGenerator.prepare_prediction_dataset_from_catalog<datarobot.DataEngineQueryGenerator.prepare_prediction_dataset_from_catalog>`
@@ -621,38 +630,32 @@
   :meth:`ImageAugmentationList.list<datarobot.models.visualai.ImageAugmentationList.list>`,
   :meth:`ImageAugmentationList.update<datarobot.models.visualai.ImageAugmentationList.update>`
 
 Bugfixes
 ********
 - Added `format` key to Batch Prediction intake and output settings for S3, GCP and Azure
 
-API Changes
+API changes
 ***********
 - The method :meth:`PredictionExplanations.is_multiclass <datarobot.PredictionExplanations.is_multiclass>` now adds an additional API call to check for multiclass target validity, which adds a small delay.
 - :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` parameter ``blend_best_models`` defaults to false
 - :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` parameter ``consider_blenders_in_recommendation`` defaults to false
 - :class:`DatetimePartitioning <datarobot.DatetimePartitioning>` has parameter ``unsupervised_mode``
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Deprecated method :meth:`Project.create_from_hdfs<datarobot.models.Project.create_from_hdfs>`.
 - Deprecated method :meth:`DatetimePartitioning.generate <datarobot.DatetimePartitioning.generate>`.
 - Deprecated parameter ``in_use`` from :meth:`ImageAugmentationList.create<datarobot.models.visualai.ImageAugmentationList.create>` as DataRobot will take care of it automatically.
 - Deprecated property ``Deployment.capabilities`` from :class:`Deployment <datarobot.models.Deployment>`.
 - ``ImageAugmentationSample.compute`` was removed in v3.1. You
   can get the same information with the method ``ImageAugmentationList.compute_samples``.
 - ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead.
 
-Configuration Changes
-*********************
-
-Experimental changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 - Update the documentation to suggest that setting `use_backtest_start_end_format` of :py:meth:`DatetimePartitioning.to_specification <datarobot.DatetimePartitioning.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 - Update the documentation to suggest setting `use_start_end_format` of :py:meth:`Backtest.to_specification <datarobot.helpers.partitioning_methods.Backtest.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 3.0.3
 =====
@@ -666,30 +669,30 @@
 
 Bugfixes
 ********
 - Restored `Model.get_leaderboard_ui_permalink`, `Model.open_model_browser`,
   These methods were accidentally removed instead of deprecated.
 - Fix for ipykernel < 6.0.0 which does not persist contextvars across cells
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Deprecated method `Model.get_leaderboard_ui_permalink`. Please use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
 - Deprecated method `Model.open_model_browser`. Please use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
 
 3.0.1
 =====
 
 Bugfixes
 ********
 - Added `typing-extensions` as a required dependency for the DataRobot Python SDK.
 
 3.0.0
 =====
 
-New Features
+New features
 ************
 - Version 3.0 of the Python client does not support Python 3.6 and earlier versions. Version 3.0 currently supports Python 3.7+.
 
 - The default Autopilot mode for :meth:`project.start_autopilot <datarobot.models.Project.start_autopilot>` has changed to Quick mode.
 
 - For datetime-aware models, you can now calculate and retrieve feature impact for backtests other than zero and holdout:
 
@@ -774,21 +777,21 @@
 Bugfixes
 ********
 - :meth:`Dataset.list <datarobot.models.Dataset.list>` no longer throws errors when listing datasets with no owner.
 - Fixed an issue with the creation of ``BatchPredictionJobDefinitions`` containing a schedule.
 - Fixed error handling in ``datarobot.helpers.partitioning_methods.get_class``.
 - Fixed issue with portions of the payload not using camelCasing in :meth:`Project.upload_dataset_from_catalog<datarobot.models.Project.upload_dataset_from_catalog>`.
 
-API Changes
+API changes
 ***********
 - The Python client now outputs a `DataRobotProjectDeprecationWarning` when you attempt to access certain resources (projects, models, deployments, etc.) that are deprecated or disabled as a result of the DataRobot platform's migration to Python 3.
 - The Python client now raises a `TypeError` when you try to retrieve a labelwise ROC on a binary model or a binary ROC on a multilabel model.
 - The method :meth:`Dataset.create_from_data_source<datarobot.models.Dataset.create_from_data_source>` now raises ``InvalidUsageError`` if ``username`` and ``password`` are not passed as a pair together.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``Model.get_leaderboard_ui_permalink`` has been removed.
   Use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
 - ``Model.open_model_browser`` has been removed.
   Use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
 - ``Project.get_leaderboard_ui_permalink`` has been removed.
   Use :meth:`Project.get_uri <datarobot.models.Project.get_uri>` instead.
@@ -809,21 +812,21 @@
 - The :class:`Deployment <datarobot.models.Deployment>` method ``create_from_custom_model_image`` was removed. Use :meth:`Deployment.create_from_custom_model_version <datarobot.models.Deployment.create_from_custom_model_version>` instead.
 - ``PredictJob.create`` has been removed. Use :meth:`Model.request_predictions <datarobot.models.Model.request_predictions>` instead.
 - ``Model.fetch_resource_data`` has been removed. Use :meth:`Model.get <datarobot.models.Model.get>` instead.
 - The class ``CustomInferenceImage`` was removed. Use :class:`CustomModelVersion <datarobot.CustomModelVersion>` with ``base_environment_id`` instead.
 - ``Project.set_target`` has been deprecated. Use :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>` instead.
 
 
-Configuration Changes
+Configuration changes
 *********************
 - Added a context manager :meth:`client_configuration <datarobot.client.client_configuration>` that can be used to change the connection configuration temporarily, for use in asynchronous or multithreaded code.
 - Upgraded the `Pillow` library to version 9.2.0. Users installing DataRobot with the "images" extra (``pip install datarobot[images]``) should note that this is a required library.
 
 Experimental changes
-*********************
+********************
 
 - Added experimental support for retrieving document thumbnails:
 
   - :class:`DocumentThumbnail <datarobot.models.documentai.document.DocumentThumbnail>`
   - :class:`DocumentPageFile <datarobot.models.documentai.document.DocumentPageFile>`
 
 - Added experimental support to retrieve document text extraction samples using:
@@ -840,15 +843,15 @@
 - Added new methods to :class:`RetrainingPolicy <datarobot._experimental.models.retraining.RetrainingPolicy>`:
   - Use :meth:`RetrainingPolicy.get <datarobot._experimental.models.retraining.RetrainingPolicy.get>` to get a retraining policy associated with a deployment.
   -  Use :meth:`RetrainingPolicy.delete <datarobot._experimental.models.retraining.RetrainingPolicy.delete>` to delete a retraining policy associated with a deployment.
 
 2.29.0b0
 ========
 
-New Features
+New features
 ************
 - Added support to pass `max_ngram_explanations` parameter in batch predictions that will trigger the
   compute of text prediction explanations.
 
   - :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`
 
 - Added support to pass calculation mode to prediction explanations
@@ -920,38 +923,38 @@
 ********
 - Don't include holdout start date, end date, or duration in datetime partitioning payload when
   holdout is disabled.
 - Removed ICE Plot capabilities from Feature Fit.
 - Handle undefined calendar_name in CalendarFile.create_calendar_from_dataset
 - Raise ValueError for submitted calendar names that are not strings
 
-API Changes
+API changes
 ***********
 - `version` field is removed from `ImportedModel` object
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Reason Codes objects deprecated in 2.13 version were removed.
   Please use Prediction Explanations instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - The upper version constraint on pandas has been removed.
 
-Documentation Changes
+Documentation changes
 *********************
 - Fixed a minor typo in the example for Dataset.create_from_data_source.
 
 - Update the documentation to suggest that `feature_derivation_window_end` of :py:class:`datarobot.DatetimePartitioningSpecification` class should be a negative or zero.
 
 
 2.28.0
 ======
 
-New Features
+New features
 ************
 - Added new parameter `upload_read_timeout` to :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`
   and :meth:`BatchPredictionJob.score_to_file <datarobot.models.BatchPredictionJob.score_to_file>` to indicate how many seconds to wait
   until intake dataset uploads to server. Default value 600s.
 
 - Added the ability to turn off supervised feature reduction for Time Series projects. Option
   `use_supervised_feature_reduction` can be set in :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>`.
@@ -1012,18 +1015,18 @@
 - Added support for governance, owners, predictionEnvironment, and fairnessHealth fields when querying for a Deployment object.
 
 - Added helper methods for working with files, images and documents. Methods support conversion of
   file contents into base64 string representations. Methods for images provide also image resize and
   transformation support.
 
   Functionality:
-    - `datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_urls.`
-    - `datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_paths`
-    - `datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_paths`
-    - `datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_urls`
+    - :meth:`get_encoded_file_contents_from_urls <datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_urls>`
+    - :meth:`get_encoded_file_contents_from_paths <datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_paths>`
+    - :meth:`get_encoded_image_contents_from_paths <datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_paths>`
+    - :meth:`get_encoded_image_contents_from_urls <datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_urls>`
 
 Enhancements
 ************
 - Requesting metadata instead of actual data of :class:`datarobot.PredictionExplanations` to reduce the amount of data transfer
 
 Bugfixes
 ********
@@ -1034,47 +1037,47 @@
 - Fix a bug where credentials were incorrectly formatted in
   :meth:`Project.upload_dataset_from_catalog <datarobot.models.Project.upload_dataset_from_catalog>`
   and
   :meth:`Project.upload_dataset_from_data_source <datarobot.models.Project.upload_dataset_from_data_source>`
 - Rejecting downloads of Batch Prediction data that was not written to the localfile output adapter
 - Fix a bug in :meth:`datarobot.models.BatchPredictionJobDefinition.create` where `schedule` was not optional for all cases
 
-API Changes
+API changes
 ***********
 
 - User can include ICE plots data in the response when requesting Feature Effects/Feature Fit. Extended methods are
     - :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>`,
     - ``Model.get_feature_fit <datarobot.models.Model.get_feature_fit>``,
     - :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` and
     - ``DatetimeModel.get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>``.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - `attrs` library is removed from library dependencies
 - ``ImageAugmentationSample.compute`` was marked as deprecated and will be removed in v2.30. You
   can get the same information with newly introduced method ``ImageAugmentationList.compute_samples``
 - ``ImageAugmentationSample.list`` using ``sample_id``
 - Deprecating scaleout parameters for projects / models. Includes ``scaleout_modeling_mode``,
   ``scaleout_max_train_pct``, and ``scaleout_max_train_rows``
 
-Configuration Changes
+Configuration changes
 *********************
 - `pandas` upper version constraint is updated to include version 1.3.5.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Fixed "from datarobot.enums" import in Unsupervised Clustering example provided in docs.
 
 
 2.27.0
 ========
 
-New Features
+New features
 ************
 - :class:`datarobot.UserBlueprint` is now mature with full support of functionality. Users
   are encouraged to use the `Blueprint Workshop <blueprint-workshop.datarobot.com>`_ instead of
   this class directly.
 - Added the arguments attribute in :class:`datarobot.CustomTaskVersion`.
 - Added the ability to retrieve detected errors in the potentially multicategorical feature types that prevented the
   feature to be identified as multicategorical.
@@ -1175,41 +1178,38 @@
 
 Bugfixes
 ********
 - fix :class:`datarobot.CustomTaskVersion` and :class:`datarobot.CustomModelVersion` to correctly format ``required_metadata_values``
   before sending them via API
 - Fixed response validation that could cause `DataError` when using :class:`datarobot.models.Dataset` for a dataset with a description that is an empty string.
 
-API Changes
+API changes
 ***********
 - :meth:`RelationshipsConfiguration.create <datarobot.models.RelationshipsConfiguration.create>` will include a
   new key ``data_source_id`` in `data_source` field when applicable
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``Model.get_all_labelwise_roc_curves`` has been removed.
   You can get the same information with multiple calls of
   :meth:`Model.get_labelwise_roc_curves <datarobot.models.Model.get_labelwise_roc_curves>`, one per data source.
 - ``Model.get_all_multilabel_lift_charts`` has been removed.
   You can get the same information with multiple calls of
   :meth:`Model.get_multilabel_lift_charts <datarobot.models.Model.get_multilabel_lift_charts>`, one per data source.
 
-Configuration Changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 - This release introduces a new documentation organization. The organization has been modified to better reflect the end-to-end modeling workflow. The new "Tutorials" section has 5 major topics that outline the major components of modeling: Data, Modeling, Predictions, MLOps, and Administration.
 - The Getting Started workflow is now hosted at `DataRobot's API Documentation Home <https://docs.datarobot.com/en/docs/api/index.html>`_.
 - Added an example of how to set up optimized datetime partitioning for time series projects.
 
 2.26.0
 ========
 
-New Features
+New features
 ************
 - Added the ability to use external baseline predictions for time series project. External
   dataset can be validated using :meth:`datarobot.models.Project.validate_external_time_series_baseline`.
   Option can be set in :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` to scale
   datarobot models' accuracy performance using external dataset's accuracy performance.
   See the :ref:`external baseline predictions documentation <external_baseline_predictions>`
   for more information.
@@ -1288,52 +1288,52 @@
 - :meth:`RelationshipsConfiguration.create <datarobot.models.RelationshipsConfiguration.create>` will return a ``catalog``
   in `data_source` field
 - Argument ``required_metadata_keys`` was not properly being sent in the update and create requests for
   :class:`datarobot.ExecutionEnvironment`.
 - Fix issue with :class:`datarobot.ExecutionEnvironment` create method failing when used against older versions of the application
 - :class:`datarobot.CustomTaskVersion` was not properly handling ``required_metadata_values`` from the API response
 
-API Changes
+API changes
 ***********
 
 - Updated :meth:`Project.start <datarobot.models.Project.start>` to use ``AUTOPILOT_MODE.QUICK`` when the
   ``autopilot_on`` param is set to True. This brings it in line with :meth:`Project.set_target
   <datarobot.models.Project.set_target>`.
 - Updated :meth:`project.start_autopilot <datarobot.models.Project.start_autopilot>` to accept
   the following new GA parameters that are already in the public API: ``consider_blenders_in_recommendation``,
   ``run_leakage_removed_feature_list``
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - The ``required_metadata`` property of :class:`datarobot.CustomModelVersion` has been deprecated.
   ``required_metadata_values`` should be used instead.
 
 - The ``required_metadata`` property of :class:`datarobot.CustomTaskVersion` has been deprecated.
   ``required_metadata_values`` should be used instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - Now requires dependency on package `scikit-learn <https://pypi.org/project/scikit-learn/>`_  rather than
   `sklearn <https://pypi.org/project/scikit-learn/>`_. Note: This dependency is only used in example code. See
   `this scikit-learn issue <https://github.com/scikit-learn/scikit-learn/issues/8215>`_ for more information.
 - Now permits dependency on package `attrs <https://pypi.org/project/attrs/>`_  to be less than version 21. This
   fixes compatibility with apache-airflow.
 
 - Allow to setup ``Authorization: <type> <token>`` type header for OAuth2 Bearer tokens.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Update the documentation with respect to the permission that controls AI Catalog dataset snapshot behavior.
 
 2.25.0
 ======
 
-New Features
+New features
 ************
 - There is a new :class:`AnomalyAssessmentRecord<datarobot.models.anomaly_assessment.AnomalyAssessmentRecord>` object that
   implements public API routes to work with anomaly assessment insight. This also adds explanations
   and predictions preview classes. The insight is available for anomaly detection models in time
   series unsupervised projects which also support calculation of Shapley values.
 
     - :class:`AnomalyAssessmentPredictionsPreview<datarobot.models.anomaly_assessment.AnomalyAssessmentPredictionsPreview>`
@@ -1418,15 +1418,15 @@
 
 - Ensure that if a configured endpoint ends in a trailing slash, the resulting full URL does
   not end up with double slashes in the path.
 
 - :meth:`Model.request_frozen_datetime_model <datarobot.models.Model.request_frozen_datetime_model>` is now implementing correct
   validation of input parameter ``training_start_date``.
 
-API Changes
+API changes
 ***********
 
 - Arguments ``secondary_datasets`` now accept :py:class:`SecondaryDataset <datarobot.helpers.feature_discovery.SecondaryDataset>`
   to create secondary dataset configurations
   - :meth:`SecondaryDatasetConfigurations.create <datarobot.models.SecondaryDatasetConfigurations.create>`
 
 - Arguments ``dataset_definitions`` and ``relationships`` now accept :py:class:`DatasetDefinition <datarobot.helpers.feature_discovery.DatasetDefinition>` :py:class:`Relationship <datarobot.helpers.feature_discovery.Relationship>`
@@ -1443,15 +1443,15 @@
 - Argument ``required_metadata`` has been added to :class:`datarobot.CustomModelVersion`.  This should be set with
   relevant values defined by the base environment's ``required_metadata_keys``
 
 
 2.24.0
 =========
 
-New Features
+New features
 ************
 
 - Partial history predictions can be made with time series time series multiseries models using the
   ``allow_partial_history_time_series_predictions`` attribute of the
   :py:class:`datarobot.DatetimePartitioningSpecification
   <datarobot.DatetimePartitioningSpecification>`.
   See the :ref:`Time Series <time_series>` documentation for more info.
@@ -1503,48 +1503,45 @@
 Bugfixes
 ********
 - Fixed response validation that could cause `DataError` when using
   :meth:`TrainingPredictions.list <datarobot.models.training_predictions.TrainingPredictions.list>` and
   :meth:`TrainingPredictions.get_all_as_dataframe <datarobot.models.training_predictions.TrainingPredictions.get_all_as_dataframe>`
   methods if there are training predictions computed with `explanation_algorithm`.
 
-API Changes
+API changes
 ***********
 - Remove `desired_memory` param from the following classes: :class:`datarobot.CustomInferenceModel`,
   :class:`datarobot.CustomModelVersion`, :class:`datarobot.CustomModelTest`
 - Remove ``desired_memory`` param from the following methods:
   :meth:`CustomInferenceModel.create <datarobot.CustomInferenceModel.create>`,
   :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>`,
   :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>`,
   :meth:`CustomModelTest.create <datarobot.CustomModelTest.create>` and
   :meth:`CustomModelTest.create <datarobot.CustomModelTest.create>`
 
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - class ``ComplianceDocumentation``
   will be deprecated in v2.24 and will be removed entirely in v2.27. Use
   :class:`AutomatedDocument<datarobot.models.automated_documentation.AutomatedDocument>`
   instead. To start off, see the
   :ref:`Automated Documentation overview<automated_documentation_overview>` for details.
 
-Configuration Changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 
 - Remove reference to S3 for :meth:`Project.upload_dataset <datarobot.models.Project.upload_dataset>` since it is not supported by the server
 
 
 2.23.0
 ======
 
-New Features
+New features
 ************
 - Calendars for time series projects can now be automatically generated by providing a country code to the method
   :meth:`CalendarFile.create_calendar_from_country_code<datarobot.CalendarFile.create_calendar_from_country_code>`.
   A list of allowed country codes can be retrieved using :meth:`CalendarFile.get_allowed_country_codes<datarobot.CalendarFile.get_allowed_country_codes>`
   For more information, see the :ref:`calendar documentation <preloaded_calendar_files>`.
 
 - Added `calculate_all_series`` param to
@@ -1631,49 +1628,49 @@
 - Using :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.download>` could in some circumstances
   result in a crash from trying to abort the job if it fails to start
 
 - Using :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.download>` or
   :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score_to_file>` would produce incomplete
   results in case a job was aborted while downloading. This will now raise an exception.
 
-API Changes
+API changes
 ***********
 - New ``sampling_method`` param in :meth:`Model.train_datetime <datarobot.models.Model.train_datetime>`,
   :meth:`Project.train_datetime <datarobot.models.Project.train_datetime>`,
   :meth:`Model.train_datetime <datarobot.models.Model.request_frozen_datetime_model>` and
   :meth:`Model.train_datetime <datarobot.models.Model.retrain>`.
 - New ``target_type`` param in :class:`datarobot.CustomInferenceModel`
 - New arguments ``secondary_datasets``, ``name``, ``creator_full_name``, ``creator_user_id``, ``created``,
     ``featurelist_id``, ``credentials_ids``, ``project_version`` and ``is_default`` in :class:`datarobot.models.SecondaryDatasetConfigurations`
 - New arguments ``secondary_datasets``, ``name``, ``featurelist_id`` to
     :meth:`SecondaryDatasetConfigurations.create <datarobot.models.SecondaryDatasetConfigurations.create>`
 - Class ``FeatureEngineeringGraph`` has been removed. Use :class:`datarobot.models.RelationshipsConfiguration` instead.
 - Param ``feature_engineering_graphs`` removed from :meth:`Project.set_target<datarobot.models.Project.set_target>`.
 - Param ``config`` removed from :meth:`SecondaryDatasetConfigurations.create<datarobot.models.SecondaryDatasetConfigurations.create>`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``supports_binary_classification`` and  ``supports_regression`` are deprecated
     for :class:`datarobot.CustomInferenceModel` and will be removed in v2.24
 - Argument ``config`` and  ``supports_regression`` are deprecated
     for :class:`datarobot.models.SecondaryDatasetConfigurations` and will be removed in v2.24
 - ``CustomInferenceImage`` has been deprecated and will be removed in v2.24.
     :class:`datarobot.CustomModelVersion` with base_environment_id should be used in their place.
 - ``environment_id`` and ``environment_version_id`` are deprecated for :meth:`CustomModelTest.create<datarobot.CustomModelTest.create>`
 
-Documentation Changes
+Documentation changes
 *********************
 
 - `feature_lineage_id` is added as a new parameter in the response for retrieval of a :class:`datarobot.models.Feature` created by automated feature discovery or time series feature derivation.
   This id is required to retrieve a :class:`datarobot.models.FeatureLineage` instance.
 
 2.22.1
 ======
 
-New Features
+New features
 ************
 
 - Batch Prediction jobs now support :ref:`dataset <batch_predictions-intake-types-dataset>` as intake settings for
   :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 
 - Create a Dataset from DataSource:
 
@@ -1764,40 +1761,34 @@
 
 - Make trafaret validator for datasets use a syntax that works properly with a wider range of trafaret versions.
 
 - Handle extra keys in CustomModelTests and CustomModelVersions
 
 - ``ImageEmbedding`` and ``ImageActivationMap`` now supports regression projects.
 
-API Changes
+API changes
 ***********
 
 - The default value for the ``mode`` param in :meth:`Project.set_target
   <datarobot.models.Project.set_target>` has been changed from ``AUTOPILOT_MODE.FULL_AUTO``
   to ``AUTOPILOT_MODE.QUICK``
 
-Deprecation Summary
-*******************
-
-Configuration Changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 
 - Added links to classes with duration parameters such as `validation_duration` and `holdout_duration` to
   provide duration string examples to users.
 
 - The :ref:`models documentation <models>` has been revised to include section on how to train a new model and how to run cross-validation
   or backtesting for a model.
 
 2.21.0
 ======
 
-New Features
+New features
 ************
 
 - Added new arguments ``explanation_algorithm`` and ``max_explanations`` to method
   :meth:`Model.request_training_predictions <datarobot.models.Model.request_training_predictions>`.
   New fields ``explanation_algorithm``, ``max_explanations`` and ``shap_warnings`` have been added to class
   :class:`TrainingPredictions <datarobot.models.training_predictions.TrainingPredictions>`.
   New fields ``prediction_explanations`` and ``shap_metadata`` have been added to class
@@ -1936,35 +1927,35 @@
 ********
 
 - An issue with input validation of the Batch Prediction module
 - parent_model_id was not visible for all frozen models
 - Batch Prediction jobs that used other output types than `local_file` failed when using `.wait_for_completion()`
 - A race condition in the Batch Prediction file scoring logic
 
-API Changes
+API changes
 ***********
 
 - Three new fields were added to the :class:`Dataset<datarobot.models.Dataset>` object. This reflects the
   updated fields in the public API routes at `api/v2/datasets/`. The added fields are:
 
     - processing_state: Current ingestion process state of the dataset
     - row_count: The number of rows in the dataset.
     - size: The size of the dataset as a CSV in bytes.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``datarobot.enums.VARIABLE_TYPE_TRANSFORM.CATEGORICAL`` for is deprecated for the following and will be removed in  v2.22.
     - meth:`Project.batch_features_type_transform`
     - meth:`Project.create_type_transform_feature`
 
 2.20.0
 ======
 
-New Features
+New features
 ************
 
 - There is a new :class:`Dataset<datarobot.models.Dataset>` object that implements some of the
   public API routes at `api/v2/datasets/`. This also adds two new feature classes and a details
   class.
 
     - :class:`DatasetFeature<datarobot.models.DatasetFeature>`
@@ -2054,30 +2045,18 @@
 ********
 - An issue where uploaded CSV's would loose quotes during serialization causing issues when columns containing line terminators where loaded in a dataframe, has been fixed
 
 - :meth:`Project.get_association_featurelists <datarobot.models.Project.get_association_featurelists>` is now using the correct endpoint name, but the old one will continue to work
 
 - Python API :class:`PredictionServer<datarobot.PredictionServer>` supports now on-premise format of API response.
 
-API Changes
-***********
-
-Deprecation Summary
-*******************
-
-Configuration Changes
-*********************
-
-Documentation Changes
-*********************
-
 2.19.0
 ======
 
-New Features
+New features
 ************
 
 - Projects can be cloned using :meth:`Project.clone_project <datarobot.models.Project.clone_project>`
 - Calendars used in time series projects now support having series-specific events, for instance if a holiday only affects some stores. This can be controlled by using new argument of the :meth:`CalendarFile.create <datarobot.CalendarFile.create>` method.
   If multiseries id columns are not provided, calendar is considered to be single series and all events are applied to all series.
 - We have expanded prediction intervals availability to the following use-cases:
 
@@ -2137,30 +2116,30 @@
     - ``order_by``: An attribute by which to sort the results
 
 
 Bugfixes
 ********
 - An issue when using :meth:`Feature.get <datarobot.models.Feature.get>` and :meth:`ModelingFeature.get <datarobot.models.ModelingFeature.get>` to retrieve summarized categorical feature has been fixed.
 
-API Changes
+API changes
 ***********
 - The datarobot package is now no longer a
   `namespace package <https://packaging.python.org/guides/packaging-namespace-packages/>`_.
 - ``datarobot.enums.BLENDER_METHOD.FORECAST_DISTANCE`` is removed (deprecated in 2.18.0).
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Updated :ref:`Residuals charts <residuals_chart>` documentation to reflect that the data rows include row numbers from the source dataset for projects
   created in DataRobot 5.3 and newer.
 
 2.18.0
 ======
 
-New Features
+New features
 ************
 - :ref:`Residuals charts <residuals_chart>` can now be retrieved for non-time-aware regression models.
 
 - :ref:`Deployment monitoring <deployment_monitoring>` can now be used to retrieve service stats, service health, accuracy info, permissions, and feature lists for deployments.
 
 - :ref:`Time series <time_series>` projects now support the Average by Forecast Distance blender, configured with more than one Forecast Distance. The blender blends the selected models, selecting the best three models based on the backtesting score for each Forecast Distance and averaging their predictions. The new blender method ``FORECAST_DISTANCE_AVG`` has been added to ``datarobot.enums.BLENDER_METHOD``.
 
@@ -2186,31 +2165,31 @@
 
 - Calls to :py:meth:`Project.start <datarobot.models.Project.start>` and :py:meth:`Project.upload_dataset <datarobot.models.Project.upload_dataset>` now support uploading data via S3 URI and `pathlib.Path` objects.
 
 - Errors upon connecting to DataRobot are now clearer when an incorrect API Token is used.
 
 - The datarobot package is now a `namespace package <https://packaging.python.org/guides/packaging-namespace-packages/>`_.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``datarobot.enums.BLENDER_METHOD.FORECAST_DISTANCE`` is deprecated and will be removed in 2.19. Use ``FORECAST_DISTANCE_ENET`` instead.
 
-Documentation Changes
+Documentation changes
 *********************
 - Various typo and wording issues have been addressed.
 
 - A new notebook showing regression-specific features is now been added to the :ref:`examples<examples_index>`.
 
 - Documentation for :ref:`Access lists <sharing>` has been added.
 
 2.17.0
 ======
 
-New Features
+New features
 ************
 - :ref:`Deployments <deployments_overview>` can now be managed via the API by using the new :py:class:`Deployment <datarobot.models.Deployment>` class.
 
 - Users can now list available prediction servers using :meth:`PredictionServer.list <datarobot.PredictionServer.list>`.
 
 - When :class:`specifying datetime partitioning <datarobot.DatetimePartitioningSpecification>` settings , :ref:`time series <time_series>` projects can now mark individual features as excluded from feature derivation using the
   :py:class:`FeatureSettings.do_not_derive <datarobot.FeatureSettings>` attribute. Any features not specified will be assigned according to the :py:class:`DatetimePartitioningSpecification.default_to_do_not_derive <datarobot.DatetimePartitioning>` value.
@@ -2237,23 +2216,23 @@
 
 Bugfixes
 ********
 - An issue affecting time series project creation for irregularly spaced dates has been fixed.
 - :class:`ComplianceDocTemplate <datarobot.models.compliance_doc_template.ComplianceDocTemplate>` now supports empty text blocks in user sections.
 - An issue when using :meth:`Predictions.get <datarobot.models.Predictions.get>` to retrieve predictions metadata has been fixed.
 
-Documentation Changes
+Documentation changes
 *********************
 - An overview on working with class ``ComplianceDocumentation`` and :class:`ComplianceDocTemplate <datarobot.models.compliance_doc_template.ComplianceDocTemplate>` has been created. :ref:`See here <automated_documentation_overview>` for more details.
 
 
 2.16.0
 ======
 
-New Features
+New features
 ************
 - Three new methods for Series Accuracy have been added to the :class:`DatetimeModel <datarobot.models.DatetimeModel>` class.
 
     - Start a request to calculate Series Accuracy with
       :meth:`DatetimeModel.compute_series_accuracy <datarobot.models.DatetimeModel.compute_series_accuracy>`
     - Once computed, Series Accuracy can be retrieved as a pandas.DataFrame using
       :meth:`DatetimeModel.get_series_accuracy_as_dataframe <datarobot.models.DatetimeModel.get_series_accuracy_as_dataframe>`
@@ -2277,15 +2256,15 @@
     - ``effective_feature_derivation_window_end``
     - ``forecast_window_start``
     - ``forecast_window_end``
     - ``windows_basis_unit``
 
 - Prediction metadata is now included in the return of :meth:`Predictions.get <datarobot.models.Predictions.get>`
 
-Documentation Changes
+Documentation changes
 *********************
 - Various typo and wording issues have been addressed.
 - The example data that was meant to accompany the Time Series examples has been added to the
   zip file of the download in the :ref:`examples<examples_index>`.
 
 2.15.1
 ======
@@ -2300,15 +2279,15 @@
 - Previously, attempting to retrieve the ``calendar_id`` of a project without a set target would result in an error.
   This has been fixed to return ``None`` instead.
 
 
 2.15.0
 ======
 
-New Features
+New features
 ************
 - Previously available for only Eureqa models, Advanced Tuning methods and objects, including
   :meth:`Model.start_advanced_tuning_session <datarobot.models.Model.start_advanced_tuning_session>`,
   :meth:`Model.get_advanced_tuning_parameters <datarobot.models.Model.get_advanced_tuning_parameters>`,
   :meth:`Model.advanced_tune <datarobot.models.Model.advanced_tune>`, and
   :class:`AdvancedTuningSession <datarobot.models.advanced_tuning.AdvancedTuningSession>`,
   now support all models other than blender, open source, and user-created models.  Use of
@@ -2331,60 +2310,57 @@
 * Information retrieval for :py:class:`ROC Curve <datarobot.models.roc_curve.RocCurve>` has been extended to include ``fraction_predicted_as_positive``, ``fraction_predicted_as_negative``, ``lift_positive`` and ``lift_negative``
 
 Bugfixes
 ********
 * Fixes an issue where the client would not be usable if it could not be sure it was compatible with the configured
   server
 
-API Changes
+API changes
 ***********
 - Methods for creating :py:class:`datarobot.models.Project`: `create_from_mysql`, `create_from_oracle`, and `create_from_postgresql`, deprecated in 2.11, have now been removed.
   Use :py:meth:`datarobot.models.Project.create_from_data_source` instead.
 - :py:class:`datarobot.FeatureSettings <datarobot.FeatureSettings>` attribute `apriori`, deprecated in 2.11, has been removed.
   Use :py:class:`datarobot.FeatureSettings.known_in_advance <datarobot.FeatureSettings>` instead.
 - :py:class:`datarobot.DatetimePartitioning <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, deprecated in 2.11, has been removed. Use
   :py:class:`datarobot.DatetimePartitioning.known_in_advance <datarobot.DatetimePartitioning>` instead.
 - :py:class:`datarobot.DatetimePartitioningSpecification <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, deprecated in 2.11, has been removed.
   Use :py:class:`datarobot.DatetimePartitioningSpecification.known_in_advance <datarobot.DatetimePartitioning>`
   instead.
 
-Deprecation Summary
-*******************
-
-Configuration Changes
+Configuration changes
 *********************
 - Now requires dependency on package `requests <https://pypi.org/project/requests/>`_  to be at least version 2.21.
 - Now requires dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be at least version 1.24.
 
-Documentation Changes
+Documentation changes
 *********************
 - Advanced model insights notebook extended to contain information on visualization of cumulative gains and lift charts.
 
 2.14.2
 ======
 
 Bugfixes
 ********
 - Fixed an issue where searches of the HTML documentation would sometimes hang indefinitely
 
-Documentation Changes
+Documentation changes
 *********************
 - Python3 is now the primary interpreter used to build the docs (this does not affect the ability to use the
   package with Python2)
 
 2.14.1
 ======
 
-Documentation Changes
+Documentation changes
 *********************
  - Documentation for the Model Deployment interface has been removed after the corresponding interface was removed in 2.13.0.
 
 2.14.0
 ======
-New Features
+New features
 ************
 - The new method :meth:`Model.get_supported_capabilities <datarobot.models.Model.get_supported_capabilities>`
   retrieves a summary of the capabilities supported by a particular model,
   such as whether it is eligible for Prime and whether it has word cloud data available.
 - New class for working with model compliance documentation feature of DataRobot:
   class ``ComplianceDocumentation``
 - New class for working with compliance documentation templates:
@@ -2424,32 +2400,32 @@
 - Timeseries projects can now accept feature derivation intervals, forecast windows, forecast points and prediction start/end dates in milliseconds.
 - :class:`DataSources <datarobot.DataSource>` and :class:`DataStores <datarobot.DataStore>` can now
   be :ref:`shared <sharing>` with other users.
 - Training predictions for datetime partitioned projects now support the new data subset
   `dr.enums.DATA_SUBSET.ALL_BACKTESTS` for requesting the predictions for all backtest validation
   folds.
 
-API Changes
-*******************
+API changes
+***********
 - The model recommendation type "Recommended" (deprecated in version 2.13.0) has been removed.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Example notebooks have been updated:
     - Notebooks now work in Python 2 and Python 3
     - A notebook illustrating time series capability has been added
     - The financial data example has been replaced with an updated introductory example.
 - To supplement the embedded Python notebooks in both the PDF and HTML docs bundles, the notebook files and supporting data can now be downloaded from the HTML docs bundle.
 - Fixed a minor typo in the code sample for ``get_or_request_feature_impact``
 
 2.13.0
 ======
 
-New Features
+New features
 ************
 - The new method :meth:`Model.get_or_request_feature_impact <datarobot.models.Model.get_or_request_feature_impact>` functionality will attempt to request feature impact
   and return the newly created feature impact object or the existing object so two calls are no longer required.
 - New methods and objects, including
   :meth:`Model.start_advanced_tuning_session <datarobot.models.Model.start_advanced_tuning_session>`,
   :meth:`Model.get_advanced_tuning_parameters <datarobot.models.Model.get_advanced_tuning_parameters>`,
   :meth:`Model.advanced_tune <datarobot.models.Model.advanced_tune>`, and
@@ -2492,52 +2468,52 @@
 
 Bugfixes
 ********
 - The Model Deployment interface which was previously visible in the client has been removed to
   allow the interface to mature, although the raw API is available as a "beta" API without full
   backwards compatibility support.
 
-API Changes
+API changes
 ***********
 - Added support for retrieving the Pareto Front of a Eureqa model. See
   :py:class:`ParetoFront <datarobot.models.pareto_front.ParetoFront>`.
 - A new recommendation type "Recommended for Deployment" has been added to
   :py:class:`ModelRecommendation <datarobot.models.ModelRecommendation>` which is now returns as the
   default recommended model when available. See :ref:`model_recommendation`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - The feature previously referred to as "Reason Codes" has been renamed to "Prediction
   Explanations", to provide increased clarity and accessibility. The old
   ReasonCodes interface has been deprecated and replaced with
   :py:class:`PredictionExplanations <datarobot.PredictionExplanations>`.
 - The recommendation type "Recommended" is deprecated and  will no longer be returned
   in v2.14 of the API.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Added a new documentation section :ref:`model_recommendation`.
 - Time series projects support multiseries as well as single series data. They are now documented in
   the :ref:`Time Series Projects <time_series>` documentation.
 
 2.12.0
 ======
 
-New Features
+New features
 ************
 - Some models now have Missing Value reports allowing users with access to uncensored blueprints to
   retrieve a detailed breakdown of how numeric imputation and categorical converter tasks handled
   missing values. See the :ref:`documentation <missing_values_report>` for more information on the
   report.
 
 2.11.0
 ======
 
-New Features
+New features
 ************
 - The new ``ModelRecommendation`` class can be used to retrieve the recommended models for a
   project.
 - A new helper method cross_validate was added to class Model. This method can be used to request
   Model's Cross Validation score.
 - Training a model with monotonic constraints is now supported. Training with monotonic
   constraints allows users to force models to learn monotonic relationships with respect to some features and the target. This helps users create accurate models that comply with regulations (e.g. insurance, banking). Currently, only certain blueprints (e.g. xgboost) support this feature, and it is only supported for regression and binary classification projects.
@@ -2547,51 +2523,51 @@
   a list of databases with tested support for DataRobot is available in the user guide
   in the web application. See :ref:`Database Connectivity <database_connectivity_overview>`
   for details.
 - Added a new feature to retrieve feature logs for time series projects. Check
   :py:meth:`datarobot.DatetimePartitioning.feature_log_list` and
   :py:meth:`datarobot.DatetimePartitioning.feature_log_retrieve` for details.
 
-API Changes
+API changes
 ***********
 - New attributes supporting monotonic constraints have been added to the
   :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>`,
   :py:class:`Project <datarobot.models.Project>`,
   :py:class:`Model <datarobot.models.Model>`, and :py:class:`Blueprint <datarobot.models.Blueprint>`
   classes. See :ref:`monotonic constraints<monotonic_constraints>` for more information on how to
   configure monotonic constraints.
 - New parameters `predictions_start_date` and `predictions_end_date` added to
   :py:meth:`Project.upload_dataset <datarobot.models.Project.upload_dataset>` to support bulk
   predictions upload for time series projects.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Methods for creating :py:class:`datarobot.models.Project`: `create_from_mysql`, `create_from_oracle`, and `create_from_postgresql`, have been deprecated and will be removed in 2.14.
   Use :py:meth:`datarobot.models.Project.create_from_data_source` instead.
 - :py:class:`datarobot.FeatureSettings <datarobot.FeatureSettings>` attribute `apriori`, has been deprecated and will be removed in 2.14.
   Use :py:class:`datarobot.FeatureSettings.known_in_advance <datarobot.FeatureSettings>` instead.
 - :py:class:`datarobot.DatetimePartitioning <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, has been deprecated and will be removed in 2.14.
   :py:class:`datarobot.DatetimePartitioning.known_in_advance <datarobot.DatetimePartitioning>` instead.
 - :py:class:`datarobot.DatetimePartitioningSpecification <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, has been deprecated and will be removed in 2.14.
   Use :py:class:`datarobot.DatetimePartitioningSpecification.known_in_advance <datarobot.DatetimePartitioning>`
   instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - Retry settings compatible with those offered by urllib3's `Retry <https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#urllib3.util.retry.Retry>`_
   interface can now be configured. By default, we will now retry connection errors that prevented requests from arriving at the server.
 
-Documentation Changes
+Documentation changes
 *********************
 - "Advanced Model Insights" example has been updated to properly handle bin weights when rebinning.
 
 2.9.0
 =====
 
-New Features
+New features
 ************
 - New ``ModelDeployment`` class can be used to track status and health of models deployed for
   predictions.
 
 Enhancements
 ************
 - DataRobot API now supports creating 3 new blender types - Random Forest, TensorFlow, LightGBM.
@@ -2616,15 +2592,15 @@
   :py:class:`datarobot.DatetimePartitioningSpecification` class to fine-tune how time-series projects
   derive modeling features. `treat_as_exponential` can control whether data is analyzed as
   an exponential trend and transformations like log-transform are applied.
   `differencing_method` can control which differencing method to use for stationary data.
   `periodicities` can be used to specify periodicities occurring within the data.
   All are optional and defaults will be chosen automatically if they are unspecified.
 
-API Changes
+API changes
 ***********
 - Now ``training_row_count`` is available on non-datetime models as well as "rowCount" based
   datetime models. It reports the number of rows used to train the model (equivalent to
   ``sample_pct``).
 - Features retrieved from ``Feature.get`` now include ``target_leakage``.
 
 2.8.1
@@ -2639,15 +2615,15 @@
 - Version of ``trafaret`` library this package depends on is now pinned to ``trafaret>=0.7,<1.1``
   since versions outside that range are known to be incompatible.
 
 
 2.8.0
 =====
 
-New Features
+New features
 ************
 - The DataRobot API supports the creation, training, and predicting of multiclass classification
   projects. DataRobot, by default, handles a dataset with a numeric target column as regression.
   If your data has a numeric cardinality of fewer than 11 classes, you can override this behavior to
   instead create a multiclass classification project from the data. To do so, use the set_target
   function, setting target_type='Multiclass'. If DataRobot recognizes your data as categorical, and
   it has fewer than 11 classes, using multiclass will create a project that classifies which label
@@ -2691,39 +2667,39 @@
   parameter 'events_count' as a part of the AdvancedOptions object to allow specifying the
   events count column. See the user guide documentation in the webapp for more information
   on events count.
 - PredictJob.get_predictions now returns predicted probability for each class in the dataframe.
 - PredictJob.get_predictions now accepts prefix parameter to prefix the classes name returned in the
   predictions dataframe.
 
-API Changes
+API changes
 ***********
 - Add `target_type` parameter to set_target() and start(), used to override the project default.
 
 2.7.2
 =====
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Updated link to the publicly hosted documentation.
 
 2.7.1
 =====
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Online documentation hosting has migrated from PythonHosted to Read The Docs. Minor code changes
   have been made to support this.
 
 2.7.0
 =====
 
-New Features
+New features
 ************
 - Lift chart data for models can be retrieved using the `Model.get_lift_chart` and
   `Model.get_all_lift_charts` methods.
 - ROC curve data for models in classification projects can be retrieved using the
   `Model.get_roc_curve` and `Model.get_all_roc_curves` methods.
 - Semi-automatic autopilot mode is removed.
 - Word cloud data for text processing models can be retrieved using `Model.get_word_cloud` method.
@@ -2737,38 +2713,38 @@
   showing the coefficients for individual stages of multistage models (e.g. Frequency-Severity
   models).
 - When training a `DatetimeModel` on a window of data, a `time_window_sample_pct` can be specified
   to take a uniform random sample of the training data instead of using all data within the window.
 - Installing of DataRobot package now has an "Extra Requirements" section that will install all of
   the dependencies needed to run the example notebooks.
 
-Documentation Changes
+Documentation changes
 *********************
 - A new example notebook describing how to visualize some of the newly available model insights
   including lift charts, ROC curves, and word clouds has been added to the examples section.
 - A new section for `Common Issues` has been added to `Getting Started` to help debug issues related to client installation and usage.
 
 
 2.6.1
 =====
 
 Bugfixes
 ********
 
 - Fixed a bug with `Model.get_parameters` raising an exception on some valid parameter values.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Fixed sorting order in Feature Impact example code snippet.
 
 2.6.0
 =====
 
-New Features
+New features
 ************
 - A new partitioning method (datetime partitioning) has been added. The recommended workflow is to
   preview the partitioning by creating a `DatetimePartitioningSpecification` and passing it into
   `DatetimePartitioning.generate`, inspect the results and adjust as needed for the specific project
   dataset by adjusting the `DatetimePartitioningSpecification` and re-generating, and then set the
   target by passing the final `DatetimePartitioningSpecification` object to the partitioning_method
   parameter of `Project.set_target`.
@@ -2815,24 +2791,24 @@
 ********
 
 - Fixed a bug (affecting Python 2 only) with printing any model (including frozen and prime models)
   whose model_type is not ascii.
 - FrozenModels were unable to correctly use methods inherited from Model. This has been fixed.
 - When calling `get_result` for a Job, ModelJob, or PredictJob that has errored, `AsyncProcessUnsuccessfulError` will now be raised instead of `JobNotFinished`, consistently with the behavior of `get_result_when_complete`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - Support for the experimental Recommender Problems projects has been removed. Any code relying on
   `RecommenderSettings` or the `recommender_settings` argument of `Project.set_target` and
   `Project.start` will error.
 - ``Project.update``, deprecated in v2.2.32, has been removed in favor of specific updates:
   ``rename``, ``unlock_holdout``, ``set_worker_count``.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - The link to Configuration from the Quickstart page has been fixed.
 
 2.5.1
 =====
 
@@ -2844,15 +2820,15 @@
 - Fixed an issue where the weights column (for weighted projects) did not appear
   in the `advanced_options` of a `Project`.
 
 
 2.5.0
 =====
 
-New Features
+New features
 ************
 
 - Methods to work with blender models have been added. Use `Project.blend` method to create new blenders,
   `Project.get_blenders` to get the list of existing blenders and `BlenderModel.get` to retrieve a model
   with blender-specific information.
 - Projects created via the API can now use smart downsampling when setting the target by passing
   `smart_downsampled` and `majority_downsampling_rate` into the `AdvancedOptions` object used with
@@ -2871,15 +2847,15 @@
 - When specifying the API endpoint in the configuration, the client will now behave correctly for
   endpoints with and without trailing slashes.
 
 
 2.4.0
 =====
 
-New Features
+New features
 ************
 
 - The premium add-on product `DataRobot Prime` has been added. You can now approximate a model
   on the leaderboard and download executable code for it. See documentation for further details, or
   talk to your account representative if the feature is not available on your account.
 - (Only relevant for on-premise users with a Standalone Scoring cluster.) Methods
   (`request_transferable_export` and `download_export`) have been added to the `Model` class for exporting models (which will only work if model export is turned on). There is a new class `ImportedModel` for managing imported models on a Standalone
@@ -2900,50 +2876,50 @@
 
 Bugfixes
 ********
 
 - Fixed an issue where `Model.request_predictions` might raise an error when predictions finished
   very quickly instead of returning the job.
 
-API Changes
+API changes
 ***********
 
 - To set the target with quickrun autopilot, call `Project.set_target` with `mode=AUTOPILOT_MODE.QUICK` instead of
   specifying `quickrun=True`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - Semi-automatic mode for autopilot has been deprecated and will be removed in 3.0.
   Use manual or fully automatic instead.
 - Use of the `quickrun` argument in `Project.set_target` has been deprecated and will be removed in
   3.0. Use `mode=AUTOPILOT_MODE.QUICK` instead.
 
-Configuration Changes
+Configuration changes
 *********************
 
 - It is now possible to control the SSL certificate verification by setting the parameter
   `ssl_verify` in the config file.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - The "Modeling Airline Delay" example notebook has been updated to work with the new 2.3
   enhancements.
 - Documentation for the generic `Job` class has been added.
 - Class attributes are now documented in the `API Reference` section of the documentation.
 - The changelog now appears in the documentation.
 - There is a new section dedicated to configuration, which lists all of the configuration
   options and their meanings.
 
 
 2.3.0
 =====
 
-New Features
+New features
 ************
 
 - The DataRobot API now includes Feature Impact, an approach to measuring the relevance of each feature
   that can be applied to any model. The `Model` class now includes methods `request_feature_impact`
   (which creates and returns a feature impact job) and `get_feature_impact` (which can retrieve completed feature impact results).
 - A new improved workflow for predictions now supports first uploading a dataset via `Project.upload_dataset`,
   then requesting predictions via `Model.request_predictions`. This allows us to better support predictions on
@@ -2996,27 +2972,27 @@
 
 Bugfixes
 ********
 
 - Fixed a bug (affecting Python 2 only) with printing features and featurelists whose names are
   not ascii.
 
-API Changes
+API changes
 ***********
 
 - Job class hierarchy is rearranged to better express the relationship between these objects. See
   documentation for `datarobot.models.job` for details.
 - `Featurelist` objects now have a `project_id` attribute to indicate which project they belong
   to. Directly accessing the `project` attribute of a `Featurelist` object is now deprecated
 - Support INI-style configuration, which was deprecated in v2.1, has been removed. yaml is the only supported
   configuration format.
 - The method `Project.get_jobs` method, which was deprecated in v2.1, has been removed. Users should use
   the `Project.get_model_jobs` method instead to get the list of model jobs.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - `PredictJob.create` has been deprecated in favor of the alternate workflow using `Model.request_predictions`.
 - Feature.converter (used internally for object construction) has been made private.
 - Model.fetch_resource_data has been deprecated and will be removed in 3.0. To fetch a model from
    its ID, use Model.get.
 - The ability to use Feature.get with feature IDs (rather than names) is deprecated and will
@@ -3028,15 +3004,15 @@
   attribute of a `Featurelist` to instantiate a `Project` instance using `Project.get`.
 - Use of the attributes `Model.project`, `Model.blueprint`, and `Model.featurelist` are all deprecated now
   to avoid use of partially instantiated objects. Please use the ids of these objects instead.
 - Using a `Project` instance as an argument in `Featurelist.get` is now deprecated.
   Please use a project_id instead. Similarly, using a `Project` instance in `Model.get` is also deprecated,
   and a project_id should be used in its place.
 
-Configuration Changes
+Configuration changes
 *********************
 
 - Previously it was possible (though unintended) that the client configuration could be mixed through
   environment variables, configuration files, and arguments to `datarobot.Client`. This logic is now
   simpler - please see the `Getting Started` section of the documentation for more information.
 
 
@@ -3056,15 +3032,15 @@
 - Fixed a bug (affecting Python 2 only) with printing projects, features, and featurelists whose names are
   not ascii.
 
 
 2.2.32
 ======
 
-New Features
+New features
 ************
 
 - ``Project.get_features`` and ``Feature.get`` methods have been added for feature retrieval.
 - A generic ``Job`` entity has been added for use in retrieving the entire queue at once. Calling
   ``Project.get_all_jobs`` will retrieve all (appropriately filtered) jobs from the queue. Those
   can be cancelled directly as generic jobs, or transformed into instances of the specific
   job class using ``ModelJob.from_job`` and ``PredictJob.from_job``, which allow all functionality
@@ -3089,15 +3065,15 @@
 ********
 
 - Fixed an issue where updating the global client would not affect existing objects with cached clients.
   Now the global client is used for every API call.
 - An issue where mistyping a filepath for use in a file upload has been resolved. Now an error will be
   raised if it looks like the raw string content for modeling or predictions is just one single line.
 
-API Changes
+API changes
 ***********
 
 - Use of username and password to authenticate is no longer supported - use an API token instead.
 - Usage of ``start_time`` and ``finish_time`` parameters in ``Project.get_models`` is not
   supported both in filtering and ordering of models
 - Default value of ``sample_pct`` parameter of ``Model.train`` method is now ``None`` instead of ``100``.
   If the default value is used, models will be trained with all of the available *training* data based on
@@ -3107,21 +3083,21 @@
 - ``recommendation_settings`` parameter of ``Project.start`` which was deprecated in v0.2 has been removed.
 - ``Project.status`` method which was deprecated in v0.2 has been removed.
 - ``Project.wait_for_aim_stage`` method which was deprecated in v0.2 has been removed.
 - ``Delay``, ``ConstantDelay``, ``NoDelay``, ``ExponentialBackoffDelay``, ``RetryManager``
   classes from ``retry`` module which were deprecated in v2.1 were removed.
 - Package renamed to ``datarobot``.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``Project.update`` deprecated in favor of specific updates:
   ``rename``, ``unlock_holdout``, ``set_worker_count``.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - A new use case involving financial data has been added to the ``examples`` directory.
 - Added documentation for the partition methods.
 
 2.1.31
 ======
@@ -3151,15 +3127,15 @@
 
 - Minimal used version of ``requests_toolbelt`` package changed from 0.4 to 0.6
 
 
 2.1.28
 ======
 
-New Features
+New features
 ************
 
 - Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
 - Allow `config_path` argument to client
 - ``wait_for_autopilot`` method added to Project. This method can be used to
   block execution until autopilot has finished running on the project.
 - Support for specifying which featurelist to use with initial autopilot in
@@ -3178,26 +3154,26 @@
   and decide if they would like to resume waiting for async process to resolve
 
 Enhancements
 ************
 
 - ``AUTOPILOT_MODE`` enum now uses string names for autopilot modes instead of numbers
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``ConstantDelay``, ``NoDelay``, ``ExponentialBackoffDelay``, and ``RetryManager`` utils are now deprecated
 - INI-style config files are now deprecated (in favor of YAML config files)
 - Several functions in the `utils` submodule are now deprecated (they are
   being moved elsewhere and are not considered part of the public interface)
 - ``Project.get_jobs`` has been renamed ``Project.get_model_jobs`` for clarity and deprecated
 - Support for the experimental date partitioning has been removed in DataRobot API,
   so it is being removed from the client immediately.
 
-API Changes
+API changes
 ***********
 
 - In several places where ``AppPlatformError`` was being raised, now ``TypeError``, ``ValueError`` or
   ``InputNotUnderstoodError`` are now used. With this change, one can now safely assume that when
   catching an ``AppPlatformError`` it is because of an unexpected response from the server.
 - ``AppPlatformError`` has gained a two new attributes, ``status_code`` which is the HTTP status code
   of the unexpected response from the server, and ``error_code`` which is a DataRobot-defined error
@@ -3212,21 +3188,21 @@
   have the status_code of the unexpected response from the server, and the location that was being
   polled to wait for the asynchronous process to resolve.
 
 
 2.0.27
 ======
 
-New Features
+New features
 ************
 
 - ``PredictJob`` class was added to work with prediction jobs
 - ``wait_for_async_predictions`` function added to `predict_job` module
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - The `order_by` parameter of the ``Project.list`` is now deprecated.
 
 
 0.2.26
 ======
@@ -3238,15 +3214,15 @@
   keeping the client side in sync with the state of the project on the
   server
 - ``Project.create_featurelist`` now throws ``DuplicateFeaturesError``
   exception if passed list of features contains duplicates
 - ``Project.get_models`` now supports snake_case arguments to its
   order_by keyword
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``Project.wait_for_aim_stage`` is now deprecated, as the REST Async
   flow is a more reliable method of determining that project creation has
   completed successfully
 - ``Project.status`` is deprecated in favor of ``Project.get_status``
 - ``recommendation_settings`` parameter of ``Project.start`` is
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/LICENSE.txt` & `datarobot_early_access-3.4.0.2024.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/PKG-INFO` & `datarobot_early_access-3.4.0.2024.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.4.0.2024.4.1
+Version: 3.4.0.2024.4.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/README.md` & `datarobot_early_access-3.4.0.2024.4.8/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/common_setup.py` & `datarobot_early_access-3.4.0.2024.4.8/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/__init__.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_compat.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/chunking_service.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/chunking_service.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/dataset.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/enums.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     """Text embedding model names for VectorDatabases."""
 
     E5_LARGE_V2 = "intfloat/e5-large-v2"
     E5_BASE_V2 = "intfloat/e5-base-v2"
     MULTILINGUAL_E5_BASE = "intfloat/multilingual-e5-base"
     ALL_MINILM_L6_V2 = "sentence-transformers/all-MiniLM-L6-v2"
     JINA_EMBEDDING_T_EN_V1 = "jinaai/jina-embedding-t-en-v1"
+    SUP_SIMCSE_JA_BASE = "cl-nagoya/sup-simcse-ja-base"
 
 
 class VectorDatabaseChunkingMethod(StrEnum):
     """Text chunking method names for VectorDatabases."""
 
     RECURSIVE = "recursive"
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat_prompt.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,36 @@
         t.Key("custom_model_id", optional=True): t.Or(t.String, t.Null),
         t.Key("evaluation_dataset_configuration_id", optional=True): t.Or(t.String, t.Null),
         t.Key("cost_configuration_id", optional=True): t.Or(t.String, t.Null),
     }
 ).ignore_extra("*")
 
 
+feedback_result_trafaret = t.Dict(
+    {
+        t.Key("positive_user_ids"): t.List(t.String),
+        t.Key("negative_user_ids"): t.List(t.String),
+    }
+)
+
+
 result_metadata_trafaret = t.Dict(
     {
         t.Key("cost", optional=True): t.Or(t.Float, t.Null),
         t.Key("output_token_count"): t.Int,
         t.Key("input_token_count"): t.Int,
         t.Key("total_token_count"): t.Int,
         t.Key("estimated_docs_token_count"): t.Int,
         t.Key("latency_milliseconds"): t.Int,
         t.Key("error_message", optional=True): t.Or(t.String, t.Null),
+        t.Key("feedback_result"): feedback_result_trafaret,
+        t.Key("metrics"): t.List(metric_metadata_trafaret),
+        t.Key("final_prompt"): t.Or(
+            t.String, t.Dict().allow_extra("*"), t.List(t.Dict().allow_extra("*")), t.Null
+        ),
     }
 ).ignore_extra("*")
 
 
 confidence_scores_trafaret = t.Dict(
     {
         t.Key("rouge"): t.Float,
@@ -159,14 +172,36 @@
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(feedback={self.feedback})"
 
     def to_dict(self) -> FeedbackMetadataDict:
         return {"feedback": self.feedback}
 
 
+class FeedbackResult(APIObject):
+    """
+    Feedback associated with a chat prompt.
+
+    Attributes
+    ----------
+    positive_user_ids : List[str]
+        The IDs of the users providing positive feedback.
+    negative_user_ids : List[str]
+        The IDs of the users providing negative feedback.
+    """
+
+    _converter = feedback_result_trafaret
+
+    def __init__(self, positive_user_ids: List[str], negative_user_ids: List[str]):
+        self.positive_user_ids = positive_user_ids
+        self.negative_user_ids = negative_user_ids
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}"
+
+
 class MetricMetadata(APIObject):
     """
     Metadata for the custom metrics associated with a chat prompt.
 
     Attributes
     ----------
     name : str
@@ -237,14 +272,20 @@
         retrieved from a vector database, if any.
     total_token_count : int
         The total number of tokens processed.
     estimated_docs_token_count : int
         The estimated number of tokens from the documents retrieved from a vector database, if any.
     latency_milliseconds : int
         The latency of the chat prompt submission in milliseconds.
+    feedback_result : FeedbackResult
+        The lists of user_ids providing positive and negative feedback.
+    metrics : MetricMetadata
+        The evaluation metrics for this prompt.
+    final_prompt : Optional[Union[str, dict]], optional
+        Representation of the final prompt sent to the LLM.
     error_message : str or None, optional
         The error message from the LLM response.
     cost : float or None, optional
         The cost of the chat prompt submission.
     """
 
     _converter = result_metadata_trafaret
@@ -252,24 +293,32 @@
     def __init__(
         self,
         output_token_count: int,
         input_token_count: int,
         total_token_count: int,
         estimated_docs_token_count: int,
         latency_milliseconds: int,
+        feedback_result: Dict[str, Any],
+        metrics: List[Dict[str, Any]],
+        final_prompt: Optional[Union[str, Dict[str, Any], List[Dict[str, Any]]]] = None,
         error_message: Optional[str] = None,
         cost: Optional[float] = None,
     ):
         self.output_token_count = output_token_count
         self.input_token_count = input_token_count
         self.total_token_count = total_token_count
         self.estimated_docs_token_count = estimated_docs_token_count
         self.latency_milliseconds = latency_milliseconds
         self.error_message = error_message
         self.cost = cost
+        self.feedback_result = FeedbackResult.from_server_data(feedback_result)
+        self.metrics = [
+            MetricMetadata.from_server_data(metric_metadata) for metric_metadata in metrics
+        ]
+        self.final_prompt = final_prompt
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(output_token_count={self.output_token_count}, "
             f"input_token_count={self.input_token_count}, "
             f"total_token_count={self.total_token_count}, "
             f"estimated_docs_token_count={self.estimated_docs_token_count}, "
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_chat.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_chat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_prompt.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_prompt.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_llm_validation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_llm_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_validation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         ),
         t.Key("tenant_id"): t.String,
         t.Key("user_id"): t.String,
         t.Key("creation_date"): t.String,
         t.Key("error_message", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("deployment_name", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("user_name", optional=True, default=None): t.Or(t.Null, t.String),
+        t.Key("use_case_id", optional=True, default=None): t.Or(t.Null, t.String),
     }
 ).ignore_extra("*")
 
 
 class CustomModelValidation(APIObject):
     """
     Validation record checking the ability of the deployment to serve
@@ -100,14 +101,16 @@
         - authorization_header - Second of two auth headers for the prediction server.
         - input_type - Either JSON or CSV - input type model expects.
         - model_type - Target type of deployed custom model.
     tenant_id : str
         Creating user's tenant ID.
     error_message : Optional[str]
         Additional information for errored validation.
+    use_case_id : Optional[str]
+        The ID of the use case associated with the validation.
     """
 
     _path: str
     _converter = custom_model_validation_trafaret
 
     def __init__(
         self,
@@ -121,14 +124,15 @@
         tenant_id: str,
         name: str,
         creation_date: str,
         user_id: str,
         error_message: Optional[str],
         deployment_name: Optional[str],
         user_name: Optional[str],
+        use_case_id: Optional[str],
     ):
         self.id = id
         self.prompt_column_name = prompt_column_name
         self.target_column_name = target_column_name
         self.deployment_id = deployment_id
         self.model_id = model_id
         self.validation_status = validation_status
@@ -136,14 +140,15 @@
         self.tenant_id = tenant_id
         self.error_message = error_message
         self.name = name
         self.creation_date = creation_date
         self.user_id = user_id
         self.deployment_name = deployment_name
         self.user_name = user_name
+        self.use_case_id = use_case_id
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id})"
 
     @classmethod
     def get(cls, validation_id: str) -> CustomModelValidation:
         """
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm_blueprint.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm_blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/playground.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/playground.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         t.Key("description"): t.String(allow_blank=True),
         t.Key("use_case_id"): t.String,
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
         t.Key("last_update_date"): t.String,
         t.Key("last_update_user_id"): t.String,
         t.Key("saved_llm_blueprints_count"): t.Int,
+        t.Key("llm_blueprints_count"): t.Int,
+        t.Key("user_name"): t.String,
     }
 ).ignore_extra("*")
 
 
 class Playground(APIObject):
     """
     Metadata for a DataRobot GenAI playground.
@@ -55,14 +57,18 @@
         ID of the creating user.
     last_update_date : str
         Date when the playground was most recently updated.
     last_update_user_id : str
         ID of the user who most recently updated the playground.
     saved_llm_blueprints_count : int
         Number of saved LLM blueprints in the playground.
+    llm_blueprints_count : int
+        Number of LLM blueprints in the playground.
+    user_name : str
+        The name of the user who created the playground.
     """
 
     _path = "api-gw/genai/playgrounds"
 
     _converter = playground_trafaret
 
     def __init__(
@@ -72,24 +78,28 @@
         description: str,
         use_case_id: str,
         creation_date: str,
         creation_user_id: str,
         last_update_date: str,
         last_update_user_id: str,
         saved_llm_blueprints_count: int,
+        llm_blueprints_count: int,
+        user_name: str,
     ):
         self.id = id
         self.name = name
         self.description = description
         self.use_case_id = use_case_id
         self.creation_date = creation_date
         self.creation_user_id = creation_user_id
         self.last_update_date = last_update_date
         self.last_update_user_id = last_update_user_id
         self.saved_llm_blueprints_count = saved_llm_blueprints_count
+        self.llm_blueprints_count = llm_blueprints_count
+        self.user_name = user_name
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id}, name={self.name})"
 
     @classmethod
     def create(
         cls,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/user_limits.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/user_limits.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/vector_database.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/vector_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,28 @@
         t.Key("embedding_model"): str,
         t.Key("description"): str,
         t.Key("max_sequence_length"): int,
         t.Key("languages"): str,
     }
 ).ignore_extra("*")
 
+supported_custom_model_embeddings_trafaret = t.Dict(
+    {
+        t.Key("id"): t.String,
+        t.Key("name"): t.String,
+    }
+)
+
 supported_embeddings_trafaret = t.Dict(
     {
         t.Key("embedding_models"): t.List(embedding_model_trafaret),
         t.Key("default_embedding_model"): t.String,
+        t.Key("custom_model_embedding_validations"): t.List(
+            supported_custom_model_embeddings_trafaret
+        ),
     }
 ).ignore_extra("*")
 
 text_chunking_parameter_fields_trafaret = t.Dict(
     {
         t.Key("name"): t.String,
         t.Key("type"): t.String,
@@ -123,14 +133,16 @@
         t.Key("execution_status"): t.String,
         t.Key("playgrounds_count"): t.Int,
         t.Key("dataset_name"): t.String(allow_blank=True),
         t.Key("user_name"): t.String,
         t.Key("source"): t.String,
         t.Key("validation_id", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("error_message", optional=True, default=None): t.Or(t.Null, t.String),
+        t.Key("embedding_validation_id", optional=True, default=None): t.Or(t.Null, t.String),
+        t.Key("is_separator_regex"): t.Bool,
     }
 ).ignore_extra("*")
 
 
 class ChunkingParameters(APIObject):
     """
     Parameters defining how documents are split and embedded.
@@ -201,14 +213,37 @@
     ):
         self.embedding_model = embedding_model
         self.description = description
         self.max_sequence_length = max_sequence_length
         self.languages = languages
 
 
+class SupportedCustomModelEmbeddings(APIObject):
+    """
+    All supported custom embedding models for the use case.
+
+    Attributes
+    ----------
+    id : str
+        ID of the custom model embedding validation.
+    name : str
+        The name of the custom model embedding validation.
+    """
+
+    _converter = supported_custom_model_embeddings_trafaret
+
+    def __init__(
+        self,
+        id: str,
+        name: str,
+    ):
+        self.id = id
+        self.name = name
+
+
 class SupportedEmbeddings(APIObject):
     """
     All supported embedding models including the recommended default model.
 
     Attributes
     ----------
     embedding_models : list[EmbeddingModel]
@@ -221,19 +256,24 @@
 
     _converter = supported_embeddings_trafaret
 
     def __init__(
         self,
         embedding_models: List[Dict[str, Any]],
         default_embedding_model: str,
+        custom_model_embedding_validations: List[Dict[str, Any]],
     ):
         self.embedding_models = [
             EmbeddingModel.from_server_data(model) for model in embedding_models
         ]
         self.default_embedding_model = default_embedding_model
+        self.custom_model_embedding_validations = [
+            SupportedCustomModelEmbeddings.from_server_data(validation)
+            for validation in custom_model_embedding_validations
+        ]
 
 
 class TextChunkingParameterFields(APIObject):
     """
     Text chunking parameter fields.
 
     Attributes
@@ -412,14 +452,18 @@
         Currently supported options are listed in VectorDatabaseSource
         but the values can differ with different platform versions.
     validation_id : Optional[str]
         ID of custom model vector database validation.
         Only filled for external vector databases.
     error_message : Optional[str]
         Additional information for errored vector database.
+    embedding_validation_id : Optional[str]
+        ID of the custom embedding validation, if any.
+    is_separator_regex : bool
+        Whether the separators should be treated as regular expressions.
     """
 
     _path = "api-gw/genai/vectorDatabases"
 
     _converter = vector_database_trafaret
 
     def __init__(
@@ -443,14 +487,16 @@
         execution_status: str,
         playgrounds_count: int,
         dataset_name: str,
         user_name: str,
         source: str,
         validation_id: Optional[str],
         error_message: Optional[str],
+        embedding_validation_id: Optional[str],
+        is_separator_regex: bool,
     ):
         self.id = id
         self.name = name
         self.size = size
         self.use_case_id = use_case_id
         self.dataset_id = dataset_id
         self.embedding_model = embedding_model
@@ -467,14 +513,16 @@
         self.execution_status = execution_status
         self.playgrounds_count = playgrounds_count
         self.dataset_name = dataset_name
         self.user_name = user_name
         self.source = source
         self.validation_id = validation_id
         self.error_message = error_message
+        self.embedding_validation_id = embedding_validation_id
+        self.is_separator_regex = is_separator_regex
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(id={self.id}, name={self.name}, "
             f"execution_status={self.execution_status})"
         )
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/incremental_learning.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/incremental_learning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/notebooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,24 +23,26 @@
 from datarobot._experimental.models.enums import (
     NotebookPermissions,
     NotebookStatus,
     NotebookType,
     RunType,
     ScheduledRunStatus,
 )
+from datarobot.errors import InvalidUsageError
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject
 from datarobot.models.use_cases.utils import resolve_use_cases, UseCaseLike
 from datarobot.utils import assert_single_parameter
 from datarobot.utils.pagination import unpaginate
 
 
 class ManualRunPayload(TypedDict, total=False):
     notebook_id: str
     title: Optional[str]
+    notebook_path: Optional[str]
     parameters: Optional[List[Dict[str, str]]]
 
 
 notebook_user_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("activated"): t.Bool,
@@ -89,14 +91,15 @@
         t.Key("org_id"): t.String,
         t.Key("use_case_id"): t.String,
         t.Key("notebook_id"): t.String,
         t.Key("notebook_name"): t.String,
         t.Key("run_type"): t.String,
         t.Key("notebook_type"): t.String,
         t.Key("parameters"): t.List(scheduled_job_param_trafaret),
+        t.Key("notebook_path", optional=True): t.String,
     }
 )
 
 
 scheduled_run_revision_metadata_trafaret = t.Dict(
     {
         t.Key("id", optional=True): t.String,
@@ -399,37 +402,41 @@
         The name of Notebook being run on a schedule.
     run_type : RunType
         The type of the run - either manual (triggered via UI or API) or scheduled.
     notebook_type: NotebookType
         The type of the notebook - either plain or codespace.
     parameters : List[ScheduledJobParam]
         The parameters being used in the Notebook Schedule. Can be an empty list.
+    notebook_path : Optional[str]
+        The path of the notebook to execute within the Codespace. Optional. Required if notebook is in a Codespace.
     """
 
     _converter = scheduled_job_payload_trafaret
 
     def __init__(
         self,
         uid: str,
         org_id: str,
         use_case_id: str,
         notebook_id: str,
         notebook_name: str,
         run_type: RunType,
         notebook_type: NotebookType,
         parameters: List[Dict[str, str]],
+        notebook_path: Optional[str] = None,
     ):
         self.uid = uid
         self.org_id = org_id
         self.use_case_id = use_case_id
         self.notebook_id = notebook_id
         self.notebook_name = notebook_name
         self.run_type = run_type
         self.notebook_type = notebook_type
         self.parameters = [ScheduledJobParam.from_server_data(param) for param in parameters]
+        self.notebook_path = notebook_path
 
 
 class NotebookScheduledJob(APIObject):
     """
     DataRobot Notebook Schedule. A scheduled job that runs a notebook.
 
     Attributes
@@ -547,15 +554,15 @@
             "job_ids": self.id,
         }
         r_data = unpaginate(url, params, self._client)
         return [NotebookScheduledRun.from_server_data(data) for data in r_data]
 
     def wait_for_completion(self, max_wait: int = 600) -> str:
         """
-        Retrieve a single notebook.
+        Wait for the completion of a scheduled notebook and return the revision ID corresponding to the run's output.
 
         Parameters
         ----------
         max_wait : int
             The number of seconds to wait before giving up.
 
         Returns
@@ -689,14 +696,22 @@
         self.settings = NotebookSettings.from_server_data(settings)
         self.org_id = org_id
         self.tenant_id = tenant_id
         self.session = NotebookSession.from_server_data(session) if session else session
         self.use_case_id = use_case_id
         self.has_enabled_schedule = has_enabled_schedule
 
+    @property
+    def is_standalone(self) -> bool:
+        return self.type == NotebookType.STANDALONE
+
+    @property
+    def is_codespace(self) -> bool:
+        return self.type == NotebookType.CODESPACE
+
     def get_uri(self) -> str:
         """
         Returns
         -------
         url : str
             Permanent static hyperlink to this Notebook in its Use Case or standalone.
         """
@@ -853,55 +868,71 @@
         url = f"{cls._client.domain}/{cls._notebooks_path}"
         r_data = unpaginate(url, params, cls._client)
         return [Notebook.from_server_data(data) for data in r_data]
 
     def run(
         self,
         title: Optional[str] = None,
+        notebook_path: Optional[str] = None,
         parameters: Optional[List[Dict[str, str]]] = None,
     ) -> NotebookScheduledJob:
         """
         Create a manual scheduled job that runs the notebook.
 
         Notes
         -----
         The notebook must be part of a Use Case.
+        If the notebook is in a Codespace then notebook_path is required.
 
         Parameters
         ----------
         title : Optional[str]
             The title of the background job. Optional.
+
+        notebook_path : Optional[str]
+            The path of the notebook to execute within the Codespace. Required if notebook is in a Codespace.
+
         parameters : Optional[List[Dict[str, str]]]
             A list of dictionaries of key value pairs representing environment variables predefined
             in the notebook. Optional.
 
         Returns
         -------
         notebook_scheduled_job : NotebookScheduledJob
             The created notebook schedule job.
 
+        Raises
+        ------
+        InvalidUsageError
+            If attempting to create a manual scheduled run for a Codespace without a notebook path.
+
         Examples
         --------
         .. code-block:: python
 
             from datarobot._experimental.models.notebooks import Notebook
 
             notebook = Notebook.get(notebook_id='6556b00dcc4ea0bb7ea48121')
             manual_run = notebook.run()
 
             # Alternatively, with title and parameters:
             # manual_run = notebook_scheduled_job = notebook.run(title="My Run", parameters=[{"FOO": "bar"}])
 
             revision_id = manual_run.wait_for_completion()
         """
+        if self.is_codespace and not notebook_path:
+            raise InvalidUsageError("Notebook path is required for Codespace notebooks.")
+
         url = f"{self._client.domain}/{self._scheduling_path}manualRun/"
         payload: ManualRunPayload = {
             "notebook_id": self.id,
             "title": title
             if title
             else f"{self.name} {datetime.now(tz=utc).strftime('%Y-%m-%d %H:%M (UTC)')}",
         }
+        if notebook_path:
+            payload["notebook_path"] = notebook_path
         if parameters:
             payload["parameters"] = parameters
 
         r_data = self._client.post(url, data=payload)
         return NotebookScheduledJob.from_server_data(r_data.json())
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipe_operations.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipe_operations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipes.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipes.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/analytics.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/client.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/config.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/config.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/context.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/enums.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,15 +712,15 @@
     BOX = 4
     HAMMING = 5
 
 
 # Defaults used for image transformations preprocessing
 # Image resize defaults
 DEFAULT_VISUAL_AI_SHOULD_RESIZE = True
-DEFAULT_VISUAL_AI_FORCE_SIZE = False
+DEFAULT_VISUAL_AI_FORCE_SIZE = True
 DEFAULT_VISUAL_AI_IMAGE_SIZE = (224, 224)
 # Image format defaults
 DEFAULT_VISUAL_AI_IMAGE_FORMAT = None  # preserve original image format
 DEFAULT_VISUAL_AI_IMAGE_SUBSAMPLING = None  # uses Pillow library default
 DEFAULT_VISUAL_AI_IMAGE_QUALITY_KEEP_IF_POSSIBLE = True
 DEFAULT_VISUAL_AI_IMAGE_QUALITY = 75
 DEFAULT_VISUAL_AI_IMAGE_RESAMPLE_METHOD = ImageResampleMethod.LANCZOS
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/errors.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/__init__.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,23 +50,23 @@
         image. If False, the resize method modifies the image to contain a thumbnail version
         of itself, no larger than the given size, that preserves the image's aspect ratio.
     image_size: Tuple[int, int]
         New image size (width, height). Both values (width, height) should be specified and contain
         a positive value. Depending on the value of `force_size`, the image will be resized exactly
         to the given image size or will be resized into a thumbnail version of itself, no larger
         than the given size.
-    image_format: enums.ImageFormat | str
+    image_format: ImageFormat | str
         What image format will be used to save result image after transformations. For example
         (ImageFormat.JPEG, ImageFormat.PNG). Values supported are in line with values supported
         by DataRobot. If no format is specified by passing `None` value original image format
         will be preserved.
     image_quality: int or None
         The image quality used when saving image. When None is specified, a value will
         not be passed and Pillow library will use its default.
-    resample_method: enum.ImageResampleMethod
+    resample_method: ImageResampleMethod
         What resampling method should be used when resizing image.
     keep_quality: bool
         Whether the image quality is kept (when possible). If True, for JPEG images quality will
         be preserved. For other types, the value specified in `image_quality` will be used.
     """
 
     def __init__(
@@ -211,11 +211,13 @@
         else:
             image.thumbnail(size=image_options.image_size, resample=image_options.resample_method)
 
     if image.mode != "RGB":
         if image.mode == "I":
             image = _scale_image_to_8bit_range(image)
         image = image.convert("RGB")
-        image.format = image_format
+
+    # Some PIL operations loose the image_format information.
+    image.format = image_format
 
     # convert to target image format and return as image_bytes
     return get_bytes_from_image(image, image_options)
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/base.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/base.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_impact.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_matrix.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_preview.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_preview.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/__init__.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/api_object.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/application.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/blueprint.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/calendar_file.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/change_request.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/connector.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/credential.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,26 @@
 from __future__ import annotations
 
 from typing import Any, cast, Dict, List, Optional, Type, TypeVar
 
 import trafaret as t
 
 from datarobot._compat import Int, String
-from datarobot.enums import CUSTOM_MODEL_TARGET_TYPE, NETWORK_EGRESS_POLICY, TARGET_TYPE
+from datarobot.enums import (
+    CUSTOM_MODEL_TARGET_TYPE,
+    DEFAULT_MAX_WAIT,
+    NETWORK_EGRESS_POLICY,
+    TARGET_TYPE,
+)
 from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import CustomModelVersion
+from datarobot.utils import deprecated
 from datarobot.utils.pagination import unpaginate
+from datarobot.utils.waiters import wait_for_async_resolution
 
 T_CustomModelBase = TypeVar("T_CustomModelBase", bound="_CustomModelBase")
 
 
 class _CustomModelBase(APIObject):  # pylint: disable=missing-class-docstring
     _path = "customModels/"
 
@@ -819,7 +826,52 @@
         ------
         datarobot.errors.ClientError
             If the server responded with 4xx status.
         datarobot.errors.ServerError
             If the server responded with 5xx status.
         """
         super().delete()
+
+    @deprecated(
+        deprecated_since_version="v3.2",
+        will_remove_version="v3.5",
+        message="Please use training data assignment on the model version level: "
+        "CustomModelVersion.create_from_previous or CustomModelVersion.create_clean",
+    )
+    def assign_training_data(
+        self,
+        dataset_id: str,
+        partition_column: Optional[str] = None,
+        max_wait: int = DEFAULT_MAX_WAIT,
+    ) -> None:
+        """Assign training data to the custom inference model.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        dataset_id: str
+            The ID of the training dataset to be assigned.
+        partition_column: str, optional
+            The name of a partition column in the training dataset.
+        max_wait: int, optional
+            The max time to wait for a training data assignment.
+            If set to None, then method will return without waiting.
+            Defaults to 10 min.
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status
+        datarobot.errors.ServerError
+            If the server responded with 5xx status
+        """
+        payload = {"dataset_id": dataset_id, "partition_column": partition_column}
+
+        path = f"{self._path}{self.id}/trainingData/"
+
+        response = self._client.patch(path, data=payload)
+
+        if max_wait is not None:
+            wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
+
+        self.refresh()
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -643,28 +643,29 @@
         initial.required_metadata = data.get("requiredMetadata")  # type: ignore[union-attr]
         return initial
 
     @classmethod
     def create_clean(
         cls,
         custom_model_id: str,
-        base_environment_id: str,
-        is_major_update: bool = True,
+        base_environment_id: Optional[str] = None,
+        is_major_update: Optional[bool] = True,
         folder_path: Optional[str] = None,
         files: Optional[List[Tuple[str, str]]] = None,
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
         maximum_memory: Optional[int] = None,
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_dataset_id: Optional[str] = None,
         partition_column: Optional[str] = None,
         holdout_dataset_id: Optional[str] = None,
         keep_training_holdout_data: Optional[bool] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
+        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
         runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
+        base_environment_version_id: Optional[str] = None,
     ) -> CustomModelVersion:
         """Create a custom model version without files from previous versions.
 
            Create a version with training or holdout data:
            If training/holdout data related parameters are provided,
            the training data is assigned asynchronously.
            In this case:
@@ -678,16 +679,25 @@
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
             The ID of the custom model.
         base_environment_id: str
-            The ID of the base environment to use with the custom model version.
-        is_major_update: bool
+            The base environment to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+        base_environment_version_id: str
+            The base environment version ID to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+            If not specified: in case previous model versions exist, the value from the latest model
+            version is inherited, otherwise, latest successfully built version of the environment
+            specified in "base_environment_id" is used.
+        is_major_update: bool, optional
             The flag defining if a custom model version will be a minor or a major version.
             Default to `True`
         folder_path: str, optional
             The path to a folder containing files to be uploaded.
             Each file in the folder is uploaded under path relative to a folder path.
         files: list, optional
             The list of tuples, where values in each tuple are the local filesystem path and
@@ -795,14 +805,15 @@
         if files and not isinstance(files[0], tuple) and isinstance(files[0], str):  # type: ignore[unreachable]
             files = [(filename, os.path.basename(filename)) for filename in files]  # type: ignore[unreachable]
         return cls._create(
             "post",
             custom_model_id,
             is_major_update,
             base_environment_id,
+            base_environment_version_id,
             folder_path,
             files,
             extra_upload_data=None,
             network_egress_policy=network_egress_policy,
             maximum_memory=maximum_memory,
             replicas=replicas,
             required_metadata_values=required_metadata_values,
@@ -814,29 +825,30 @@
             runtime_parameter_values=runtime_parameter_values,
         )
 
     @classmethod
     def create_from_previous(
         cls,
         custom_model_id: str,
-        base_environment_id: str,
-        is_major_update: bool = True,
+        base_environment_id: Optional[str] = None,
+        is_major_update: Optional[bool] = True,
         folder_path: Optional[str] = None,
         files: Optional[List[Tuple[str, str]]] = None,
         files_to_delete: Optional[List[str]] = None,
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
         maximum_memory: Optional[int] = None,
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_dataset_id: Optional[str] = None,
         partition_column: Optional[str] = None,
         holdout_dataset_id: Optional[str] = None,
         keep_training_holdout_data: Optional[bool] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
+        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
         runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
+        base_environment_version_id: Optional[str] = None,
     ) -> CustomModelVersion:
         """Create a custom model version containing files from a previous version.
 
            Create a version with training/holdout data:
            If training/holdout data related parameters are provided,
            the training data is assigned asynchronously.
            In this case:
@@ -851,15 +863,24 @@
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
             The ID of the custom model.
         base_environment_id: str
-            The ID of the base environment to use with the custom model version.
+            The base environment to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+        base_environment_version_id: str
+            The base environment version ID to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+            If not specified: in case previous model versions exist, the value from the latest model
+            version is inherited, otherwise, latest successfully built version of the environment
+            specified in "base_environment_id" is used.
         is_major_update: bool, optional
             The flag defining if a custom model version will be a minor or a major version.
             Defaults to `True`.
         folder_path: str, optional
             The path to a folder containing files to be uploaded.
             Each file in the folder is uploaded under path relative to a folder path.
         files: list, optional
@@ -978,14 +999,15 @@
         else:
             upload_data = None
         return cls._create(
             "patch",
             custom_model_id,
             is_major_update,
             base_environment_id,
+            base_environment_version_id,
             folder_path,
             files,
             upload_data,
             network_egress_policy,
             maximum_memory,
             replicas,
             required_metadata_values=required_metadata_values,
@@ -998,16 +1020,17 @@
         )
 
     @classmethod
     def _create(
         cls,
         method: str,
         custom_model_id: str,
-        is_major_update: bool,
-        base_environment_id: str,
+        is_major_update: Optional[bool],
+        base_environment_id: Optional[str],
+        base_environment_version_id: Optional[str],
         folder_path: Optional[str],
         files: Optional[List[Tuple[str, str]]],
         extra_upload_data: Optional[List[Tuple[str, Any]]],
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY],
         maximum_memory: Optional[int],
         replicas: Optional[int],
         required_metadata_values: Optional[List[RequiredMetadataValue]],
@@ -1064,16 +1087,20 @@
             if keep_training_holdout_data and (training_dataset_id or holdout_dataset_id):
                 raise InvalidUsageError(
                     "It is not allowed to keep existing training/holdout data and to provide a new ones."
                 )
 
             upload_data: List[Tuple[str, Any]] = [
                 ("isMajorUpdate", str(is_major_update)),
-                ("baseEnvironmentId", base_environment_id),
             ]
+            if base_environment_id:
+                upload_data.append(("baseEnvironmentId", base_environment_id))
+
+            if base_environment_version_id:
+                upload_data.append(("baseEnvironmentVersionId", base_environment_version_id))
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
                     for path in file_paths:
                         file_path = os.path.join(root_path, path)
                         file = stack.enter_context(open(file_path, "rb"))
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_slice.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_source.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_store.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/dataset.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/__init__.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/challenger.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/challenger.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/champion_model_package.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/champion_model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/custom_metrics.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/custom_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -620,23 +620,23 @@
             payload["segments"] = segments
 
         path = "{}{}/fromJSON/".format(self._path.format(self.deployment_id), self.id)
         response = self._client.post(path, data=payload)
         if not dry_run:
             wait_for_async_resolution(self._client, response.headers["Location"], DEFAULT_MAX_WAIT)
 
-    def report_single_value(
+    def submit_single_value(
         self,
         value: float,
         model_id: Optional[str] = None,
         model_package_id: Optional[str] = None,
         dry_run: Optional[bool] = False,
         segments: Optional[List[CustomMetricSegmentFromJSON]] = None,
     ) -> None:
-        """Report single custom metric value at the current moment.
+        """Submit a single custom metric value at the current moment.
 
         Parameters
         ----------
         value: float
             Single numeric custom metric value.
         model_id: Optional[str]
             For a model metric: the ID of the associated champion/challenger model, used to update the metric values.
@@ -661,25 +661,25 @@
 
             custom_metric = CustomMetric.get(
                 deployment_id="5c939e08962d741e34f609f0",
                 custom_metric_id="65f17bdcd2d66683cdfc1113"
             )
 
             # for deployment specific metrics
-            custom_metric.report_single_value(value=121)
+            custom_metric.submit_single_value(value=121)
 
             # for model specific metrics pass model_package_id or model_id
-            custom_metric.report_single_value(value=121, model_package_id="6421df32525c58cc6f991f25")
+            custom_metric.submit_single_value(value=121, model_package_id="6421df32525c58cc6f991f25")
 
             # dry run
-            custom_metric.report_single_value(value=121, model_package_id="6421df32525c58cc6f991f25", dry_run=True)
+            custom_metric.submit_single_value(value=121, model_package_id="6421df32525c58cc6f991f25", dry_run=True)
 
             # for segmented analysis
             segments = [{"name": "custom_seg", "value": "val_1"}]
-            custom_metric.report_single_value(value=121, model_package_id="6421df32525c58cc6f991f25", segments=segments)
+            custom_metric.submit_single_value(value=121, model_package_id="6421df32525c58cc6f991f25", segments=segments)
         """
         bucket = {"sampleSize": 1, "value": value, "timestamp": datetime.now().isoformat()}
         payload: Dict[str, Any] = {"buckets": [bucket], "dryRun": dry_run}
         if model_id:
             payload["modelId"] = model_id
         if model_package_id:
             payload["modelPackageId"] = model_package_id
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_exports.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_exports.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/document.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/driver.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_effect.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_impact.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/featurelist.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/imported_model.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/key_values.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/key_values.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from typing import List, Optional, Set
+from typing import List, Optional, Set, Union
 
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.enums import KeyValueCategory, KeyValueEntityType, KeyValueType
 from datarobot.models.api_object import APIObject
 from datarobot.utils.pagination import unpaginate
@@ -201,24 +201,59 @@
             cls._path,
             {"entityId": entity_id, "entityType": entity_type.value},
             cls._client,
         )
         return [cls.from_server_data(item) for item in data]
 
     @classmethod
+    def find(cls, entity_id: str, entity_type: KeyValueEntityType, name: str) -> Optional[KeyValue]:
+        """Find Key-Value by name.
+
+        .. versionadded:: v3.4
+
+        Parameters
+        ----------
+        entity_id: str
+            ID of the related Entity
+        entity_type: KeyValueEntityType
+            type of the related Entity
+        name: str
+            name of the Key-Value
+
+        Returns
+        -------
+        List[KeyValue]
+            a list of Key-Values
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status
+        datarobot.errors.ServerError
+            if the server responded with 5xx status
+        """
+        data = unpaginate(
+            cls._path,
+            {"entityId": entity_id, "entityType": entity_type.value, "name": name},
+            cls._client,
+        )
+        kv_data = next(data, None)
+        if not kv_data:
+            return None
+        return cls.from_server_data(kv_data)
+
+    @classmethod
     def create(
         cls,
         entity_id: str,
         entity_type: KeyValueEntityType,
         name: str,
         category: KeyValueCategory,
         value_type: KeyValueType,
-        value: Optional[str] = None,
-        numeric_value: Optional[float] = None,
-        boolean_value: Optional[bool] = None,
+        value: Optional[Union[str, float, bool]] = None,
         description: Optional[str] = None,
     ) -> KeyValue:
         """Create a Key-Value.
 
         .. versionadded:: v3.4
 
         Parameters
@@ -229,20 +264,16 @@
             type of the associated resource
         name: str
             name of the Key-Value. Cannot contain: { } ; |
         category: KeyValueCategory
             category of the Key-Value
         value_type: KeyValueType
             type of the Key-Value value
-        value: Optional[str]
-            value of non-numeric Key-Value
-        numeric_value: Optional[float]
-            value of numeric type Key-Value
-        boolean_value: Optional[bool]
-            value of boolean type Key-Value
+        value: Optional[Union[str, float, bool]]
+            value of Key-Value
         description: Optional[str]
             description of the Key-Value
 
         Returns
         -------
         KeyValue
             created Key-Value
@@ -250,93 +281,99 @@
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status.
         datarobot.errors.ServerError
             if the server responded with 5xx status.
         """
+        value_keys = {
+            KeyValueType.NUMERIC: "numericValue",
+            KeyValueType.BOOLEAN: "booleanValue",
+        }
+        value_key = value_keys.get(value_type, "value")
+
         response = cls._client.post(
             cls._path,
             data={
                 "entityId": entity_id,
                 "entityType": entity_type.value,
                 "name": name,
                 "category": category.value,
                 "value_type": value_type.value,
-                "value": value,
-                "numericValue": numeric_value,
-                "booleanValue": boolean_value,
+                value_key: value,
                 "description": description,
             },
         )
 
         return cls.get(response.json()["id"])
 
     def update(
         self,
-        entity_id: str,
-        entity_type: KeyValueEntityType,
-        name: str,
-        category: KeyValueCategory,
-        value_type: KeyValueType,
-        value: Optional[str] = None,
-        numeric_value: Optional[float] = None,
-        boolean_value: Optional[bool] = None,
+        entity_id: Optional[str] = None,
+        entity_type: Optional[KeyValueEntityType] = None,
+        name: Optional[str] = None,
+        category: Optional[KeyValueCategory] = None,
+        value_type: Optional[KeyValueType] = None,
+        value: Optional[Union[str, float, bool]] = None,
         description: Optional[str] = None,
         comment: Optional[str] = None,
     ) -> None:
         """Update Key-Value.
 
         .. versionadded:: v3.4
 
         Parameters
         ----------
-        entity_id: str
+        entity_id: Optional[str]
             ID of the associated resource
-        entity_type: KeyValueEntityType
+        entity_type: Optional[KeyValueEntityType]
             type of the associated resource
-        name: str
+        name: Optional[str]
             name of the Key-Value. Cannot contain: { } ; |
-        category: KeyValueCategory
+        category: Optional[KeyValueCategory]
             category of the Key-Value
-        value_type: KeyValueType
+        value_type: Optional[KeyValueType]
             type of the Key-Value value
-        value: Optional[str]
-            value of non-numeric Key-Value
-        numeric_value: Optional[float]
-            value of numeric type Key-Value
-        boolean_value: Optional[bool]
-            value of boolean type Key-Value
+        value: Optional[[Union[str, float, bool]]
+            value of Key-Value
         description: Optional[str]
             description of the Key-Value
         comment: Optional[str]
             user comment explaining the change
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status.
         datarobot.errors.ServerError
             if the server responded with 5xx status.
         """
-        response = self._client.patch(
-            self._key_value_path(self.id),
-            data={
-                "entityId": entity_id,
-                "entityType": entity_type.value,
-                "name": name,
-                "category": category.value,
-                "valueType": value_type.value,
-                "value": value,
-                "numericValue": numeric_value,
-                "booleanValue": boolean_value,
-                "description": description,
-                "comment": comment,
-            },
-        )
+        payload = {
+            "entityId": entity_id if entity_id is not None else self.entity_id,
+            "entityType": entity_type.value if entity_type is not None else self.entity_type.value,
+            "name": name if name is not None else self.name,
+            "category": category.value if category is not None else self.category.value,
+            "valueType": value_type.value if value_type is not None else self.value_type.value,
+            "value": self.value
+            if value is None
+            else None,  # backend expects `value` to be always provided
+        }
+        if value is not None:
+            value_keys = {
+                KeyValueType.NUMERIC: "numericValue",
+                KeyValueType.BOOLEAN: "booleanValue",
+            }
+            value_key = value_keys.get(value_type if value_type else self.value_type, "value")
+            payload[value_key] = value  # type: ignore[assignment]
+        if description is not None:
+            payload["description"] = description
+        if comment is not None:
+            payload["comment"] = comment
+
+        response = self._client.patch(self._key_value_path(self.id), data=payload)
 
         data = response.json()
         new_version = self.from_server_data(data)
         self._update_values(new_version)
 
     def refresh(self) -> None:
         """Update Key-Value with the latest data from server.
@@ -364,7 +401,24 @@
         datarobot.errors.ClientError
             If the server responded with 4xx status.
         datarobot.errors.ServerError
             If the server responded with 5xx status.
         """
         path = self._key_value_path(self.id)
         self._client.delete(path)
+
+    def get_value(self) -> Union[str, float, bool]:
+        """Get a value of Key-Value.
+
+        .. versionadded:: v3.4
+
+        Returns
+        -------
+        Union[str, float, boolean]
+            value depending on the value type
+        """
+        if self.value_type == KeyValueType.NUMERIC:
+            return self.numeric_value
+        elif self.value_type == KeyValueType.BOOLEAN:
+            return self.boolean_value
+        else:
+            return self.value
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/lift_chart.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/missing_report.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/deployment.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model_version.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/modeljob.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pareto_front.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predict_job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_environment.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_server.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predictions.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prime_file.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project_options.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/rating_table.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/recommended_model.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job_run.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job_run.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/residuals.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/roc_curve.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/ruleset.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/runtime_parameters.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/segmentation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_impact.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_impact.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from typing import List, Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
-from datarobot.utils import get_id_from_response
+from datarobot.utils import deprecation, get_id_from_response
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.job import Job
 
     class ShapImpactType(TypedDict):
@@ -67,26 +67,36 @@
                         t.Key("impact_unnormalized"): t.Float(),
                     }
                 ).allow_extra("*")
             ),
         }
     ).allow_extra("*")
 
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapImpact' instead.",
+    )
     def __init__(
         self, count: int, shap_impacts: List[ShapImpactType], row_count: Optional[int] = None
     ) -> None:
         self.count = count
         self.shap_impacts = shap_impacts
         self.row_count = row_count
 
     def __repr__(self) -> str:
         template = "{}(count={!r})"
         return template.format(type(self).__name__, self.count)
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapImpact.create' instead.",
+    )
     def create(cls, project_id: str, model_id: str, row_count: Optional[int] = None) -> Job:
         """Create SHAP impact for the specified model.
 
         Parameters
         ----------
         project_id : str
             id of the project the model belongs to
@@ -105,14 +115,19 @@
         response = cls._client.post(url, data=payload)
         job_id = get_id_from_response(response)
         from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
         return Job.get(project_id=project_id, job_id=job_id)
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapImpact.list' instead.",
+    )
     def get(cls, project_id: str, model_id: str) -> ShapImpact:
         """
         Retrieve SHAP impact scores for features in a model.
 
         Parameters
         ----------
         project_id : str
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pandas as pd
 import trafaret as t
 
 from datarobot import errors
 from datarobot._compat import String
 from datarobot.enums import DEFAULT_TIMEOUT
 from datarobot.models.api_object import APIObject
-from datarobot.utils import get_id_from_response
+from datarobot.utils import deprecation, get_id_from_response
 from datarobot.utils.pagination import unpaginate
 
 if TYPE_CHECKING:
     from datarobot.models.shap_matrix_job import ShapMatrixJob
 
 
 class ShapMatrix(APIObject):
@@ -67,14 +67,19 @@
             t.Key("id"): String(),
             t.Key("project_id"): String(),
             t.Key("model_id"): String(),
             t.Key("dataset_id"): String(),
         }
     ).allow_extra("*")
 
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix' instead.",
+    )
     def __init__(
         self,
         project_id: str,
         id: str,
         model_id: Optional[str] = None,
         dataset_id: Optional[str] = None,
     ) -> None:
@@ -90,14 +95,19 @@
             self.id,
             self.project_id,
             self.model_id,
             self.dataset_id,
         )
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix.create' instead.",
+    )
     def create(cls, project_id: str, model_id: str, dataset_id: str) -> ShapMatrixJob:
         """Calculate SHAP based prediction explanations against previously uploaded dataset.
 
         Parameters
         ----------
         project_id : str
             id of the project the model belongs to
@@ -138,17 +148,24 @@
         cls,
         location: str,
         model_id: Optional[str] = None,
         dataset_id: Optional[str] = None,
     ) -> ShapMatrix:
         head, tail = location.split("/shapMatrices/", 1)
         project_id, id = head.split("/")[-1], tail.split("/")[0]
-        return cls(project_id=project_id, id=id, model_id=model_id, dataset_id=dataset_id)
+        return cls(  # type: ignore[no-any-return]
+            project_id=project_id, id=id, model_id=model_id, dataset_id=dataset_id
+        )
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix.list' instead.",
+    )
     def list(cls, project_id: str) -> List[ShapMatrix]:
         """
         Fetch all the computed SHAP prediction explanations for a project.
 
         Parameters
         ----------
         project_id : str
@@ -169,14 +186,19 @@
         data = unpaginate(
             initial_url=cls._path.format(project_id), initial_params=None, client=cls._client
         )
         result = [cls.from_server_data(item) for item in data]
         return result
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix.list' instead.",
+    )
     def get(cls, project_id: str, id: str) -> ShapMatrix:
         """
         Retrieve the specific SHAP matrix.
 
         Parameters
         ----------
         project_id : str
@@ -184,16 +206,21 @@
         id : str
             id of the SHAP matrix
 
         Returns
         -------
         :py:class:`ShapMatrix <datarobot.models.ShapMatrix>` object representing specified record
         """
-        return cls(project_id=project_id, id=id)
+        return cls(project_id=project_id, id=id)  # type: ignore[no-any-return]
 
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix' instead.",
+    )
     def get_as_dataframe(self, read_timeout: int = DEFAULT_TIMEOUT.READ) -> pd.DataFrame:
         """
         Retrieve SHAP matrix values as dataframe.
 
         Returns
         -------
         dataframe : pandas.DataFrame
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             data,
             model_id=model_id,
             dataset_id=dataset_id,
             completed_resource_url=completed_url,
         )
 
     def _make_result_from_location(self, location: str, params: Optional[Any] = None) -> ShapMatrix:
-        return ShapMatrix.from_location(
+        return ShapMatrix.from_location(  # type: ignore[no-any-return]
             location,
             model_id=self._model_id,
             dataset_id=self._dataset_id,
         )
 
     def refresh(self) -> None:
         """
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/sharing.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/status_check_job.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/trafarets.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/training_predictions.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/types.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/use_case.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/validators.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/images.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/word_cloud.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/rest.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/__init__.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/deprecation.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/pagination.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/retry.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/source.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/waiters.py` & `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.4.0.2024.4.1
+Version: 3.4.0.2024.4.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 datarobot/_experimental/models/genai/comparison_chat.py
 datarobot/_experimental/models/genai/comparison_prompt.py
 datarobot/_experimental/models/genai/custom_model_llm_validation.py
 datarobot/_experimental/models/genai/custom_model_validation.py
 datarobot/_experimental/models/genai/llm.py
 datarobot/_experimental/models/genai/llm_blueprint.py
 datarobot/_experimental/models/genai/playground.py
+datarobot/_experimental/models/genai/prompt_trace.py
 datarobot/_experimental/models/genai/user_limits.py
 datarobot/_experimental/models/genai/vector_database.py
 datarobot/helpers/__init__.py
 datarobot/helpers/binary_data_utils.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
 datarobot/helpers/image_utils.py
```

### Comparing `datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/pyproject.toml` & `datarobot_early_access-3.4.0.2024.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/setup.py` & `datarobot_early_access-3.4.0.2024.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.1/setup_weekly.py` & `datarobot_early_access-3.4.0.2024.4.8/setup_weekly.py`

 * *Files identical despite different names*

