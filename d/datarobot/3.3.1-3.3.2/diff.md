# Comparing `tmp/datarobot-3.3.1.tar.gz` & `tmp/datarobot-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot-3.3.1.tar", last modified: Mon Dec 18 19:39:48 2023, max compression
+gzip compressed data, was "dist/datarobot-3.3.2.tar", last modified: Mon Apr  8 17:20:56 2024, max compression
```

## Comparing `datarobot-3.3.1.tar` & `datarobot-3.3.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   195174 2023-12-18 19:03:39.000000 datarobot-3.3.1/CHANGES.rst
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7555 2023-07-24 12:53:40.000000 datarobot-3.3.1/LICENSE.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      421 2023-10-25 11:01:02.000000 datarobot-3.3.1/MANIFEST.in
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3438 2023-12-18 19:39:48.000000 datarobot-3.3.1/PKG-INFO
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8911 2023-10-25 11:01:02.000000 datarobot-3.3.1/README.md
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5760 2023-12-18 17:29:20.000000 datarobot-3.3.1/common_setup.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2443 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      687 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/_compat.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      311 2023-12-18 19:03:39.000000 datarobot-3.3.1/datarobot/_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5241 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/analytics.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21787 2023-12-18 19:03:39.000000 datarobot-3.3.1/datarobot/client.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4664 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/context.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    29414 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/enums.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8984 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/errors.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/helpers/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    25496 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/helpers/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13002 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/helpers/binary_data_utils.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1156 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/helpers/eligibility_result.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14350 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/helpers/feature_discovery.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8696 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/helpers/image_utils.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   101561 2023-10-25 11:01:02.000000 datarobot-3.3.1/datarobot/helpers/partitioning_methods.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/mixins/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-07-24 12:53:40.000000 datarobot-3.3.1/datarobot/mixins/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1134 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/mixins/browser_mixin.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1112 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/mixins/update_attributes_mixin.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4266 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     9166 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/advanced_tuning.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    27075 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/anomaly_assessment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2925 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/api_object.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8969 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/application.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15447 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/automated_documentation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    20521 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/batch_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    37053 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/batch_monitoring_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    82734 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/batch_prediction_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11451 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/blueprint.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    23822 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/calendar_file.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13301 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/change_request.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3978 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/cluster.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7233 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/cluster_insight.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12910 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/compliance_doc_template.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4887 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/confusion_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6953 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/connector.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13004 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/credential.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    33397 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/custom_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12413 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/custom_model_test.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    59820 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/custom_model_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15411 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/custom_task.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    22991 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/custom_task_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2315 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/custom_task_version_dependency_build.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17613 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/data_engine_query_generator.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17013 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/data_slice.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    16402 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/data_source.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    20035 2023-11-27 20:25:42.000000 datarobot-3.3.1/datarobot/models/data_store.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    73460 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/dataset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    30524 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/datetime_trend_plots.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/deployment/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      417 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/deployment/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    16779 2023-12-18 19:03:39.000000 datarobot-3.3.1/datarobot/models/deployment/accuracy.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5688 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/deployment/bias_and_fairness.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12650 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/deployment/data_drift.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   104548 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/deployment/deployment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1131 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/deployment/mixins.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10065 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/deployment/service_stats.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3450 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/deployment/sharing.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/documentai/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/documentai/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    27024 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/documentai/document.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6583 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/driver.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     9411 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/execution_environment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11344 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/execution_environment_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5374 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_baseline_validation.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      355 2023-07-24 12:53:40.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6403 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4915 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4523 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5208 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4521 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6789 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    53938 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/feature.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/feature_association_matrix/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      237 2023-07-24 12:53:40.000000 datarobot-3.3.1/datarobot/models/feature_association_matrix/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2600 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6177 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4753 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18187 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/feature_effect.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7003 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/feature_impact.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17463 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/featurelist.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7336 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/imported_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21166 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6516 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/lift_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5468 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/missing_report.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   283117 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/model.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/model_registry/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      204 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/model_registry/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      408 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/model_registry/common.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3453 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/model_registry/deployment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    26372 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/model_registry/registered_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21702 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/model_registry/registered_model_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7215 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/modeljob.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14320 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/pairwise_statistics.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5438 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/pareto_front.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8726 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/payoff_matrix.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7403 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/predict_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10218 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/prediction_dataset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10973 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/prediction_environment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    34744 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/prediction_explanations.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2426 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/prediction_server.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15940 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/predictions.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2655 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/prime_file.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   204934 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/project.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    56833 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/project_options.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8774 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/rating_table.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4337 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/recommended_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    19064 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/relationships_configuration.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6645 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/residuals.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4524 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/restore_discarded_features.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11692 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/roc_curve.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2927 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/ruleset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    19381 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/secondary_dataset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14217 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/segmentation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4070 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/shap_impact.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7057 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/shap_matrix.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2645 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/shap_matrix_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7314 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/sharing.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6267 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/status_check_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1431 2023-07-24 12:53:40.000000 datarobot-3.3.1/datarobot/models/trafarets.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    28260 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/training_predictions.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1822 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/types.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/use_cases/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      262 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/use_cases/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    24589 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/use_cases/use_case.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13520 2023-12-18 17:29:20.000000 datarobot-3.3.1/datarobot/models/use_cases/utils.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/user_blueprints/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)       49 2023-07-24 12:53:40.000000 datarobot-3.3.1/datarobot/models/user_blueprints/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    69649 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/user_blueprints/models.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8758 2023-07-24 12:53:40.000000 datarobot-3.3.1/datarobot/models/user_blueprints/trafarets.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2749 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/validators.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/models/visualai/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      226 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/visualai/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18528 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/visualai/augmentation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10521 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/visualai/images.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13615 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/visualai/insights.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4936 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/models/word_cloud.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/py.typed
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18404 2023-12-14 18:07:41.000000 datarobot-3.3.1/datarobot/rest.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot/utils/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15618 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2997 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/deprecation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      495 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/logger.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1200 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/pagination.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1461 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/retry.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1282 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/source.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4109 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/sourcedata.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4193 2023-10-25 11:01:03.000000 datarobot-3.3.1/datarobot/utils/waiters.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot.egg-info/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3438 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot.egg-info/PKG-INFO
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5539 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot.egg-info/SOURCES.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        1 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot.egg-info/dependency_links.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1128 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot.egg-info/requires.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)       10 2023-12-18 19:39:48.000000 datarobot-3.3.1/datarobot.egg-info/top_level.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3066 2023-10-25 11:01:03.000000 datarobot-3.3.1/pyproject.toml
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      123 2023-12-18 19:39:48.000000 datarobot-3.3.1/setup.cfg
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      965 2023-10-25 11:01:03.000000 datarobot-3.3.1/setup.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1213 2023-10-25 11:01:03.000000 datarobot-3.3.1/setup_major.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   195398 2024-04-08 17:17:24.000000 datarobot-3.3.2/CHANGES.rst
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7555 2023-07-24 12:53:40.000000 datarobot-3.3.2/LICENSE.txt
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      421 2023-10-25 11:01:02.000000 datarobot-3.3.2/MANIFEST.in
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3438 2024-04-08 17:20:56.000000 datarobot-3.3.2/PKG-INFO
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8911 2023-10-25 11:01:02.000000 datarobot-3.3.2/README.md
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5760 2024-04-08 17:17:19.000000 datarobot-3.3.2/common_setup.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2443 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      687 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/_compat.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      311 2024-04-08 17:17:24.000000 datarobot-3.3.2/datarobot/_version.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5241 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/analytics.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21787 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/client.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4664 2024-01-12 10:49:15.000000 datarobot-3.3.2/datarobot/context.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    29414 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/enums.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8984 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/errors.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot/helpers/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    25496 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/helpers/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13002 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/binary_data_utils.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1156 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/eligibility_result.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14350 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/feature_discovery.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8696 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/helpers/image_utils.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   101561 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/partitioning_methods.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot/mixins/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/mixins/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1134 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/mixins/browser_mixin.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1112 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/mixins/update_attributes_mixin.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4266 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     9166 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/advanced_tuning.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    27075 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/anomaly_assessment.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2925 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/api_object.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8969 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/application.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15447 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/automated_documentation.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    20521 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/batch_job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    37053 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/batch_monitoring_job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    82734 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/batch_prediction_job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11451 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/blueprint.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    23822 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/calendar_file.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13301 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/change_request.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3978 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/cluster.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7233 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/cluster_insight.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12910 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/compliance_doc_template.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4887 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/confusion_chart.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6953 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/connector.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13004 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/credential.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    33397 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/custom_model.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12413 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/custom_model_test.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    59820 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/custom_model_version.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15411 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/custom_task.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    22991 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/custom_task_version.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2315 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/custom_task_version_dependency_build.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17613 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/data_engine_query_generator.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17013 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/data_slice.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    16402 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/data_source.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    20035 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/data_store.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    73460 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/dataset.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    30524 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/datetime_trend_plots.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/deployment/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      417 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/deployment/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    16779 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/deployment/accuracy.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5688 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/deployment/bias_and_fairness.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12650 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/data_drift.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   104548 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/deployment/deployment.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1131 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/mixins.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10065 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/service_stats.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3450 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/sharing.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/documentai/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/documentai/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    27024 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/documentai/document.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6583 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/driver.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     9411 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/execution_environment.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11344 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/execution_environment_version.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5374 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/external_baseline_validation.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      355 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6403 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4915 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4523 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5208 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4521 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6789 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    53938 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      237 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2600 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6177 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4753 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18187 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/feature_effect.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7003 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature_impact.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17463 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/featurelist.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7336 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/imported_model.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21166 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6516 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/lift_chart.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5468 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/missing_report.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   283117 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/model.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/model_registry/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      204 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/model_registry/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      408 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/model_registry/common.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3453 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/model_registry/deployment.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    26372 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/model_registry/registered_model.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21702 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/model_registry/registered_model_version.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7215 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/modeljob.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14320 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/pairwise_statistics.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5438 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/pareto_front.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8726 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/payoff_matrix.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7403 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/predict_job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10218 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/prediction_dataset.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10973 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/prediction_environment.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    34876 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/prediction_explanations.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2426 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/prediction_server.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15940 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/predictions.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2655 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/prime_file.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   204934 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/project.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    56833 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/project_options.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8774 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/rating_table.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4337 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/recommended_model.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    19064 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/relationships_configuration.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6645 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/residuals.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4524 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/restore_discarded_features.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11692 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/roc_curve.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2927 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/ruleset.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    19381 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/secondary_dataset.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14217 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/segmentation.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4070 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/shap_impact.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7057 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/shap_matrix.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2645 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/shap_matrix_job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7314 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/sharing.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6267 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/status_check_job.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1431 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/trafarets.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    28260 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/training_predictions.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1822 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/types.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/use_cases/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      262 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/use_cases/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    24589 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/use_cases/use_case.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13520 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/use_cases/utils.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/user_blueprints/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)       49 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/user_blueprints/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    69649 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/user_blueprints/models.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8758 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/user_blueprints/trafarets.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2749 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/validators.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/visualai/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      226 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18528 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/augmentation.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10521 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/images.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13615 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/insights.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4936 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/word_cloud.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/py.typed
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18404 2023-12-14 18:07:41.000000 datarobot-3.3.2/datarobot/rest.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/utils/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15618 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/__init__.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2997 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/deprecation.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      495 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/logger.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1200 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/pagination.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1461 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/retry.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1282 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/source.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4109 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/sourcedata.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4193 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/waiters.py
+drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3438 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/PKG-INFO
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5539 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/SOURCES.txt
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        1 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/dependency_links.txt
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1128 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/requires.txt
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)       10 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/top_level.txt
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3066 2023-10-25 11:01:03.000000 datarobot-3.3.2/pyproject.toml
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      123 2024-04-08 17:20:56.000000 datarobot-3.3.2/setup.cfg
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      965 2023-10-25 11:01:03.000000 datarobot-3.3.2/setup.py
+-rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1213 2023-10-25 11:01:03.000000 datarobot-3.3.2/setup_major.py
```

### Comparing `datarobot-3.3.1/CHANGES.rst` & `datarobot-3.3.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 #########
 Changelog
 #########
 
+3.3.2
+========
+
+Bugfixes
+********
+- Fix `per_ngram_text_explanations` retrieving.  In some cases `per_ngram_text_explanations` are missing in prediction explanations, causing SDK to fail when trying to retrieve the values.
+
 3.3.1
 ========
 
 Bugfixes
 ********
 - Fixed setting ssl_verify by env variables in :meth: `config_from_env <datarobot.client._config_from_env>`
```

### Comparing `datarobot-3.3.1/LICENSE.txt` & `datarobot-3.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/PKG-INFO` & `datarobot-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.3.1
+Version: 3.3.2
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot-3.3.1/README.md` & `datarobot-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/common_setup.py` & `datarobot-3.3.2/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/__init__.py` & `datarobot-3.3.2/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/_compat.py` & `datarobot-3.3.2/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/analytics.py` & `datarobot-3.3.2/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/client.py` & `datarobot-3.3.2/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/context.py` & `datarobot-3.3.2/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/enums.py` & `datarobot-3.3.2/datarobot/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/errors.py` & `datarobot-3.3.2/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/helpers/__init__.py` & `datarobot-3.3.2/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/helpers/binary_data_utils.py` & `datarobot-3.3.2/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/helpers/eligibility_result.py` & `datarobot-3.3.2/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/helpers/feature_discovery.py` & `datarobot-3.3.2/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/helpers/image_utils.py` & `datarobot-3.3.2/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/helpers/partitioning_methods.py` & `datarobot-3.3.2/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/mixins/browser_mixin.py` & `datarobot-3.3.2/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/mixins/update_attributes_mixin.py` & `datarobot-3.3.2/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/__init__.py` & `datarobot-3.3.2/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/advanced_tuning.py` & `datarobot-3.3.2/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/anomaly_assessment.py` & `datarobot-3.3.2/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/api_object.py` & `datarobot-3.3.2/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/application.py` & `datarobot-3.3.2/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/automated_documentation.py` & `datarobot-3.3.2/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/batch_job.py` & `datarobot-3.3.2/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/batch_monitoring_job.py` & `datarobot-3.3.2/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/batch_prediction_job.py` & `datarobot-3.3.2/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/blueprint.py` & `datarobot-3.3.2/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/calendar_file.py` & `datarobot-3.3.2/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/change_request.py` & `datarobot-3.3.2/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/cluster.py` & `datarobot-3.3.2/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/cluster_insight.py` & `datarobot-3.3.2/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/compliance_doc_template.py` & `datarobot-3.3.2/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/confusion_chart.py` & `datarobot-3.3.2/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/connector.py` & `datarobot-3.3.2/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/credential.py` & `datarobot-3.3.2/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/custom_model.py` & `datarobot-3.3.2/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/custom_model_test.py` & `datarobot-3.3.2/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/custom_model_version.py` & `datarobot-3.3.2/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/custom_task.py` & `datarobot-3.3.2/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/custom_task_version.py` & `datarobot-3.3.2/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/custom_task_version_dependency_build.py` & `datarobot-3.3.2/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/data_engine_query_generator.py` & `datarobot-3.3.2/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/data_slice.py` & `datarobot-3.3.2/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/data_source.py` & `datarobot-3.3.2/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/data_store.py` & `datarobot-3.3.2/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/dataset.py` & `datarobot-3.3.2/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/datetime_trend_plots.py` & `datarobot-3.3.2/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/accuracy.py` & `datarobot-3.3.2/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/bias_and_fairness.py` & `datarobot-3.3.2/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/data_drift.py` & `datarobot-3.3.2/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/deployment.py` & `datarobot-3.3.2/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/mixins.py` & `datarobot-3.3.2/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/service_stats.py` & `datarobot-3.3.2/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/deployment/sharing.py` & `datarobot-3.3.2/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/documentai/document.py` & `datarobot-3.3.2/datarobot/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/driver.py` & `datarobot-3.3.2/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/execution_environment.py` & `datarobot-3.3.2/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/execution_environment_version.py` & `datarobot-3.3.2/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_baseline_validation.py` & `datarobot-3.3.2/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/feature.py` & `datarobot-3.3.2/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/feature_effect.py` & `datarobot-3.3.2/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/feature_impact.py` & `datarobot-3.3.2/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/featurelist.py` & `datarobot-3.3.2/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/imported_model.py` & `datarobot-3.3.2/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/job.py` & `datarobot-3.3.2/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/lift_chart.py` & `datarobot-3.3.2/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/missing_report.py` & `datarobot-3.3.2/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/model.py` & `datarobot-3.3.2/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/model_registry/deployment.py` & `datarobot-3.3.2/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/model_registry/registered_model.py` & `datarobot-3.3.2/datarobot/models/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/model_registry/registered_model_version.py` & `datarobot-3.3.2/datarobot/models/model_registry/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/modeljob.py` & `datarobot-3.3.2/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/pairwise_statistics.py` & `datarobot-3.3.2/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/pareto_front.py` & `datarobot-3.3.2/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/payoff_matrix.py` & `datarobot-3.3.2/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/predict_job.py` & `datarobot-3.3.2/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/prediction_dataset.py` & `datarobot-3.3.2/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/prediction_environment.py` & `datarobot-3.3.2/datarobot/models/prediction_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/prediction_explanations.py` & `datarobot-3.3.2/datarobot/models/prediction_explanations.py`

 * *Files 2% similar despite different names*

```diff
@@ -620,15 +620,17 @@
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
                     if has_text_explanations:
                         data.append(
-                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
+                            json.dumps(
+                                pred_expl.get("per_ngram_text_explanations"), ensure_ascii=False
+                            )
                         )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
             else:
                 for pred_expl in row.prediction_explanations:
                     data.extend(
                         [
                             pred_expl["feature"],
@@ -636,15 +638,17 @@
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
                     if has_text_explanations:
                         data.append(
-                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
+                            json.dumps(
+                                pred_expl.get("per_ngram_text_explanations"), ensure_ascii=False
+                            )
                         )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
 
         return pd.DataFrame(data=pred_expl_list, columns=columns)
 
     def download_to_csv(self, filename, encoding="utf-8", exclude_adjusted_predictions=True):
         """
```

### Comparing `datarobot-3.3.1/datarobot/models/prediction_server.py` & `datarobot-3.3.2/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/predictions.py` & `datarobot-3.3.2/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/prime_file.py` & `datarobot-3.3.2/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/project.py` & `datarobot-3.3.2/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/project_options.py` & `datarobot-3.3.2/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/rating_table.py` & `datarobot-3.3.2/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/recommended_model.py` & `datarobot-3.3.2/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/relationships_configuration.py` & `datarobot-3.3.2/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/residuals.py` & `datarobot-3.3.2/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/restore_discarded_features.py` & `datarobot-3.3.2/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/roc_curve.py` & `datarobot-3.3.2/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/ruleset.py` & `datarobot-3.3.2/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/secondary_dataset.py` & `datarobot-3.3.2/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/segmentation.py` & `datarobot-3.3.2/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/shap_impact.py` & `datarobot-3.3.2/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/shap_matrix.py` & `datarobot-3.3.2/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/shap_matrix_job.py` & `datarobot-3.3.2/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/sharing.py` & `datarobot-3.3.2/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/status_check_job.py` & `datarobot-3.3.2/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/trafarets.py` & `datarobot-3.3.2/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/training_predictions.py` & `datarobot-3.3.2/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/types.py` & `datarobot-3.3.2/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/use_cases/use_case.py` & `datarobot-3.3.2/datarobot/models/use_cases/use_case.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/use_cases/utils.py` & `datarobot-3.3.2/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/user_blueprints/models.py` & `datarobot-3.3.2/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/user_blueprints/trafarets.py` & `datarobot-3.3.2/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/validators.py` & `datarobot-3.3.2/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/visualai/augmentation.py` & `datarobot-3.3.2/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/visualai/images.py` & `datarobot-3.3.2/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/visualai/insights.py` & `datarobot-3.3.2/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/models/word_cloud.py` & `datarobot-3.3.2/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/rest.py` & `datarobot-3.3.2/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/__init__.py` & `datarobot-3.3.2/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/deprecation.py` & `datarobot-3.3.2/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/pagination.py` & `datarobot-3.3.2/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/retry.py` & `datarobot-3.3.2/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/source.py` & `datarobot-3.3.2/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/sourcedata.py` & `datarobot-3.3.2/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot/utils/waiters.py` & `datarobot-3.3.2/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot.egg-info/PKG-INFO` & `datarobot-3.3.2/datarobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.3.1
+Version: 3.3.2
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot-3.3.1/datarobot.egg-info/SOURCES.txt` & `datarobot-3.3.2/datarobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/datarobot.egg-info/requires.txt` & `datarobot-3.3.2/datarobot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/pyproject.toml` & `datarobot-3.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/setup.py` & `datarobot-3.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.1/setup_major.py` & `datarobot-3.3.2/setup_major.py`

 * *Files identical despite different names*

