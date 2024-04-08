# Comparing `tmp/tmlt_analytics-0.8.3.tar.gz` & `tmp/tmlt_analytics-0.9.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.8.3.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.9.0rc5.tar", max compression
```

## Comparing `tmlt_analytics-0.8.3.tar` & `tmlt_analytics-0.9.0rc5.tar`

### file list

```diff
@@ -1,173 +1,180 @@
--rw-r--r--   0        0        0    20711 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/LICENSE
--rw-r--r--   0        0        0    20138 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/LICENSE.docs
--rw-r--r--   0        0        0      121 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/NOTICE
--rw-r--r--   0        0        0     3251 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/README.md
--rw-r--r--   0        0        0     1154 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/_templates/package-name.html
--rw-r--r--   0        0        0     7175 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/conf.py
--rw-r--r--   0        0        0    10498 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/aws-glue.rst
--rw-r--r--   0        0        0     1599 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/bigquery-setup.rst
--rw-r--r--   0        0        0     3005 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/docker-image.rst
--rw-r--r--   0        0        0     1225 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/index.rst
--rw-r--r--   0        0        0     6280 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/inputs-outputs.rst
--rw-r--r--   0        0        0     5761 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/parameters.rst
--rw-r--r--   0        0        0     4733 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/running-the-program.rst
--rw-r--r--   0        0        0     1706 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/bigquery/setup.rst
--rw-r--r--   0        0        0     6911 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/databricks.rst
--rw-r--r--   0        0        0      339 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/index.rst
--rw-r--r--   0        0        0     4782 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/installation.rst
--rw-r--r--   0        0        0     4126 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/howto-guides/troubleshooting.rst
--rw-r--r--   0        0        0   118378 2024-02-27 22:26:57.147525 tmlt_analytics-0.8.3/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0    34101 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_books_by_unique_members.png
--rw-r--r--   0        0        0   104926 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    59042 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    30330 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_genres_by_age.png
--rw-r--r--   0        0        0    14782 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2024-02-27 22:26:57.151525 tmlt_analytics-0.8.3/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    20226 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    18639 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/flat_map_row_example.svg
--rw-r--r--   0        0        0    23590 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/flow_chart_truncation.svg
--rw-r--r--   0        0        0   116752 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/glue_graph.png
--rw-r--r--   0        0        0    14685 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/index_api.svg
--rw-r--r--   0        0        0      609 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/index_howto_guides.svg
--rw-r--r--   0        0        0     1196 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    23369 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/intuitive_noise_visualization.png
--rw-r--r--   0        0        0    30903 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/logo.png
--rw-r--r--   0        0        0    85314 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/mock_checkout_logs.svg
--rw-r--r--   0        0        0    59239 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/private_join_example.svg
--rw-r--r--   0        0        0    35838 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/private_join_tables.svg
--rw-r--r--   0        0        0    32227 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/images/public_join_example_zips.svg
--rw-r--r--   0        0        0     5640 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/index.rst
--rw-r--r--   0        0        0      662 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     3169 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/privacy-policy.rst
--rw-r--r--   0        0        0     2024 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3440 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/templates/python/module.rst
--rw-r--r--   0        0        0      396 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11697 2024-02-27 22:26:57.155525 tmlt_analytics-0.8.3/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8597 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     6589 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     7802 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0    12492 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/topic-guides/understanding-sensitivity.rst
--rw-r--r--   0        0        0     8462 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9118 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7243 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18802 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0      430 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/index.rst
--rw-r--r--   0        0        0    12394 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/more-with-privacy-ids.rst
--rw-r--r--   0        0        0     8452 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    15179 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/privacy-id-basics.rst
--rw-r--r--   0        0        0    16233 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0    15435 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/examples/demo_video_notebook.ipynb
--rw-r--r--   0        0        0     4789 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/examples/interactive_evaluation.ipynb
--rw-r--r--   0        0        0     5459 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/examples/private_join.ipynb
--rw-r--r--   0        0        0     6570 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/examples/zcdp_puredp_switching.ipynb
--rw-r--r--   0        0        0     6268 2024-02-27 22:27:37.675505 tmlt_analytics-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      108 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/__init__.py
--rw-r--r--   0        0        0     7451 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/conftest.py
--rw-r--r--   0        0        0      115 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/__init__.py
--rw-r--r--   0        0        0      108 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/__init__.py
--rw-r--r--   0        0        0     5642 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/conftest.py
--rw-r--r--   0        0        0      151 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/__init__.py
--rw-r--r--   0        0        0    15227 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/test_constraint_propagation.py
--rw-r--r--   0        0        0     6531 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/test_count_distinct_optimization.py
--rw-r--r--   0        0        0     9106 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/test_id_col_operations.py
--rw-r--r--   0        0        0    22175 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/test_l0_linf_truncation.py
--rw-r--r--   0        0        0    14250 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/test_l1_truncation.py
--rw-r--r--   0        0        0     3965 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/ids/test_partition.py
--rw-r--r--   0        0        0      143 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/mixed/__init__.py
--rw-r--r--   0        0        0     5087 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/mixed/test_mixed_session.py
--rw-r--r--   0        0        0      152 2024-02-27 22:26:57.159525 tmlt_analytics-0.8.3/test/system/session/rows/__init__.py
--rw-r--r--   0        0        0    26385 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/rows/conftest.py
--rw-r--r--   0        0        0    45324 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/rows/test_add_max_rows.py
--rw-r--r--   0        0        0     6122 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/rows/test_add_max_rows_in_max_groups.py
--rw-r--r--   0        0        0    18921 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/rows/test_add_max_rows_infs_nulls.py
--rw-r--r--   0        0        0    11005 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/rows/test_invalid.py
--rw-r--r--   0        0        0     4465 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/test_budgets.py
--rw-r--r--   0        0        0     2212 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/system/session/test_invalid_constraints.py
--rw-r--r--   0        0        0      108 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/__init__.py
--rw-r--r--   0        0        0      298 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    76602 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    60081 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0      107 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/__init__.py
--rw-r--r--   0        0        0    17843 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/conftest.py
--rw-r--r--   0        0        0    24106 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
--rw-r--r--   0        0        0    36803 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
--rw-r--r--   0        0        0     7610 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
--rw-r--r--   0        0        0    15631 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     2301 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_catalog.py
--rw-r--r--   0        0        0      657 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_cleanup.py
--rw-r--r--   0        0        0     5285 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_constraints.py
--rw-r--r--   0        0        0    21123 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_keyset.py
--rw-r--r--   0        0        0    14053 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3401 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     5865 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5480 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     3011 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    40466 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    63674 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16767 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     5021 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    93116 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_session.py
--rw-r--r--   0        0        0     1604 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_table_identifiers.py
--rw-r--r--   0        0        0     5372 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_transformation_utils.py
--rw-r--r--   0        0        0      741 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test/unit/test_utils.py
--rw-r--r--   0        0        0       18 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/test_requirements.txt
--rw-r--r--   0        0        0      447 2024-02-27 22:26:57.163525 tmlt_analytics-0.8.3/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     3666 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0    16162 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_neighboring_relation.py
--rw-r--r--   0        0        0     7164 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0     5683 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     4021 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    11046 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0     7694 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
--rw-r--r--   0        0        0    46362 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    47708 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0    60365 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    12795 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0     1250 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_table_identifier.py
--rw-r--r--   0        0        0     3980 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_table_reference.py
--rw-r--r--   0        0        0    10148 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_transformation_utils.py
--rw-r--r--   0        0        0      420 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/_type_checking.py
--rw-r--r--   0        0        0    12087 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      306 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0      458 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/constraints/__init__.py
--rw-r--r--   0        0        0     1101 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/constraints/_base.py
--rw-r--r--   0        0        0      735 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/constraints/_simplify.py
--rw-r--r--   0        0        0    12758 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/constraints/_truncation.py
--rw-r--r--   0        0        0    11850 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0    10546 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     5482 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   132256 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    41983 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    81606 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3917 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     6104 2024-02-27 22:26:57.167525 tmlt_analytics-0.8.3/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 tmlt_analytics-0.8.3/setup.py
--rw-r--r--   0        0        0     5082 1970-01-01 00:00:00.000000 tmlt_analytics-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/LICENSE
+-rw-r--r--   0        0        0    20138 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/LICENSE.docs
+-rw-r--r--   0        0        0      121 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/NOTICE
+-rw-r--r--   0        0        0     3303 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/README.md
+-rw-r--r--   0        0        0     1231 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1078 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_static/logo.png
+-rw-r--r--   0        0        0      133 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      491 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_templates/layout.html
+-rw-r--r--   0        0        0      106 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/_templates/package-name.html
+-rw-r--r--   0        0        0    22344 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/changelog.rst
+-rw-r--r--   0        0        0     8408 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/conf.py
+-rw-r--r--   0        0        0    10498 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/aws-glue.rst
+-rw-r--r--   0        0        0     1599 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3005 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1225 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6475 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5897 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4733 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1706 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0     6911 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/databricks.rst
+-rw-r--r--   0        0        0      339 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/index.rst
+-rw-r--r--   0        0        0     4895 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/installation.rst
+-rw-r--r--   0        0        0     4126 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/howto-guides/troubleshooting.rst
+-rw-r--r--   0        0        0   118378 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2024-04-08 13:09:56.959987 tmlt_analytics-0.9.0rc5/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0   344848 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_books_borrowed_by_zip.png
+-rw-r--r--   0        0        0    34101 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2024-04-08 13:09:56.963987 tmlt_analytics-0.9.0rc5/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    30778 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/chart_total_books_borrowed_in_zipcodes.png
+-rw-r--r--   0        0        0    20226 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    18639 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/flat_map_row_example.svg
+-rw-r--r--   0        0        0    23590 2024-04-08 13:09:56.967987 tmlt_analytics-0.9.0rc5/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0   116752 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/glue_graph.png
+-rw-r--r--   0        0        0    14685 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_api.svg
+-rw-r--r--   0        0        0      609 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_howto_guides.svg
+-rw-r--r--   0        0        0     1196 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    23369 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/intuitive_noise_visualization.png
+-rw-r--r--   0        0        0    30903 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/logo.png
+-rw-r--r--   0        0        0    85314 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/mock_checkout_logs.svg
+-rw-r--r--   0        0        0    59239 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/private_join_example.svg
+-rw-r--r--   0        0        0    35838 2024-04-08 13:09:56.971987 tmlt_analytics-0.9.0rc5/doc/images/private_join_tables.svg
+-rw-r--r--   0        0        0    32227 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/images/public_join_example_zips.svg
+-rw-r--r--   0        0        0    64480 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/images/tuning-parameters-error-vs-clamping-varied-budgets.png
+-rw-r--r--   0        0        0    27218 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/images/tuning-parameters-error-vs-clamping.png
+-rw-r--r--   0        0        0     5717 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/index.rst
+-rw-r--r--   0        0        0      662 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     3245 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/privacy-policy.rst
+-rw-r--r--   0        0        0     2100 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3516 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/templates/python/module.rst
+-rw-r--r--   0        0        0      396 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11868 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8665 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6589 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7849 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0    12509 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/understanding-sensitivity.rst
+-rw-r--r--   0        0        0     8467 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9126 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7219 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18785 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0     1133 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    12370 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     8434 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    15155 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16248 2024-04-08 13:09:56.975988 tmlt_analytics-0.9.0rc5/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     6579 2024-04-08 13:11:25.732937 tmlt_analytics-0.9.0rc5/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/__init__.py
+-rw-r--r--   0        0        0    11799 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/conftest.py
+-rw-r--r--   0        0        0      115 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/__init__.py
+-rw-r--r--   0        0        0     3447 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/conftest.py
+-rw-r--r--   0        0        0      108 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/__init__.py
+-rw-r--r--   0        0        0     2323 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0     6598 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_count_distinct_optimization.py
+-rw-r--r--   0        0        0     9173 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_id_col_operations.py
+-rw-r--r--   0        0        0    22198 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    14273 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     3969 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    26385 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    45748 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6122 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    18977 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0    10496 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     4465 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/test_budgets.py
+-rw-r--r--   0        0        0     2279 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/__init__.py
+-rw-r--r--   0        0        0     4726 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/base_builder/test_builder.py
+-rw-r--r--   0        0        0     7322 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/base_builder/test_mixins.py
+-rw-r--r--   0        0        0      298 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    65734 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    60081 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24188 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36803 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    15631 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      724 2024-04-08 13:09:56.979987 tmlt_analytics-0.9.0rc5/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21123 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    14053 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3751 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5480 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     2931 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40466 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    56419 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16768 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     5021 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    87198 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5372 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      741 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test/unit/test_utils.py
+-rw-r--r--   0        0        0       85 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/test_requirements.txt
+-rw-r--r--   0        0        0      681 2024-04-08 13:11:25.736937 tmlt_analytics-0.9.0rc5/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     5573 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_base_builder.py
+-rw-r--r--   0        0        0     3666 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16206 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     6824 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     6583 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     4838 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    60500 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_measurement_visitor.py
+-rw-r--r--   0        0        0    63111 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_transformation_visitor.py
+-rw-r--r--   0        0        0    11321 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7778 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0     5993 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    47962 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0      393 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12795 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3980 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10581 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0      487 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_type_checking.py
+-rw-r--r--   0        0        0      452 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/_utils.py
+-rw-r--r--   0        0        0    12094 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      374 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      458 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      802 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12758 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11801 2024-04-08 13:09:56.983987 tmlt_analytics-0.9.0rc5/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0    10828 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5429 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   133339 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41985 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    73619 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3913 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     6292 2024-04-08 13:09:56.987988 tmlt_analytics-0.9.0rc5/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     4743 1970-01-01 00:00:00.000000 tmlt_analytics-0.9.0rc5/setup.py
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 tmlt_analytics-0.9.0rc5/PKG-INFO
```

### Comparing `tmlt_analytics-0.8.3/CHANGELOG.rst` & `tmlt_analytics-0.9.0rc5/doc/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,47 @@
+..
+    SPDX-License-Identifier: CC-BY-SA-4.0
+    Copyright Tumult Labs 2024
 .. _analytics-changelog:
 
 Changelog
 =========
 
+Unreleased
+----------
+
+Changed
+~~~~~~~
+
+- :class:`~tmlt.analytics.keyset.KeySet` equality is now performed without
+  converting the underlying dataframe to Pandas.
+- :meth:`~tmlt.analytics.session.Session.partition_and_create`: the ``column`` and ``splits``
+  arguments are now annotated as required.
+
+Removed
+~~~~~~~
+- *Backwards-incompatible*: The ``stability`` and ``grouping_column`` parameters to :meth:`Session.from_dataframe <tmlt.analytics.session.Session.from_dataframe>` and :meth:`Session.Builder.with_private_dataframe <tmlt.analytics.session.Session.Builder.with_private_dataframe>` have been removed (deprecated since Tumult Analytics 0.7.0).
+  As a result, the ``protected_change`` parameter to those methods is now required.
+
+Fixed
+~~~~~
+- Improved the error message when attempting to overspend an ApproxDPBudget to more clearly indicate which component of the budget was insufficient to evaluate the query.
+- Updated the default behavior for the function :meth:`QueryBuilder.get_groups <tmlt.analytics.query_builder.QueryBuilder.get_groups>` to avoid using ID columns.
+- Flat maps now correctly ignore max_rows. Previously they would raise a warning saying that max_rows was ignored, but would still use it to limit the number of rows in the output.
+- Upgrades to version 0.12.0 of Tumult Core.
+
+.. _v0.8.3:
+
 0.8.3 - 2024-02-27
 ------------------
 
 This is a maintenance release that adds support for newer versions of Tumult Core. It contains no API changes.
 
+.. _v0.8.2:
+
 0.8.2 - 2023-11-29
 ------------------
 
 This release addresses a serious security vulnerability in PyArrow: `CVE-2023-47248 <https://nvd.nist.gov/vuln/detail/CVE-2023-47248>`__.
 It is **strongly recommended** that all users update to this version of Analytics or apply one of the mitigations described in the `GitHub Advisory <https://github.com/advisories/GHSA-5wvp-7f3h-6wmm>`__.
 
 Changed
@@ -21,48 +51,56 @@
   As a result:
 
   - Increased the minimum supported version of PyArrow to 14.0.1 for Python 3.8 and above.
   - Added dependency on ``pyarrow-hotfix`` on Python 3.7.
     Note that if you are using Python 3.7, the hotfix must be imported before using PySpark in order to be effective.
     Analytics imports the hotfix, so importing Analytics before using Spark will also work.
 
+.. _v0.8.1:
+
 0.8.1 - 2023-10-30
 ------------------
 
 This release adds support for Python 3.11, as well as compatibility with newer versions of various dependencies, including PySpark.
 It also includes documentation improvements, but no API changes.
 
+.. _v0.8.0:
+
 0.8.0 - 2023-08-15
 ------------------
 
 This is a maintenance release that addresses a performance regression for complex queries and improves naming consistency in some areas of the Tumult Analytics API.
 
 Added
 ~~~~~
 
 -  Added the :meth:`QueryBuilder.get_groups <tmlt.analytics.query_builder.QueryBuilder.get_groups>` function, for determining groupby keys for a table in a differentially private way.
 
 Changed
 ~~~~~~~
-- **Backwards-incompatible**: Renamed ``DropExcess.max_records`` to :attr:`~tmlt.analytics.truncation_strategy.TruncationStrategy.DropExcess.max_rows`.
-- **Backwards-incompatible**: Renamed ``FlatMap.max_num_rows`` to :attr:`~tmlt.analytics.query_expr.FlatMap.max_rows`.
+- *Backwards-incompatible*: Renamed ``DropExcess.max_records`` to :attr:`~tmlt.analytics.truncation_strategy.TruncationStrategy.DropExcess.max_rows`.
+- *Backwards-incompatible*: Renamed ``FlatMap.max_num_rows`` to :attr:`~tmlt.analytics.query_expr.FlatMap.max_rows`.
 - Changed the name of an argument for :meth:`QueryBuilder.flat_map()<tmlt.analytics.query_builder.QueryBuilder.flat_map>` from ``max_num_rows`` to ``max_rows``. The old ``max_num_rows`` argument is deprecated and will be removed in a future release.
 
 Fixed
 ~~~~~
 - Upgrades to version 0.11 of Tumult Core.
   This addresses a performance issue introduced in Tumult Analytics 0.7.0 where some complex queries compiled much more slowly than they had previously.
 
+.. _v0.7.3:
+
 0.7.3 - 2023-07-13
 ------------------
 
 Fixed
 ~~~~~
 - Fixed a crash in public and private joins.
 
+.. _v0.7.2:
+
 0.7.2 - 2023-06-15
 ------------------
 
 This release adds support for running Tumult Analytics on Python 3.10.
 It also enables adding continuous Gaussian noise to query results, and addresses a number of bugs and API inconsistencies.
 
 Added
@@ -82,20 +120,24 @@
   Bins with edges of other types are not affected.
 
 Fixed
 ~~~~~
 - Creating a :class:`~tmlt.analytics.session.Session` with multiple tables in an ID space used to fail if some of those tables' ID columns allowed nulls and others did not.
   This no longer occurs, and in such cases all of the tables' ID columns are made nullable.
 
+.. _v0.7.1:
+
 0.7.1 - 2023-05-23
 ------------------
 
 This is a maintenance release that mainly contains documentation updates.
 It also fixes a bug where installing Tumult Analytics using pip 23 and above could fail due to a dependency mismatch.
 
+.. _v0.7.0:
+
 0.7.0 - 2023-04-27
 ------------------
 
 This release adds support for *privacy identifiers*:
 Tumult Analytics can now protect input tables in which the differential privacy guarantee needs to hide the presence of arbitrarily many rows sharing the same value in a particular column.
 For example, this may be used to protect each user of a service when every row in a table is associated with a user ID.
 
@@ -141,19 +183,23 @@
 - :meth:`Session.add_public_datafame()<tmlt.analytics.session.Session.add_public_dataframe>` used to allow creation of a public table with the same name as an existing public table, which was neither intended nor fully supported by some :class:`~tmlt.analytics.session.Session` methods.
   It now raises a ``ValueError`` in this case.
 - Some query patterns on tables containing nulls could cause grouped aggregations to produce the wrong set of group keys in their output.
   This no longer happens.
 - In certain unusual cases, join transformations could erroneously drop rows containing nulls in columns that were not being joined on.
   These rows are no longer dropped.
 
+.. _v0.6.1:
+
 0.6.1 - 2022-12-07
 ------------------
 
 This is a maintenance release which introduces a number of documentation improvements, but has no publicly-visible API changes.
 
+.. _v0.6.0:
+
 0.6.0 - 2022-12-06
 ------------------
 
 .. _changelog#protected-change:
 
 This release introduces a new way to specify what unit of data is protected by the privacy guarantee of a :class:`~tmlt.analytics.session.Session`.
 A new ``protected_change`` parameter is available when creating a :class:`~tmlt.analytics.session.Session`, taking an instance of the new :class:`~tmlt.analytics.protected_change.ProtectedChange` class which describes the largest unit of data in the resulting table on which the differential privacy guarantee will hold.
@@ -172,14 +218,16 @@
 ------------------
 
 Changed
 ~~~~~~~
 
 -  Updated to Tumult Core 0.6.0.
 
+.. _v0.5.0:
+
 0.5.0 - 2022-10-17
 ------------------
 
 Added
 ~~~~~
 
 -  Added a diagram to the API reference page.
@@ -196,22 +244,26 @@
    As a result, ``python-flint`` is no longer a transitive dependency, simplifying the Analytics installation process.
 
 Deprecated
 ~~~~~~~~~~
 
 -  The contents of the ``cleanup`` module have been moved to the ``utils`` module. The ``cleanup`` module will be removed in a future version.
 
+.. _v0.4.2:
+
 0.4.2 - 2022-09-06
 ------------------
 
 Fixed
 ~~~~~
 
 -  Switched to Core version 0.4.3 to avoid warnings when evaluating some queries.
 
+.. _v0.4.1:
+
 0.4.1 - 2022-08-25
 ------------------
 
 Added
 ~~~~~
 
 -  Added ``QueryBuilder.histogram`` function, which provides a shorthand for generating binned data counts.
@@ -223,24 +275,28 @@
 -  Improved documentation for ``QueryBuilder.map`` and ``QueryBuilder.flat_map``.
 
 Fixed
 ~~~~~
 
 -  Switched to Core version 0.4.2, which contains a fix for an issue that sometimes caused queries to fail to be compiled.
 
+.. _v0.4.0:
+
 0.4.0 - 2022-07-22
 ------------------
 
 Added
 ~~~~~
 
 -  ``Session.from_dataframe`` and ``Session.Builder.with_private_dataframe`` now have a ``grouping_column`` option and support non-integer stabilities.
    This allows setting up grouping columns like those that result from grouping flatmaps when loading data.
    This is an advanced feature, and should be used carefully.
 
+.. _v0.3.0:
+
 0.3.0 - 2022-06-23
 ------------------
 
 Added
 ~~~~~
 
 -  Added ``QueryBuilder.bin_column`` and an associated ``BinningSpec`` type.
@@ -278,14 +334,16 @@
 -  *Backwards-incompatible*: ``KeySet``\ s now explicitly check for and disallow the use of floats and timestamps as keys.
    This has always been the intended behavior, but it was previously not checked for and could work or cause non-obvious errors depending on the situation.
 -  ``KeySet.dataframe()`` now always returns a dataframe where all rows are distinct.
 -  Under certain circumstances, evaluating a ``GroupByCountDistinct`` query expression used to modify the input ``QueryExpr``.
    This no longer occurs.
 -  It is now possible to partition on a column created by a grouping flat map, which used to raise exception from Core.
 
+.. _v0.2.1:
+
 0.2.1 - 2022-04-14 (internal release)
 -------------------------------------
 
 Added
 ~~~~~
 
 -  Added support for basic operations (filter, map, etc.) on Spark date and timestamp columns.
@@ -293,14 +351,16 @@
 -  Future documentation will now include any exceptions defined in Analytics.
 
 Changed
 ~~~~~~~
 
 -  Switch session to use Persist/Unpersist instead of Cache.
 
+.. _v0.2.0:
+
 0.2.0 - 2022-03-28 (internal release)
 -------------------------------------
 
 Removed
 ~~~~~~~
 
 -  Multi-query evaluate support is entirely removed.
@@ -318,14 +378,16 @@
    Sessions can be manually closed with ``session.stop()``.
 
 Fixed
 ~~~~~
 
 -  Joining with a public table that contains no NaNs, but has a column where NaNs are allowed, previously caused an error when compiling queries. This is now handled correctly.
 
+.. _v0.1.1:
+
 0.1.1 - 2022-02-28 (internal release)
 -------------------------------------
 
 Added
 ~~~~~
 
 -  Added a ``KeySet`` class, which will eventually be used for all GroupBy queries.
@@ -342,14 +404,16 @@
 
 Deprecated
 ~~~~~~~~~~
 
 -  ``QueryBuilder.groupby_domains()`` and ``QueryBuilder.groupby_public_source()`` are now deprecated in favor of using ``QueryBuilder.groupby()`` with ``KeySet``\ s.
    They will be removed in a future version.
 
+.. _v0.1.0:
+
 0.1.0 - 2022-02-15 (internal release)
 -------------------------------------
 
 Added
 ~~~~~
 
 -  Initial release.
```

### Comparing `tmlt_analytics-0.8.3/LICENSE` & `tmlt_analytics-0.9.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/LICENSE.docs` & `tmlt_analytics-0.9.0rc5/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/README.md` & `tmlt_analytics-0.9.0rc5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 If you have any questions, feedback, or feature requests, please reach out to us on [Slack](https://tmlt.dev/slack).
 
 ## Contributing
 
 We do not yet have a process in place to accept external contributions, but we are open to collaboration opportunities.
 If you are interested in contributing, please let us know [via Slack](https://tmlt.dev/slack).
 
-See [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.
+See [CONTRIBUTING.md](https://gitlab.com/tumult-labs/analytics/-/blob/dev/CONTRIBUTING.md) for information about installing our development dependencies and running tests.
 
 ## Citing Tumult Analytics
 
 If you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.
 
 ```
 @software{tumultanalyticssoftware,
```

### Comparing `tmlt_analytics-0.8.3/doc/_static/css/custom.css` & `tmlt_analytics-0.9.0rc5/doc/_static/css/custom.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+/* SPDX-License-Identifier: CC-BY-SA-4.0 */
+/* Copyright Tumult Labs 2024 */
 caption {
     padding: 0px;
     caption-side: top;
     font-weight: bold;
     color: rgba(var(--pst-color-paragraph),1);
 }
```

### Comparing `tmlt_analytics-0.8.3/doc/_static/favicon.ico` & `tmlt_analytics-0.9.0rc5/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/_static/js/version-banner.js` & `tmlt_analytics-0.9.0rc5/doc/_static/js/version-banner.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,9 @@
+/* SPDX-License-Identifier: CC-BY-SA-4.0 */
+/* Copyright Tumult Labs 2024 */
 function injectBanner(content) {
     var body = document.getElementsByClassName('bd-content')[0];
     if (body) {
         body.prepend(content);
     } else {
         console.warn("Unable to find body element, skipping banner injection");
     }
```

### Comparing `tmlt_analytics-0.8.3/doc/_static/logo.png` & `tmlt_analytics-0.9.0rc5/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/conf.py` & `tmlt_analytics-0.9.0rc5/doc/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # pylint: skip-file
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import logging
 import os
 import sys
 import datetime
 
 _logger = logging.getLogger(__name__)
 
 # Project information
 
 project = "Tumult Analytics"
-author = "Tumult Labs"
-copyright = "Tumult Labs 2023"
-
 package_name = "tmlt.analytics"
+author = "Tumult Labs"
+copyright = "Tumult Labs 2024"
 
 # TODO(#1256): Fix import failure in nested class; `tmlt.core` and remove suppress_warnings setting
 suppress_warnings = ["autoapi.python_import_resolution", "autodoc.import_object"]
 
 
 # Build information
 
@@ -143,14 +142,31 @@
     ("py:class", "BinNameT"),
     ("py:class", "Generic[BinT, BinNameT]"),
     ("py:class", "tmlt.core.domains.spark_domains.SparkColumnsDescriptor"),
     ("py:class", "sympy.core.expr.Expr"),
     ("py:class", "Epsilon"),
     ("py:class", "Delta"),
     ("py:class", "Rho"),
+    ("py:class", "Transformation"),
+    ("py:class", "pydantic.BaseModel"),
+    ("py:class", "Model"),
+    ("py:class", "Literal"),
+    ("py:class", "IncEx"),
+    ("py:class", "pydantic.json_schema.GenerateJsonSchema"),
+    ("py:class", "pydantic.json_schema.JsonSchemaMode"),
+    ("py:class", "pydantic.json_schema.JsonSchemaValue"),
+    ("py:exc", "ValidationError"),
+    ("py:class", "BaseModel"),
+    ("py:class", "pydantic.annotated_handlers.GetCoreSchemaHandler"),
+    ("py:class", "pydantic_core.CoreSchema"),
+    ("py:class", "pydantic.annotated_handlers.GetJsonSchemaHandler"),
+    ("py:class", "TupleGenerator"),
+    ("py:class", "AbstractSetIntStr"),
+    ("py:class", "MappingIntStrAny"),
+    ("py:class", "pydantic.fields.ComputedFieldInfo"),
 ]
 
 # Remove this after intersphinx can use core
 nitpick_ignore_regex = [(r"py:.*", r"tmlt.core.*")]
 
 # Theme settings
 templates_path = ["_templates"]
@@ -201,28 +217,42 @@
     "numpy": ("https://numpy.org/doc/1.18/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/version/1.2.0/", None),
     "sympy": ("https://docs.sympy.org/latest/", None),
     "pyspark": ("https://spark.apache.org/docs/3.0.0/api/python/", None),
 }
 
 
+# Substitutions
+
+rst_epilog = """
+.. |PRO| raw:: html
+    
+    <a href="https://tmlt.dev" style="text-decoration : none">
+        <img src="https://img.shields.io/badge/PRO-c53a58" alt="This is only applicable to Analytics Pro." title="This is only available in Analytics Pro">
+    </a>
+.. |PRO_NOTE| replace:: This is only available on a paid version of Tumult Analytics. If you
+    would like to hear more, please contact us at info@tmlt.io.
+"""
+
+
 def skip_members(app, what, name, obj, skip, options):
     """Skip some members."""
     excluded_methods = [
         "__dir__",
         "__format__",
         "__hash__",
         "__post_init__",
         "__reduce__",
         "__reduce_ex__",
         "__repr__",
         "__setattr__",
         "__sizeof__",
         "__str__",
         "__subclasshook__",
+        "__init_subclass__",
     ]
     excluded_attributes = ["__slots__"]
     if what == "method" and name.split(".")[-1] in excluded_methods:
         return True
     if what == "attribute" and name.split(".")[-1] in excluded_attributes:
         return True
     if "@nodoc" in obj.docstring:
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/aws-glue.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/aws-glue.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Using Tumult Analytics on AWS Glue
 ==================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This guide covers using Tumult Analytics as part of an `AWS Glue <https://aws.amazon.com/glue/>`__ data pipeline.
 The instructions use `AWS Glue Studio <https://docs.aws.amazon.com/glue/latest/ug/what-is-glue-studio.html>`__, Glue's visual job editor and management interface, but the general steps apply to other ways of configuring Glue jobs as well.
 
 Setting up requirements
 ^^^^^^^^^^^^^^^^^^^^^^^
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/bigquery-setup.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/bigquery-setup.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _BigQuery setup:
 
 Introduction to BigQuery
 ========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 BigQuery is a serverless, highly scalable, cost-effective, and fully managed
 cloud data warehouse for analytics.
 
 In this first section, we will upload a file to BigQuery to use as input for our DP query.
 We will use the same input data as for the Tumult Analytics :ref:`tutorial<first steps>`, which is provided
 as a CSV file.
@@ -28,9 +28,9 @@
 
 With our data in place, we can explore the data in BigQuery.
 We can expand the dataset we previously created, open up the table
 to see the schema, and query the data in the query editor
 using SQL.
 
 Now that we've set up our environment in BigQuery, let's move on to the :ref:`next part<bigquery inputs and outputs>`
-of the topic guide and see how we would modify a simple Tumult Analtyics program to be able
+of the topic guide and see how we would modify a simple Tumult Analytics program to be able
 to run in BigQuery.
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/docker-image.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/docker-image.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _GCP Docker Image:
 
 Creating a Docker image for GCP
 ===============================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In this final part of the topic guide, we will customize our own
 Docker image to contain additional libraries and dependencies.
 A working knowledge of Docker is useful to understand this section,
 but if you have never used Docker before, you can still follow the
 instructions below.
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/index.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Using Tumult Analytics on BigQuery
 ==================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This guide explains how to use Tumult Analytics on BigQuery.
 We will guide you to getting a minimal example of a Tumult
 Analytics program running on BigQuery, then we will explain how to
 modify this program to work with custom parameters and custom
 libraries.
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/inputs-outputs.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/inputs-outputs.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 .. _BigQuery inputs and outputs:
 
 BigQuery inputs and outputs
 ===========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In this section, we will show how to adapt a Tumult Analytics
 program to use BigQuery inputs and outputs, and provide a minimal
 example of a BigQuery-compatible program.
 
-We will use the simple program from :ref:`the first tutorial<first steps>`
+We will use the simple program from :ref:`first steps tutorial<first steps>`
 which constructs a differentially private count of the number of
 members in a fake dataset containing members of a public library
 ``library-members``.
 
 .. testcode::
 
     from pyspark import SparkFiles
     from pyspark.sql import SparkSession
     from tmlt.analytics.privacy_budget import PureDPBudget
+    from tmlt.analytics.protected_change import AddOneRow
     from tmlt.analytics.query_builder import QueryBuilder
     from tmlt.analytics.session import Session
 
     spark = SparkSession.builder.getOrCreate()
 
     spark.sparkContext.addFile(
         "https://tumult-public.s3.amazonaws.com/library-members.csv"
@@ -32,15 +33,16 @@
     members_df = spark.read.csv(
         SparkFiles.get("library-members.csv"), header=True, inferSchema=True
     )
 
     session = Session.from_dataframe(
         privacy_budget=PureDPBudget(3),
         source_id="members",
-        dataframe=members_df
+        dataframe=members_df,
+        protected_change=AddOneRow()
     )
 
     count_query = QueryBuilder("members").count()
     total_count = session.evaluate(
         count_query,
         privacy_budget=PureDPBudget(epsilon=1)
     )
@@ -151,24 +153,25 @@
     )
 
 The format for table names is ``[PROJECT]:[DATASET].[TABLE]``.
 
 Full example
 ------------
 
-In the end, your program should look structually similar to this final program.
+In the end, your program should look structurally similar to this final program.
 
 .. code-block:: python
 
     import json
     import os
 
     from pyspark.sql import SparkSession
 
     from tmlt.analytics.privacy_budget import PureDPBudget
+    from tmlt.analytics.protected_change import AddOneRow
     from tmlt.analytics.query_builder import QueryBuilder
     from tmlt.analytics.session import Session
 
     BUCKET = "tumult-warehouse"
     INPUT_TABLE = "tumult-labs.analytics_tutorial.library_members"
     OUTPUT_TABLE = "tumult-labs.analytics_tutorial.member_counts"
 
@@ -185,15 +188,16 @@
         .option("table", INPUT_TABLE)
         .load()
     )
 
     session = Session.from_dataframe(
         privacy_budget=PureDPBudget(3),
         source_id="members",
-        dataframe=members_df
+        dataframe=members_df,
+        protected_change=AddOneRow()
     )
 
     count_query = QueryBuilder("members").count()
     total_count = session.evaluate(
         count_query,
         privacy_budget=PureDPBudget(epsilon=1)
     )
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/parameters.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/parameters.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Passing parameters to a stored procedure:
 
 Passing parameters to a stored procedure
 ========================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In this additional section of the topic guide, we will explain how
 to pass parameters from BigQuery to the stored procedure containing
 our Tumult Analytics program. This makes it possible to customize the
 call, by specifying e.g. different inputs or outputs table, or privacy
 parameters, without modifying the underlying program.
 
@@ -66,14 +66,15 @@
 
     import json
     import os
 
     from pyspark.sql import SparkSession
 
     from tmlt.analytics.privacy_budget import PureDPBudget
+    from tmlt.analytics.protected_change import AddOneRow
     from tmlt.analytics.query_builder import QueryBuilder
     from tmlt.analytics.session import Session
 
     BUCKET = "tumult-warehouse"
     INPUT_TABLE = "tumult-labs.analytics_tutorial.library_members"
     OUTPUT_TABLE = "tumult-labs.analytics_tutorial.member_counts"
 
@@ -90,15 +91,16 @@
         .option("table", INPUT_TABLE)
         .load()
     )
 
     session = Session.from_dataframe(
         privacy_budget=PureDPBudget(3),
         source_id="members",
-        dataframe=members_df
+        dataframe=members_df,
+        protected_change=AddOneRow(),
     )
 
     count_query = QueryBuilder("members").count()
     total_count = session.evaluate(
         count_query,
         privacy_budget=PureDPBudget(epsilon=1)
     )
@@ -129,15 +131,15 @@
     +BUCKET = json.loads(os.environ["BIGQUERY_PROC_PARAM.bucket"])
     +INPUT_TABLE = json.loads(os.environ["BIGQUERY_PROC_PARAM.input"])
     +OUTPUT_TABLE = json.loads(os.environ["BIGQUERY_PROC_PARAM.output"])
 
 Full example
 ------------
 
-In the end, your program should look structually similar to this final program.
+In the end, your program should look structurally similar to this final program.
 
 .. code-block:: python
 
    import json
    import os
 
    from pyspark.sql import SparkSession
@@ -163,15 +165,16 @@
      .option("table", INPUT_TABLE)
      .load()
    )
 
    session = Session.from_dataframe(
        privacy_budget=PureDPBudget(3),
        source_id="members",
-       dataframe=members_df
+       dataframe=members_df,
+       protected_change=AddOneRow(),
    )
 
    count_query = QueryBuilder("members").count()
    total_count = session.evaluate(
        count_query,
        privacy_budget=PureDPBudget(epsilon=1)
    )
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/running-the-program.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/running-the-program.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Running the program:
 
 Calling Tumult Analytics from a BigQuery stored procedure
 =========================================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In this section, we will explain how to run a Tumult Analytics
 program directly from BigQuery. We will do so using the sample
 program from the :ref:`second part<bigquery inputs and outputs>`
 of this topic guide.
 
 You should also have data in BigQuery, and a Google Cloud Storage bucket
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/bigquery/setup.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/bigquery/setup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _GCP setup:
 
 GCP setup
 =========
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 When entering Google Cloud Platform (GCP) for the first time,
 you will be greeted with your project dashboard.
 
 The search bar on top of the page can be used to search for,
 and navigate to, any service in GCP.
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/databricks.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/databricks.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Using Tumult Analytics on Databricks
 ====================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This guide covers installing and running Tumult Analytics in notebooks on `Databricks <https://www.databricks.com/>`__.
 It assumes that you have an existing Databricks workspace with a compatible compute cluster available.
 Tumult Analytics is currently compatible with versions 7.3 LTS through 12.2 LTS of the `Databricks runtime <https://docs.databricks.com/release-notes/runtime/releases.html>`__.
 
 Installation
 ^^^^^^^^^^^^
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/installation.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 .. _Installation instructions:
+..
+    SPDX-License-Identifier: CC-BY-SA-4.0
+    Copyright Tumult Labs 2024
 
 Installation instructions
 =========================
 
 This guide will help you set up Tumult Analytics on your local machine.
 
 Prerequisites
@@ -22,15 +25,15 @@
 .. tabbed:: Linux (Debian-based)
 
     Python and ``pip``, Python's package manager, are likely already installed.
     If they are not, install them with:
 
     .. code-block:: bash
 
-        apt install python3 python3-pip
+        apt install python3.11 python3-pip
 
     Java may already be installed as well.
     If it is not, install the Java Runtime Environment with:
 
     .. code-block:: bash
 
         apt install default-jre-headless
@@ -40,15 +43,15 @@
 
     Python and ``pip``, Python's package manager, may already be installed.
     On some releases, Python 2 may be installed by default, but not Python 3.
     To install Python 3, run:
 
     .. code-block:: bash
 
-        yum install python3 python3-pip
+        yum install python3.11 python3-pip
 
     To install Java, run:
 
     .. code-block:: bash
 
         yum install java-1.8.0-openjdk-headless
 
@@ -64,46 +67,46 @@
 
         /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 
     Python may be installed with:
 
     .. code-block:: bash
 
-        brew install python@3.7
+        brew install python@3.11
 
     And Java may be installed with:
 
     .. code-block:: bash
 
         brew install openjdk@8
 
     You may need to explicitly add this OpenJDK installation to your ``PATH`` for it to be detected and usable by Spark.
     This can be done by, for example, adding ``export PATH="/usr/local/opt/openjdk/bin:$PATH"`` to ``.bashrc`` and then restarting your shell.
 
 
 .. tabbed:: macOS (Apple silicon)
 
-    Since Python 3.7 is not supported on the Apple silicon processor architecture, you will need to first install `Rosetta 2 <https://support.apple.com/en-us/HT211861>`__ and the x86_64 version of Homebrew.
+    Since some dependencies of Tumult Analytics are not supported on the Apple silicon processor architecture, you will need to first install `Rosetta 2 <https://support.apple.com/en-us/HT211861>`__ and the x86_64 version of Homebrew.
     If you do not already have Rosetta 2, it can be installed with:
 
     .. code-block:: bash
 
         softwareupdate --install-rosetta
 
     The x86_64 version of Homebrew can be installed with:
 
     .. code-block:: bash
 
         arch -x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
 
-    Now, you can install Python 3.7 with:
+    Now, you can install Python 3.11 with:
 
     .. code-block:: bash
 
-        arch -x86_64 /usr/local/bin/brew install python@3.7
+        arch -x86_64 /usr/local/bin/brew install python@3.11
 
     And Java may be installed with:
 
     .. code-block:: bash
 
         arch -x86_64 /usr/local/bin/brew install openjdk@8
```

### Comparing `tmlt_analytics-0.8.3/doc/howto-guides/troubleshooting.rst` & `tmlt_analytics-0.9.0rc5/doc/howto-guides/troubleshooting.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Troubleshooting:
 
 Troubleshooting
 ===============
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This page lists common issues that can arise when using Tumult Analytics,
 and explains how to address them.
 
 Handling large amounts of data
 ------------------------------
```

### Comparing `tmlt_analytics-0.8.3/doc/images/api_diagram.svg` & `tmlt_analytics-0.9.0rc5/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_books_by_unique_members.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_books_by_unique_members.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_counts_education.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_favorite_genres.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_favorite_genres.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_filters_education.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_genres_by_age.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_genres_by_age.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.9.0rc5/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.9.0rc5/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/flat_map_row_example.svg` & `tmlt_analytics-0.9.0rc5/doc/images/flat_map_row_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/flow_chart_truncation.svg` & `tmlt_analytics-0.9.0rc5/doc/images/flow_chart_truncation.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/glue_graph.png` & `tmlt_analytics-0.9.0rc5/doc/images/glue_graph.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.9.0rc5/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/index_api.svg` & `tmlt_analytics-0.9.0rc5/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/index_howto_guides.svg` & `tmlt_analytics-0.9.0rc5/doc/images/index_howto_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/index_more.svg` & `tmlt_analytics-0.9.0rc5/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/index_topic_guides.svg` & `tmlt_analytics-0.9.0rc5/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/index_tutorials.svg` & `tmlt_analytics-0.9.0rc5/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/intuitive_noise_visualization.png` & `tmlt_analytics-0.9.0rc5/doc/images/intuitive_noise_visualization.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/logo.png` & `tmlt_analytics-0.9.0rc5/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/mock_checkout_logs.svg` & `tmlt_analytics-0.9.0rc5/doc/images/mock_checkout_logs.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/private_join_example.svg` & `tmlt_analytics-0.9.0rc5/doc/images/private_join_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/private_join_tables.svg` & `tmlt_analytics-0.9.0rc5/doc/images/private_join_tables.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/images/public_join_example_zips.svg` & `tmlt_analytics-0.9.0rc5/doc/images/public_join_example_zips.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/index.rst` & `tmlt_analytics-0.9.0rc5/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+..
+    SPDX-License-Identifier: CC-BY-SA-4.0
+    Copyright Tumult Labs 2024
+
 Tumult Analytics documentation
 ==============================
 
 .. toctree::
    :hidden:
    :maxdepth: 1
 
@@ -137,15 +141,15 @@
         journal={arXiv preprint arXiv:2212.04133},
         month = dec,
         year={2022}
     }
 
 License
 ^^^^^^^
-The Tumult Analytics source code and documentation are copyright Tumult Labs 2023.
+The Tumult Analytics source code and documentation are copyright Tumult Labs 2024.
 
 This documentation is licensed under the
 Creative Commons Attribution-ShareAlike 4.0 Unported License.
 To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/
 or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
 
 The Tumult Analytics source code is licensed under the Apache License, version 2.0 (`Apache-2.0 <https://gitlab.com/tumult-labs/core/-/blob/dev/LICENSE>`_).
```

### Comparing `tmlt_analytics-0.8.3/doc/intersphinx_mapping.json` & `tmlt_analytics-0.9.0rc5/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.8.3/doc/privacy-policy.rst` & `tmlt_analytics-0.9.0rc5/doc/privacy-policy.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 :orphan:
 
+..
+    SPDX-License-Identifier: CC-BY-SA-4.0
+    Copyright Tumult Labs 2024
 .. _privacy-policy:
 
 Privacy Policy
 ==============
 
 Effective Date: Aug 26th, 2022
```

### Comparing `tmlt_analytics-0.8.3/doc/templates/python/class.rst` & `tmlt_analytics-0.9.0rc5/doc/templates/python/class.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 {% if obj.display %}
 
+..
+    SPDX-License-Identifier: CC-BY-SA-4.0
+    Copyright Tumult Labs 2024
 .. py:{{ obj.type }}:: {{ obj.short_name }}{% if obj.args %}({{ obj.args }}){% endif %}
 
    {% if obj.bases %}
 
    Bases: {% for base in obj.bases %}:class:`{{ base }}`{% if not loop.last %}, {% endif %}{% endfor %}
 
    {% endif %}
```

### Comparing `tmlt_analytics-0.8.3/doc/templates/python/module.rst` & `tmlt_analytics-0.9.0rc5/doc/templates/python/module.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 {% if not obj.display %}
 :orphan:
 {% endif %}
 
+..
+    SPDX-License-Identifier: CC-BY-SA-4.0
+    Copyright Tumult Labs 2024
 {% set name_parts = obj.name.split('.') %}
 
 {% if obj.name == package_name %}
    {% set module_title = "API Reference" %}
 {% elif name_parts|length > 2 %}
    {% set module_title = obj.short_name %}
 {% else %}
```

### Comparing `tmlt_analytics-0.8.3/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.9.0rc5/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Nulls, NaNs, and infinite values:
 
 Nulls, NaNs, and infinite values
 ================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This topic guide details how 
 `null values <https://en.wikipedia.org/wiki/Null_(SQL)>`__,
 `NaN values <https://en.wikipedia.org/wiki/NaN>`__, and 
 `infinite values <https://en.wikipedia.org/wiki/IEEE_754-1985#Positive_and_negative_infinity>`__
 (positive and negative infinity) are handled in Tumult Analytics.
 
@@ -18,14 +18,15 @@
 
     # Hidden block for imports to make examples testable.
     import pandas as pd
     from pyspark.sql import SparkSession
 
     from tmlt.analytics.keyset import KeySet
     from tmlt.analytics.privacy_budget import PureDPBudget
+    from tmlt.analytics.protected_change import AddOneRow
     from tmlt.analytics.query_builder import QueryBuilder
     from tmlt.analytics.session import Session
 
 Constructing Sessions with Null, NaN, and infinite values
 ---------------------------------------------------------
 
 By default, Tumult Analytics allows you to use DataFrames that contain
@@ -48,14 +49,15 @@
 
 .. testcode::
    
    session_with_nulls = Session.from_dataframe(
        privacy_budget=PureDPBudget(2),
        source_id="my_private_data",
        dataframe=spark_df,
+       protected_change=AddOneRow(),
    )
    spark_df.show()
 
 .. testoutput::
     :options: +NORMALIZE_WHITESPACE
 
     +-----+---+--------+
@@ -181,14 +183,15 @@
 
 .. testcode::
 
     session = Session.from_dataframe(
         privacy_budget=PureDPBudget(float("inf")),
         source_id="checkouts",
         dataframe=private_data,
+        protected_change=AddOneRow(),
     )
     private_data.show()
 
 .. testoutput::
    :options: +NORMALIZE_WHITESPACE
 
     +-----+-------+-----------+
@@ -289,14 +292,15 @@
 
 .. testcode::
 
     session = Session.from_dataframe(
         privacy_budget=PureDPBudget(float("inf")),
         source_id="checkouts",
         dataframe=private_data,
+        protected_change=AddOneRow(),
     )
     private_data.show()
 
 .. testoutput::
    :options: +NORMALIZE_WHITESPACE
 
     +-------+---------------+-----------+
```

### Comparing `tmlt_analytics-0.8.3/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-budgets.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 
 Privacy budget fundamentals
 ===========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This topic guide goes into more depth on the concept of *privacy budgets* that
-we discussed in :ref:`tutorial two <Working with privacy budgets>`. At a high
+we discussed in :ref:`working with privacy budgets tutorial<Working with privacy budgets>`. At a high
 level, a privacy budget associates one or more numeric *privacy parameters* with
 a *privacy definition*. Together, this information determines the privacy
 guarantees provided by each query, and by the Session as a whole.
 
 In particular, a privacy budget determines how much randomization is added
 to the computation of a query. Choosing an appropriate budget
 for a given query is ultimately an exercise in balancing privacy and accuracy
@@ -41,16 +41,16 @@
 
 Tumult Analytics provides the :class:`~tmlt.analytics.privacy_budget.PrivacyBudget`
 interface and two concrete implementations for specifying privacy budgets,
 depending on which privacy definition you wish to use:
 :class:`~tmlt.analytics.privacy_budget.PureDPBudget`
 and :class:`~tmlt.analytics.privacy_budget.RhoZCDPBudget`.
 
-Recall from tutorials :ref:`one <First steps>` and
-:ref:`two <Working with privacy budgets>` that when you initialize a Session,
+Recall from tutorials :ref:`first steps<First steps>` and
+:ref:`working with privacy budgets<Working with privacy budgets>` that when you initialize a Session,
 you must allocate a total privacy budget for it. Then, each time you evaluate a
 query through the Session, you must specify how much budget the query should
 use, which is then subtracted from the Session's total. For example, if you
 initialize a Session with :code:`PureDPBudget(epsilon=5)`, and then evaluate a
 query with :code:`PureDPBudget(epsilon=2)`, then your Session's remaining budget
 will be :code:`PureDPBudget(epsilon=3)`.
 
@@ -73,16 +73,16 @@
 
 When you're deciding how much privacy budget to use for a query, there is no single
 "right" choice. The choice of budget
 is ultimately a balance between accuracy and privacy, with lower budgets
 yielding noisier results and higher budgets yielding more accurate
 (and thus less private) results.
 
-To better understand how epsilon impacts this tradeoff, let's look at a simple
-example. We'll use the example dataset from :ref:`tutorial one <First steps>`,
+To better understand how epsilon impacts this trade-off, let's look at a simple
+example. We'll use the example dataset from the :ref:`first steps tutorial<First steps>`,
 and we'll perform a simple query to count the number of rows in the dataset.
 The figure below plots the results of running this count query using a
 :code:`PureDPBudget` with 3 different epsilon values, 50 times each:
 
 .. image:: ../images/chart_counts_different_eps.png
     :scale: 100%
     :alt: Graph plotting noisy counts under different epsilon values. The values are
@@ -136,15 +136,15 @@
 
 For an even more in-depth explanation of this topic, you can check out the following
 `blog post <https://desfontain.es/privacy/differential-privacy-in-more-detail.html>`__.
 
 The impact of data size
 ^^^^^^^^^^^^^^^^^^^^^^^
 
-Another factor that impacts the privacy/accuracy tradeoff associated with a given
+Another factor that impacts the privacy/accuracy trade-off associated with a given
 budget is the size of each group on which aggregations are computed. In our first example
 above, even with the smallest budget of 0.2, all the noisy results were within
 about +/- 25 of the true count, which is a relative spread of about 0.05%.
 But what happens if we aggregate the data in smaller groups?
 Consider again our database of library members. Instead of counting all rows 
 in the database, we'll first group members by age and education level, and then
 count how many members fall in each group. The below graph plots the percentage error
```

### Comparing `tmlt_analytics-0.8.3/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.9.0rc5/doc/topic-guides/privacy-promise.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Privacy promise:
 
 Tumult Analytics' privacy promise
 =================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This topic guide outlines the "privacy promise" provided by Tumult Analytics,
 along with its caveats. This guarantee is based on one of the core abstractions
 of Tumult Analytics: :class:`Sessions <tmlt.analytics.session.Session>`.
 
 At a high level, a Session allows you to evaluate queries on private data in a
 way that satisfies differential privacy. When creating a Session, private data
```

### Comparing `tmlt_analytics-0.8.3/doc/topic-guides/spark.rst` & `tmlt_analytics-0.9.0rc5/doc/topic-guides/spark.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Spark:
 
 Spark
 =====
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 Tumult Analytics uses Spark as its underlying data processing
 framework. This topic guide covers relevant information about Spark
 for Tumult Analytics users.
 
 Configuring Spark sessions
 --------------------------
@@ -40,17 +40,18 @@
     will result in Spark raising ``java.lang.UnsupportedOperationException: sun.misc.Unsafe`` or ``java.nio.DirectByteBuffer.(long, int) not available`` 
     when evaluating queries. 
     
     Tumult Analytics attempts to set these options automatically, but if you are encountering issues, you may want to try:
 
     .. code-block::
 
-        from tmlt.analytics.utils import get_java11_config
+        from pyspark.sql import SparkSession
+        from tmlt.analytics.utils import get_java_11_config
 
-        spark = SparkSession.builder.config(conf=get_java11_config()).getOrCreate()
+        spark = SparkSession.builder.config(conf=get_java_11_config()).getOrCreate()
 
     instead of:
 
     .. code-block::
 
         spark = SparkSession.builder.getOrCreate()
```

### Comparing `tmlt_analytics-0.8.3/doc/topic-guides/understanding-sensitivity.rst` & `tmlt_analytics-0.9.0rc5/doc/topic-guides/understanding-sensitivity.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 Understanding sensitivity
 =========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This topic guide goes into detail on the concept of *sensitivity* in
 differential privacy.
 
 Sensitivity is the maximum impact that a protected change can have on a query's
 results. It directly impacts how much noise must be added to achieve differential
 privacy: the bigger the sensitivity, the more noise needs to be added to the result.
@@ -45,15 +45,15 @@
 :meth:`private joins<tmlt.analytics.query_builder.QueryBuilder.join_private>`.
 
 Flat maps
 ~~~~~~~~~
 
 A :meth:`flat_map<tmlt.analytics.query_builder.QueryBuilder.flat_map>` maps each
 input row to zero or more new rows. Consider the example from
-:ref:`tutorial five <flat-map-tutorial-5>`, where each input row is mapped to up
+:ref:`simple transformations tutorial<flat-map-tutorial-5>`, where each input row is mapped to up
 to three new rows, using to the ``max_rows=3`` parameter. On a per-row basis, this operation might look like this:
 
 .. image:: ../images/flat_map_row_example.svg
     :alt: On the left, one row containing a list of genres. On the right, three rows, each containing one genre from the list.
     :align: center
 
 In this example, the input table was initialized with the
```

### Comparing `tmlt_analytics-0.8.3/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.9.0rc5/doc/topic-guides/working-with-sessions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Working with Sessions:
 
 Working with Sessions
 =====================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 This topic guide covers how to work with one of the core abstractions of Tumult
 Analytics: :class:`Session <tmlt.analytics.session.Session>`. In particular, we
 will demonstrate the different ways that a Session can be initialized and
 examined. For a simple end-to-end usage example of a Session, a better place to
 start is the :ref:`privacy budget tutorial <Working with privacy budgets>`.
 
@@ -77,15 +77,15 @@
         source_id="my_private_data",
         dataframe=spark_df,
         protected_change=AddOneRow(),
     )
 
 When you load a Spark DataFrame into a Session, you don't need to specify the
 schema of the source; it is automatically inferred from the DataFrame's schema.
-Recall from the :ref:`first tutorial <First steps>` that :code:`source_id` is
+Recall from the :ref:`first steps tutorial<First steps>` that :code:`source_id` is
 simply a unique identifier for the private data that is used when constructing
 queries.
 
 Using a Session Builder
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 For analysis use cases involving only one private data source,
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/clamping-bounds.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .. _Clamping bounds:
 
-Tutorial 3: Introduction to clamping bounds
-===========================================
+Numerical aggregations
+======================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
-Counting queries, which we saw in tutorials :ref:`one <First steps>` and
-:ref:`two <Working with privacy budgets>`, are very useful, but we often need a
+Counting queries, which we saw in tutorials :ref:`first steps tutorial<First steps>` and
+:ref:`working with privacy budgets tutorial<Working with privacy budgets>`, are very useful, but we often need a
 little more: sums, averages, medians… In this tutorial, we'll see how to compute
 this larger class of aggregations with Tumult Analytics. These operations
 require us to learn and use a new concept: *clamping bounds*. In this tutorial,
 we'll tell you what these are, how they work, and how to specify them in
 practice.
 
 Setup
@@ -90,15 +90,15 @@
 `high`. These are *clamping bounds*, and they indicate the possible range of the
 input data. Here, clamping bounds of `low=0` and `high=120` indicate that the
 individual values for column `age` will be in the interval `[0, 120]`.
 
 When you know that there is a reasonable minimum and maximum for each value of a
 column, you can use those as clamping bounds. This is what we did here: without
 looking at the dataset, we made the assumption that all members of our library
-were younger than 120 years old, and that ages have to be a nonnegative value.
+were younger than 120 years old, and that ages have to be a non-negative value.
 
 Sometimes, the situation is not so clear. To understand what to do in more
 complex cases, let's first explain what these clamping bounds actually *do*.
 
 What do clamping bounds actually do?
 ------------------------------------
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/first-steps.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _First steps:
 
-Tutorial 1: First steps with Tumult Analytics
-=============================================
+First steps with Tumult Analytics
+=================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In this first tutorial, we will demonstrate how to load data, run a simple
 aggregation query, and get our first differentially private results. You can run
 this tutorial (as well as the next ones) as you go: simply follow the
 :ref:`installation instructions <Installation instructions>`, and use the copy/paste button of each code
 block to reproduce it.
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/groupby-queries.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Group-by queries:
 
-Tutorial 4: Group-by queries
-============================
+Group-by queries
+================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In all previous tutorials, all aggregations we saw were global aggregations,
 returning a single statistic for all the data. But many common data analysis
 operations are *group-by queries*: they partition the data into groups, and
 compute one aggregation per group. In this tutorial, we will demonstrate how to
 express such queries using Tumult Analytics.
 
@@ -376,15 +376,15 @@
 
 Once we have our KeySet, we can use it in the desired aggregation…
 
 .. testcode::
 
     teen_edu_query = (
         QueryBuilder("members")
-        .groupby(teen_edu_keys)
+        .groupby(teen_edu_subset_keys)
         .count()
     )
     teen_edu_counts = session.evaluate(
         teen_edu_query,
         PureDPBudget(0.2),
     )
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/more-with-privacy-ids.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/more-with-privacy-ids.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Advanced IDs features:
 
-Tutorial 7: Doing more with privacy IDs
-=======================================
+Doing more with privacy IDs
+===========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In the previous tutorial, we covered the basics of privacy IDs: how to
 initialize a :class:`Session<tmlt.analytics.session.Session>` where each person appears in multiple rows, and run simple queries.
 But privacy IDs also make it easier to run more complex queries, especially those involving multiple
 tables. In this tutorial, we will build a
 :class:`Session<tmlt.analytics.session.Session>` that protects library patrons across multiple
 tables, and highlight the differences that arise when performing queries on tables with
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-budget-basics.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .. _Working with privacy budgets:
 
-Tutorial 2: Working with privacy budgets
-========================================
+Working with privacy budgets
+============================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 
-In our :ref:`first tutorial<First steps>`, we saw how to run a simple aggregation
+In our :ref:`first steps tutorial<First steps>`, we saw how to run a simple aggregation
 query on private data. When loading the private data into a Session, we had to
 specify a *privacy budget*. This raises two kinds of questions.
 
 1. What is a privacy budget, what formal guarantee does it provide, and how can
    we choose the value of this parameter?
 2. How do we work with privacy budgets using Tumult Analytics, and what is the
    privacy promise of the interface?
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/privacy-id-basics.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/privacy-id-basics.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Working with privacy IDs:
 
-Tutorial 6: Working with privacy IDs
-====================================
+Working with privacy IDs
+========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 In previous tutorials, we were working with a table where each person in the
 data was associated with exactly one row. But this is not always the case: in
 some datasets, the same person can appears in many rows. In this case, it is
 common to associate each person with an *identifier*. Then, the
 goal becomes to hide whether *all rows that share a given identifier* are present
 in the data.
```

### Comparing `tmlt_analytics-0.8.3/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.9.0rc5/doc/tutorials/simple-transformations.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Simple transformations:
 
-Tutorial 5: Simple transformations
-==================================
+Simple transformations
+======================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2023
+    Copyright Tumult Labs 2024
 
 So far we have learned how to perform aggregations on our data, but sometimes we need
 to transform our data before they are ready to be aggregated. In this tutorial, we'll
 demonstrate a few ways that we can transform our data using filters, maps, flat maps,
 binning, and public joins.
 
 Setup
@@ -52,15 +52,15 @@
        protected_change=AddOneRow(),
    )
 
 Revisiting the filter transformation
 ------------------------------------
 
 You might recall that we already used a transformation in
-:ref:`tutorial 2 <Working with privacy budgets>`! Let's run that query again.
+:ref:`working with privacy budgets tutorial<Working with privacy budgets>`! Let's run that query again.
 
 .. testcode::
 
    minor_query = QueryBuilder("members").filter("age < 18").count()
    minor_count = session.evaluate(
        minor_query,
        privacy_budget=PureDPBudget(epsilon=1),
@@ -235,15 +235,15 @@
     [{'genre': 'Romance'}, {'genre': 'Classics/Literature'}, {'genre': 'Current affairs'}]
 
 Like ``map``, ``flat_map`` has the ``new_column_types`` and ``augment`` options.
 In this example, we leave ``augment`` with its default value of ``False``.
 
 Unlike ``map``, ``flat_map`` has an argument ``max_rows``. It clamps the maximum number
 of new rows that can be created for each input row. This serves a similar function as
-the clamping bounds on aggregations we used in :ref:`tutorial 3 <Clamping bounds>`, and
+the clamping bounds on aggregations we used in :ref:`clamping bounds tutorial<Clamping bounds>`, and
 also has the analogous trade-offs: higher values for ``max_rows`` will result in more
 noise in the final results, while lower values may cause more rows to be silently
 dropped. In this case, the choice is easy: no members have more than three favorites and
 there are many members with three, so we set ``max_rows=3``.
 
 .. testcode::
```

### Comparing `tmlt_analytics-0.8.3/pyproject.toml` & `tmlt_analytics-0.9.0rc5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
+
 name = "tmlt.analytics"
+license = "Apache-2.0"
+
 description = "Tumult's differential privacy analytics API"
 readme = "README.md"
 authors = []
-license = "Apache-2.0"
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
+
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.8.3"
+version = "0.9.0-rc.5"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
@@ -23,29 +26,29 @@
 ]
 include = [
   { path = "doc/", format = "sdist" },
   { path = "examples/", format = "sdist" },
   { path = "test/", format = "sdist" },
   { path = "CHANGELOG.md", format = "sdist" },
   { path = "test_requirements.txt", format = "sdist" },
-  { path = "LICENSE", format = "sdist" },
   { path = "NOTICE", format = "sdist" },
+  { path = "LICENSE", format = "sdist" },
 ]
 packages = [
   { include = "tmlt" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.1, <3.12.0"
 
 # When updating Core, PySpark, Pandas or SymPy, remember to update
 # test_multi_deps in the Noxfile.
 
-"tmlt.core" = ">=0.11.5,<0.13.0"
+"tmlt.core" = "^0.12.0"
 
 pandas = [
   { version = ">=1.2.0,<1.4.0", python = "<3.8" },
   { version = ">=1.2.0,<2.0.0", python = ">=3.8,<3.10" },
   { version = ">=1.4.0,<2.0.0", python = ">=3.10,<3.11" },
   { version = ">=1.5.0,<2.0.0", python = ">=3.11" },
 ]
@@ -54,16 +57,15 @@
   { version = "^3.0.0,<3.6.0", extras = ["sql"], python = ">=3.8,<3.11" },
   { version = "^3.4.0,<3.6.0", extras = ["sql"], python = ">=3.11" },
 ]
 sympy = "^1.8,<1.10"
 typeguard = "^2.12.1,<2.13.0"
 typing-extensions = "^4.1.0"
 
-[tool.poetry.dev-dependencies]
-
+[tool.poetry.group.fix-lock.dependencies]
 # This is a hack to convince Poetry to allow different versions of various
 # transitive dependencies on different Python versions, as there is not a single
 # version of these dependencies that works across our entire supported Python
 # version range. Just having `version = "*"` does not work, as Poetry merges
 # such constraints, but having an extra irrelevant version constraint prevents
 # that behavior.
 numpy = [
@@ -77,27 +79,27 @@
   { version = "*,!=0.0.1", python = "<3.8" },
   { version = "*,!=0.0.2", python = ">=3.8,<3.9" },
   { version = "*,!=0.0.3", python = ">=3.9,<3.10" },
   { version = "*,!=0.0.4", python = ">=3.10,<3.11" },
   { version = "*,!=0.0.5", python = ">=3.11" },
 ]
 
-# Build scripting
-nox = "2022.8.7"
-nox_poetry = "1.0.1"
+[tool.poetry.group.dev.dependencies]
 
 # Linters, formatters
 black = "^23.3"
 isort = { version = "^5.11", extras = ["pyproject"] }
 mypy = "^1.2, !=1.4.0" # 1.4.0 incompatible with typing extensions 3.10.0 https://github.com/python/mypy/issues/15487
 pydocstyle = { version = "^6.3", extras = ["toml"] }
 pylint = "^2.13"
 
 # CI, testing, docs
 pytest = "^7.1.2"
+pytest-xdist = "^3.5.0"
+pytest-cov = "^4.1.0"
 coverage = "^6.5"
 pydata-sphinx-theme = "0.9.0"
 scanpydoc = "0.7.3" # 0.7.4 doesn't work
 sphinx = "^4.3.0"
 sphinx-autoapi = "^1.7.0"
 sphinx-autodoc-typehints = "1.12.0" # 1.13.0 doesn't work https://gitlab.com/tumult-labs/tumult/-/issues/1565
 sphinx-copybutton = "^0.4.0"
@@ -113,23 +115,33 @@
 seaborn = "^0.11.1"
 
 # dunamai 1.19.0 introduces a breaking change that some of our dev dependencies don't seem
 # to handle yet. If we ever update them (scanpydoc is a particular problem I think), try
 # removing this pin.
 dunamai = "<1.19.0"
 
+[tool.poetry.group.scripting.dependencies]
+nox = "2022.8.7"
+nox_poetry = "1.0.1"
+
+[tool.poetry.group.ci-tools.dependencies]
+requests = "^2.31.0"
+
 
 [build-system]
+requires = ["poetry-core>=1.3.2", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
-requires = ["poetry-core>=1.3.2", "poetry-dynamic-versioning"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-(?P<stage>[a-zA-Z]+)\\.(?P<revision>\\d+))?"
+fix-shallow-repository = true
+[tool.poetry-dynamic-versioning.substitution]
+files = ["tmlt/analytics/__init__.py"]
 
 [tool.black]
 force-exclude = "noxfile.py"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `tmlt_analytics-0.8.3/test/conftest.py` & `tmlt_analytics-0.9.0rc5/test/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """Creates a Spark Context to use for each testing session."""
 
-
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # TODO(#2206): Import these fixtures from core once it is rewritten
 
 import logging
-from typing import Any, Optional, Sequence
+from typing import Any, Dict, List, Optional, Sequence, TypeVar, Union, cast, overload
 from unittest.mock import Mock, create_autospec
 
 import numpy as np
 import pandas as pd
 import pytest
-from pyspark.sql import SparkSession
+from pyspark.sql import DataFrame, SparkSession
 from tmlt.core.domains.base import Domain
+from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
+from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measures import Measure, PureDP
 from tmlt.core.metrics import AbsoluteDifference, Metric
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber
 
+from tmlt.analytics.privacy_budget import (
+    ApproxDPBudget,
+    PrivacyBudget,
+    PureDPBudget,
+    RhoZCDPBudget,
+)
+
 
 def quiet_py4j():
     """Remove noise in the logs irrelevant to testing."""
     print("Calling PySparkTest:suppress_py4j_logging")
     logger = logging.getLogger("py4j")
     # This is to silence py4j.java_gateway: DEBUG logs.
     logger.setLevel(logging.ERROR)
@@ -42,19 +50,30 @@
     spark = (
         SparkSession.builder.appName(__name__)
         .master("local[4]")
         .config("spark.sql.warehouse.dir", "/tmp/hive_tables")
         .config("spark.hadoop.fs.defaultFS", "file:///")
         .config("spark.eventLog.enabled", "false")
         .config("spark.driver.allowMultipleContexts", "true")
-        .config("spark.ui.showConsoleProgress", "false")
         .config("spark.sql.execution.arrow.pyspark.enabled", "true")
         .config("spark.default.parallelism", "5")
         .config("spark.memory.offHeap.enabled", "true")
         .config("spark.memory.offHeap.size", "16g")
+        .config("spark.port.maxRetries", "30")
+        .config("spark.sql.shuffle.partitions", "1")
+        # Disable Spark UI / Console display
+        .config("spark.ui.showConsoleProgress", "false")
+        .config("spark.ui.enabled", "false")
+        .config("spark.ui.dagGraph.retainedRootRDDs", "1")
+        .config("spark.ui.retainedJobs", "1")
+        .config("spark.ui.retainedStages", "1")
+        .config("spark.ui.retainedTasks", "1")
+        .config("spark.sql.ui.retainedExecutions", "1")
+        .config("spark.worker.ui.retainedExecutors", "1")
+        .config("spark.worker.ui.retainedDrivers", "1")
         .getOrCreate()
     )
     # This is to silence pyspark logs.
     spark.sparkContext.setLogLevel("OFF")
     return spark
 
 
@@ -73,15 +92,15 @@
         first_df: First dataframe to compare.
         second_df: Second dataframe to compare.
         sort_columns: Names of column to sort on. By default sorts by all columns.
         **kwargs: Keyword arguments that will be passed to assert_frame_equal().
     """
     if sorted(first_df.columns) != sorted(second_df.columns):
         raise ValueError(
-            "Dataframes must have matching columns. "
+            "DataFrames must have matching columns. "
             f"first_df: {sorted(first_df.columns)}. "
             f"second_df: {sorted(second_df.columns)}."
         )
     if first_df.empty and second_df.empty:
         return
     if sort_columns is None:
         sort_columns = list(first_df.columns)
@@ -184,7 +203,97 @@
     """
     argnames = sorted({k for v in d.values() for k in v.keys()})
     return pytest.mark.parametrize(
         argnames=argnames,
         argvalues=[[v.get(k) for k in argnames] for v in d.values()],
         ids=d.keys(),
     )
+
+
+T = TypeVar("T", bound=PrivacyBudget)
+
+
+def assert_approx_equal_budgets(
+    budget1: T, budget2: T, atol: float = 1e-8, rtol: float = 1e-5
+):
+    """Asserts that two budgets are approximately equal.
+
+    Args:
+        budget1: The first budget.
+        budget2: The second budget.
+        atol: The absolute tolerance for the comparison.
+        rtol: The relative tolerance for the comparison.
+    """
+    if not isinstance(budget1, type(budget2)) or not isinstance(budget2, type(budget1)):
+        raise AssertionError(
+            f"Budgets are not of the same type: {type(budget1)} and {type(budget2)}"
+        )
+    if isinstance(budget1, PureDPBudget) and isinstance(budget2, PureDPBudget):
+        if not np.allclose(budget1.epsilon, budget2.epsilon, atol=atol, rtol=rtol):
+            raise AssertionError(
+                f"Epsilon values are not approximately equal: {budget1} and {budget2}"
+            )
+        return
+    if isinstance(budget1, ApproxDPBudget) and isinstance(budget2, ApproxDPBudget):
+        if not np.allclose(budget1.epsilon, budget2.epsilon, atol=atol, rtol=rtol):
+            raise AssertionError(
+                "Epsilon values are not approximately equal: "
+                f"{budget1.epsilon} and {budget2.epsilon}"
+            )
+        if not np.allclose(budget1.delta, budget2.delta, atol=atol, rtol=rtol):
+            raise AssertionError(
+                "Delta values are not approximately equal: "
+                f"{budget1.delta} and {budget2.delta}"
+            )
+        return
+    if isinstance(budget1, RhoZCDPBudget) and isinstance(budget2, RhoZCDPBudget):
+        if not np.allclose(budget1.rho, budget2.rho, atol=atol, rtol=rtol):
+            raise AssertionError(
+                f"Rho values are not approximately equal: "
+                f"{budget1.rho} and {budget2.rho}"
+            )
+        return
+    raise AssertionError(f"Budget type not recognized: {type(budget1)}")
+
+
+@overload
+def create_empty_input(domain: DictDomain) -> Dict:
+    ...
+
+
+@overload
+def create_empty_input(domain: SparkDataFrameDomain) -> DataFrame:
+    ...
+
+
+def create_empty_input(domain):  # pylint: disable=missing-type-doc
+    """Returns an empty input for a given domain.
+
+    Args:
+        domain: The domain for which to create an empty input.
+    """
+    spark = SparkSession.builder.getOrCreate()
+    if isinstance(domain, DictDomain):
+        return {
+            k: create_empty_input(cast(Union[DictDomain, SparkDataFrameDomain], v))
+            for k, v in domain.key_to_domain.items()
+        }
+    if isinstance(domain, SparkDataFrameDomain):
+        # TODO(#3092): the row is only necessary b/c of a bug in core for empty dfs
+        row: List[Any] = []
+        for field in domain.spark_schema.fields:
+            if field.dataType.simpleString() == "string":
+                row.append("")
+            elif field.dataType.simpleString() == "integer":
+                row.append(0)
+            elif field.dataType.simpleString() == "double":
+                row.append(0.0)
+            elif field.dataType.simpleString() == "boolean":
+                row.append(False)
+            elif field.dataType.simpleString() == "bigint":
+                row.append(0)
+            else:
+                raise ValueError(
+                    f"Unsupported field type: {field.dataType.simpleString()}"
+                )
+        return spark.createDataFrame([row], domain.spark_schema)
+    raise ValueError(f"Unsupported domain type: {type(domain)}")
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/ids/test_constraint_propagation.py` & `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_constraint_propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Integration tests for constraint propagation."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from typing import Dict, List
 
 import pandas as pd
 import pytest
 
 from tmlt.analytics._table_identifier import NamedTable
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/ids/test_count_distinct_optimization.py` & `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_count_distinct_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Tests for constraint inference and optimization on count-distinct queries."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from typing import List
 
 import pandas as pd
 import pytest
 
 from tmlt.analytics.constraints import MaxGroupsPerID, MaxRowsPerID
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/ids/test_id_col_operations.py` & `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_id_col_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Integration tests for operations directly on ID columns."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pytest
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.metrics import AddRemoveKeys
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/ids/test_l0_linf_truncation.py` & `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l0_linf_truncation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Integration tests for aggregations using L0 + L-inf truncation."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import statistics
 from typing import List, Optional, Set, Tuple
 
 import pytest
 
 from tmlt.analytics.constraints import (
@@ -15,15 +15,16 @@
     MaxRowsPerID,
 )
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
 
-from ..conftest import INF_BUDGET, INF_BUDGET_ZCDP, closest_value
+from ...conftest import closest_value
+from ..conftest import INF_BUDGET, INF_BUDGET_ZCDP
 
 _TRUNCATED_N = {
     1: [{4, 7, 8}, {4, 7, 9}, {5, 7, 8}, {5, 7, 9}, {6, 7, 8}, {6, 7, 9}],
     2: [{4, 5, 7, 8, 9}, {4, 6, 7, 8, 9}, {5, 6, 7, 8, 9}],
     3: [{4, 5, 6, 7, 8, 9}],
 }
 """Possible sets of values of n at different truncation thresholds."""
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/ids/test_l1_truncation.py` & `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_l1_truncation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Integration tests for aggregations using L1 truncation."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import statistics
 from typing import List, Set, Tuple
 
 import pytest
 
 from tmlt.analytics.constraints import MaxRowsPerID
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
 
-from ..conftest import INF_BUDGET, INF_BUDGET_ZCDP, closest_value
+from ...conftest import closest_value
+from ..conftest import INF_BUDGET, INF_BUDGET_ZCDP
 
 _BASE_QUERIES = [QueryBuilder("id_a1").enforce(MaxRowsPerID(n)) for n in range(1, 4)]
 _BASE_QUERY_NS_GROUPED: List[Set[Tuple[Tuple[int, ...], Tuple[int, ...]]]] = [
     {
         ((4, 7, 8), ()),
         ((5, 7, 8), ()),
         ((6, 7, 8), ()),
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/ids/test_partition.py` & `tmlt_analytics-0.9.0rc5/test/system/session/ids/test_partition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Integration tests for partition_and_create for IDs tables."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 
 import pandas as pd
 import pytest
 import sympy as sp
 from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
 from tmlt.core.metrics import DictMetric
@@ -25,30 +25,30 @@
 
 @pytest.mark.parametrize("session", [INF_BUDGET], indirect=True, ids=["puredp"])
 def test_invalid_constraint_partition_and_create(session):
     """Tests that :func:`partition_and_create` with invalid constraint errors."""
     with pytest.raises(
         ValueError,
         match=(
-            "You must create MaxGroupsPerID constraint before using "
+            "You must create a MaxGroupsPerID constraint before using "
             "partition_and_create on tables with the AddRowsWithID protected change."
         ),
     ):
         session.create_view(QueryBuilder("id_a1"), "truncated_ids", cache=True)
         session.partition_and_create(
             source_id="truncated_ids",
             privacy_budget=PureDPBudget(10),
             column="group",
             splits={"part0": "0", "part1": "1"},
         )
 
     with pytest.raises(
         ValueError,
         match=(
-            "You must create MaxGroupsPerID constraint before using "
+            "You must create a MaxGroupsPerID constraint before using "
             "partition_and_create on tables with the AddRowsWithID protected change."
         ),
     ):
         session.create_view(
             QueryBuilder("id_a1").enforce(MaxRowsPerID(5)), "truncated_ids2", cache=True
         )
         session.partition_and_create(
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/mixed/test_mixed_session.py` & `tmlt_analytics-0.9.0rc5/test/system/session/mixed/test_mixed_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for Sessions that employ a mixture of IDs and non-IDs features.
 
 These are not meant to be exhaustive, but rather to ensure that the Session
 functions properly when used with a mixture of IDs and non-IDs protected changes."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 
 import pytest
 
 from tmlt.analytics._table_identifier import NamedTable
 from tmlt.analytics.constraints import (
     MaxGroupsPerID,
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/rows/conftest.py` & `tmlt_analytics-0.9.0rc5/test/system/session/rows/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Common fixtures for non-IDs Session tests."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Any, List
 
 import pandas as pd
 import pytest
 from pyspark.sql import SparkSession
@@ -38,15 +38,15 @@
     SumMechanism,
 )
 
 # Shorthands for some values used in tests
 _DATE1 = datetime.date.fromisoformat("2022-01-01")
 _DATE2 = datetime.date.fromisoformat("2022-01-02")
 
-# Dataframes for public data,
+# DataFrames for public data,
 # placed here so that test case KeySets can use them
 GROUPBY_TWO_COLUMNS = pd.DataFrame([["0", 0], ["0", 1], ["1", 1]], columns=["A", "B"])
 GET_GROUPBY_TWO_COLUMNS = lambda: SparkSession.builder.getOrCreate().createDataFrame(
     GROUPBY_TWO_COLUMNS
 )
 GROUPBY_ONE_COLUMN = pd.DataFrame([["0"], ["1"], ["2"]], columns=["A"])
 GET_GROUPBY_ONE_COLUMN = lambda: SparkSession.builder.getOrCreate().createDataFrame(
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/rows/test_add_max_rows.py` & `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Tests for Session with the AddMaxRows ProtectedChange."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=no-self-use
 
-import math
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
 from tmlt.core.measurements.interactive_measurements import PrivacyAccountantState
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
@@ -22,15 +21,15 @@
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
     PrivacyBudget,
     PureDPBudget,
     RhoZCDPBudget,
 )
-from tmlt.analytics.protected_change import AddOneRow
+from tmlt.analytics.protected_change import AddMaxRowsInMaxGroups, AddOneRow
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountMechanism,
     FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
@@ -356,18 +355,23 @@
             dataframe=self.sdf,
             protected_change=AddOneRow(),
         )
         query = QueryBuilder("private").get_groups(columns)
         with pytest.raises(ValueError, match="Nonexistent columns in get_groups query"):
             session.evaluate(query, session.remaining_privacy_budget)
 
-    def test_get_groups_errors(self):
-        """Test that the GetGroups query errors with PureDP."""
+    @pytest.mark.parametrize(
+        "session_budget", [(PureDPBudget(float("inf"))), (RhoZCDPBudget(float("inf")))]
+    )
+    def test_get_groups_errors(
+        self, session_budget: Union[PureDPBudget, ApproxDPBudget]
+    ):
+        """Test that the GetGroups query errors with non ApproxDPBudgets."""
         session = Session.from_dataframe(
-            privacy_budget=PureDPBudget(1),
+            privacy_budget=session_budget,
             source_id="private",
             dataframe=self.sdf,
             protected_change=AddOneRow(),
         )
         query = QueryBuilder("private").get_groups([])
         with pytest.raises(
             ValueError, match="GetGroups is only supported with ApproxDPBudgets."
@@ -455,14 +459,15 @@
                 PureDPBudget(10000),
                 pd.DataFrame({"sum": [12]}),
             ),
             (  # GAUSSIAN noise since RhoZCDP
                 RhoZCDPBudget(10000),
                 pd.DataFrame({"sum": [12]}),
             ),
+            (ApproxDPBudget(10000, 1 / 2), pd.DataFrame({"sum": [12]})),
         ],
     )
     def test_create_view_with_stability(
         self, privacy_budget: PrivacyBudget, expected: pd.DataFrame
     ):
         """Smoke test for querying on views with stability changes"""
         session = Session.from_dataframe(
@@ -857,15 +862,18 @@
 
     @pytest.mark.parametrize(
         "budget", [(PureDPBudget(20)), (ApproxDPBudget(20, 0.5)), (RhoZCDPBudget(20))]
     )
     def test_partition_on_flatmap_grouping_column(self, budget: PrivacyBudget):
         """Tests that you can partition on columns created by grouping flat maps."""
         session = Session.from_dataframe(
-            privacy_budget=budget, source_id="private", dataframe=self.sdf
+            privacy_budget=budget,
+            source_id="private",
+            dataframe=self.sdf,
+            protected_change=AddOneRow(),
         )
         grouping_flat_map = QueryBuilder("private").flat_map(
             f=lambda row: [{"new": 1}, {"new": 2}],
             new_column_types={"new": ColumnType.INTEGER},
             augment=True,
             grouping=True,
             max_rows=2,
@@ -1132,11 +1140,12 @@
         ks = KeySet.from_dict({"group": [0, 1]})
         query = QueryBuilder("id").groupby(ks).count()
 
         session = Session.from_dataframe(
             RhoZCDPBudget(float("inf")),
             "id",
             grouped_df,
-            stability=math.sqrt(2),
-            grouping_column="group",
+            protected_change=AddMaxRowsInMaxGroups(
+                grouping_column="group", max_groups=2, max_rows_per_group=1
+            ),
         )
         session.evaluate(query, RhoZCDPBudget(1))
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/rows/test_add_max_rows_in_max_groups.py` & `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_in_max_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Note that these tests are not intended to be exhaustive. They are intended to be a
 sanity check that the Session is working correctly with AddMaxRowsInMaxGroups. More
 thorough tests for Session are in
 test/system/session/rows/test_add_max_rows.py."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=no-self-use
 
 from typing import Any, Dict, List
 
 import pandas as pd
 import pytest
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/rows/test_add_max_rows_infs_nulls.py` & `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_add_max_rows_infs_nulls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """System tests for Sessions with Nulls and Infs."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Any, Dict, List, Mapping, Tuple, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame, SparkSession
@@ -273,16 +273,18 @@
 
         The query used to evaluate this is a GroupByCount on the joined dataframe,
         using the keyset provided.
         """
         session = (
             Session.Builder()
             .with_privacy_budget(PureDPBudget(float("inf")))
-            .with_private_dataframe("private", self.sdf)
-            .with_private_dataframe("private2", spark.createDataFrame(private_df))
+            .with_private_dataframe("private", self.sdf, AddOneRow())
+            .with_private_dataframe(
+                "private2", spark.createDataFrame(private_df), AddOneRow()
+            )
             .build()
         )
         result = session.evaluate(
             QueryBuilder("private")
             .join_private(
                 QueryBuilder("private2"),
                 TruncationStrategy.DropExcess(100),
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/rows/test_invalid.py` & `tmlt_analytics-0.9.0rc5/test/system/session/rows/test_invalid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for invalid session configurations."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable= no-self-use
 
 from typing import Dict, Tuple, Type, Union
 from unittest.mock import Mock
 
 import pytest
@@ -81,49 +81,41 @@
         session.create_view(PrivateSource("private"), "view", cache=False)
         with pytest.raises(error_type, match=expected_error_msg):
             session.evaluate(query_expr, privacy_budget=PureDPBudget(float("inf")))
 
     @pytest.mark.parametrize(
         "requested,remaining,budget_type,expected_msg",
         [
-            # TOD0(2476): Uncomment once we support Delta consumption
-            # Also remove the first uncommented test. That msg will be incorrect
-            # (
-            #     (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
-            #     (ExactNumber(2), ExactNumber.from_float(0.4, round_up=True)),
-            #     ApproxDPBudget(2, 0.4),
-            #   "\nRequested: ε=3.000, δ=0.500\nRemaining:"
-            #     " ε=2.000, δ=0.400\nDifference: ε=1.000, δ=0.1000",
-            # ),
-            # (
-            #     (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
-            #     (ExactNumber(2), ExactNumber.from_float(0.5, round_up=True)),
-            #     ApproxDPBudget(2, 0.5),
-            #   "\nRequested: ε=3.000, δ=0.500\nRemaining:"
-            #     " ε=2.000, δ=0.500\nDifference: ε=1.000",
-            # ),
-            # (
-            #     (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
-            #     (ExactNumber(3), ExactNumber.from_float(0.4, round_up=True)),
-            #     ApproxDPBudget(3, 0.4),
-            #   "\nRequested: ε=3.000, δ=0.500\nRemaining:"
-            #     " ε=3.000, δ=0.400\nDifference: δ=0.100",
-            # ),
-            # (
-            #     (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
-            #     (ExactNumber(3), ExactNumber.from_float(0.41, round_up=True)),
-            #     ApproxDPBudget(3, 0.41),
-            #   "\nRequested: ε=3.000, δ=0.500\nRemaining:"
-            #     " ε=3.000, δ=0.400\nDifference: δ=9.000e-02",
-            # ),
             (
                 (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
                 (ExactNumber(2), ExactNumber.from_float(0.4, round_up=True)),
                 ApproxDPBudget(2, 0.4),
-                "\nRequested: ε=3.000\nRemaining: ε=2.000\nDifference: ε=1.000",
+                "\nRequested: ε=3.000, δ=0.500\nRemaining:"
+                " ε=2.000, δ=0.400\nDifference: ε=1.000, δ=0.100",
+            ),
+            (
+                (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
+                (ExactNumber(2), ExactNumber.from_float(0.5, round_up=True)),
+                ApproxDPBudget(2, 0.5),
+                "\nRequested: ε=3.000, δ=0.500\nRemaining:"
+                " ε=2.000, δ=0.500\nDifference: ε=1.000",
+            ),
+            (
+                (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
+                (ExactNumber(3), ExactNumber.from_float(0.4, round_up=True)),
+                ApproxDPBudget(3, 0.4),
+                "\nRequested: ε=3.000, δ=0.500\nRemaining:"
+                " ε=3.000, δ=0.400\nDifference: δ=0.100",
+            ),
+            (
+                (ExactNumber(3), ExactNumber.from_float(0.5, round_up=True)),
+                (ExactNumber(3), ExactNumber.from_float(0.41, round_up=True)),
+                ApproxDPBudget(3, 0.41),
+                "\nRequested: ε=3.000, δ=0.500\nRemaining:"
+                " ε=3.000, δ=0.410\nDifference: δ=9.000e-02",
             ),
             (
                 ExactNumber(3),
                 ExactNumber(2),
                 PureDPBudget(2),
                 "\nRequested: ε=3.000\nRemaining: ε=2.000\nDifference: ε=1.000",
             ),
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/test_budgets.py` & `tmlt_analytics-0.9.0rc5/test/system/session/test_budgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for passing different types of budgets and querying with them."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import sys
 
 import pytest
 
 from tmlt.analytics.constraints import MaxRowsPerID
 from tmlt.analytics.privacy_budget import (
```

### Comparing `tmlt_analytics-0.8.3/test/system/session/test_invalid_constraints.py` & `tmlt_analytics-0.9.0rc5/test/system/session/test_invalid_constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Tests for invalid constraint enforcement."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 import pytest
 
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
```

### Comparing `tmlt_analytics-0.8.3/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 """Tests for MeasurementVisitor."""
-
-# SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
-
-# pylint: disable=no-self-use
-
+from test.conftest import create_empty_input
 from typing import List, Optional, Union
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
-import sympy as sp
-from pyspark.sql import DataFrame
 from pyspark.sql.types import LongType, StringType, StructField, StructType
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkColumnDescriptor,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
-    SparkGroupedDataFrameDomain,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.measurements.aggregations import NoiseMechanism
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.chaining import ChainTM
 from tmlt.core.measures import PureDP, RhoZCDP
 from tmlt.core.metrics import (
     DictMetric,
     HammingDistance,
     IfGroupedBy,
-    RootSumOfSquared,
-    SumOf,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.spark_transformations.groupby import GroupBy
-from tmlt.core.transformations.spark_transformations.select import (
-    Select as SelectTransformation,
-)
 from tmlt.core.utils.exact_number import ExactNumber
 from tmlt.core.utils.type_utils import assert_never
 
 from tmlt.analytics._catalog import Catalog
-from tmlt.analytics._query_expr_compiler._measurement_visitor import (
-    MeasurementVisitor,
+from tmlt.analytics._noise_info import NoiseInfo, _NoiseMechanism
+from tmlt.analytics._query_expr_compiler._base_measurement_visitor import (
     _get_query_bounds,
 )
-from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
+from tmlt.analytics._query_expr_compiler._measurement_visitor import MeasurementVisitor
+from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
+    OutputSchemaVisitor,
+)
+from tmlt.analytics._schema import (
+    ColumnDescriptor,
+    ColumnType,
+    Schema,
+    spark_schema_to_analytics_columns,
+)
 from tmlt.analytics._table_identifier import NamedTable
-from tmlt.analytics._table_reference import lookup_domain, lookup_metric
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
 )
@@ -79,15 +73,16 @@
 )
 from tmlt.analytics.query_expr import ReplaceInfinity as ReplaceInfExpr
 from tmlt.analytics.query_expr import ReplaceNullAndNan
 from tmlt.analytics.query_expr import Select as SelectExpr
 from tmlt.analytics.query_expr import StdevMechanism, SumMechanism, VarianceMechanism
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
-from ...conftest import assert_frame_equal_with_sort
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 
 def chain_to_list(t: ChainTT) -> List[Transformation]:
     """Turns a ChainTT's tree into a list."""
     left: List[Transformation]
     if not isinstance(t.transformation1, ChainTT):
         left = [t.transformation1]
@@ -314,14 +309,41 @@
     """Tests for Measurement Visitor."""
 
     visitor: MeasurementVisitor
     pick_noise_visitor: MeasurementVisitor
     catalog: Catalog
     base_query: QueryExpr
 
+    def run_with_empty_data_and_check_schema(
+        self, query: QueryExpr, output_measure: Union[PureDP, RhoZCDP]
+    ):
+        """Run a query and check the schema of the result."""
+        expected_column_types = query.accept(
+            OutputSchemaVisitor(self.catalog)
+        ).column_types
+        self.visitor.output_measure = output_measure
+        measurement, _ = query.accept(self.visitor)
+        empty_data = create_empty_input(measurement.input_domain)
+        result = measurement(empty_data)
+        actual_column_types = Schema(
+            spark_schema_to_analytics_columns(result.schema)
+        ).column_types
+        assert actual_column_types == expected_column_types
+
+    def check_noise_info(
+        self,
+        query: QueryExpr,
+        output_measure: Union[PureDP, RhoZCDP],
+        expected_noise_info: NoiseInfo,
+    ):
+        """Check the noise info for a query."""
+        self.pick_noise_visitor.output_measure = output_measure
+        _, noise_info = query.accept(self.pick_noise_visitor)
+        assert noise_info == expected_noise_info
+
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,expected_mechanism",
         [
             (CountMechanism.DEFAULT, PureDP(), NoiseMechanism.GEOMETRIC),
             (CountMechanism.DEFAULT, RhoZCDP(), NoiseMechanism.DISCRETE_GAUSSIAN),
             (CountMechanism.LAPLACE, PureDP(), NoiseMechanism.GEOMETRIC),
             (CountMechanism.LAPLACE, RhoZCDP(), NoiseMechanism.GEOMETRIC),
@@ -460,40 +482,42 @@
         query_mechanism: AverageMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
         # if expected_mechanism is None, this combination is not supported
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedAverage query exprs."""
+        if isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+            measure_column = "B"
+        elif isinstance(measure_column_type, SparkFloatColumnDescriptor):
+            measure_column = "X"
+        else:
+            raise AssertionError("Unknown measure column type")
         query = GroupByBoundedAverage(
             child=self.base_query,
-            measure_column="",
+            measure_column=measure_column,
             low=0,
             high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
-            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
-                query, measure_column_type
-            )
+            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(query)
             assert got_mechanism == expected_mechanism
         else:
             with pytest.raises(
                 ValueError,
                 match=(
                     "Gaussian noise is not supported under PureDP. "
                     "Please use RhoZCDP or another measure."
                 ),
             ):
-                self.pick_noise_visitor._pick_noise_for_non_count(
-                    query, measure_column_type
-                )
+                self.pick_noise_visitor._pick_noise_for_non_count(query)
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,measure_column_type,expected_mechanism",
         [
             (
                 SumMechanism.DEFAULT,
@@ -564,40 +588,42 @@
         query_mechanism: SumMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
         # if expected_mechanism is None, this combination is not supported
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedSum query exprs."""
+        if isinstance(measure_column_type, SparkFloatColumnDescriptor):
+            measure_column = "X"
+        elif isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+            measure_column = "B"
+        else:
+            raise AssertionError("Unknown measure column type")
         query = GroupByBoundedSum(
             child=self.base_query,
-            measure_column="",
+            measure_column=measure_column,
             low=0,
             high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
-            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
-                query, measure_column_type
-            )
+            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(query)
             assert got_mechanism == expected_mechanism
         else:
             with pytest.raises(
                 ValueError,
                 match=(
                     "Gaussian noise is not supported under PureDP. "
                     "Please use RhoZCDP or another measure."
                 ),
             ):
-                self.pick_noise_visitor._pick_noise_for_non_count(
-                    query, measure_column_type
-                )
+                self.pick_noise_visitor._pick_noise_for_non_count(query)
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,measure_column_type,expected_mechanism",
         [
             (
                 VarianceMechanism.DEFAULT,
@@ -673,40 +699,42 @@
         query_mechanism: VarianceMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
         # if expected_mechanism is None, this combination is not supported
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedVariance query exprs."""
+        if isinstance(measure_column_type, SparkFloatColumnDescriptor):
+            measure_column = "X"
+        elif isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+            measure_column = "B"
+        else:
+            raise AssertionError("Unknown measure column type")
         query = GroupByBoundedVariance(
             child=self.base_query,
-            measure_column="",
+            measure_column=measure_column,
             low=0,
             high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
-            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
-                query, measure_column_type
-            )
+            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(query)
             assert got_mechanism == expected_mechanism
         else:
             with pytest.raises(
                 ValueError,
                 match=(
                     "Gaussian noise is not supported under PureDP. "
                     "Please use RhoZCDP or another measure."
                 ),
             ):
-                self.pick_noise_visitor._pick_noise_for_non_count(
-                    query, measure_column_type
-                )
+                self.pick_noise_visitor._pick_noise_for_non_count(query)
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,measure_column_type,expected_mechanism",
         [
             (
                 StdevMechanism.DEFAULT,
@@ -777,40 +805,42 @@
         query_mechanism: StdevMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
         # if expected_mechanism is None, this combination is not supported
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedSTDEV query exprs."""
+        if isinstance(measure_column_type, SparkFloatColumnDescriptor):
+            measure_column = "X"
+        elif isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+            measure_column = "B"
+        else:
+            raise AssertionError("Unknown measure column type")
         query = GroupByBoundedSTDEV(
             child=self.base_query,
-            measure_column="",
+            measure_column=measure_column,
             low=0,
             high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
-            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
-                query, measure_column_type
-            )
+            got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(query)
             assert got_mechanism == expected_mechanism
         else:
             with pytest.raises(
                 ValueError,
                 match=(
                     "Gaussian noise is not supported under PureDP. "
                     "Please use RhoZCDP or another measure."
                 ),
             ):
-                self.pick_noise_visitor._pick_noise_for_non_count(
-                    query, measure_column_type
-                )
+                self.pick_noise_visitor._pick_noise_for_non_count(query)
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "mechanism",
         [
             (AverageMechanism.LAPLACE),
             (StdevMechanism.LAPLACE),
@@ -833,286 +863,56 @@
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
         ]
         if isinstance(mechanism, AverageMechanism):
             query = GroupByBoundedAverage(
                 child=self.base_query,
-                measure_column="",
+                measure_column="A",
                 low=0,
                 high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         elif isinstance(mechanism, StdevMechanism):
             query = GroupByBoundedSTDEV(
                 child=self.base_query,
-                measure_column="",
+                measure_column="A",
                 low=0,
                 high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         elif isinstance(mechanism, SumMechanism):
             query = GroupByBoundedSum(
                 child=self.base_query,
-                measure_column="",
+                measure_column="A",
                 low=0,
                 high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         elif isinstance(mechanism, VarianceMechanism):
             query = GroupByBoundedVariance(
                 child=self.base_query,
-                measure_column="",
+                measure_column="A",
                 low=0,
                 high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         else:
             assert_never(mechanism)
         with pytest.raises(
             AssertionError, match="Query's measure column should be numeric."
         ):
             # pylint: disable=protected-access
-            self.visitor._pick_noise_for_non_count(query, SparkStringColumnDescriptor())
+            self.visitor._pick_noise_for_non_count(query)
             # pylint: enable=protected-access
 
-    @pytest.mark.parametrize(
-        "input_metric,mechanism,expected_output_metric",
-        [
-            (HammingDistance(), NoiseMechanism.LAPLACE, SumOf(SymmetricDifference())),
-            (HammingDistance(), NoiseMechanism.GEOMETRIC, SumOf(SymmetricDifference())),
-            (
-                HammingDistance(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
-                RootSumOfSquared(SymmetricDifference()),
-            ),
-            (
-                HammingDistance(),
-                NoiseMechanism.GAUSSIAN,
-                RootSumOfSquared(SymmetricDifference()),
-            ),
-            (
-                SymmetricDifference(),
-                NoiseMechanism.LAPLACE,
-                SumOf(SymmetricDifference()),
-            ),
-            (
-                SymmetricDifference(),
-                NoiseMechanism.GEOMETRIC,
-                SumOf(SymmetricDifference()),
-            ),
-            (
-                SymmetricDifference(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
-                RootSumOfSquared(SymmetricDifference()),
-            ),
-            (
-                SymmetricDifference(),
-                NoiseMechanism.GAUSSIAN,
-                RootSumOfSquared(SymmetricDifference()),
-            ),
-            (
-                IfGroupedBy(column="A", inner_metric=SumOf(SymmetricDifference())),
-                NoiseMechanism.LAPLACE,
-                SumOf(SymmetricDifference()),
-            ),
-            (
-                IfGroupedBy(column="A", inner_metric=SumOf(SymmetricDifference())),
-                NoiseMechanism.GEOMETRIC,
-                SumOf(SymmetricDifference()),
-            ),
-            (
-                IfGroupedBy(
-                    column="A", inner_metric=RootSumOfSquared(SymmetricDifference())
-                ),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
-                RootSumOfSquared(SymmetricDifference()),
-            ),
-        ],
-    )
-    def test_build_groupby(
-        self,
-        input_metric: Union[HammingDistance, SymmetricDifference, IfGroupedBy],
-        mechanism: NoiseMechanism,
-        expected_output_metric: Union[RootSumOfSquared, SumOf],
-    ) -> None:
-        """Test _build_groupby (without a _public_id)."""
-        input_domain = SparkDataFrameDomain(
-            schema={
-                "A": SparkStringColumnDescriptor(),
-                "B": SparkIntegerColumnDescriptor(),
-            }
-        )
-        keyset = KeySet.from_dict({"A": ["zero", "one"], "B": [0, 1]})
-        # pylint: disable=protected-access
-        got = self.visitor._build_groupby(
-            input_domain=input_domain,
-            input_metric=input_metric,
-            groupby_keys=keyset,
-            mechanism=mechanism,
-        )
-        # pylint: enable=protected-access
-        assert got.input_domain == input_domain
-        assert got.input_metric == input_metric
-        assert_frame_equal_with_sort(
-            got.group_keys.toPandas(), keyset.dataframe().toPandas()
-        )
-        expected_output_domain = SparkGroupedDataFrameDomain(
-            schema=input_domain.schema, groupby_columns=["A", "B"]
-        )
-        assert isinstance(got.output_domain, SparkGroupedDataFrameDomain)
-        assert got.output_domain.schema == expected_output_domain.schema
-        assert (
-            got.output_domain.groupby_columns == expected_output_domain.groupby_columns
-        )
-        assert got.output_metric == expected_output_metric
-
-    @pytest.mark.parametrize(
-        "query,expected_mid_stability,expected_mechanism",
-        [
-            (
-                GroupByBoundedAverage(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="B",
-                    low=-100,
-                    high=100,
-                    mechanism=AverageMechanism.LAPLACE,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.GEOMETRIC,
-            ),
-            (
-                GroupByBoundedAverage(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="nan",
-                    low=-100,
-                    high=100,
-                    mechanism=AverageMechanism.LAPLACE,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.LAPLACE,
-            ),
-            (
-                GroupByBoundedSum(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="X",
-                    low=-100,
-                    high=100,
-                    mechanism=SumMechanism.LAPLACE,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.LAPLACE,
-            ),
-            (
-                GroupByBoundedSum(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="null",
-                    low=-100,
-                    high=100,
-                    mechanism=SumMechanism.LAPLACE,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.LAPLACE,
-            ),
-            (
-                GroupByBoundedVariance(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="B",
-                    low=-100,
-                    high=100,
-                    mechanism=VarianceMechanism.DEFAULT,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.GEOMETRIC,
-            ),
-            (
-                GroupByBoundedVariance(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="inf",
-                    low=-100,
-                    high=100,
-                    mechanism=VarianceMechanism.LAPLACE,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.LAPLACE,
-            ),
-            (
-                GroupByBoundedSTDEV(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="B",
-                    low=-100,
-                    high=100,
-                    mechanism=StdevMechanism.DEFAULT,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.GEOMETRIC,
-            ),
-            (
-                GroupByBoundedSTDEV(
-                    child=PrivateSource("private"),
-                    groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
-                    measure_column="null_and_nan_and_inf",
-                    low=-100,
-                    high=100,
-                    mechanism=StdevMechanism.DEFAULT,
-                ),
-                ExactNumber(3).expr,
-                NoiseMechanism.LAPLACE,
-            ),
-        ],
-    )
-    def test_build_common(
-        self,
-        query: Union[
-            GroupByBoundedAverage,
-            GroupByBoundedSTDEV,
-            GroupByBoundedSum,
-            GroupByBoundedVariance,
-        ],
-        expected_mid_stability: sp.Expr,
-        expected_mechanism: NoiseMechanism,
-    ):
-        """Test _build_common."""
-        info = self.visitor._build_common(query)  # pylint: disable=protected-access
-        transformation: ChainTT
-        assert isinstance(info.transformation, ChainTT)
-        transformation = info.transformation
-
-        assert transformation.input_domain == self.visitor.input_domain
-        assert transformation.input_metric == self.visitor.input_metric
-
-        assert info.mechanism == expected_mechanism
-        assert info.mid_stability == expected_mid_stability
-        assert info.lower_bound == ExactNumber.from_float(query.low, round_up=True)
-        assert info.upper_bound == ExactNumber.from_float(query.high, round_up=False)
-
-        assert isinstance(info.groupby, GroupBy)
-        table_domain = transformation.output_domain
-        assert isinstance(table_domain, SparkDataFrameDomain)
-        expected_groupby_domain = SparkGroupedDataFrameDomain(
-            schema=dict(table_domain.schema), groupby_columns=["A"]
-        )
-        assert isinstance(info.groupby.output_domain, SparkGroupedDataFrameDomain)
-        assert info.groupby.output_domain.schema == expected_groupby_domain.schema
-        assert (
-            info.groupby.output_domain.groupby_columns
-            == expected_groupby_domain.groupby_columns
-        )
-
     def test_validate_measurement(self):
         """Test _validate_measurement."""
         with patch(
             "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
             autospec=True,
         ) as mock_measurement:
             mock_measurement.privacy_function.return_value = self.visitor.budget.value
@@ -1153,892 +953,831 @@
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         assert (
             measurement.transformation.output_metric
             == measurement.measurement.input_metric
         )
 
-    def check_mock_groupby_call(
-        self,
-        mock_groupby,
-        transformation: Transformation,
-        keys: KeySet,
-        expected_mechanism: NoiseMechanism,
-    ) -> None:
-        """Check that the mock groupby was called with the right arguments."""
-        groupby_df: DataFrame = keys.dataframe()
-        mock_groupby.assert_called_with(
-            input_domain=transformation.output_domain,
-            input_metric=transformation.output_metric,
-            use_l2=(expected_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN),
-            group_keys=groupby_df,
-        )
-
-    def _setup_mock_measurement(
-        self,
-        mock_measurement,
-        child_query: QueryExpr,
-        expected_mechanism: NoiseMechanism,
-    ) -> None:
-        """Initialize a mock measurement."""
-        # pylint: disable=protected-access
-        transformation, reference, _ = self.visitor._visit_child_transformation(
-            child_query, expected_mechanism
-        )
-        # pylint: enable=protected-access
-        mock_measurement.input_domain = lookup_domain(
-            transformation.output_domain, reference
-        )
-        mock_measurement.input_metric = lookup_metric(
-            transformation.output_metric, reference
-        )
-        mock_measurement.privacy_function.return_value = self.visitor.budget.value
-
     @pytest.mark.parametrize(
-        "query,output_measure,expected_mechanism",
+        "query,output_measure,noise_info",
         [
             (
                 GroupByCount(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     mechanism=CountMechanism.DEFAULT,
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.3,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCount(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     mechanism=CountMechanism.LAPLACE,
                     output_column="count",
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.3,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCount(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=CountMechanism.GAUSSIAN,
                     output_column="custom_count_column",
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.449999999999999,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCount(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     mechanism=CountMechanism.DEFAULT,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.449999999999999,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCount(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     mechanism=CountMechanism.LAPLACE,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.6708203932499359,
+                        }
+                    ]
+                ),
             ),
         ],
     )
     def test_visit_groupby_count(
         self,
         query: GroupByCount,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_mechanism: NoiseMechanism,
+        noise_info: NoiseInfo,
     ) -> None:
         """Test visit_groupby_count."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_count_measurement",
-            autospec=True,
-        ) as mock_create_count:
-            self.visitor.output_measure = output_measure
-            self._setup_mock_measurement(
-                mock_measurement, query.child, expected_mechanism
-            )
-            mock_create_count.return_value = mock_measurement
-
-            measurement = self.visitor.visit_groupby_count(query)
-            assert isinstance(measurement, ChainTM)
-
-            self._check_measurement(measurement)
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-            mock_create_count.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                noise_mechanism=expected_mechanism,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                count_column=query.output_column,
-            )
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
-        "query,output_measure,expected_mechanism",
+        "query,output_measure,noise_info",
         [
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     mechanism=CountDistinctMechanism.DEFAULT,
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.3,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     mechanism=CountDistinctMechanism.LAPLACE,
                     output_column="count",
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.3,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     columns_to_count=["A"],
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.3,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=CountDistinctMechanism.GAUSSIAN,
                     output_column="custom_count_column",
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.449999999999999,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     mechanism=CountDistinctMechanism.DEFAULT,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.449999999999999,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     mechanism=CountDistinctMechanism.LAPLACE,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.6708203932499359,
+                        }
+                    ]
+                ),
             ),
         ],
     )
     def test_visit_groupby_count_distinct(
         self,
         query: GroupByCountDistinct,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_mechanism: NoiseMechanism,
+        noise_info: NoiseInfo,
     ) -> None:
         """Test visit_groupby_count_distinct."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_count_distinct_measurement",
-            autospec=True,
-        ) as mock_create_count_distinct:
-            self.visitor.output_measure = output_measure
-
-            mock_create_count_distinct.return_value = mock_measurement
-            self._setup_mock_measurement(
-                mock_measurement, query.child, expected_mechanism
-            )
-            if query.columns_to_count:
-                select_columns = query.columns_to_count + list(
-                    query.groupby_keys.schema().keys()
-                )
-                mock_measurement.input_domain = SparkDataFrameDomain(
-                    {
-                        c: d
-                        for c, d in mock_measurement.input_domain.schema.items()
-                        if c in select_columns
-                    }
-                )
-
-            measurement = self.visitor.visit_groupby_count_distinct(query)
-
-            self._check_measurement(measurement)
-            assert isinstance(measurement, ChainTM)
-            assert measurement.measurement == mock_measurement
-            if query.columns_to_count:
-                assert isinstance(measurement.transformation, ChainTT)
-                assert isinstance(
-                    measurement.transformation.transformation2, SelectTransformation
-                )
-                assert (
-                    measurement.transformation.transformation2.columns == select_columns
-                )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-
-            assert measurement.measurement == mock_measurement
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-
-            mock_create_count_distinct.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                noise_mechanism=expected_mechanism,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                count_column=query.output_column,
-            )
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
-        "query,output_measure,expected_new_child",
+        "query,output_measure,noise_info",
         [
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     low=-100,
                     high=100,
                     output_column="custom_output_column",
                     measure_column="B",
                     quantile=0.1,
                 ),
                 PureDP(),
-                None,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 3.3333333333333326,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     low=-100,
                     high=100,
                     output_column="custom_output_column",
                     measure_column="null_and_nan",
                     quantile=0.1,
                 ),
                 PureDP(),
-                DropNullAndNan(PrivateSource("private"), ["null_and_nan"]),
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 3.3333333333333326,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
                     output_column="quantile",
                     low=123.345,
                     high=987.65,
                     quantile=0.25,
                 ),
                 PureDP(),
-                None,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 3.3333333333333326,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="null_and_inf",
                     output_column="quantile",
                     low=123.345,
                     high=987.65,
                     quantile=0.25,
                 ),
                 PureDP(),
-                ReplaceInfExpr(
-                    DropNullAndNan(PrivateSource("private"), ["null_and_inf"]),
-                    {"null_and_inf": (123.345, 987.65)},
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 3.3333333333333326,
+                        }
+                    ]
                 ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     quantile=0.5,
                     measure_column="X",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                None,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 2.9814239699997196,
+                        }
+                    ]
+                ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     quantile=0.5,
                     measure_column="nan_and_inf",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                ReplaceInfExpr(
-                    DropNullAndNan(PrivateSource("private"), ["nan_and_inf"]),
-                    {"nan_and_inf": (0, 1)},
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 2.9814239699997196,
+                        }
+                    ]
                 ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     quantile=0.5,
                     measure_column="inf",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                ReplaceInfExpr(PrivateSource("private"), {"inf": (0, 1)}),
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                            "noise_parameter": 2.9814239699997196,
+                        }
+                    ]
+                ),
             ),
         ],
     )
     def test_visit_groupby_quantile(
         self,
         query: GroupByQuantile,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_new_child: Optional[QueryExpr],
+        noise_info: NoiseInfo,
     ) -> None:
         """Test visit_groupby_quantile."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_quantile_measurement",
-            autospec=True,
-        ) as mock_create_quantile:
-            self.visitor.output_measure = output_measure
-
-            expected_mechanism = self.visitor.default_mechanism
-            expected_child_query: QueryExpr
-            if expected_new_child is not None:
-                expected_child_query = expected_new_child
-            else:
-                expected_child_query = query.child
-            self._setup_mock_measurement(
-                mock_measurement, expected_child_query, expected_mechanism
-            )
-            mock_create_quantile.return_value = mock_measurement
-
-            measurement = self.visitor.visit_groupby_quantile(query)
-
-            self._check_measurement(measurement)
-            assert isinstance(measurement, ChainTM)
-            assert measurement.measurement == mock_measurement
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-            mock_create_quantile.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                measure_column=query.measure_column,
-                quantile=query.quantile,
-                lower=query.low,
-                upper=query.high,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                quantile_column=query.output_column,
-            )
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
-        "query,output_measure,expected_mechanism",
+        "query,output_measure,noise_info",
         [
             (
-                GroupByBoundedSum(
+                GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     low=-100,
                     high=100,
-                    mechanism=SumMechanism.DEFAULT,
+                    mechanism=AverageMechanism.DEFAULT,
                     output_column="custom_output_column",
                     measure_column="B",
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 60,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.6,
+                        },
+                    ]
+                ),
             ),
             (
-                GroupByBoundedSum(
+                GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
-                    mechanism=SumMechanism.DEFAULT,
+                    mechanism=AverageMechanism.DEFAULT,
                     output_column="sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 259.2915,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 0.6,
+                        },
+                    ]
+                ),
             ),
             (
-                GroupByBoundedSum(
+                GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
-                    mechanism=SumMechanism.LAPLACE,
+                    mechanism=AverageMechanism.LAPLACE,
                     output_column="different_sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 259.2915,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 0.6,
+                        },
+                    ]
+                ),
             ),
             (
-                GroupByBoundedSum(
+                GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
-                    mechanism=SumMechanism.DEFAULT,
+                    mechanism=AverageMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
         ],
     )
-    def test_visit_groupby_bounded_sum(
+    def test_visit_groupby_bounded_average(
         self,
-        query: GroupByBoundedSum,
+        query: GroupByBoundedAverage,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_mechanism: NoiseMechanism,
+        noise_info: NoiseInfo,
     ) -> None:
-        """Test visit_groupby_bounded_sum."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_sum_measurement",
-            autospec=True,
-        ) as mock_create_sum:
-            self.visitor.output_measure = output_measure
-
-            self._setup_mock_measurement(
-                mock_measurement, query.child, expected_mechanism
-            )
-            mock_create_sum.return_value = mock_measurement
-
-            measurement = self.visitor.visit_groupby_bounded_sum(query)
-
-            self._check_measurement(measurement)
-            assert isinstance(measurement, ChainTM)
-            assert measurement.measurement == mock_measurement
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-            lower, upper = _get_query_bounds(query)
-            mock_create_sum.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                measure_column=query.measure_column,
-                lower=lower,
-                upper=upper,
-                noise_mechanism=expected_mechanism,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                sum_column=query.output_column,
-            )
+        """Test visit_groupby_bounded_average."""
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
-        "query,output_measure,expected_mechanism",
+        "query,output_measure,noise_info",
         [
             (
-                GroupByBoundedAverage(
+                GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     low=-100,
                     high=100,
-                    mechanism=AverageMechanism.DEFAULT,
+                    mechanism=SumMechanism.DEFAULT,
                     output_column="custom_output_column",
                     measure_column="B",
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 30,
+                        }
+                    ]
+                ),
             ),
             (
-                GroupByBoundedAverage(
+                GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
-                    mechanism=AverageMechanism.DEFAULT,
+                    mechanism=SumMechanism.DEFAULT,
                     output_column="sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 296.2949999999999,
+                        }
+                    ]
+                ),
             ),
             (
-                GroupByBoundedAverage(
+                GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
-                    mechanism=AverageMechanism.LAPLACE,
+                    mechanism=SumMechanism.LAPLACE,
                     output_column="different_sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 296.2949999999999,
+                        }
+                    ]
+                ),
             ),
             (
-                GroupByBoundedAverage(
+                GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
-                    mechanism=AverageMechanism.DEFAULT,
+                    mechanism=SumMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 0.449999999999999,
+                        }
+                    ]
+                ),
             ),
         ],
     )
-    def test_visit_groupby_bounded_average(
+    def test_visit_groupby_bounded_sum(
         self,
-        query: GroupByBoundedAverage,
+        query: GroupByBoundedSum,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_mechanism: NoiseMechanism,
+        noise_info: NoiseInfo,
     ) -> None:
-        """Test visit_groupby_bounded_average."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_average_measurement",
-            autospec=True,
-        ) as mock_create_average:
-            self.visitor.output_measure = output_measure
-
-            self._setup_mock_measurement(
-                mock_measurement, query.child, expected_mechanism
-            )
-            mock_create_average.return_value = mock_measurement
-
-            measurement = self.visitor.visit_groupby_bounded_average(query)
-
-            self._check_measurement(measurement)
-            assert isinstance(measurement, ChainTM)
-            assert measurement.measurement == mock_measurement
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-            lower, upper = _get_query_bounds(query)
-            mock_create_average.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                measure_column=query.measure_column,
-                lower=lower,
-                upper=upper,
-                noise_mechanism=expected_mechanism,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                average_column=query.output_column,
-            )
+        """Test visit_groupby_bounded_sum."""
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
-        "query,output_measure,expected_mechanism",
+        "query,output_measure,noise_info",
         [
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     low=-100,
                     high=100,
                     mechanism=VarianceMechanism.DEFAULT,
                     output_column="custom_output_column",
                     measure_column="B",
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 90,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 4500,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
                     mechanism=VarianceMechanism.DEFAULT,
                     output_column="sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 388.9372499999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 432107.34006374987,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
                     mechanism=VarianceMechanism.LAPLACE,
                     output_column="different_sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 388.9372499999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 432107.34006374987,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=VarianceMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 1.349999999999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 1.349999999999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 1.349999999999999,
+                        },
+                    ]
+                ),
             ),
         ],
     )
     def test_visit_groupby_bounded_variance(
         self,
         query: GroupByBoundedVariance,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_mechanism: NoiseMechanism,
+        noise_info: NoiseInfo,
     ) -> None:
         """Test visit_groupby_bounded_variance."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_variance_measurement",
-            autospec=True,
-        ) as mock_create_variance:
-            self.visitor.output_measure = output_measure
-
-            self._setup_mock_measurement(
-                mock_measurement, query.child, expected_mechanism
-            )
-            mock_create_variance.return_value = mock_measurement
-
-            measurement = self.visitor.visit_groupby_bounded_variance(query)
-
-            self._check_measurement(measurement)
-            assert isinstance(measurement, ChainTM)
-            assert measurement.measurement == mock_measurement
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-            lower, upper = _get_query_bounds(query)
-            mock_create_variance.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                measure_column=query.measure_column,
-                lower=lower,
-                upper=upper,
-                noise_mechanism=expected_mechanism,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                variance_column=query.output_column,
-            )
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
-        "query,output_measure,expected_mechanism",
+        "query,output_measure,noise_info",
         [
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
                     low=-100,
                     high=100,
                     mechanism=StdevMechanism.DEFAULT,
                     output_column="custom_output_column",
                     measure_column="B",
                 ),
                 PureDP(),
-                NoiseMechanism.GEOMETRIC,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 90,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 4500,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.GEOMETRIC,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
                     mechanism=StdevMechanism.DEFAULT,
                     output_column="sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 388.9372499999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 432107.34006374987,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"B": [0, 1]}),
                     measure_column="X",
                     mechanism=StdevMechanism.LAPLACE,
                     output_column="different_sum",
                     low=123.345,
                     high=987.65,
                 ),
                 PureDP(),
-                NoiseMechanism.LAPLACE,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 388.9372499999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 432107.34006374987,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.LAPLACE,
+                            "noise_parameter": 0.899999999999999,
+                        },
+                    ]
+                ),
             ),
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=StdevMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
                     high=1,
                 ),
                 RhoZCDP(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseInfo(
+                    [
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 1.349999999999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 1.349999999999999,
+                        },
+                        {
+                            "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                            "noise_parameter": 1.349999999999999,
+                        },
+                    ]
+                ),
             ),
         ],
     )
     def test_visit_groupby_bounded_stdev(
         self,
         query: GroupByBoundedSTDEV,
         output_measure: Union[PureDP, RhoZCDP],
-        expected_mechanism: NoiseMechanism,
+        noise_info: NoiseInfo,
     ) -> None:
         """Test visit_groupby_bounded_stdev."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.GroupBy",
-            autospec=True,
-        ) as mock_groupby, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
-            autospec=True,
-        ) as mock_measurement, patch(
-            "tmlt.analytics._query_expr_compiler."
-            + "_measurement_visitor.create_standard_deviation_measurement",
-            autospec=True,
-        ) as mock_create_stdev:
-            self.visitor.output_measure = output_measure
-            self.visitor.output_measure = output_measure
-
-            self._setup_mock_measurement(
-                mock_measurement, query.child, expected_mechanism
-            )
-            mock_create_stdev.return_value = mock_measurement
-
-            measurement = self.visitor.visit_groupby_bounded_stdev(query)
-
-            self._check_measurement(measurement)
-            assert isinstance(measurement, ChainTM)
-            assert measurement.measurement == mock_measurement
-            self.check_mock_groupby_call(
-                mock_groupby,
-                measurement.transformation,
-                query.groupby_keys,
-                expected_mechanism,
-            )
-
-            mid_stability = measurement.transformation.stability_function(
-                self.visitor.stability
-            )
-            lower, upper = _get_query_bounds(query)
-            mock_create_stdev.assert_called_with(
-                input_domain=measurement.transformation.output_domain,
-                input_metric=measurement.transformation.output_metric,
-                measure_column=query.measure_column,
-                lower=lower,
-                upper=upper,
-                noise_mechanism=expected_mechanism,
-                d_in=mid_stability,
-                d_out=self.visitor.budget.value,
-                output_measure=self.visitor.output_measure,
-                groupby_transformation=mock_groupby.return_value,
-                standard_deviation_column=query.output_column,
-            )
+        self.run_with_empty_data_and_check_schema(query, output_measure)
+        self.check_noise_info(query, output_measure, noise_info)
 
     @pytest.mark.parametrize(
         "query",
         [
             (PrivateSource("private")),
             (Rename(child=PrivateSource("private"), column_mapper={"A": "A2"})),
             (Filter(child=PrivateSource("private"), condition="B > 2")),
```

### Comparing `tmlt_analytics-0.8.3/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for OutputSchemaVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Dict, List, Type
 
 import pytest
 from pyspark.sql import SparkSession
 from pyspark.sql.types import LongType, StringType, StructField, StructType
```

### Comparing `tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/conftest.py` & `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Fixtures and data for TransformationVisitor tests."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Dict, List, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
```

### Comparing `tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py` & `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for TransformationVisitor on tables with AddRemoveKeys metrics."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Dict, List, Mapping, Tuple, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
@@ -240,24 +240,25 @@
                     [[1, "0", 0, 0.1, DATE1, TIMESTAMP1, 1]],
                     columns=["id", "S", "I", "F", "D", "T", "S_is_zero"],
                 ),
             ),
             (
                 FlatMap(
                     child=PrivateSource("ids1"),
-                    f=lambda row: [{"X": n} for n in range(row["I"] + 10)],
+                    f=lambda row: [{"X": n} for n in range(row["I"] + 4)],
                     schema_new_columns=Schema({"X": "INTEGER"}),
                     augment=True,
-                    max_rows=3,
+                    max_rows=3,  # this is ignored
                 ),
                 pd.DataFrame(
                     [
                         [1, "0", 0, 0.1, DATE1, TIMESTAMP1, 0],
                         [1, "0", 0, 0.1, DATE1, TIMESTAMP1, 1],
                         [1, "0", 0, 0.1, DATE1, TIMESTAMP1, 2],
+                        [1, "0", 0, 0.1, DATE1, TIMESTAMP1, 3],
                     ],
                     columns=["id", "S", "I", "F", "D", "T", "X"],
                 ),
             ),
         ],
     )
     def test_visit_flat_map(self, query: FlatMap, expected_df: DataFrame) -> None:
```

### Comparing `tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py` & `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for TransformationVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Dict, List, Mapping, Optional, Tuple, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
```

### Comparing `tmlt_analytics-0.8.3/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py` & `tmlt_analytics-0.9.0rc5/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for constraint handling in TransformationVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from typing import Dict, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
 from tmlt.core.metrics import SymmetricDifference
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_binning_spec.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_binning_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for BinningSpec."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Any, List
 
 import pytest
 
 from tmlt.analytics._schema import ColumnDescriptor
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_catalog.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for catalog."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 
 from typing import Optional
 
 import pytest
 
 from tmlt.analytics._catalog import Catalog, PrivateTable
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_cleanup.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_cleanup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Tests for Analytics cleanup functions."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 
 from unittest.mock import patch
 
 from tmlt.analytics.utils import cleanup, remove_all_temp_tables
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_constraints.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for Constraints."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from typing import List
 
 import pytest
 
 from tmlt.analytics.constraints import (
     Constraint,
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_keyset.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_keyset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for KeySet."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from typing import Dict, List, Mapping, Optional, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import Column
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_neighboring_relations.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_neighboring_relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for neighboring relations."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=no-self-use
 
 from cmath import inf, pi
 from typing import Dict
 
 import pandas as pd
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_noise_info.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_noise_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for noise info."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from typing import Dict
 
 import pytest
 import sympy as sp
 from tmlt.core.domains.numpy_domains import NumpyFloatDomain, NumpyIntegerDomain
 from tmlt.core.domains.pandas_domains import PandasSeriesDomain
@@ -16,56 +16,72 @@
     AddGeometricNoise,
     AddLaplaceNoise,
 )
 from tmlt.core.measurements.pandas_measurements.series import NoisyQuantile
 from tmlt.core.measures import PureDP
 
 from tmlt.analytics._noise_info import (
+    NoiseInfo,
     _inverse_cdf,
     _noise_from_measurement,
     _NoiseMechanism,
 )
 
 
 @pytest.mark.parametrize(
     "measurement,expected",
     [
         (
             AddLaplaceNoise(NumpyIntegerDomain(), scale=sp.Rational(2.5)),
-            [{"noise_mechanism": _NoiseMechanism.LAPLACE, "noise_parameter": 2.5}],
+            NoiseInfo(
+                [{"noise_mechanism": _NoiseMechanism.LAPLACE, "noise_parameter": 2.5}]
+            ),
         ),
         (
             AddGeometricNoise(alpha=sp.Rational(3.5)),
-            [{"noise_mechanism": _NoiseMechanism.GEOMETRIC, "noise_parameter": 3.5}],
+            NoiseInfo(
+                [{"noise_mechanism": _NoiseMechanism.GEOMETRIC, "noise_parameter": 3.5}]
+            ),
         ),
         (
             AddDiscreteGaussianNoise(sigma_squared=sp.Rational(4.5)),
-            [
-                {
-                    "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
-                    "noise_parameter": 4.5,
-                }
-            ],
+            NoiseInfo(
+                [
+                    {
+                        "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
+                        "noise_parameter": 4.5,
+                    }
+                ]
+            ),
         ),
         (
             AddGaussianNoise(
                 input_domain=NumpyFloatDomain(), sigma_squared=sp.Rational(5.5)
             ),
-            [{"noise_mechanism": _NoiseMechanism.GAUSSIAN, "noise_parameter": 5.5}],
+            NoiseInfo(
+                [{"noise_mechanism": _NoiseMechanism.GAUSSIAN, "noise_parameter": 5.5}]
+            ),
         ),
         (
             NoisyQuantile(
                 PandasSeriesDomain(element_domain=NumpyIntegerDomain()),
                 PureDP(),
                 quantile=0.5,
                 lower=0,
                 upper=10,
                 epsilon=sp.Rational(5.5),
             ),
-            [{"noise_mechanism": _NoiseMechanism.EXPONENTIAL, "noise_parameter": 5.5}],
+            NoiseInfo(
+                [
+                    {
+                        "noise_mechanism": _NoiseMechanism.EXPONENTIAL,
+                        "noise_parameter": 5.5,
+                    }
+                ],
+            ),
         ),
     ],
 )
 def test_noise_from_measurement(measurement: Measurement, expected: Dict):
     """Get noise from measurement."""
     noise_info = _noise_from_measurement(measurement)
     assert noise_info == expected
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_privacy_budget.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for :mod:`tmlt.analytics.privacy_budget`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 # pylint: disable=pointless-string-statement
 
 import pytest
 
 from tmlt.analytics.privacy_budget import ApproxDPBudget, PureDPBudget, RhoZCDPBudget
 
 """Tests for :class:`tmlt.analytics.privacy_budget.PureDPBudget`."""
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for :mod:`tmlt.analytics._privacy_budget_rounding_helper`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 # pylint: disable=pointless-string-statement
 
 
 from tmlt.core.utils.exact_number import ExactNumber
 from typeguard import typechecked
 
 from tmlt.analytics._privacy_budget_rounding_helper import (
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_protected_change.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_protected_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for :mod:`tmlt.analytics.protected_change`."""
 
-# Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from contextlib import nullcontext as does_not_raise
 from typing import Any, ContextManager, List
 
 import pytest
 
 from tmlt.analytics.protected_change import (
@@ -65,18 +65,15 @@
                 TypeError, match="^type of max_groups must be int; got str instead$"
             ),
         ),
         (
             ["x", 1, "y"],
             pytest.raises(
                 TypeError,
-                match=(
-                    r"^type of max_rows_per_group must be one of \(int, float\); got"
-                    r" str instead$"
-                ),
+                match=(r"^type of max_rows_per_group must be int; got str instead$"),
             ),
         ),
     ],
 )
 def test_add_max_rows_per_group_invalid(
     args: List[Any], expectation: ContextManager[None]
 ):
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_query_builder.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_query_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for :mod:`~tmlt.analytics.query_builder`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 # pylint: disable=no-self-use
 import datetime
 import re
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import pandas as pd
 import pytest
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_query_expr_compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Tests for QueryExprCompiler."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=protected-access, no-self-use
 
 import datetime
 from typing import Dict, List, Union
-from unittest.mock import patch
 
 import pandas as pd
 import pytest
 import sympy as sp
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.functions import col
 from pyspark.sql.types import (
@@ -26,27 +25,26 @@
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
-from tmlt.core.measurements.aggregations import NoiseMechanism
 from tmlt.core.measures import PureDP, RhoZCDP
 from tmlt.core.metrics import DictMetric, SymmetricDifference
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler import QueryExprCompiler
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
 )
-from tmlt.analytics._table_identifier import Identifier, NamedTable
+from tmlt.analytics._table_identifier import NamedTable
 from tmlt.analytics._transformation_utils import get_table_from_ref
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountMechanism,
     Filter,
@@ -68,15 +66,15 @@
     Select,
     StdevMechanism,
     SumMechanism,
     VarianceMechanism,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
-from ..conftest import assert_frame_equal_with_sort, create_mock_measurement
+from ..conftest import assert_frame_equal_with_sort
 
 GROUPBY_TWO_COLUMNS = pd.DataFrame([["0", 0], ["0", 1], ["1", 1]], columns=["A", "B"])
 GROUPBY_TWO_SCHEMA = StructType(
     [StructField("A", StringType(), False), StructField("B", LongType(), False)]
 )
 GET_GROUPBY_TWO = lambda: SparkSession.builder.getOrCreate().createDataFrame(
     GROUPBY_TWO_COLUMNS, schema=GROUPBY_TWO_SCHEMA
@@ -693,15 +691,15 @@
                     ["0", 0, 1.0],
                     ["0", 1, 2.0],
                     ["1", 0, 3.0],
                 ],
                 columns=["A", "B", "X"],
             )
         )
-        measurement = self.compiler(
+        measurement, _ = self.compiler(
             [query_expr],
             privacy_budget=PureDPBudget(float("inf")),
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={
                 "public": self.join_df,
@@ -719,15 +717,15 @@
     def test_queries(self, query_exprs: List[QueryExpr], expected: List[pd.DataFrame]):
         """Tests that compiled measurement produces correct results.
 
         Args:
             query_exprs: The queries to evaluate.
             expected: The expected answers.
         """
-        measurement = self.compiler(
+        measurement, _ = self.compiler(
             query_exprs,
             privacy_budget=PureDPBudget(float("inf")),
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={
                 "public": self.join_df,
@@ -1051,15 +1049,15 @@
         """Tests aggregation with various privacy definition and mechanism."""
         compiler = QueryExprCompiler(output_measure=output_measure)
         privacy_budget = (
             PureDPBudget(float("inf"))
             if isinstance(output_measure, PureDP)
             else RhoZCDPBudget(float("inf"))
         )
-        measurement = compiler(
+        measurement, _ = compiler(
             [query],
             privacy_budget=privacy_budget,
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={"public": self.join_df},
             catalog=self.catalog,
@@ -1301,15 +1299,15 @@
                 measure_column="X",
                 low=0.0,
                 high=1.0,
                 output_column="sum",
                 mechanism=SumMechanism.LAPLACE,
             )
         ]
-        measurement = QueryExprCompiler()(
+        measurement, _ = QueryExprCompiler()(
             query_exprs,
             privacy_budget=PureDPBudget(float("inf")),
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
@@ -1412,15 +1410,15 @@
         input_metric = DictMetric(
             {
                 NamedTable("doubled"): self.input_metric[NamedTable("private")],
                 **self.input_metric.key_to_metric,
             }
         )
 
-        measurement = self.compiler(
+        measurement, _ = self.compiler(
             query_exprs,
             privacy_budget=PureDPBudget(10),
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             public_sources={"public": self.join_df},
             catalog=self.catalog,
@@ -1505,15 +1503,15 @@
             groupby_keys=KeySet.from_dict({"Gender": ["M", "F"]}),
             measure_column="Age",
             quantile=0.5,
             low=22,
             high=29,
             output_column="out",
         )
-        measurement = compiler(
+        measurement, _ = compiler(
             [query_expr],
             privacy_budget=privacy_budget,
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             public_sources={},
             catalog=catalog,
@@ -1545,178 +1543,7 @@
         }
     )
     request.cls._input_metric = DictMetric({NamedTable("test"): SymmetricDifference()})
     request.cls._catalog = Catalog()
     request.cls._catalog.add_private_table(
         source_id="test", col_types={"A": ColumnType.VARCHAR, "X": ColumnType.INTEGER}
     )
-
-
-@pytest.mark.usefixtures("test_component_data")
-class TestComponentIsUsed:
-    """Tests that specific components are used inside of compiled measurements."""
-
-    _stability: Dict[Identifier, sp.Integer]
-    _privacy_budget: sp.Integer
-    _input_domain: DictDomain
-    _input_metric: DictMetric
-    _catalog: Catalog
-
-    @pytest.mark.parametrize(
-        "output_measure,query_expr,column,preprocessing_stability",
-        [
-            (output_measure, query_expr, column, preprocessing_stability)
-            for output_measure in [PureDP(), RhoZCDP()]
-            for preprocessing_expr, preprocessing_stability in [
-                (
-                    ReplaceNullAndNan(
-                        replace_with={},
-                        child=FlatMap(
-                            child=PrivateSource(source_id="test"),
-                            f=lambda row: [{}, {}],
-                            schema_new_columns=Schema({}),
-                            augment=True,
-                            max_rows=2,
-                        ),
-                    ),
-                    2,
-                ),
-                (PrivateSource(source_id="test"), 1),
-            ]
-            for query_expr, column in [
-                (
-                    GroupByCount(
-                        child=preprocessing_expr,
-                        groupby_keys=KeySet.from_dict({"A": ["a1", "a2"]}),
-                    ),
-                    "count",
-                ),
-                (
-                    GroupByBoundedSum(
-                        child=preprocessing_expr,
-                        groupby_keys=KeySet.from_dict({"A": ["a1", "a2"]}),
-                        measure_column="X",
-                        low=-1,
-                        high=5,
-                        output_column="sum",
-                    ),
-                    "sum",
-                ),
-                (
-                    GroupByBoundedAverage(
-                        child=preprocessing_expr,
-                        groupby_keys=KeySet.from_dict({"A": ["a1", "a2"]}),
-                        measure_column="X",
-                        low=-1,
-                        high=5,
-                        output_column="average",
-                    ),
-                    "average",
-                ),
-                (
-                    GroupByBoundedSTDEV(
-                        child=preprocessing_expr,
-                        groupby_keys=KeySet.from_dict({"A": ["a1", "a2"]}),
-                        measure_column="X",
-                        low=-1,
-                        high=5,
-                        output_column="standard deviation",
-                    ),
-                    "standard deviation",
-                ),
-                (
-                    GroupByBoundedVariance(
-                        child=preprocessing_expr,
-                        groupby_keys=KeySet.from_dict({"A": ["a1", "a2"]}),
-                        measure_column="X",
-                        low=-1,
-                        high=5,
-                        output_column="variance",
-                    ),
-                    "variance",
-                ),
-                (
-                    GroupByQuantile(
-                        child=preprocessing_expr,
-                        groupby_keys=KeySet.from_dict({"A": ["a1", "a2"]}),
-                        measure_column="X",
-                        quantile=0.6,
-                        low=-1,
-                        high=5,
-                        output_column="quantile",
-                    ),
-                    "quantile",
-                ),
-            ]
-        ],
-    )
-    def test_used_create_measurement(
-        self,
-        output_measure: Union[PureDP, RhoZCDP],
-        query_expr: QueryExpr,
-        column: str,
-        preprocessing_stability: int,
-    ):
-        """Compiled measurements contain aggregations with the expected noise scale."""
-        with patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor."
-            "create_quantile_measurement"
-        ) as mock_create_quantile_measurement, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor."
-            "create_standard_deviation_measurement"
-        ) as mock_create_standard_deviation_measurement, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor."
-            "create_variance_measurement"
-        ) as mock_create_variance_measurement, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor."
-            "create_average_measurement"
-        ) as mock_create_average_measurement, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor."
-            "create_sum_measurement"
-        ) as mock_create_sum_measurement, patch(
-            "tmlt.analytics._query_expr_compiler._measurement_visitor."
-            "create_count_measurement"
-        ) as mock_create_count_measurement:
-            d_in = sp.Integer(3)
-            d_out = sp.Integer(5)
-            compiler = QueryExprCompiler(output_measure=output_measure)
-            mock_create_measurement_dict = {
-                "count": mock_create_count_measurement,
-                "sum": mock_create_sum_measurement,
-                "average": mock_create_average_measurement,
-                "variance": mock_create_variance_measurement,
-                "standard deviation": mock_create_standard_deviation_measurement,
-                "quantile": mock_create_quantile_measurement,
-            }
-            mock_create_measurement = mock_create_measurement_dict[column]
-            mock_create_measurement.return_value = create_mock_measurement(
-                input_domain=self._input_domain[NamedTable("test")],
-                input_metric=self._input_metric[NamedTable("test")],
-                output_measure=output_measure,
-                privacy_function_return_value=d_out,
-                privacy_function_implemented=True,
-            )
-            _ = compiler(
-                [query_expr],
-                privacy_budget=self._privacy_budget,
-                stability=self._stability,
-                input_domain=self._input_domain,
-                input_metric=self._input_metric,
-                public_sources={},
-                catalog=self._catalog,
-                table_constraints={t: [] for t in self._stability.keys()},
-            )
-            expected_arguments = {  # Other arguments are not checked
-                "input_domain": self._input_domain[NamedTable("test")],
-                "input_metric": self._input_metric[NamedTable("test")],
-                "d_in": d_in * preprocessing_stability,
-                "d_out": d_out,
-            }
-            if column != "quantile":
-                expected_arguments["noise_mechanism"] = (
-                    NoiseMechanism.GEOMETRIC
-                    if isinstance(output_measure, PureDP)
-                    else NoiseMechanism.DISCRETE_GAUSSIAN
-                )
-            _, kwargs = mock_create_measurement.call_args_list[-1]
-            for kwarg, value in expected_arguments.items():
-                assert kwargs[kwarg] == value
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_query_expression.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_query_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for QueryExpr."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=too-many-arguments, unidiomatic-typecheck, pointless-string-statement
 
 import datetime
 import re
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, Union
 
@@ -149,15 +149,15 @@
     [
         (  # Invalid max_rows
             PrivateSource("private"),
             lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
             -1,
             Schema({"i": "INTEGER"}),
             False,
-            "Limit on number of rows '-1' must be nonnegative.",
+            "Limit on number of rows '-1' must be non-negative.",
         ),
         (  # Invalid augment
             FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"Repeat": 1 if row["A"] == "0" else 2}],
                 schema_new_columns=Schema({"Repeat": "INTEGER"}),
                 augment=True,
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_query_expression_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for QueryExprVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import pytest
 
 from tmlt.analytics._schema import Schema
 from tmlt.analytics.constraints import MaxRowsPerID
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_schema.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for schema."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 # pylint: disable=pointless-string-statement
 import re
 
 import pytest
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_schema_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests conversion functions in :mod:`~tmlt.analytics._schema`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 # pylint: disable=no-self-use
 import datetime
 
 import pytest
 from pyspark.sql import types as spark_types
 from tmlt.core.domains.spark_domains import (
     SparkColumnsDescriptor,
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_session.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Unit tests for Session."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=no-self-use, unidiomatic-typecheck
 
 import re
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Dict, List, Tuple, Type, Union
 from unittest.mock import ANY, Mock, patch
 
 import pandas as pd
 import pytest
 import sympy as sp
 from pyspark.sql import DataFrame
 from pyspark.sql.types import (
@@ -42,19 +42,17 @@
     DictMetric,
     IfGroupedBy,
     Metric,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
-from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.chaining import ChainTT
 from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
 from tmlt.core.utils.exact_number import ExactNumber
-from typeguard import check_type
 
 from tmlt.analytics._neighboring_relation import (
     AddRemoveKeys,
     AddRemoveRows,
     AddRemoveRowsAcrossGroups,
     Conjunction,
     NeighboringRelation,
@@ -64,15 +62,14 @@
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
     spark_schema_to_analytics_columns,
 )
 from tmlt.analytics._table_identifier import NamedTable, TableCollection
-from tmlt.analytics._table_reference import TableReference
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
 )
 from tmlt.analytics.keyset import KeySet
@@ -88,15 +85,15 @@
     AddOneRow,
     AddRowsWithID,
 )
 from tmlt.analytics.query_builder import GroupedQueryBuilder, QueryBuilder
 from tmlt.analytics.query_expr import PrivateSource, QueryExpr
 from tmlt.analytics.session import Session
 
-from ..conftest import assert_frame_equal_with_sort, create_mock_transformation
+from ..conftest import assert_frame_equal_with_sort
 
 
 def _privacy_budget_to_exact_number(
     budget: Union[PureDPBudget, RhoZCDPBudget]
 ) -> ExactNumber:
     """Turn a privacy budget into an Exact Number."""
     if isinstance(budget, (PureDPBudget, RhoZCDPBudget)):
@@ -193,101 +190,84 @@
     join_col_types: Schema
     join_input_domain: DictDomain
     private_schema: Dict[str, ColumnDescriptor]
     public_schema: Dict[str, ColumnDescriptor]
     combined_input_domain: DictDomain
 
     @pytest.mark.parametrize(
-        "budget_value,output_measure,expected_budget",
+        "budget_values,output_measure,expected_budget",
         [
             pytest.param(ExactNumber(10), PureDP(), PureDPBudget(10), id="puredp"),
             pytest.param(ExactNumber(10), RhoZCDP(), RhoZCDPBudget(10), id="zcdp"),
+            pytest.param(
+                (ExactNumber(10), ExactNumber("0.5")),
+                ApproxDP(),
+                ApproxDPBudget(10, 0.5),
+                id="approxdp",
+            ),
         ],
     )
     def test_remaining_privacy_budget(
-        self, budget_value, output_measure, expected_budget
+        self, budget_values, output_measure, expected_budget
     ):
         """Test that remaining_privacy_budget returns the right type of budget."""
         with patch(
-            "tmlt.analytics.session.QueryExprCompiler", autospec=True
-        ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant(
-                mock_accountant, privacy_budget=budget_value, d_in=ExactNumber(1)
+                mock_accountant, privacy_budget=budget_values, d_in=ExactNumber(1)
             )
             mock_accountant.output_measure = output_measure
 
-            mock_compiler.output_measure = output_measure
-
-            session = Session(mock_accountant, {}, mock_compiler)
+            session = Session(mock_accountant, {})
             privacy_budget = session.remaining_privacy_budget
+            # Check that the output privacy_budget is the correct Type
             assert type(expected_budget) == type(privacy_budget)
-            if isinstance(expected_budget, PureDPBudget):
-                assert budget_value == ExactNumber(expected_budget.epsilon)
-            elif isinstance(expected_budget, RhoZCDPBudget):
-                assert budget_value == ExactNumber(expected_budget.rho)
+
+            # Check that the correct privacy budget values are returned
+            if isinstance(privacy_budget, PureDPBudget):
+                assert budget_values == ExactNumber(privacy_budget.epsilon)
+            elif isinstance(privacy_budget, RhoZCDPBudget):
+                assert budget_values == ExactNumber(privacy_budget.rho)
+            elif isinstance(privacy_budget, ApproxDPBudget):
+                assert budget_values == (
+                    ExactNumber(privacy_budget.epsilon),
+                    ExactNumber(str(privacy_budget.delta)),
+                )
             else:
                 raise RuntimeError(
                     f"Unexpected budget type: found {type(expected_budget)}"
                 )
 
     @pytest.mark.parametrize(
         "budget,expected_output_measure,expected_metric,from_dataframe_args",
         [
             pytest.param(
                 PureDPBudget(float("inf")),
                 PureDP(),
                 SymmetricDifference(),
-                {"stability": 21, "grouping_column": None, "protected_change": None},
-                id="puredp-stability",
-            ),
-            pytest.param(
-                PureDPBudget(float("inf")),
-                PureDP(),
-                SymmetricDifference(),
                 {
-                    "stability": None,
-                    "grouping_column": None,
                     "protected_change": AddMaxRows(21),
                 },
                 id="puredp-protected_change",
             ),
             pytest.param(
                 PureDPBudget(float("inf")),
                 PureDP(),
                 IfGroupedBy("X", SumOf(SymmetricDifference())),
-                {"stability": 21, "grouping_column": "X", "protected_change": None},
-                id="puredp-grouped-stability",
-            ),
-            pytest.param(
-                RhoZCDPBudget(float("inf")),
-                RhoZCDP(),
-                IfGroupedBy("X", RootSumOfSquared(SymmetricDifference())),
-                {"stability": 21, "grouping_column": "X", "protected_change": None},
-                id="zcdp-grouped-stability",
-            ),
-            pytest.param(
-                PureDPBudget(float("inf")),
-                PureDP(),
-                IfGroupedBy("X", SumOf(SymmetricDifference())),
                 {
-                    "stability": None,
-                    "grouping_column": None,
                     "protected_change": AddMaxRowsInMaxGroups("X", 3, 7),
                 },
                 id="puredp-grouped-protected_change",
             ),
             pytest.param(
                 RhoZCDPBudget(float("inf")),
                 RhoZCDP(),
                 IfGroupedBy("X", RootSumOfSquared(SymmetricDifference())),
                 {
-                    "stability": None,
-                    "grouping_column": None,
                     "protected_change": AddMaxRowsInMaxGroups("X", 9, 7),
                 },
                 id="zcdp-grouped-protected_change",
             ),
         ],
     )
     def test_from_dataframe(
@@ -331,15 +311,15 @@
             assert_frame_equal_with_sort(
                 mock_composition_init.return_value.mock_calls[0][1][0][
                     NamedTable("private")
                 ].toPandas(),
                 self.sdf.toPandas(),
             )
             mock_session_init.assert_called_with(
-                self=ANY, accountant=ANY, public_sources={}, compiler=ANY
+                self=ANY, accountant=ANY, public_sources={}
             )
 
     @pytest.mark.parametrize(
         "budget,expected_output_measure,expected_metric,from_dataframe_args",
         [
             pytest.param(
                 PureDPBudget(float("inf")),
@@ -348,16 +328,14 @@
                     {
                         TableCollection("default_id_space"): CoreAddRemoveKeys(
                             {NamedTable("private"): "A"}
                         )
                     }
                 ),
                 {
-                    "stability": None,
-                    "grouping_column": None,
                     "protected_change": AddRowsWithID("A"),
                 },
                 id="puredp-addrowswithID-protected_change",
             )
         ],
     )
     def test_from_dataframe_add_remove_keys(
@@ -409,15 +387,15 @@
             assert_frame_equal_with_sort(
                 mock_composition_init.return_value.mock_calls[0][1][0][
                     TableCollection("default_id_space")
                 ][NamedTable("private")].toPandas(),
                 self.sdf.toPandas(),
             )
             mock_session_init.assert_called_with(
-                self=ANY, accountant=ANY, public_sources={}, compiler=ANY
+                self=ANY, accountant=ANY, public_sources={}
             )
 
     @pytest.mark.parametrize(
         "budget,relation,expected_metric,expected_output_measure",
         [
             pytest.param(
                 PureDPBudget(float("inf")),
@@ -583,124 +561,33 @@
         assert sess._accountant.output_measure == expected_output_measure
         # pylint: enable=protected-access
 
     def test_add_public_dataframe(self):
         """Tests that :func:`add_public_dataframe` works correctly."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics.session.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = self.sdf_input_domain
             mock_accountant.d_in = {NamedTable("private"): ExactNumber(1)}
-            mock_compiler.output_measure = PureDP()
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
             session.add_public_dataframe(source_id="public", dataframe=self.join_df)
             assert "public" in session.public_source_dataframes
             assert_frame_equal_with_sort(
                 session.public_source_dataframes["public"].toPandas(),
                 self.join_df.toPandas(),
             )
             expected_schema = self.join_df.schema
             actual_schema = session.public_source_dataframes["public"].schema
             assert actual_schema == expected_schema
 
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
-    def test_create_view(self, d_in):
-        """Creating views without caching works."""
-        with patch.object(
-            QueryExprCompiler, "build_transformation", autospec=True
-        ) as mock_compiler_transform, patch(
-            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant",
-            autospec=True,
-        ) as mock_accountant:
-            mock_accountant.output_measure = PureDP()
-            # Use RootSumOfSquared since SymmetricDifference
-            # doesn't allow non-ints. Wrap
-            # that in IfGroupedBy since RootSumOfSquared on its own is not valid in many
-            # places in the framework.
-            mock_accountant.input_metric = DictMetric(
-                {
-                    NamedTable("private"): IfGroupedBy(
-                        "A", RootSumOfSquared(SymmetricDifference())
-                    )
-                }
-            )
-            mock_accountant.input_domain = self.sdf_input_domain
-            mock_accountant.d_in = {NamedTable("private"): ExactNumber(d_in)}
-            view_transformation = create_mock_transformation(
-                input_domain=self.sdf_input_domain,
-                input_metric=DictMetric(
-                    {
-                        NamedTable("private"): IfGroupedBy(
-                            "A", RootSumOfSquared(SymmetricDifference())
-                        )
-                    }
-                ),
-                output_domain=self.sdf_input_domain,
-                output_metric=DictMetric(
-                    {
-                        NamedTable("private"): IfGroupedBy(
-                            "A", RootSumOfSquared(SymmetricDifference())
-                        )
-                    }
-                ),
-                stability_function_implemented=True,
-                stability_function_return_value=ExactNumber(13),
-            )
-            mock_compiler_transform.return_value = (
-                view_transformation,
-                TableReference(path=[NamedTable("private")]),
-                [],
-            )
-            session = Session(accountant=mock_accountant, public_sources={})
-            session.create_view(
-                query_expr=PrivateSource("private"),
-                source_id="identity_transformation",
-                cache=False,
-            )
-
-            mock_compiler_transform.assert_called_with(
-                self=ANY,
-                query=PrivateSource("private"),
-                input_domain=mock_accountant.input_domain,
-                input_metric=mock_accountant.input_metric,
-                public_sources={},
-                catalog=ANY,
-                table_constraints=ANY,
-            )
-
-    @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
-    def test_evaluate_puredp_session(self, spark, d_in):
-        """Tests that :func:`evaluate` calls the right things given a puredp session."""
-        with patch.object(
-            QueryExprCompiler, "__call__", autospec=True
-        ) as mock_compiler, patch(
-            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant:
-            self._setup_accountant_and_compiler(
-                spark, d_in, mock_accountant, mock_compiler
-            )
-            mock_accountant.privacy_budget = ExactNumber(10)
-            session = Session(accountant=mock_accountant, public_sources={})
-            answer = session.evaluate(
-                query_expr=PrivateSource("private"), privacy_budget=PureDPBudget(10)
-            )
-            self._assert_test_evaluate_correctness(
-                session, mock_accountant, mock_compiler, PureDPBudget(10)
-            )
-            check_type("answer", answer, DataFrame)
-
-    @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_puredp_session_approxdp_query(self, spark, d_in):
         """Confirm that using an approxdp query on a puredp accountant raises an
         error."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
@@ -718,14 +605,15 @@
                 ),
             ):
                 session.evaluate(
                     query_expr=PrivateSource("private"),
                     privacy_budget=ApproxDPBudget(10, 0.5),
                 )
 
+    # Checks that every privacy budget type has an error with zero budget.
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_with_zero_budget(self, spark, d_in):
         """Confirm that calling evaluate with a 'budget' of 0 fails."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
@@ -750,14 +638,26 @@
                 ValueError,
                 match="You need a non-zero privacy budget to evaluate a query.",
             ):
                 session.evaluate(
                     query_expr=PrivateSource("private"), privacy_budget=RhoZCDPBudget(0)
                 )
 
+            # set output measures to ApproxDP
+            mock_accountant.output_measure = ApproxDP()
+            mock_compiler.output_measure = ApproxDP()
+            with pytest.raises(
+                ValueError,
+                match="You need a non-zero privacy budget to evaluate a query.",
+            ):
+                session.evaluate(
+                    query_expr=PrivateSource("private"),
+                    privacy_budget=ApproxDPBudget(0, 0),
+                )
+
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_zcdp_session_puredp_query(self, spark, d_in):
         """Confirm that using a puredp query on a zcdp accountant raises an error."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
@@ -802,38 +702,14 @@
                 ),
             ):
                 session.evaluate(
                     query_expr=PrivateSource("private"),
                     privacy_budget=RhoZCDPBudget(10),
                 )
 
-    @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
-    def test_evaluate_zcdp_session(self, spark, d_in):
-        """Tests that :func:`evaluate` calls the right things given a zcdp session."""
-        with patch.object(
-            QueryExprCompiler, "__call__", autospec=True
-        ) as mock_compiler, patch(
-            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant:
-            self._setup_accountant_and_compiler(
-                spark, d_in, mock_accountant, mock_compiler
-            )
-            mock_accountant.privacy_budget = ExactNumber(5)
-            # Set the output measures manually
-            mock_accountant.output_measure = RhoZCDP()
-            mock_compiler.output_measure = RhoZCDP()
-            session = Session(accountant=mock_accountant, public_sources={})
-            answer = session.evaluate(
-                query_expr=PrivateSource("private"), privacy_budget=RhoZCDPBudget(5)
-            )
-            self._assert_test_evaluate_correctness(
-                session, mock_accountant, mock_compiler, RhoZCDPBudget(5)
-            )
-            check_type("answer", answer, DataFrame)
-
     def _setup_accountant(
         self, mock_accountant, d_in=None, privacy_budget=None
     ) -> None:
         """Initialize only a mock accountant."""
         mock_accountant.output_measure = PureDP()
         mock_accountant.input_metric = DictMetric(
             {NamedTable("private"): SymmetricDifference()}
@@ -903,72 +779,44 @@
         # containing 1 empty dataframe
         mock_accountant.measure.return_value = [
             spark.createDataFrame(spark.sparkContext.emptyRDD(), StructType([]))
         ]
         mock_compiler.output_measure = PureDP()
         mock_compiler.return_value = Mock(spec_set=Measurement)
 
-    def _assert_test_evaluate_correctness(
-        self, session, mock_accountant, mock_compiler, privacy_budget
-    ):
-        """Confirm that :func:`evaluate` worked correctly."""
-        assert "private" in session.private_sources
-        assert session.get_schema("private") == self.sdf_col_types
-
-        mock_compiler.assert_called_with(
-            self=ANY,
-            queries=[PrivateSource("private")],
-            stability=mock_accountant.d_in,
-            input_domain=mock_accountant.input_domain,
-            input_metric=mock_accountant.input_metric,
-            privacy_budget=privacy_budget,
-            public_sources={},
-            catalog=ANY,
-            table_constraints={t: [] for t in mock_accountant.d_in.keys()},
-        )
-
-        mock_accountant.measure.assert_called_with(
-            mock_compiler.return_value, d_out=privacy_budget.value
-        )
-
     def test_partition_and_create(self):
         """Tests that :func:`partition_and_create` calls the right things."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant(mock_accountant, privacy_budget=ExactNumber(10))
+            input_spark_domain = self.sdf_input_domain.key_to_domain[
+                NamedTable("private")
+            ]
             mock_accountant.split.return_value = [
                 Mock(
                     spec_set=PrivacyAccountant,
-                    input_metric=DictMetric({"part0": SymmetricDifference()}),
-                    input_domain=self.sdf_input_domain,
+                    input_metric=DictMetric(
+                        {NamedTable("part0"): SymmetricDifference()}
+                    ),
+                    input_domain=DictDomain({NamedTable("part0"): input_spark_domain}),
                     output_measure=PureDP(),
                 ),
                 Mock(
                     spec_set=PrivacyAccountant,
-                    input_metric=DictMetric({"part1": SymmetricDifference()}),
-                    input_domain=self.sdf_input_domain,
+                    input_metric=DictMetric(
+                        {NamedTable("part1"): SymmetricDifference()}
+                    ),
+                    input_domain=DictDomain({NamedTable("part1"): input_spark_domain}),
                     output_measure=PureDP(),
                 ),
             ]
 
             session = Session(accountant=mock_accountant, public_sources={})
 
-        # Test that you need to provide splits
-        with pytest.raises(
-            ValueError,
-            match=re.escape(
-                "You must provide a dictionary mapping split names (new source_ids) to"
-                " values on which to partition"
-            ),
-        ):
-            session.partition_and_create(
-                source_id="private", privacy_budget=PureDPBudget(10), column="A"
-            )
-
         new_sessions = session.partition_and_create(
             source_id="private",
             privacy_budget=PureDPBudget(10),
             column="A",
             splits={"part0": "0", "part1": "1"},
         )
 
@@ -1000,44 +848,185 @@
         "protected_change",
         [
             (AddMaxRowsInMaxGroups("B", max_groups=1, max_rows_per_group=1)),
             (AddOneRow()),
         ],
     )
     @pytest.mark.parametrize(
-        "columns,expected_df",
+        "columns,expected_df,privacy_budget,possible_df",
         [
-            (["count"], pd.DataFrame({"count": [0]})),
-            (["B"], pd.DataFrame({"B": [0, 1]})),
-            (["count", "B"], pd.DataFrame({"count": [0, 0], "B": [0, 1]})),
-            ([], pd.DataFrame({"count": [0, 0], "B": [0, 1]})),
-            (None, pd.DataFrame({"count": [0, 0], "B": [0, 1]})),
+            # Tests without infinite privacy budget
+            # Note: The count of records with [0,0] and [0,1] is large enough that they
+            # should almost always appear in the output; [1,3] shouldn't appear.
+            (
+                ["count"],
+                pd.DataFrame({"count": [0]}),
+                ApproxDPBudget(1, 1e-5),
+                pd.DataFrame({"count": [0, 1]}),
+            ),
+            (
+                ["B"],
+                pd.DataFrame({"B": [0, 1]}),
+                ApproxDPBudget(1, 1e-5),
+                pd.DataFrame({"B": [0, 1, 3]}),
+            ),
+            (
+                ["count", "B"],
+                pd.DataFrame({"count": [0, 0], "B": [0, 1]}),
+                ApproxDPBudget(1, 1e-5),
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+            ),
+            (
+                [],
+                pd.DataFrame({"count": [0, 0], "B": [0, 1]}),
+                ApproxDPBudget(1, 1e-5),
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+            ),
+            (
+                None,
+                pd.DataFrame({"count": [0, 0], "B": [0, 1]}),
+                ApproxDPBudget(1, 1e-5),
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+            ),
+            # Tests with infinite privacy budget
+            # Note: If either the epsilon is infinite or the delta is 1, the output
+            # budget is infinite. Exact results should be returned.
+            (
+                ["count"],
+                pd.DataFrame({"count": [0, 1]}),
+                ApproxDPBudget(float("inf"), 1e-5),
+                None,
+            ),
+            (["count"], pd.DataFrame({"count": [0, 1]}), ApproxDPBudget(1e-5, 1), None),
+            (
+                ["B"],
+                pd.DataFrame({"B": [0, 1, 3]}),
+                ApproxDPBudget(float("inf"), 1),
+                None,
+            ),
+            (["B"], pd.DataFrame({"B": [0, 1, 3]}), ApproxDPBudget(1e-5, 1), None),
+            (
+                ["count", "B"],
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+                ApproxDPBudget(float("inf"), 1),
+                None,
+            ),
+            (
+                ["count", "B"],
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+                ApproxDPBudget(1e-5, 1),
+                None,
+            ),
+            (
+                [],
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+                ApproxDPBudget(float("inf"), 1),
+                None,
+            ),
+            (
+                [],
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+                ApproxDPBudget(1e-5, 1),
+                None,
+            ),
+            (
+                None,
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+                ApproxDPBudget(float("inf"), 1),
+                None,
+            ),
+            (
+                None,
+                pd.DataFrame({"count": [0, 0, 1], "B": [0, 1, 3]}),
+                ApproxDPBudget(1e-5, 1),
+                None,
+            ),
         ],
     )
     def test_get_groups_with_various_protected_change(
-        self, spark, protected_change, columns: List[str], expected_df: pd.DataFrame
+        self,
+        spark,
+        protected_change,
+        columns: List[str],
+        expected_df: pd.DataFrame,
+        privacy_budget: PrivacyBudget,
+        possible_df: Union[pd.DataFrame, None],
     ):
         """GetGroups works with AddMaxRowsInMaxGroups and AddOneRow protected change."""
         sdf = spark.createDataFrame(
             pd.DataFrame(
                 [[0, 0] for _ in range(10000)]
                 + [[0, 1] for _ in range(10000)]
                 + [[1, 3]],
                 columns=["count", "B"],
             )
         )
+
         session = Session.from_dataframe(
-            privacy_budget=ApproxDPBudget(1, 1e-5),
+            privacy_budget=privacy_budget,
             source_id="private",
             dataframe=sdf,
             protected_change=protected_change,
         )
         query = QueryBuilder("private").get_groups(columns)
         actual_sdf = session.evaluate(query, session.remaining_privacy_budget)
-        assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
+
+        try:
+            assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
+        except AssertionError:
+            # Deals with the case where the DFs mismatched due to noise.
+            assert_frame_equal_with_sort(actual_sdf.toPandas(), possible_df)
+
+    @pytest.mark.parametrize(
+        "protected_change",
+        [
+            (AddMaxRowsInMaxGroups("B", max_groups=1, max_rows_per_group=1)),
+            (AddOneRow()),
+        ],
+    )
+    @pytest.mark.parametrize(
+        "privacy_budget",
+        [
+            # Large Alpha, Low Epsilon
+            ApproxDPBudget(1e-5, 0.99999),
+            # Large Epsilon, Low Alpha
+            ApproxDPBudget(10000, 0.01),
+            # Large Epsilon, Large Alpha
+            ApproxDPBudget(10000, 0.99999),
+        ],
+    )
+    def test_get_groups_with_high_budget(
+        self,
+        spark,
+        protected_change,
+        privacy_budget: PrivacyBudget,
+    ):
+        """Smoke test for GetGroups with large but not infinite budgets."""
+        # This test is required because there was a bug where get_groups would return
+        # an empty dataframe when the budget was large but not infinite.
+        sdf = spark.createDataFrame(
+            pd.DataFrame(
+                [[0, 0] for _ in range(10000)]
+                + [[0, 1] for _ in range(10000)]
+                + [[1, 3]],
+                columns=["count", "B"],
+            )
+        )
+
+        session = Session.from_dataframe(
+            privacy_budget=privacy_budget,
+            source_id="private",
+            dataframe=sdf,
+            protected_change=protected_change,
+        )
+        query = QueryBuilder("private").get_groups()
+        actual_sdf = session.evaluate(query, session.remaining_privacy_budget)
+
+        # Checks that the result is non-empty
+        assert len(actual_sdf.toPandas()) > 0
 
     def test_get_groups_with_add_rows_with_id(self, spark):
         """GetGroups with AddRowsWithID protected change works on non-ID column."""
         sdf = spark.createDataFrame(
             pd.DataFrame([[0, i] for i in range(10000)], columns=["count", "B"])
         )
         session = Session.from_dataframe(
@@ -1047,35 +1036,74 @@
             protected_change=AddRowsWithID("B"),
         )
         query = QueryBuilder("private").enforce(MaxRowsPerID(1)).get_groups(["count"])
         expected_df = pd.DataFrame({"count": [0]})
         actual_sdf = session.evaluate(query, session.remaining_privacy_budget)
         assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
 
-    @pytest.mark.parametrize("columns", [(["B"]), (["count", "B"]), ([]), (None)])
+    @pytest.mark.parametrize("columns", [(["B"]), (["count", "B"])])
     def test_get_groups_on_id_column(self, spark, columns: List[str]):
         """Test that the GetGroups on ID column errors."""
         sdf = spark.createDataFrame(
             pd.DataFrame([[0, i] for i in range(10000)], columns=["count", "B"])
         )
         session = Session.from_dataframe(
             privacy_budget=ApproxDPBudget(1, 1e-5),
             source_id="private",
             dataframe=sdf,
             protected_change=AddRowsWithID("B"),
         )
+        match_str = re.escape(
+            "get_groups cannot be used on the privacy ID column"
+            " (B) of a table with the AddRowsWithID protected change."
+        )
         with pytest.raises(
             RuntimeError,
-            match="^GetGroups is not supported on ID column provided in AddRowsWithID",
+            match=match_str,
         ):
             session.evaluate(
                 QueryBuilder("private").enforce(MaxRowsPerID(1)).get_groups(columns),
                 session.remaining_privacy_budget,
             )
 
+    @pytest.mark.parametrize(
+        "test_df,id_column,expected_columns",
+        [
+            (pd.DataFrame({"ID": [1, 2, 3], "VAR": [4, 5, 6]}), "ID", ["VAR"]),
+            (
+                pd.DataFrame(
+                    {
+                        "CUST_ID": [1, 2, 3],
+                        "VARONE": [4, 5, 6],
+                        "VARTWO": ["A", "B", "C"],
+                    }
+                ),
+                "CUST_ID",
+                ["VARONE", "VARTWO"],
+            ),
+        ],
+    )
+    def test_get_groups_defaults_to_non_id_columns(
+        self, spark, test_df: pd.DataFrame, id_column: str, expected_columns: List[str]
+    ):
+        """Tests that get_groups applies to all non-ID cols if no cols are provided."""
+        sdf = spark.createDataFrame(test_df)
+        session = Session.from_dataframe(
+            privacy_budget=ApproxDPBudget(1, 1e-5),
+            source_id="private",
+            dataframe=sdf,
+            protected_change=AddRowsWithID(id_column),
+        )
+
+        get_groups_query = QueryBuilder("private").enforce(MaxRowsPerID(1)).get_groups()
+
+        end_df = session.evaluate(get_groups_query, session.remaining_privacy_budget)
+
+        assert set(expected_columns) == set(end_df.columns)
+
     def test_describe(self, spark):
         """Test that :func:`_describe` works correctly."""
         with patch("builtins.print") as mock_print, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant(mock_accountant, privacy_budget=ExactNumber(10))
             mock_accountant.state = PrivacyAccountantState.ACTIVE
@@ -1506,15 +1534,15 @@
                     " performed"
                 ),
             ):
                 session.partition_and_create(
                     "private",
                     privacy_budget=PureDPBudget(1),
                     column="A",
-                    splits={"part0": 0, "part1": 1},
+                    splits={"part0": "0", "part1": "1"},
                 )
 
 
 @pytest.fixture(name="test_data_invalid", scope="class")
 def setup_invalid_session_data(spark, request) -> None:
     """Set up test data for invalid session tests."""
     pdf = pd.DataFrame(
@@ -1561,27 +1589,14 @@
             {NamedTable("private"): SymmetricDifference()}
         )
         mock_accountant.input_domain = DictDomain(
             {NamedTable("private"): self.sdf_input_domain}
         )
         mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
 
-    def test_invalid_compiler_initialization(self):
-        """session errors if compiler is not a QueryExprCompiler."""
-        with patch(
-            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant:
-            with pytest.raises(
-                TypeError,
-                match=r"type of compiler must be one of "
-                r"\(QueryExprCompiler, NoneType\); got list instead",
-            ):
-                self._setup_accountant(mock_accountant)
-                Session(mock_accountant, public_sources={}, compiler=[])  # type: ignore
-
     def test_invalid_dataframe_initialization(self):
         """session raises error on invalid dataframe type"""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             # Private
             with pytest.raises(
@@ -1694,47 +1709,28 @@
         ):
             Session.from_dataframe(
                 PureDPBudget(1),
                 "private",
                 self.sdf,
                 protected_change=AddMaxRowsInMaxGroups("not_a_column", 1, 1),
             )
-        with pytest.raises(
-            ValueError,
-            match=(
-                "^Grouping column 'not_a_column' does not exist in the input. Available"
-                " columns: A, B, X$"
-            ),
-        ):
-            Session.from_dataframe(
-                PureDPBudget(1), "private", self.sdf, grouping_column="not_a_column"
-            )
 
         float_df = spark.createDataFrame(pd.DataFrame({"A": [1, 2], "F": [0.1, 0.2]}))
         with pytest.raises(
             ValueError,
             match=(
                 "^Grouping column 'F' is not of a type on which grouping is supported.*"
             ),
         ):
             Session.from_dataframe(
                 PureDPBudget(1),
                 "private",
                 float_df,
                 protected_change=AddMaxRowsInMaxGroups("F", 1, 1),
             )
-        with pytest.raises(
-            ValueError,
-            match=(
-                "^Grouping column 'F' is not of a type on which grouping is supported.*"
-            ),
-        ):
-            Session.from_dataframe(
-                PureDPBudget(1), "private", float_df, grouping_column="F"
-            )
 
     def test_invalid_key_column(self) -> None:
         """Builder raises an error if table's key column is not in dataframe."""
         with pytest.raises(
             ValueError,
             match=(
                 "^Key column 'not_a_column' does not exist in the input. Available"
@@ -1748,75 +1744,71 @@
                 protected_change=AddRowsWithID("not_a_column", "random_id"),
             )
 
     @pytest.mark.parametrize(
         "source_id,exception_type,expected_error_msg",
         [
             (2, TypeError, 'type of argument "source_id" must be str; got int instead'),
-            ("@str", ValueError, "source_id must be a valid Python identifier."),
+            (
+                "@str",
+                ValueError,
+                "Names must be valid Python identifiers: they can only contain "
+                "alphanumeric characters and underscores, and cannot begin with a "
+                "number.",
+            ),
         ],
     )
     def test_invalid_source_id(
         self, source_id: str, exception_type: Type[Exception], expected_error_msg: str
     ):
         """session raises error on invalid source_id."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
 
             #### from spark dataframe ####
             # Private
             with pytest.raises(exception_type, match=expected_error_msg):
                 Session.from_dataframe(
                     privacy_budget=PureDPBudget(1),
                     source_id=source_id,
                     dataframe=self.sdf,
                     protected_change=AddOneRow(),
                 )
             # Public
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(exception_type, match=expected_error_msg):
                 session.add_public_dataframe(source_id, dataframe=self.sdf)
             # create_view
             with pytest.raises(exception_type, match=expected_error_msg):
                 session.create_view(PrivateSource("private"), source_id, cache=False)
 
     def test_invalid_public_source(self):
         """Session raises an error adding a public source with duplicate source_id."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
 
-            session = Session(
-                accountant=mock_accountant, compiler=mock_compiler, public_sources={}
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
 
             # This should work
             session.add_public_dataframe("public_df", dataframe=self.sdf)
 
             # But this should not
             with pytest.raises(
                 ValueError, match="This session already has a table named 'public_df'."
@@ -1826,31 +1818,26 @@
     @pytest.mark.parametrize(
         "query_expr", [(["filter private A == 0"]), ([PrivateSource("private")])]
     )
     def test_invalid_queries_evaluate(self, query_expr: Any):
         """evaluate raises error on invalid queries."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
 
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(
                 TypeError,
                 match=(
                     "type of query_expr must be tmlt.analytics.query_expr.QueryExpr;"
                     " got list instead"
                 ),
             ):
@@ -1872,115 +1859,82 @@
         query_expr: QueryExpr,
         exception_type: Type[Exception],
         expected_error_msg: str,
     ):
         """create functions raise error on invalid input queries."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
 
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(exception_type, match=expected_error_msg):
                 session.create_view(query_expr, source_id="view", cache=True)
 
     def test_invalid_column(self):
         """Tests that invalid column name for column errors."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
-
-            mock_compiler.build_transformation.return_value = (
-                Mock(
-                    spec_set=Transformation,
-                    output_domain=self.sdf_input_domain,
-                    output_metric=SymmetricDifference(),
-                ),
-                sp.Integer(1),
-            )
 
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
 
             expected_schema = spark_schema_to_analytics_columns(self.sdf.schema)
             # We expect a transformation that will disallow NaNs on floats and infs
             expected_schema["X"].allow_nan = False
             expected_schema["X"].allow_inf = False
 
             with pytest.raises(
                 KeyError,
                 match=re.escape(
-                    "'T' not present in transformed dataframe's columns; "
-                    "schema of transformed dataframe is "
+                    "'T' not present in transformed DataFrame's columns; "
+                    "schema of transformed DataFrame is "
                     f"{expected_schema}"
                 ),
             ):
                 session.partition_and_create(
                     "private",
                     privacy_budget=PureDPBudget(1),
                     column="T",
                     splits={"private0": "0", "private1": "1"},
                 )
 
     def test_invalid_splits_name(self):
         """Tests that invalid splits name errors."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
 
-            mock_compiler.build_transformation.return_value = (
-                Mock(
-                    spec_set=Transformation,
-                    output_domain=self.sdf_input_domain,
-                    output_metric=SymmetricDifference(),
-                ),
-                sp.Integer(1),
-            )
-
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
 
             with pytest.raises(
                 ValueError,
                 match=(
                     "The string passed as split name must be a valid Python identifier"
                 ),
             ):
@@ -1991,40 +1945,26 @@
                     splits={" ": 0, "space present": 1, "2startsWithNumber": 2},
                 )
 
     def test_splits_value_type(self):
         """Tests error when given invalid splits value type on partition."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
-        ) as mock_accountant, patch(
-            "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
-        ) as mock_compiler:
+        ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
-            mock_compiler.output_measure = PureDP()
-
-            mock_compiler.build_transformation.return_value = (
-                Mock(
-                    spec_set=Transformation,
-                    output_domain=self.sdf_input_domain,
-                    output_metric=SymmetricDifference(),
-                ),
-                sp.Integer(1),
-            )
 
-            session = Session(
-                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
-            )
+            session = Session(accountant=mock_accountant, public_sources={})
 
             with pytest.raises(
                 TypeError,
                 match=(
                     r"'A' column is of type 'StringType\(?\)?'; 'StringType\(?\)?' "
                     "column not compatible with splits value type 'int'"
                 ),
@@ -2105,96 +2045,54 @@
     dataframes: Dict[str, DataFrame]
 
     @pytest.mark.parametrize(
         "builder,error_msg",
         [
             (
                 Session.Builder(),
-                "Privacy budget must be specified.",
+                "This builder must have a privacy budget set",
             ),  # No Privacy Budget
             (
                 Session.Builder().with_privacy_budget(PureDPBudget(10)),
-                "At least one private source must be provided.",
+                "At least one private dataframe must be specified",
             ),  # No Private Sources
         ],
     )
     def test_invalid_build(self, builder: Session.Builder, error_msg: str):
         """Tests that builds raise relevant errors when builder is not configured."""
         with pytest.raises(ValueError, match=error_msg):
             builder.build()
 
-    def test_invalid_stability(self):
-        """Tests that private source cannot be added with an invalid stability."""
-        with pytest.raises(ValueError, match="Stability must be a positive integer"):
-            Session.Builder().with_private_dataframe(
-                source_id="df1", dataframe=self.dataframes["df1"], stability=0
-            )
-        with pytest.raises(ValueError, match="Stability must be a positive integer"):
-            Session.Builder().with_private_dataframe(
-                source_id="df1", dataframe=self.dataframes["df1"], stability=-1
-            )
-
-    @pytest.mark.parametrize(
-        "stability,grouping_column,error_msg",
-        [
-            (None, None, "Using a default for protected_change is deprecated"),
-            (
-                None,
-                "A",
-                "Providing a grouping_column parameter instead of a"
-                " protected_change parameter is deprecated",
-            ),
-            (
-                1,
-                None,
-                "Providing a stability instead of a protected_change is deprecated",
-            ),
-            (
-                1,
-                "A",
-                "Providing a grouping_column parameter instead of a"
-                " protected_change parameter is deprecated",
-            ),
-        ],
-    )
-    def test_stability_deprecation(
-        self, stability: Optional[int], grouping_column: Optional[str], error_msg: str
-    ):
-        """Test that stability and grouping_column give deprecation warnings."""
-        with pytest.warns(DeprecationWarning, match=error_msg):
-            Session.Builder().with_private_dataframe(
-                source_id="df1",
-                dataframe=self.dataframes["df1"],
-                stability=stability,
-                grouping_column=grouping_column,
-            )
-
     @pytest.mark.parametrize("initial_budget", [(PureDPBudget(1)), (RhoZCDPBudget(1))])
     def test_invalid_to_add_budget_twice(self, initial_budget: PrivacyBudget):
         """Test that you can't call ``with_privacy_budget()`` twice."""
         builder = Session.Builder().with_privacy_budget(initial_budget)
         with pytest.raises(
-            ValueError, match="This Builder already has a privacy budget"
+            ValueError, match="This builder already has a privacy budget set"
         ):
             builder.with_privacy_budget(PureDPBudget(1))
         with pytest.raises(
-            ValueError, match="This Builder already has a privacy budget"
+            ValueError, match="This builder already has a privacy budget set"
         ):
             builder.with_privacy_budget(RhoZCDPBudget(1))
 
     def test_duplicate_source_id(self):
         """Tests that a repeated source id raises appropriate error."""
         builder = Session.Builder().with_private_dataframe(
-            source_id="A", dataframe=self.dataframes["df1"], stability=1
+            source_id="A",
+            dataframe=self.dataframes["df1"],
+            protected_change=AddOneRow(),
         )
-        with pytest.raises(ValueError, match="Duplicate source id: 'A'"):
+        with pytest.raises(ValueError, match="Table 'A' already exists"):
             builder.with_private_dataframe(
-                source_id="A", dataframe=self.dataframes["df2"], stability=2
+                source_id="A",
+                dataframe=self.dataframes["df2"],
+                protected_change=AddOneRow(),
             )
-        with pytest.raises(ValueError, match="Duplicate source id: 'A'"):
+        with pytest.raises(ValueError, match="Table 'A' already exists"):
             builder.with_public_dataframe(
                 source_id="A", dataframe=self.dataframes["df2"]
             )
 
     def test_build_invalid_identifier(self):
         """Tests that build fails if protected change does
         not have associated ID space."""
@@ -2226,15 +2124,15 @@
                 "An AddRowsWithID protected change was specified without an "
                 "associated identifier space"
             ),
         ):
             builder.build()
         ### build should succeed when the identifier space is added
         builder = builder.with_id_space("random_id")
-        with pytest.raises(ValueError, match="This Builder already has an ID space"):
+        with pytest.raises(ValueError, match="ID space 'random_id' already exists"):
             builder.with_id_space("random_id")
         assert len(builder._id_spaces) == 2  # pylint: disable=protected-access
         builder.build()
 
     def test_build_multiple_ids(self):
         """Tests that build succeeds with multiple ID spaces."""
         builder = (
@@ -2348,44 +2246,41 @@
 
         public_sources = session._public_sources
         assert public_sources.keys() == expected_public_sources.keys()
         for key in public_sources:
             assert_frame_equal_with_sort(
                 public_sources[key].toPandas(), expected_public_sources[key].toPandas()
             )
-
-        compiler = session._compiler
-        # pylint: enable=protected-access
-        assert isinstance(compiler, QueryExprCompiler)
-        assert compiler.output_measure == expected_output_measure
+        assert session._output_measure == expected_output_measure
 
     @pytest.mark.parametrize("nullable", [(True), (False)])
     def test_builder_with_dataframe_keep_nullable_status(self, spark, nullable: bool):
         """with_dataframe methods use the nullable status of the dataframe."""
         builder = Session.Builder()
         builder = builder.with_private_dataframe(
             source_id="private_df",
             dataframe=spark.createDataFrame(
                 [(1,)],
                 schema=StructType([StructField("A", LongType(), nullable=nullable)]),
             ),
+            protected_change=AddOneRow(),
         )
         builder = builder.with_public_dataframe(
             source_id="public_df",
             dataframe=spark.createDataFrame(
                 [(1,)],
                 schema=StructType([StructField("A", LongType(), nullable=nullable)]),
             ),
         )
         actual_private_schema = (
-            builder._private_sources[  # pylint: disable=protected-access
+            builder._private_dataframes[  # pylint: disable=protected-access
                 "private_df"
             ].dataframe.schema
         )
         actual_public_schema = (
-            builder._public_sources[  # pylint: disable=protected-access
+            builder._public_dataframes[  # pylint: disable=protected-access
                 "public_df"
             ].schema
         )
         expected_schema = StructType([StructField("A", LongType(), nullable=nullable)])
         assert actual_private_schema == expected_schema
         assert actual_public_schema == expected_schema
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_table_identifiers.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_table_identifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for table identifier types."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import pytest
 
 from tmlt.analytics._table_identifier import NamedTable, TableCollection, TemporaryTable
 from tmlt.analytics._table_reference import TableReference
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_transformation_utils.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_transformation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for transofrmation utils."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_truncation_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for TruncationStrategy."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import pytest
 
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
 
 @pytest.mark.parametrize("threshold", [(1), (8)])
```

### Comparing `tmlt_analytics-0.8.3/test/unit/test_utils.py` & `tmlt_analytics-0.9.0rc5/test/unit/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for :mod:`~tmlt.analytics.utils`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 from tmlt.analytics.utils import check_installation
 
 
 ### Test for tmlt.analytics.utils.check_installation()
 # We want the `spark` argument here so that the test will use the
 # (session-wide, pytest-provided) spark session.
 def test_check_installation(spark) -> None:  # pylint: disable=unused-argument
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_catalog.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Contains classes for specifying schemas and constraints for tables."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from abc import ABC
 from dataclasses import dataclass
 from typing import Dict, Mapping, Optional, Union
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_coerce_spark_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Logic for coercing Spark dataframes into forms usable by Tumult Analytics."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from typing import Dict
 
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import (
     DataType,
     DateType,
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_neighboring_relation.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Module containing supported variants of neighboring relations."""
 # pylint: disable=protected-access, no-self-use
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql.types import DateType, IntegerType, LongType, StringType
@@ -79,15 +81,15 @@
 
     def _validate(self, dfs: Dict[str, DataFrame]) -> List[str]:
         """Private validation checks.
 
         These are the validation checks to be done
         in any case, i.e. regardless of if the relation is top-level.
         """
-        # validation checks that can be called by other relations. this
+        # validation checks that can be called by other relations. This
         # just verifies that the initialized table is in the dfs input,
         # and that it points to a dataframe object in the Dict.
         coerce_spark_schema_or_fail(dfs[self.table])
         if self.table not in dfs.keys():
             raise ValueError(
                 f"""The provided input doesn't contain the relation table
                 Input table names: {dfs.keys()}
@@ -112,25 +114,25 @@
     """The name of the table in this relation."""
     grouping_column: str
     """The column that must be grouped over for the privacy guarantee to hold."""
     max_groups: int
     """The maximum number of groups which may differ for two instances of the table
      to be neighbors.
     """
-    per_group: Union[int, float]
+    per_group: int
     """The max number of rows in any single group that may differ for two instances of
      the table to be neighbors.
      """
 
     def __post_init__(self) -> None:
         """Checks arguments to constructor."""
         check_type("table", self.table, str)
         check_type("grouping_column", self.grouping_column, str)
         check_type("max_groups", self.max_groups, int)
-        check_type("per_group", self.per_group, (int, float))
+        check_type("per_group", self.per_group, int)
 
     def validate_input(self, dfs: Dict[str, DataFrame]) -> bool:
         """Does nothing if input is valid, otherwise raises an informative exception.
 
         Used only for top-level validation.
         """
         # checks to be done in any case: the table is in the relation,
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module to define NeighboringRelationVisitors."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import dataclasses
 from typing import Any, Dict, NamedTuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
 from tmlt.core.domains.base import Domain
@@ -115,31 +115,23 @@
         domain = SparkDataFrameDomain.from_spark_schema(data.schema)
         return self.Output(domain, metric, distance, data)
 
     def visit_add_remove_rows_across_groups(
         self, relation: AddRemoveRowsAcrossGroups
     ) -> Output:
         """Build Core state from ``AddRemoveRowsAcrossGroups`` neighboring relation."""
-        # This is needed because it's currently allowed to pass float-valued
-        # stabilities in the per_group parameter (for backwards compatibility).
-        # TODO(#2272): Remove this.
-        per_group = (
-            sp.Rational(relation.per_group)
-            if isinstance(relation.per_group, float)
-            else relation.per_group
-        )
         agg_metric: Union[RootSumOfSquared, SumOf]
         if isinstance(self.output_measure, RhoZCDP):
             agg_metric = RootSumOfSquared(SymmetricDifference())
             distance = ExactNumber(
-                per_group * ExactNumber(sp.sqrt(relation.max_groups))
+                relation.per_group * ExactNumber(sp.sqrt(relation.max_groups))
             )
         elif isinstance(self.output_measure, (PureDP, ApproxDP)):
             agg_metric = SumOf(SymmetricDifference())
-            distance = ExactNumber(per_group * relation.max_groups)
+            distance = ExactNumber(relation.per_group * relation.max_groups)
         else:
             raise TypeError(
                 f"The provided output measure {self.output_measure} for this visitor is"
                 " not supported."
             )
 
         metric = IfGroupedBy(relation.grouping_column, agg_metric)
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_noise_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,55 @@
 """Get noise scale from a Measurement."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from copy import deepcopy
 from enum import Enum
 from functools import singledispatch
-from typing import Any, Dict, List, Set, Tuple, Union
+from typing import Any, Dict, Iterable, List, Set, Tuple, Union
 
 from pyspark.sql import DataFrame
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.noise_mechanisms import (
     AddDiscreteGaussianNoise,
     AddGaussianNoise,
     AddGeometricNoise,
     AddLaplaceNoise,
 )
 from tmlt.core.measurements.pandas_measurements.series import NoisyQuantile
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber
 
 
+class NoiseInfo:
+    """Container for noise information."""
+
+    def __init__(self, noise_info: List[Dict[str, Any]]):
+        """Constructor."""
+        self._noise_info = noise_info
+
+    def __getitem__(self, n: int) -> Dict[str, Any]:
+        """Get the nth noise info."""
+        return self._noise_info[n]
+
+    def __iter__(self) -> Iterable[Dict[str, Any]]:
+        """Iterate over noise info."""
+        return iter(self._noise_info)
+
+    def __repr__(self) -> str:
+        """Return a string representation of this object."""
+        return f"NoiseInfo({self._noise_info})"
+
+    def __eq__(self, other: Any) -> bool:
+        """Check if this object is equal to another object."""
+        if not isinstance(other, NoiseInfo):
+            return NotImplemented
+        return list(iter(self)) == list(iter(other))
+
+
 class _NoiseMechanism(Enum):
     LAPLACE = 1
     GEOMETRIC = 2
     DISCRETE_GAUSSIAN = 3
     EXPONENTIAL = 4
     GAUSSIAN = 5
 
@@ -89,28 +117,28 @@
 @_get_info.register(set)
 def _(s: Set) -> Set:
     return set(_get_info(e) for e in s)
 
 
 @_get_info.register(DataFrame)
 def _(df: DataFrame) -> str:
-    # Deepcopying dataframes doesn't work
+    # Deep-copying dataframes doesn't work
     # (If you try, you'll see an error about being unable to
     # pickle threads.)
     # for now, just report that there was a DataFrame here
     return f"<a Spark DataFrame with columns: {df.columns}>"
 
 
-def _noise_from_measurement(m: Measurement) -> List[Dict[str, Any]]:
+def _noise_from_measurement(m: Measurement) -> NoiseInfo:
     """Get noise information from a measurement.
 
     Each dictionary will look like:
     {"noise_mechanism": _NoiseMechanism.LAPLACE, "noise_parameter": 1}
     """
-    return _noise_from_info(_get_info(m))
+    return NoiseInfo(_noise_from_info(_get_info(m)))
 
 
 def _inverse_cdf(noise_info: Dict[str, Any], p: float) -> float:
     """Get the inverse cdf of a measurement at a probability.
 
     Args:
         noise_info: A dictionary of the type returned by _noise_from_measurement.
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_privacy_budget_rounding_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Helper functions for dealing with budget floating point imprecision."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import sympy as sp
 from tmlt.core.utils.exact_number import ExactNumber
 from typeguard import typechecked
 
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
@@ -105,7 +105,29 @@
     # pylint: enable=protected-access
     else:
         raise ValueError(
             "Unable to compute a privacy budget with the requested budget "
             f"of {requested_privacy_budget} and a remaining budget of "
             f"{remaining_privacy_budget}."
         )
+
+
+@typechecked
+def get_infinite_budget(privacy_budget: PrivacyBudget) -> PrivacyBudget:
+    """Creates a privacy budget with infinite epsilon/rho and 0 delta.
+
+    Args:
+        privacy_budget: The privacy budget to use as a template.
+    """
+    if isinstance(privacy_budget, PureDPBudget):
+        return PureDPBudget(ExactNumber.from_float(float("inf"), round_up=False))
+
+    elif isinstance(privacy_budget, ApproxDPBudget):
+        return ApproxDPBudget(ExactNumber.from_float(float("inf"), round_up=False), 0)
+
+    elif isinstance(privacy_budget, RhoZCDPBudget):
+        return RhoZCDPBudget(ExactNumber.from_float(float("inf"), round_up=False))
+    else:
+        raise ValueError(
+            "Unable to return an infinite version of budget with the input budget "
+            f"of {privacy_budget}."
+        )
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Defines :class:`QueryExprCompiler` for building transformations from query exprs."""
 # TODO(#746): Check for UnaryExpr.
 # TODO(#1044): Put the PureDPToZCDP converter directly on Vector measurements.
 # TODO(#1547): Associate metric with output measure instead of algorithm for
 #              adding noise.
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from typing import Any, Dict, List, Sequence, Tuple, Union
 
 from pyspark.sql import DataFrame
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.measurements.aggregations import NoiseMechanism as CoreNoiseMechanism
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.composition import Composition
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
 from tmlt.core.metrics import DictMetric
 from tmlt.core.transformations.base import Transformation
 
 from tmlt.analytics._catalog import Catalog
+from tmlt.analytics._noise_info import NoiseInfo
 from tmlt.analytics._query_expr_compiler._measurement_visitor import MeasurementVisitor
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
 )
@@ -122,16 +123,16 @@
         privacy_budget: PrivacyBudget,
         stability: Any,
         input_domain: DictDomain,
         input_metric: DictMetric,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
         table_constraints: Dict[Identifier, List[Constraint]],
-    ) -> Measurement:
-        """Returns a compiled DP measurement.
+    ) -> Tuple[Measurement, NoiseInfo]:
+        """Returns a compiled DP measurement and its noise information.
 
         Args:
             queries: Queries representing measurements to compile.
             privacy_budget: The total privacy budget for answering the queries.
             stability: The stability of the input to compiled query.
             input_domain: The input domain of the compiled query.
             input_metric: The input metric of the compiled query.
@@ -153,18 +154,19 @@
             default_mechanism=self._mechanism,
             public_sources=public_sources,
             catalog=catalog,
             table_constraints=table_constraints,
         )
 
         measurements: List[Measurement] = []
+        noise_infos: List[NoiseInfo] = []
         # Note: Each query is re-using the adjusted_budget from the same visitor, which
         # could become a problem if we go back to supporting multiple queries.
         for query in queries:
-            query_measurement = query.accept(visitor)
+            query_measurement, noise_info = query.accept(visitor)
             if not isinstance(query_measurement, Measurement):
                 raise AssertionError(
                     "This query did not create a measurement. "
                     "This is probably a bug; please let us know so we can fix it!"
                 )
 
             if isinstance(visitor.adjusted_budget.value, tuple):
@@ -185,16 +187,19 @@
             if privacy_function_budget_mismatch:
                 raise AssertionError(
                     "Query measurement privacy function does not match "
                     "privacy budget value. This is probably a bug; "
                     "please let us know so we can fix it!"
                 )
             measurements.append(query_measurement)
+            noise_infos.append(noise_info)
 
         measurement = Composition(measurements)
+        assert len(noise_infos) == 1
+        noise_info = noise_infos[0]
 
         if isinstance(visitor.adjusted_budget.value, tuple):
             # TODO(#2754): add a log message.
             privacy_function_budget_mismatch = any(
                 x > y
                 for x, y in zip(
                     measurement.privacy_function(stability),
@@ -208,15 +213,15 @@
 
         if privacy_function_budget_mismatch:
             raise AssertionError(
                 "Measurement privacy function does not match "
                 "privacy budget. This is probably a bug; "
                 "please let us know so we can fix it!"
             )
-        return measurement
+        return measurement, noise_info
 
     def build_transformation(
         self,
         query: QueryExpr,
         input_domain: DictDomain,
         input_metric: DictMetric,
         public_sources: Dict[str, DataFrame],
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Defines a visitor for propagating constraints through transformations."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
-from typing import List, Optional, Set, Union
+from typing import List, Optional, Set, Union, cast
 
+import pandas as pd
 from pyspark.sql import DataFrame
 
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
@@ -192,21 +193,24 @@
 def propagate_join_public(
     join_cols: Set[str],
     overlapping_cols: Set[str],
     public_df: DataFrame,
     constraints: List[Constraint],
 ) -> List[Constraint]:
     """Propagate a list of constraints through a JoinPublic transformation."""
-    join_stability = max(
+    count_df = cast(
+        pd.DataFrame,
         public_df.select(*join_cols)
         .groupby(*join_cols)
         .count()
         .select("count")
-        .toPandas()["count"]
-        .to_list(),
+        .toPandas(),
+    )
+    join_stability = max(
+        count_df["count"].to_list(),
         default=0,
     )
     propagated = [
         _propagate_join_by_stability(
             c, join_stability, overlapping_cols, suffix="_left"
         )
         for c in constraints
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_measurement_visitor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,119 @@
-"""Defines a visitor for creating noisy measurements from query expressions."""
-
-# SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
-
+"""Defines a base class for building measurement visitors."""
 import dataclasses
 import math
 import warnings
-from typing import Any, Dict, List, Optional, Tuple, Union
+from abc import abstractmethod
+from datetime import datetime
+from decimal import Decimal
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import sympy as sp
-from pyspark.sql import DataFrame
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import (
-    SparkColumnDescriptor,
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-    SparkIntegerColumnDescriptor,
+from pyspark.sql import DataFrame, SparkSession
+
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
+from pyspark.sql.types import (
+    BooleanType,
+    ByteType,
+    DateType,
+    DecimalType,
+    DoubleType,
+    FloatType,
+    IntegerType,
+    LongType,
+    ShortType,
+    StringType,
+    StructType,
+    TimestampType,
 )
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.measurements.aggregations import (
     NoiseMechanism,
     create_average_measurement,
     create_count_distinct_measurement,
     create_count_measurement,
-    create_partition_selection_measurement,
     create_quantile_measurement,
     create_standard_deviation_measurement,
     create_sum_measurement,
     create_variance_measurement,
 )
 from tmlt.core.measurements.base import Measurement
-from tmlt.core.measurements.postprocess import PostProcess
+from tmlt.core.measurements.interactive_measurements import (
+    MeasurementQuery,
+    Queryable,
+    SequentialComposition,
+    create_adaptive_composition,
+)
+from tmlt.core.measurements.postprocess import NonInteractivePostProcess
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
 from tmlt.core.metrics import (
     DictMetric,
     HammingDistance,
     IfGroupedBy,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.converters import UnwrapIfGroupedBy
 from tmlt.core.transformations.spark_transformations.groupby import GroupBy
 from tmlt.core.transformations.spark_transformations.select import (
     Select as SelectTransformation,
 )
 from tmlt.core.utils.exact_number import ExactNumber
-from tmlt.core.utils.misc import get_nonconflicting_string
 
 from tmlt.analytics._catalog import Catalog
+from tmlt.analytics._noise_info import NoiseInfo, _noise_from_measurement
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
-from tmlt.analytics._query_expr_compiler._transformation_visitor import (
-    TransformationVisitor,
-)
-from tmlt.analytics._schema import (
-    ColumnType,
-    Schema,
-    analytics_to_spark_columns_descriptor,
-)
+from tmlt.analytics._schema import ColumnType, Schema
 from tmlt.analytics._table_identifier import Identifier
 from tmlt.analytics._table_reference import TableReference
 from tmlt.analytics._transformation_utils import get_table_from_ref
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
 )
 from tmlt.analytics.keyset import KeySet
-from tmlt.analytics.privacy_budget import ApproxDPBudget, PrivacyBudget
+from tmlt.analytics.privacy_budget import (
+    ApproxDPBudget,
+    PrivacyBudget,
+    PureDPBudget,
+    RhoZCDPBudget,
+)
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
-    DropNullAndNan,
-    EnforceConstraint,
+)
+from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
+from tmlt.analytics.query_expr import DropNullAndNan, EnforceConstraint
+from tmlt.analytics.query_expr import Filter as FilterExpr
+from tmlt.analytics.query_expr import FlatMap as FlatMapExpr
+from tmlt.analytics.query_expr import (
     GetGroups,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
     GroupByCountDistinct,
     GroupByQuantile,
-    QueryExpr,
-    QueryExprVisitor,
-    ReplaceInfinity,
-    StdevMechanism,
-    SumMechanism,
-    VarianceMechanism,
 )
+from tmlt.analytics.query_expr import JoinPrivate as JoinPrivateExpr
+from tmlt.analytics.query_expr import JoinPublic as JoinPublicExpr
+from tmlt.analytics.query_expr import Map as MapExpr
+from tmlt.analytics.query_expr import PrivateSource as PrivateSourceExpr
+from tmlt.analytics.query_expr import QueryExpr, QueryExprVisitor
+from tmlt.analytics.query_expr import Rename as RenameExpr
+from tmlt.analytics.query_expr import ReplaceInfinity, ReplaceNullAndNan
+from tmlt.analytics.query_expr import Select as SelectExpr
+from tmlt.analytics.query_expr import StdevMechanism, SumMechanism, VarianceMechanism
 
 
 def _get_query_bounds(
     query: Union[
         GroupByBoundedAverage,
         GroupByBoundedSTDEV,
         GroupByBoundedSum,
@@ -230,15 +250,15 @@
             groupby_keys=query.groupby_keys,
             output_column=query.output_column,
             mechanism=mechanism,
         )
     elif len(groupby_columns) == 1:
         # A groupby on exactly one column is performed; if that column has a
         # MaxGroupsPerID constraint, then this is equivalent to a
-        # MaxRowsPerGroupsPerID(grouping_column, 1) constraint.
+        # MaxRowsPerGroupPerID(grouping_column, 1) constraint.
         grouping_column = groupby_columns[0]
         constraint = next(
             (
                 c
                 for c in constraints
                 if isinstance(c, MaxGroupsPerID)
                 and c.grouping_column == grouping_column
@@ -255,15 +275,47 @@
                 mechanism=mechanism,
             )
 
     # If none of the above cases are true, no optimization is possible.
     return None
 
 
-class MeasurementVisitor(QueryExprVisitor):
+def _create_single_row_df_with_spark_schema(schema: StructType) -> DataFrame:
+    """Create a single-row DataFrame with the given schema."""
+    spark = SparkSession.builder.getOrCreate()
+    default_values = []
+    for field in schema.fields:
+        default_value: Any
+        if isinstance(field.dataType, (ByteType, ShortType, IntegerType, LongType)):
+            default_value = 0
+        elif isinstance(field.dataType, (FloatType, DoubleType)):
+            default_value = 0.0
+        elif isinstance(field.dataType, StringType):
+            default_value = ""
+        elif isinstance(field.dataType, BooleanType):
+            default_value = False
+        elif isinstance(field.dataType, DateType):
+            default_value = datetime.strptime("1970-01-01", "%Y-%m-%d").date()
+        elif isinstance(field.dataType, TimestampType):
+            default_value = datetime.strptime(
+                "1970-01-01 00:00:00", "%Y-%m-%d %H:%M:%S"
+            )
+        elif isinstance(field.dataType, DecimalType):
+            default_value = Decimal("0.0")
+        else:
+            raise ValueError(f"Unsupported data type {field.dataType}")
+        default_values.append(default_value)
+
+    # Create a DataFrame with a single row using the default values
+    df = spark.createDataFrame([tuple(default_values)], schema=schema)
+    assert df.schema == schema
+    return df
+
+
+class BaseMeasurementVisitor(QueryExprVisitor):
     """A visitor to create a measurement from a query expression."""
 
     def __init__(
         self,
         privacy_budget: PrivacyBudget,
         stability: Any,
         input_domain: DictDomain,
@@ -282,30 +334,158 @@
         self.input_metric = input_metric
         self.default_mechanism = default_mechanism
         self.public_sources = public_sources
         self.output_measure = output_measure
         self.catalog = catalog
         self.table_constraints = table_constraints
 
+    def _get_zero_budget(self) -> PrivacyBudget:
+        """Return a budget with zero epsilon and zero delta."""
+        if isinstance(self.budget, PureDPBudget):
+            return PureDPBudget(0)
+        if isinstance(self.budget, ApproxDPBudget):
+            return ApproxDPBudget(0, 0)
+        if isinstance(self.budget, RhoZCDPBudget):
+            return RhoZCDPBudget(0)
+        raise AssertionError(
+            f"Unknown budget type {type(self.budget)}. This is probably a bug; "
+            "please let us know about it so we can fix it!"
+        )
+
+    @staticmethod
+    def _build_groupby(
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        mechanism: NoiseMechanism,
+        keyset: KeySet,
+    ) -> GroupBy:
+        """Build a groupby transformation."""
+        # TODO(#1044 and #1547): Update condition to when issue is resolved.
+        # isinstance(self._output_measure, RhoZCDP)
+        use_l2 = mechanism in (
+            NoiseMechanism.DISCRETE_GAUSSIAN,
+            NoiseMechanism.GAUSSIAN,
+        )
+        return GroupBy(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            use_l2=use_l2,
+            group_keys=keyset.dataframe(),
+        )
+
+    def _build_adaptive_groupby_agg_and_noise_info(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        stability: Any,
+        mechanism: NoiseMechanism,
+        columns: List[str],
+        keyset: Optional[KeySet],
+        build_groupby_agg_from_groupby: Callable[[GroupBy, PrivacyBudget], Measurement],
+        keyset_budget: PrivacyBudget,
+        agg_budget: PrivacyBudget,
+    ) -> Tuple[Measurement, NoiseInfo]:
+        """Builds a measurement which gets a keyset and performs a groupby aggregation.
+
+        Args:
+            input_domain: The domain of the input data.
+            input_metric: The metric of the input data.
+            stability: The stability of the transformation.
+            mechanism: The noise mechanism to use for the aggregation. This is used
+                to determine whether to use L1/L2 for the groupby transformation.
+            columns: The columns to get the keyset for.
+            keyset: The KeySet to use, if using a public keyset. Must match
+                `columns`.
+            build_groupby_agg_from_groupby: A function that builds a groupby aggregation
+                from a groupby. The resulting measurement should satisfy
+                `measurement.privacy_relation(stability, agg_budget.value)`.
+            keyset_budget: The budget to use for the keyset measurement.
+            agg_budget: The budget to use for the aggregation measurement.
+
+        Returns:
+            A tuple of the groupby aggregation measurement and the noise info.
+        """
+        assert keyset is not None  # TODO: parameter is for implicit partition selection
+        assert keyset.dataframe().columns == columns
+
+        def perform_groupby_agg(
+            queryable: Queryable,
+        ):
+            measurement_keyset = queryable(
+                MeasurementQuery(
+                    self._build_get_keyset_measurement(
+                        input_domain=input_domain,
+                        input_metric=input_metric,
+                        stability=stability,
+                        budget=keyset_budget,
+                        columns=columns,
+                        keyset=keyset,
+                    )
+                )
+            )
+            groupby = self._build_groupby(
+                input_domain, input_metric, mechanism, measurement_keyset
+            )
+            agg = build_groupby_agg_from_groupby(groupby, agg_budget)
+            return queryable(MeasurementQuery(agg))
+
+        groupby_agg = NonInteractivePostProcess(
+            create_adaptive_composition(
+                input_domain=input_domain,
+                input_metric=input_metric,
+                d_in=stability,
+                privacy_budget=self.adjusted_budget.value,
+                output_measure=self.output_measure,
+            ),
+            perform_groupby_agg,
+        )
+        # Now calculate noise info, it needs to have the same privacy analysis as the
+        # groupby_agg measurement without being adaptive.
+        # The key assumption is that a keyset with 1 arbitrary row will have the same
+        # privacy analysis as the adaptively selected keyset.
+        groupby_schema = StructType(
+            [
+                struct_field
+                for struct_field in input_domain.spark_schema
+                if struct_field.name in columns
+            ]
+        )
+        one_row_keyset = KeySet.from_dataframe(
+            _create_single_row_df_with_spark_schema(groupby_schema)
+        )
+        groupby_one_row_keyset = self._build_groupby(
+            input_domain, input_metric, mechanism, one_row_keyset
+        )
+        groupby_agg_one_row_keyset = build_groupby_agg_from_groupby(
+            groupby_one_row_keyset, agg_budget
+        )
+        noise_info = _noise_from_measurement(groupby_agg_one_row_keyset)
+        return groupby_agg, noise_info
+
+    @abstractmethod
     def _visit_child_transformation(
         self, expr: QueryExpr, mechanism: NoiseMechanism
     ) -> Tuple[Transformation, TableReference, List[Constraint]]:
-        """Visit a child transformation, producing a transformation."""
-        tv = TransformationVisitor(
-            input_domain=self.input_domain,
-            input_metric=self.input_metric,
-            mechanism=mechanism,
-            public_sources=self.public_sources,
-            table_constraints=self.table_constraints,
-        )
-        child, reference, constraints = expr.accept(tv)
+        pass
 
-        tv.validate_transformation(expr, child, reference, self.catalog)
+    @abstractmethod
+    def _handle_enforce(
+        self,
+        constraint: Constraint,
+        child_transformation: Transformation,
+        child_ref: TableReference,
+        **kwargs,
+    ) -> Tuple[Transformation, TableReference]:
+        """Append the constraint to the end of the transformation.
+
+        This is a helper method for :meth:`~._truncate_table`.
 
-        return child, reference, constraints
+        It is pulled out to make it easier to override in subclasses which change the
+        behavior of constraints, not for code maintainability.
+        """
 
     def _truncate_table(
         self,
         transformation: Transformation,
         reference: TableReference,
         constraints: List[Constraint],
         grouping_columns: List[str],
@@ -330,31 +510,30 @@
 
             for c in truncatable_constraints[0]:
                 assert isinstance(
                     c, (MaxRowsPerID, MaxGroupsPerID, MaxRowsPerGroupPerID)
                 )
                 if isinstance(c, MaxGroupsPerID):
                     # Taking advantage of the L2 noise behavior only works for
-                    # RhoZCDP Sessions, and then only when the grouping column
+                    # Sessions initialized with a RhoZCDP privacy budget,
+                    # and then only when the grouping column
                     # of the constraints is being grouped on.
                     use_l2 = (
                         isinstance(self.output_measure, RhoZCDP)
                         and c.grouping_column in grouping_columns
                     )
-                    # pylint: disable=protected-access
-                    transformation, reference = c._enforce(
-                        transformation, reference, update_metric=True, use_l2=use_l2
+                    transformation, reference = self._handle_enforce(
+                        c, transformation, reference, update_metric=True, use_l2=use_l2
                     )
-                    # pylint: enable=protected-access
                 else:
                     (
                         transformation,
                         reference,
-                    ) = c._enforce(  # pylint: disable=protected-access
-                        transformation, reference, update_metric=True
+                    ) = self._handle_enforce(
+                        c, transformation, reference, update_metric=True
                     )
             return transformation, reference
 
         else:
             # Tables without IDs don't need truncation
             return transformation, reference
 
@@ -400,84 +579,91 @@
         expr: Union[
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
             GroupByCount,
             GroupByCountDistinct,
+            GroupByQuantile,
         ],
     ) -> None:
         """Validate and set adjusted_budget for ApproxDP queries.
 
         First, validate that the user is not using a Gaussian noise mechanism with
         ApproxDP. Then, for queries that use noise addition mechanisms replace non-zero
         deltas with zero in self.adjusted_budget. If the user chose this mechanism
         (i.e. didn't use the DEFAULT mechanism) we warn them of this replacement.
         """
         if not isinstance(self.budget, ApproxDPBudget):
             return
 
-        if expr.mechanism in (
+        mechanism: Any = getattr(expr, "mechanism", None)
+        if mechanism in (
             AverageMechanism.GAUSSIAN,
             CountDistinctMechanism.GAUSSIAN,
             CountMechanism.GAUSSIAN,
             StdevMechanism.GAUSSIAN,
             SumMechanism.GAUSSIAN,
             VarianceMechanism.GAUSSIAN,
         ):
             raise NotImplementedError(
-                "Gaussian noise is only supported with RhoZCDP. Please use "
+                "Gaussian noise is only supported with a RhoZCDPBudget. Please use "
                 "CountMechanism.LAPLACE instead."
             )
 
         epsilon, delta = self.budget.value
         if delta != 0:
-            if expr.mechanism in (
+            if mechanism in (
                 AverageMechanism.LAPLACE,
                 CountDistinctMechanism.LAPLACE,
                 CountMechanism.LAPLACE,
                 StdevMechanism.LAPLACE,
                 SumMechanism.LAPLACE,
                 VarianceMechanism.LAPLACE,
             ):
                 warnings.warn(
                     "When using LAPLACE with an ApproxDPBudget, the delta value of "
                     "the budget will be replaced with zero."
                 )
                 self.adjusted_budget = ApproxDPBudget(epsilon, 0)
-            elif expr.mechanism in (
+            elif mechanism in (
                 AverageMechanism.DEFAULT,
                 CountDistinctMechanism.DEFAULT,
                 CountMechanism.DEFAULT,
                 StdevMechanism.DEFAULT,
                 SumMechanism.DEFAULT,
                 VarianceMechanism.DEFAULT,
             ):
                 self.adjusted_budget = ApproxDPBudget(epsilon, 0)
+            elif mechanism is None:
+                # Quantile has no mechanism
+                self.adjusted_budget = ApproxDPBudget(epsilon, 0)
             else:
                 raise AssertionError(
-                    f"Unknown mechanism {expr.mechanism}. This is probably a bug; "
+                    f"Unknown mechanism {mechanism}. This is probably a bug; "
                     "please let us know so we can fix it!"
                 )
 
     def _pick_noise_for_non_count(
         self,
         query: Union[
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
         ],
-        measure_column_type: SparkColumnDescriptor,
     ) -> NoiseMechanism:
         """Pick the noise mechanism for non-count queries.
 
         GroupByQuantile only supports one noise mechanism, so it is not
         included here.
         """
+        measure_column_type = query.child.accept(OutputSchemaVisitor(self.catalog))[
+            query.measure_column
+        ].column_type
         requested_mechanism: NoiseMechanism
         if query.mechanism in (
             SumMechanism.DEFAULT,
             AverageMechanism.DEFAULT,
             VarianceMechanism.DEFAULT,
             StdevMechanism.DEFAULT,
         ):
@@ -504,17 +690,17 @@
             raise ValueError(
                 f"Did not recognize requested mechanism {query.mechanism}."
                 " Supported mechanisms are DEFAULT, LAPLACE,  and GAUSSIAN."
             )
 
         # If the query requested a Laplace measure ...
         if requested_mechanism == NoiseMechanism.LAPLACE:
-            if isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+            if measure_column_type == ColumnType.INTEGER:
                 return NoiseMechanism.GEOMETRIC
-            elif isinstance(measure_column_type, SparkFloatColumnDescriptor):
+            elif measure_column_type == ColumnType.DECIMAL:
                 return NoiseMechanism.LAPLACE
             else:
                 raise AssertionError(
                     "Query's measure column should be numeric. This should"
                     " not happen and is probably a bug;  please let us know"
                     " so we can fix it!"
                 )
@@ -522,17 +708,17 @@
         # If the query requested a Gaussian measure...
         elif requested_mechanism == NoiseMechanism.GAUSSIAN:
             if isinstance(self.output_measure, PureDP):
                 raise ValueError(
                     "Gaussian noise is not supported under PureDP. "
                     "Please use RhoZCDP or another measure."
                 )
-            if isinstance(measure_column_type, SparkFloatColumnDescriptor):
+            if measure_column_type == ColumnType.DECIMAL:
                 return NoiseMechanism.GAUSSIAN
-            elif isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+            elif measure_column_type == ColumnType.INTEGER:
                 return NoiseMechanism.DISCRETE_GAUSSIAN
             else:
                 raise AssertionError(
                     "Query's measure column should be numeric. This should"
                     " not happen and is probably a bug;  please let us know"
                     " so we can fix it!"
                 )
@@ -541,143 +727,65 @@
         # GAUSSIAN, so something has gone awry
         else:
             raise AssertionError(
                 f"Did not recognize requested mechanism {requested_mechanism}."
                 " This is probably a bug; please let us know about it so we can fix it!"
             )
 
-    @staticmethod
-    def _build_groupby(
-        input_domain: SparkDataFrameDomain,
-        input_metric: Union[HammingDistance, SymmetricDifference, IfGroupedBy],
-        groupby_keys: KeySet,
-        mechanism: NoiseMechanism,
-    ) -> GroupBy:
-        """Build a groupby query from the parameters provided.
-
-        This groupby query will run after the provided Transformation.
-        """
-        # TODO(#1044 and #1547): Update condition to when issue is resolved.
-        # isinstance(self._output_measure, RhoZCDP)
-        use_l2 = mechanism in (
-            NoiseMechanism.DISCRETE_GAUSSIAN,
-            NoiseMechanism.GAUSSIAN,
-        )
-
-        groupby_df: DataFrame = groupby_keys.dataframe()
-
-        return GroupBy(
-            input_domain=input_domain,
-            input_metric=input_metric,
-            use_l2=use_l2,
-            group_keys=groupby_df,
-        )
-
-    @dataclasses.dataclass
-    class _AggInfo:
-        """All the information you need for some query exprs.
-
-        Supported types:
-        - GroupByBoundedAverage
-        - GroupByBoundedSTDEV
-        - GroupByBoundedSum
-        - GroupByBoundedVariance
-        """
-
-        mechanism: NoiseMechanism
-        transformation: Transformation
-        mid_stability: sp.Expr
-        groupby: GroupBy
-        lower_bound: ExactNumber
-        upper_bound: ExactNumber
-
-    def _build_common(
+    def _add_special_value_handling_to_query(
         self,
         query: Union[
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
+            GroupByQuantile,
         ],
-    ) -> _AggInfo:
-        """Everything you need to build a measurement for these query types.
+    ):
+        """Returns a new query that handles nulls, NaNs and infinite values.
 
-        This function also checks to see if the measure_column allows
-        invalid values (nulls, NaNs, and infinite values), and adds
-        DropNullAndNan and/or DropInfinity queries to remove them if they are present.
-        """
-        lower_bound, upper_bound = _get_query_bounds(query)
+        If the measure column allows nulls or NaNs, the new query
+        will drop those values.
+
+        If the measure column allows infinite values, the new query will replace those
+        values with the low and high values specified in the query.
 
+        These changes are added immediately before the groupby aggregation in the query.
+        """
         expected_schema = query.child.accept(OutputSchemaVisitor(self.catalog))
 
         # You can't perform these queries on nulls, NaNs, or infinite values
         # so check for those
         try:
             measure_desc = expected_schema[query.measure_column]
         except KeyError as e:
             raise KeyError(
                 f"Measure column {query.measure_column} is not in the input schema."
             ) from e
 
-        new_child: Optional[QueryExpr] = None
+        new_child: QueryExpr
         # If null or NaN values are allowed ...
         if measure_desc.allow_null or (
             measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_nan
         ):
             # then drop those values
             # (but don't mutate the original query)
             new_child = DropNullAndNan(
                 child=query.child, columns=[query.measure_column]
             )
             query = dataclasses.replace(query, child=new_child)
-            expected_schema = query.child.accept(OutputSchemaVisitor(self.catalog))
-
         # If infinite values are allowed...
         if measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_inf:
             # then clamp them (to low/high values)
             new_child = ReplaceInfinity(
                 child=query.child,
                 replace_with={query.measure_column: (query.low, query.high)},
             )
             query = dataclasses.replace(query, child=new_child)
-            expected_schema = query.child.accept(OutputSchemaVisitor(self.catalog))
-
-        expected_output_domain = SparkDataFrameDomain(
-            analytics_to_spark_columns_descriptor(expected_schema)
-        )
-        measure_column_type = expected_output_domain[query.measure_column]
-
-        mechanism = self._pick_noise_for_non_count(query, measure_column_type)
-        child_transformation, table_ref = self._truncate_table(
-            *self._visit_child_transformation(query.child, mechanism),
-            grouping_columns=query.groupby_keys.dataframe().columns,
-        )
-        transformation = get_table_from_ref(child_transformation, table_ref)
-        # _visit_child_transformation already raises an error if these aren't true
-        # these assert statements are just here for MyPy's benefit
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
-        mid_stability = transformation.stability_function(self.stability)
-        groupby = self._build_groupby(
-            transformation.output_domain,
-            transformation.output_metric,
-            query.groupby_keys,
-            mechanism,
-        )
-        return MeasurementVisitor._AggInfo(
-            mechanism=mechanism,
-            transformation=transformation,
-            mid_stability=mid_stability,
-            groupby=groupby,
-            lower_bound=lower_bound,
-            upper_bound=upper_bound,
-        )
+        return query
 
     def _validate_measurement(self, measurement: Measurement, mid_stability: sp.Expr):
         """Validate a measurement."""
         if isinstance(self.adjusted_budget.value, tuple):
             # TODO(#2754): add a log message.
             privacy_function_budget_mismatch = any(
                 x > y
@@ -696,451 +804,715 @@
         if privacy_function_budget_mismatch:
             raise AssertionError(
                 "Privacy function does not match per-query privacy budget. "
                 "This is probably a bug; please let us know so we can "
                 "fix it!"
             )
 
-    def visit_get_groups(self, expr: GetGroups) -> Measurement:
-        """Create a measurement from a GetGroups query expression."""
-        if not isinstance(self.budget, ApproxDPBudget):
-            raise ValueError("GetGroups is only supported with ApproxDPBudgets.")
+    # these don't produce measurements, so they return an error
+    def visit_private_source(self, expr: PrivateSourceExpr) -> Any:
+        """Visit a PrivateSource query expression (raises an error)."""
+        raise NotImplementedError
 
-        # Peek at the schema, to see if there are errors there
-        expr.accept(OutputSchemaVisitor(self.catalog))
+    def visit_rename(self, expr: RenameExpr) -> Any:
+        """Visit a Rename query expression (raises an error)."""
+        raise NotImplementedError
 
-        schema = expr.child.accept(OutputSchemaVisitor(self.catalog))
-        # Check if ID column is one of the columns in get_groups
-        # Note: if get_groups columns is None or empty, all of the columns in the table
-        # is used for partition selection, hence that needs to be checked as well
-        if schema.id_column and (
-            not expr.columns or (schema.id_column in expr.columns)
-        ):
-            raise RuntimeError(
-                "GetGroups is not supported on ID column provided in AddRowsWithID "
-                "protected change."
-            )
+    def visit_filter(self, expr: FilterExpr) -> Any:
+        """Visit a Filter query expression (raises an error)."""
+        raise NotImplementedError
 
-        child_transformation, child_ref = self._truncate_table(
-            *self._visit_child_transformation(expr.child, NoiseMechanism.GEOMETRIC),
-            grouping_columns=[],
-        )
+    def visit_select(self, expr: SelectExpr) -> Any:
+        """Visit a Select query expression (raises an error)."""
+        raise NotImplementedError
 
-        transformation = get_table_from_ref(child_transformation, child_ref)
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
+    def visit_map(self, expr: MapExpr) -> Any:
+        """Visit a Map query expression (raises an error)."""
+        raise NotImplementedError
 
-        # squares the sensitivity in zCDP, which is a worst-case analysis
-        # that we may be able to improve.
-        if isinstance(transformation.output_metric, IfGroupedBy):
-            transformation |= UnwrapIfGroupedBy(
-                transformation.output_domain, transformation.output_metric
-            )
+    def visit_flat_map(self, expr: FlatMapExpr) -> Any:
+        """Visit a FlatMap query expression (raises an error)."""
+        raise NotImplementedError
 
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
-        if expr.columns:
-            transformation |= SelectTransformation(
-                transformation.output_domain, transformation.output_metric, expr.columns
-            )
+    def visit_join_private(self, expr: JoinPrivateExpr) -> Any:
+        """Visit a JoinPrivate query expression (raises an error)."""
+        raise NotImplementedError
 
-        mid_stability = transformation.stability_function(self.stability)
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        count_column = "count"
-        if count_column in set(transformation.output_domain.schema):
-            count_column = get_nonconflicting_string(
-                list(transformation.output_domain.schema)
-            )
+    def visit_join_public(self, expr: JoinPublicExpr) -> Any:
+        """Visit a JoinPublic query expression (raises an error)."""
+        raise NotImplementedError
 
-        epsilon, delta = self.budget.value
-        agg = create_partition_selection_measurement(
-            input_domain=transformation.output_domain,
-            epsilon=epsilon,
-            delta=delta,
-            d_in=mid_stability,
-            count_column=count_column,
-        )
+    def visit_replace_null_and_nan(self, expr: ReplaceNullAndNan) -> Any:
+        """Visit a ReplaceNullAndNan query expression (raises an error)."""
+        raise NotImplementedError
 
-        self._validate_measurement(agg, mid_stability)
+    def visit_replace_infinity(self, expr: ReplaceInfinity) -> Any:
+        """Visit a ReplaceInfinity query expression (raises an error)."""
+        raise NotImplementedError
 
-        measurement = PostProcess(
-            transformation | agg, lambda result: result.drop(count_column)
+    def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Any:
+        """Visit a DropNullAndNan query expression (raises an error)."""
+        raise NotImplementedError
+
+    def visit_drop_infinity(self, expr: DropInfExpr) -> Any:
+        """Visit a DropInfinity query expression (raises an error)."""
+        raise NotImplementedError
+
+    def visit_enforce_constraint(self, expr: EnforceConstraint) -> Any:
+        """Visit a EnforceConstraint query expression (raises an error)."""
+        raise NotImplementedError
+
+    def visit_get_groups(self, expr: GetGroups) -> Any:
+        """Visit a GetGroups query expression (raises an error)."""
+        raise NotImplementedError
+
+    def _build_get_keyset_measurement(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        stability: ExactNumber,
+        budget: PrivacyBudget,
+        columns: List[str],
+        keyset: Optional[KeySet] = None,
+    ) -> Measurement:
+        """Build a Measurement that returns a KeySet.
+
+        Args:
+            input_domain: The domain of the input data.
+            input_metric: The metric of the input data.
+            stability: The input stability the measurement will be applied on.
+            budget: The privacy budget to use. Should be zero if using a public keyset.
+            columns: The columns to get the keyset for.
+            keyset: The KeySet to return, if using a public keyset. Must match
+                `columns`.
+        """
+        if keyset is None:
+            raise NotImplementedError()
+        assert columns == keyset.dataframe().columns
+        if isinstance(budget, PureDPBudget):
+            assert budget.epsilon == 0
+        elif isinstance(budget, ApproxDPBudget):
+            assert budget.epsilon == 0
+            assert budget.delta == 0
+        elif isinstance(budget, RhoZCDPBudget):
+            assert budget.rho == 0
+        else:
+            raise AssertionError(f"Unrecognized budget type {type(budget)}")
+        no_op = SequentialComposition(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            output_measure=self.output_measure,
+            d_in=stability,
+            privacy_budget=budget.value,
+        )
+        return NonInteractivePostProcess(no_op, lambda _: keyset)
+
+    def build_groupby_count(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        stability: Any,
+        mechanism: NoiseMechanism,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByCount query."""
+        return create_count_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            noise_mechanism=mechanism,
+            d_in=stability,
+            d_out=budget.value,
+            output_measure=self.output_measure,
+            groupby_transformation=groupby,
+            count_column=output_column,
         )
-        return measurement
 
-    def visit_groupby_count(self, expr: GroupByCount) -> Measurement:
+    def visit_groupby_count(self, expr: GroupByCount) -> Tuple[Measurement, NoiseInfo]:
         """Create a measurement from a GroupByCount query expression."""
         self._validate_approxDP_and_adjust_budget(expr)
 
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_count(expr)
+
         mechanism = self._pick_noise_for_count(expr)
         child_transformation, child_ref = self._truncate_table(
             *self._visit_child_transformation(expr.child, mechanism),
             grouping_columns=expr.groupby_keys.dataframe().columns,
         )
-
         transformation = get_table_from_ref(child_transformation, child_ref)
-        # _visit_child_transformation already raises an error if these aren't true
-        # these are just here for MyPy's benefit
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
             transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         mid_stability = transformation.stability_function(self.stability)
-        groupby = self._build_groupby(
-            transformation.output_domain,
-            transformation.output_metric,
-            expr.groupby_keys,
-            mechanism,
+
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByCount query."""
+            return self.build_groupby_count(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                stability=mid_stability,
+                mechanism=mechanism,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
+
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
         )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
 
-        agg = create_count_measurement(
-            input_domain=transformation.output_domain,
-            input_metric=transformation.output_metric,
+    def build_count_distinct_measurement(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        mechanism: NoiseMechanism,
+        stability: Any,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByCountDistinct query."""
+        return create_count_distinct_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
             noise_mechanism=mechanism,
-            d_in=mid_stability,
-            d_out=self.adjusted_budget.value,
+            d_in=stability,
+            d_out=budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
-            count_column=expr.output_column,
+            count_column=output_column,
         )
-        self._validate_measurement(agg, mid_stability)
-        return transformation | agg
 
-    def visit_groupby_count_distinct(self, expr: GroupByCountDistinct) -> Measurement:
+    def visit_groupby_count_distinct(
+        self, expr: GroupByCountDistinct
+    ) -> Tuple[Measurement, NoiseInfo]:
         """Create a measurement from a GroupByCountDistinct query expression."""
         self._validate_approxDP_and_adjust_budget(expr)
+
+        # Peek at the schema, to see if there are errors there
+        expr.accept(OutputSchemaVisitor(self.catalog))
+
         mechanism = self._pick_noise_for_count(expr)
         (
             child_transformation,
             child_ref,
             child_constraints,
         ) = self._visit_child_transformation(expr.child, mechanism)
         constrained_query = _generate_constrained_count_distinct(
             expr,
             expr.child.accept(OutputSchemaVisitor(self.catalog)),
             child_constraints,
         )
         if constrained_query is not None:
             return constrained_query.accept(self)
 
-        # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_count_distinct(expr)
-
         child_transformation, child_ref = self._truncate_table(
             child_transformation,
             child_ref,
             child_constraints,
             grouping_columns=expr.groupby_keys.dataframe().columns,
         )
         transformation = get_table_from_ref(child_transformation, child_ref)
 
-        # _visit_child_transformation already raises an error if these aren't true
-        # these are just here for MyPy's benefit
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
             transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         # If not counting all columns, drop the ones that are neither counted
         # nor grouped on.
         if expr.columns_to_count:
             groupby_columns = list(expr.groupby_keys.schema().keys())
             transformation |= SelectTransformation(
-                transformation.output_domain,
-                transformation.output_metric,
+                mid_domain,
+                mid_metric,
                 list(set(expr.columns_to_count + groupby_columns)),
             )
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
+            mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+            mid_metric = cast(
+                Union[IfGroupedBy, HammingDistance, SymmetricDifference],
+                transformation.output_metric,
+            )
 
         mid_stability = transformation.stability_function(self.stability)
-        groupby = self._build_groupby(
-            transformation.output_domain,
-            transformation.output_metric,
-            expr.groupby_keys,
-            mechanism,
+
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByCountDistinct query."""
+            return self.build_count_distinct_measurement(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                mechanism=mechanism,
+                stability=mid_stability,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
+
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
         )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
 
-        agg = create_count_distinct_measurement(
-            input_domain=transformation.output_domain,
-            input_metric=transformation.output_metric,
-            noise_mechanism=mechanism,
-            d_in=mid_stability,
-            d_out=self.adjusted_budget.value,
+    def build_groupby_quantile(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        measure_column: str,
+        quantile: float,
+        lower: Union[int, float],
+        upper: Union[int, float],
+        stability: Any,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByQuantile query."""
+        return create_quantile_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            measure_column=measure_column,
+            quantile=quantile,
+            lower=lower,
+            upper=upper,
+            d_in=stability,
+            d_out=budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
-            count_column=expr.output_column,
+            quantile_column=output_column,
         )
-        self._validate_measurement(agg, mid_stability)
-        return transformation | agg
-
-    def visit_groupby_quantile(self, expr: GroupByQuantile) -> Measurement:
-        """Create a measurement from a GroupByQuantile query expression.
 
-        This method also checks to see if the schema allows invalid values
-        (nulls, NaNs, and infinite values) on the measure column; if so,
-        the query has DropNullAndNan and/or DropInfinity queries
-        inserted immediately before it is executed.
-        """
-        child_schema: Schema = expr.child.accept(OutputSchemaVisitor(self.catalog))
-        # Check the measure column for nulls/NaNs/infs (which aren't allowed)
-        try:
-            measure_desc = child_schema[expr.measure_column]
-        except KeyError as e:
-            raise KeyError(
-                f"Measure column '{expr.measure_column}' is not in the input schema."
-            ) from e
-        # If null or NaN values are allowed ...
-        if measure_desc.allow_null or (
-            measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_nan
-        ):
-            # Those values aren't allowed! Drop them
-            # (without mutating the original QueryExpr)
-            drop_null_and_nan_query = DropNullAndNan(
-                child=expr.child, columns=[expr.measure_column]
-            )
-            expr = dataclasses.replace(expr, child=drop_null_and_nan_query)
-
-        # If infinite values are allowed ...
-        if measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_inf:
-            # Clamp those values
-            # (without mutating the original QueryExpr)
-            replace_infinity_query = ReplaceInfinity(
-                child=expr.child,
-                replace_with={expr.measure_column: (expr.low, expr.high)},
-            )
-            expr = dataclasses.replace(expr, child=replace_infinity_query)
+    def visit_groupby_quantile(
+        self, expr: GroupByQuantile
+    ) -> Tuple[Measurement, NoiseInfo]:
+        """Create a measurement from a GroupByQuantile query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+        expr = self._add_special_value_handling_to_query(expr)
 
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_quantile(expr)
+        expr.accept(OutputSchemaVisitor(self.catalog))
 
         child_transformation, child_ref = self._truncate_table(
             *self._visit_child_transformation(expr.child, self.default_mechanism),
             grouping_columns=expr.groupby_keys.dataframe().columns,
         )
         transformation = get_table_from_ref(child_transformation, child_ref)
-        # _visit_child_transformation already raises an error if these aren't true
-        # these are just here for MyPy's benefit
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
             transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         mid_stability = transformation.stability_function(self.stability)
-        groupby = self._build_groupby(
-            transformation.output_domain,
-            transformation.output_metric,
-            expr.groupby_keys,
-            self.default_mechanism,
+
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByQuantile query."""
+            return self.build_groupby_quantile(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                measure_column=expr.measure_column,
+                quantile=expr.quantile,
+                lower=expr.low,  # Uses floats, so doesn't use _get_query_bounds
+                upper=expr.high,
+                stability=mid_stability,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
+
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=self.default_mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
         )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
 
-        # For ApproxDP keep epsilon value, but always pass 0 for delta
-        self.adjusted_budget = (
-            ApproxDPBudget(self.budget.value[0], 0)
-            if isinstance(self.budget, ApproxDPBudget)
-            else self.budget
-        )
-
-        agg = create_quantile_measurement(
-            input_domain=transformation.output_domain,
-            input_metric=transformation.output_metric,
-            measure_column=expr.measure_column,
-            quantile=expr.quantile,
-            lower=expr.low,
-            upper=expr.high,
-            d_in=mid_stability,
-            d_out=self.adjusted_budget.value,
+    def build_groupby_bounded_sum(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        measure_column: str,
+        lower: ExactNumber,
+        upper: ExactNumber,
+        stability: Any,
+        mechanism: NoiseMechanism,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByBoundedSum query."""
+        return create_sum_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            measure_column=measure_column,
+            lower=lower,
+            upper=upper,
+            noise_mechanism=mechanism,
+            d_in=stability,
+            d_out=budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
-            quantile_column=expr.output_column,
+            sum_column=output_column,
         )
-        self._validate_measurement(agg, mid_stability)
-        return transformation | agg
 
-    def visit_groupby_bounded_sum(self, expr: GroupByBoundedSum) -> Measurement:
+    def visit_groupby_bounded_sum(
+        self, expr: GroupByBoundedSum
+    ) -> Tuple[Measurement, NoiseInfo]:
         """Create a measurement from a GroupByBoundedSum query expression."""
         self._validate_approxDP_and_adjust_budget(expr)
+        expr = self._add_special_value_handling_to_query(expr)
 
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_sum(expr)
+        expr.accept(OutputSchemaVisitor(self.catalog))
+
+        mechanism = self._pick_noise_for_non_count(expr)
+        lower, upper = _get_query_bounds(expr)
+
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(expr.child, mechanism),
+            grouping_columns=expr.groupby_keys.dataframe().columns,
+        )
+        transformation = get_table_from_ref(child_transformation, child_ref)
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
+            transformation.output_metric,
+        )
+        mid_stability = transformation.stability_function(self.stability)
 
-        info = self._build_common(expr)
-        # _build_common already checks these;
-        # these asserts are just for mypy's benefit
-        assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            info.transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
-
-        agg = create_sum_measurement(
-            input_domain=info.transformation.output_domain,
-            input_metric=info.transformation.output_metric,
-            measure_column=expr.measure_column,
-            lower=info.lower_bound,
-            upper=info.upper_bound,
-            noise_mechanism=info.mechanism,
-            d_in=info.mid_stability,
-            d_out=self.adjusted_budget.value,
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByBoundedSum query."""
+            return self.build_groupby_bounded_sum(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                measure_column=expr.measure_column,
+                lower=lower,
+                upper=upper,
+                stability=mid_stability,
+                mechanism=mechanism,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
+
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
+        )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
+
+    def build_groupby_bounded_average(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        measure_column: str,
+        lower: ExactNumber,
+        upper: ExactNumber,
+        stability: Any,
+        mechanism: NoiseMechanism,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByBoundedAverage query."""
+        return create_average_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            measure_column=measure_column,
+            lower=lower,
+            upper=upper,
+            noise_mechanism=mechanism,
+            d_in=stability,
+            d_out=budget.value,
             output_measure=self.output_measure,
-            groupby_transformation=info.groupby,
-            sum_column=expr.output_column,
+            groupby_transformation=groupby,
+            average_column=output_column,
         )
-        self._validate_measurement(agg, info.mid_stability)
-        return info.transformation | agg
 
-    def visit_groupby_bounded_average(self, expr: GroupByBoundedAverage) -> Measurement:
+    def visit_groupby_bounded_average(
+        self, expr: GroupByBoundedAverage
+    ) -> Tuple[Measurement, NoiseInfo]:
         """Create a measurement from a GroupByBoundedAverage query expression."""
         self._validate_approxDP_and_adjust_budget(expr)
+        expr = self._add_special_value_handling_to_query(expr)
 
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_average(expr)
-        info = self._build_common(expr)
-        # _visit_child_transformation already raises an error if these aren't true
-        # these are just here for MyPy's benefit
-        assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            info.transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
-
-        agg = create_average_measurement(
-            input_domain=info.transformation.output_domain,
-            input_metric=info.transformation.output_metric,
-            measure_column=expr.measure_column,
-            lower=info.lower_bound,
-            upper=info.upper_bound,
-            noise_mechanism=info.mechanism,
-            d_in=info.mid_stability,
-            d_out=self.adjusted_budget.value,
+        expr.accept(OutputSchemaVisitor(self.catalog))
+
+        lower, upper = _get_query_bounds(expr)
+        mechanism = self._pick_noise_for_non_count(expr)
+
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(expr.child, self.default_mechanism),
+            grouping_columns=expr.groupby_keys.dataframe().columns,
+        )
+        transformation = get_table_from_ref(child_transformation, child_ref)
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
+            transformation.output_metric,
+        )
+        mid_stability = transformation.stability_function(self.stability)
+
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByBoundedAverage query."""
+            return self.build_groupby_bounded_average(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                measure_column=expr.measure_column,
+                lower=lower,
+                upper=upper,
+                stability=mid_stability,
+                mechanism=mechanism,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
+
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
+        )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
+
+    def build_groupby_bounded_variance(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        measure_column: str,
+        lower: ExactNumber,
+        upper: ExactNumber,
+        stability: Any,
+        mechanism: NoiseMechanism,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByBoundedVariance query."""
+        return create_variance_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            measure_column=measure_column,
+            lower=lower,
+            upper=upper,
+            noise_mechanism=mechanism,
+            d_in=stability,
+            d_out=budget.value,
             output_measure=self.output_measure,
-            groupby_transformation=info.groupby,
-            average_column=expr.output_column,
+            groupby_transformation=groupby,
+            variance_column=output_column,
         )
-        self._validate_measurement(agg, info.mid_stability)
-        return info.transformation | agg
 
     def visit_groupby_bounded_variance(
         self, expr: GroupByBoundedVariance
-    ) -> Measurement:
+    ) -> Tuple[Measurement, NoiseInfo]:
         """Create a measurement from a GroupByBoundedVariance query expression."""
         self._validate_approxDP_and_adjust_budget(expr)
+        expr = self._add_special_value_handling_to_query(expr)
 
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_variance(expr)
-        info = self._build_common(expr)
-        # _visit_child_transformation already raises an error if these aren't true
-        # these are just here for MyPy's benefit
-        assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            info.transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
-
-        agg = create_variance_measurement(
-            input_domain=info.transformation.output_domain,
-            input_metric=info.transformation.output_metric,
-            measure_column=expr.measure_column,
-            lower=info.lower_bound,
-            upper=info.upper_bound,
-            noise_mechanism=info.mechanism,
-            d_in=info.mid_stability,
-            d_out=self.adjusted_budget.value,
-            output_measure=self.output_measure,
-            groupby_transformation=info.groupby,
-            variance_column=expr.output_column,
-        )
-        self._validate_measurement(agg, info.mid_stability)
-        return info.transformation | agg
+        expr.accept(OutputSchemaVisitor(self.catalog))
 
-    def visit_groupby_bounded_stdev(self, expr: GroupByBoundedSTDEV) -> Measurement:
-        """Create a measurement from a GroupByBoundedStdev query expression."""
-        self._validate_approxDP_and_adjust_budget(expr)
+        lower, upper = _get_query_bounds(expr)
+        mechanism = self._pick_noise_for_non_count(expr)
 
-        # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_stdev(expr)
-        info = self._build_common(expr)
-        # _visit_child_transformation already raises an error if these aren't true
-        # these are just here for MyPy's benefit
-        assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            info.transformation.output_metric,
-            (IfGroupedBy, HammingDistance, SymmetricDifference),
-        )
-
-        agg = create_standard_deviation_measurement(
-            input_domain=info.transformation.output_domain,
-            input_metric=info.transformation.output_metric,
-            measure_column=expr.measure_column,
-            lower=info.lower_bound,
-            upper=info.upper_bound,
-            noise_mechanism=info.mechanism,
-            d_in=info.mid_stability,
-            d_out=self.adjusted_budget.value,
-            output_measure=self.output_measure,
-            groupby_transformation=info.groupby,
-            standard_deviation_column=expr.output_column,
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(expr.child, mechanism),
+            grouping_columns=expr.groupby_keys.dataframe().columns,
         )
+        transformation = get_table_from_ref(child_transformation, child_ref)
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
+            transformation.output_metric,
+        )
+        mid_stability = transformation.stability_function(self.stability)
 
-        self._validate_measurement(agg, info.mid_stability)
-        return info.transformation | agg
-
-    # None of these produce measurements, so they all return a NotImplementedError
-    def visit_private_source(self, expr) -> Any:
-        """Visit a PrivateSource query expression (raises an error)."""
-        raise NotImplementedError
-
-    def visit_rename(self, expr) -> Any:
-        """Visit a Rename query expression (raises an error)."""
-        raise NotImplementedError
-
-    def visit_filter(self, expr) -> Any:
-        """Visit a Filter query expression (raises an error)."""
-        raise NotImplementedError
-
-    def visit_select(self, expr) -> Any:
-        """Visit a Select query expression (raises an error)."""
-        raise NotImplementedError
-
-    def visit_map(self, expr) -> Any:
-        """Visit a Map query expression (raises an error)."""
-        raise NotImplementedError
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByBoundedVariance query."""
+            return self.build_groupby_bounded_variance(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                measure_column=expr.measure_column,
+                lower=lower,
+                upper=upper,
+                stability=mid_stability,
+                mechanism=mechanism,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
 
-    def visit_flat_map(self, expr) -> Any:
-        """Visit a FlatMap query expression (raises an error)."""
-        raise NotImplementedError
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
+        )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
 
-    def visit_join_private(self, expr) -> Any:
-        """Visit a JoinPrivate query expression (raises an error)."""
-        raise NotImplementedError
+    def build_groupby_bounded_stdev(
+        self,
+        input_domain: SparkDataFrameDomain,
+        input_metric: Union[IfGroupedBy, SymmetricDifference, HammingDistance],
+        measure_column: str,
+        lower: ExactNumber,
+        upper: ExactNumber,
+        stability: Any,
+        mechanism: NoiseMechanism,
+        budget: PrivacyBudget,
+        groupby: GroupBy,
+        output_column: str,
+    ) -> Measurement:
+        """Build a Measurement for a GroupByBoundedStdev query."""
+        return create_standard_deviation_measurement(
+            input_domain=input_domain,
+            input_metric=input_metric,
+            measure_column=measure_column,
+            lower=lower,
+            upper=upper,
+            noise_mechanism=mechanism,
+            d_in=stability,
+            d_out=budget.value,
+            output_measure=self.output_measure,
+            groupby_transformation=groupby,
+            standard_deviation_column=output_column,
+        )
 
-    def visit_join_public(self, expr) -> Any:
-        """Visit a JoinPublic query expression (raises an error)."""
-        raise NotImplementedError
+    def visit_groupby_bounded_stdev(
+        self, expr: GroupByBoundedSTDEV
+    ) -> Tuple[Measurement, NoiseInfo]:
+        """Create a measurement from a GroupByBoundedStdev query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+        expr = self._add_special_value_handling_to_query(expr)
 
-    def visit_replace_null_and_nan(self, expr) -> Any:
-        """Visit a ReplaceNullAndNan query expression (raises an error)."""
-        raise NotImplementedError
+        # Peek at the schema, to see if there are errors there
+        expr.accept(OutputSchemaVisitor(self.catalog))
 
-    def visit_replace_infinity(self, expr) -> Any:
-        """Visit a ReplaceInfinity query expression (raises an error)."""
-        raise NotImplementedError
+        lower, upper = _get_query_bounds(expr)
+        mechanism = self._pick_noise_for_non_count(expr)
 
-    def visit_drop_infinity(self, expr) -> Any:
-        """Visit a DropInfinity query expression (raises an error)."""
-        raise NotImplementedError
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(expr.child, mechanism),
+            grouping_columns=expr.groupby_keys.dataframe().columns,
+        )
+        transformation = get_table_from_ref(child_transformation, child_ref)
+        mid_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+        mid_metric = cast(
+            Union[IfGroupedBy, HammingDistance, SymmetricDifference],
+            transformation.output_metric,
+        )
+        mid_stability = transformation.stability_function(self.stability)
 
-    def visit_drop_null_and_nan(self, expr) -> Any:
-        """Visit a DropNullAndNan query expression (raises an error)."""
-        raise NotImplementedError
+        def _build_groupby_agg_from_groupby(
+            groupby: GroupBy, budget: PrivacyBudget
+        ) -> Measurement:
+            """Build a Measurement for a GroupByBoundedStdev query."""
+            return self.build_groupby_bounded_stdev(
+                input_domain=mid_domain,
+                input_metric=mid_metric,
+                measure_column=expr.measure_column,
+                lower=lower,
+                upper=upper,
+                stability=mid_stability,
+                mechanism=mechanism,
+                budget=budget,
+                groupby=groupby,
+                output_column=expr.output_column,
+            )
 
-    def visit_enforce_constraint(self, expr) -> Any:
-        """Visit an EnforceConstraint query expression (raises an error)."""
-        raise NotImplementedError
+        (
+            adaptive_groupby_agg,
+            noise_info,
+        ) = self._build_adaptive_groupby_agg_and_noise_info(
+            input_domain=mid_domain,
+            input_metric=mid_metric,
+            stability=transformation.stability_function(self.stability),
+            mechanism=mechanism,
+            columns=expr.groupby_keys.dataframe().columns,
+            keyset=expr.groupby_keys,
+            build_groupby_agg_from_groupby=_build_groupby_agg_from_groupby,
+            agg_budget=self.adjusted_budget,
+            keyset_budget=self._get_zero_budget(),
+        )
+        self._validate_measurement(adaptive_groupby_agg, mid_stability)
+        return transformation | adaptive_groupby_agg, noise_info
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Defines a visitor for determining the output schemas of query expressions."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from copy import deepcopy
 from typing import KeysView, List, Optional, Union, cast
 
 from pyspark.sql import SparkSession
 
 from tmlt.analytics._catalog import Catalog, PrivateTable, PublicTable
@@ -719,15 +719,15 @@
             for col, val in expr.replace_with.items():
                 if col not in input_schema.keys():
                     raise ValueError(
                         f"Column '{col}' does not exist in this table, "
                         f"available columns are {list(input_schema.keys())}"
                     )
                 if not isinstance(val, pytypes[col]):
-                    # it's ok to use an int as a float
+                    # it's okay to use an int as a float
                     # so don't raise an error in that case
                     if not (isinstance(val, int) and pytypes[col] == float):
                         raise ValueError(
                             f"Column '{col}' cannot have nulls replaced with "
                             f"{repr(val)}, as that value's type does not match the "
                             f"column type {input_schema[col].column_type.name}"
                         )
@@ -957,14 +957,23 @@
                 raise ValueError(
                     f"Nonexistent columns in get_groups query: {nonexistent_columns}"
                 )
             input_schema = Schema(
                 {column: input_schema[column] for column in expr.columns}
             )
 
+        else:
+            input_schema = Schema(
+                {
+                    column: input_schema[column]
+                    for column in input_schema
+                    if column != input_schema.id_column
+                }
+            )
+
         return input_schema
 
     def visit_groupby_count(self, expr: GroupByCount) -> Schema:
         """Returns the resulting schema from evaluating a GroupByCount.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_query_expr_compiler/_base_transformation_visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Defines a visitor for creating a transformation from a query expression."""
+"""Defines a base class for visitors for transformations."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import dataclasses
 import datetime
 import warnings
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, Union
 
 from pyspark.sql import DataFrame
@@ -169,16 +169,16 @@
 from tmlt.analytics.query_expr import QueryExpr, QueryExprVisitor
 from tmlt.analytics.query_expr import Rename as RenameExpr
 from tmlt.analytics.query_expr import ReplaceInfinity, ReplaceNullAndNan
 from tmlt.analytics.query_expr import Select as SelectExpr
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
 
-class TransformationVisitor(QueryExprVisitor):
-    """A visitor to create a transformation from a query expression."""
+class BaseTransformationVisitor(QueryExprVisitor):
+    """A base visitor to create a transformation from a query expression."""
 
     class Output(NamedTuple):
         """A container for the outputs of the visitor."""
 
         transformation: Transformation
         reference: TableReference
         constraints: List[Constraint]
@@ -202,14 +202,31 @@
         """
         self.input_domain = input_domain
         self.input_metric = input_metric
         self.mechanism = mechanism
         self.public_sources = public_sources
         self.table_constraints = table_constraints
 
+    def _new_visitor_after_transformation(self, transformation: Transformation):
+        """Return a new visitor that is expecting queries that follow `transformation`.
+
+        The visitor will be initialized with a new domain and metric that match the
+        output of the given transformation, but otherwise will be configured the same
+        as the original visitor.
+        """
+        assert isinstance(transformation.output_domain, DictDomain)
+        assert isinstance(transformation.output_metric, DictMetric)
+        return self.__class__(
+            transformation.output_domain,
+            transformation.output_metric,
+            self.mechanism,
+            self.public_sources,
+            self.table_constraints,
+        )
+
     def validate_transformation(
         self,
         query: QueryExpr,
         transformation: Transformation,
         reference: TableReference,
         catalog: Catalog,
     ):
@@ -225,15 +242,14 @@
             and expected_schema.id_column is not None
         ):
             raise AssertionError(
                 "Output schema from a transformation had both an ID column "
                 "and a grouping column, which is not allowed. This is probably a bug; "
                 "please let us know about it so we can fix it!"
             )
-
         if expected_schema.grouping_column is not None:
             expected_output_metric = IfGroupedBy(
                 expected_schema.grouping_column, self.inner_metric()
             )
         elif expected_schema.id_column is not None:
             expected_output_metric = IfGroupedBy(
                 expected_schema.id_column, SymmetricDifference()
@@ -594,15 +610,46 @@
         return self.Output(
             *generate_nested_transformation(
                 child_transformation, child_ref.parent, transformation_generators
             ),
             simplify_constraints(propagate_map(expr, child_constraints)),
         )
 
-    def visit_flat_map(self, expr: FlatMapExpr) -> Output:
+    def build_flat_map(  # pylint: disable=no-self-use
+        self,
+        input_metric: Union[IfGroupedBy, SymmetricDifference],
+        row_transformer: RowToRowsTransformation,
+        max_rows: Optional[int],
+    ) -> Transformation:
+        """Build a Transformation for a FlatMap query expression with grouping=False."""
+        transformation = FlatMapTransformation(
+            metric=input_metric,
+            row_transformer=row_transformer,
+            max_num_rows=max_rows,
+        )
+        return transformation
+
+    def build_grouping_flat_map(  # pylint: disable=no-self-use
+        self,
+        inner_metric: Union[SumOf, RootSumOfSquared],
+        row_transformer: RowToRowsTransformation,
+        max_rows: int,
+    ) -> Transformation:
+        """Build a Transformation for a FlatMap query expression with grouping=True."""
+        transformation = GroupingFlatMap(
+            output_metric=inner_metric,
+            row_transformer=row_transformer,
+            max_num_rows=max_rows,
+        )
+        return transformation
+
+    def visit_flat_map(
+        self,
+        expr: FlatMapExpr,
+    ) -> Output:
         """Create a transformation from a FlatMap query expression."""
         child_transformation, child_ref, child_constraints = self._ensure_not_hamming(
             *expr.child.accept(self)
         )
 
         input_domain = lookup_domain(child_transformation.output_domain, child_ref)
         if not isinstance(input_domain, SparkDataFrameDomain):
@@ -649,24 +696,24 @@
             if not isinstance(input_metric, (IfGroupedBy, SymmetricDifference)):
                 raise AssertionError(
                     "Unrecognized input metric. This is probably a bug; "
                     "please let us know about it so we can fix it!"
                 )
             transformation: Transformation
             if expr.schema_new_columns.grouping_column is not None:
-                transformation = GroupingFlatMap(
-                    output_metric=self.inner_metric(),
+                transformation = self.build_grouping_flat_map(
+                    inner_metric=self.inner_metric(),
                     row_transformer=row_transformer,
-                    max_num_rows=expr.max_rows,
+                    max_rows=expr.max_rows,
                 )
             else:
-                transformation = FlatMapTransformation(
-                    metric=input_metric,
+                transformation = self.build_flat_map(
+                    input_metric=input_metric,
                     row_transformer=row_transformer,
-                    max_num_rows=expr.max_rows,
+                    max_rows=expr.max_rows,
                 )
 
             return create_copy_and_transform_value(
                 parent_domain,
                 parent_metric,
                 child_ref.identifier,
                 target,
@@ -693,39 +740,58 @@
                 )
             return FlatMapValueTransformation(
                 parent_domain,
                 parent_metric,
                 child_ref.identifier,
                 target,
                 row_transformer=row_transformer,
-                max_num_rows=expr.max_rows,
+                max_num_rows=None,
             )
 
         transformation_generators: Dict[Type[Metric], Callable] = {
             DictMetric: gen_transformation_dictmetric,
             AddRemoveKeys: gen_transformation_ark,
         }
 
         return self.Output(
             *generate_nested_transformation(
                 child_transformation, child_ref.parent, transformation_generators
             ),
             simplify_constraints(propagate_flat_map(expr, child_constraints)),
         )
 
+    def build_private_join_transformation(  # pylint: disable=no-self-use
+        self,
+        input_domain: DictDomain,
+        left_key: Any,
+        right_key: Any,
+        left_truncation_strategy: CoreTruncationStrategy,
+        right_truncation_strategy: CoreTruncationStrategy,
+        left_truncation_threshold: int,
+        right_truncation_threshold: int,
+        join_cols: Union[List[str], None] = None,
+        join_on_nulls: bool = False,
+    ) -> Transformation:
+        """Build a Transformation for a private join."""
+        return PrivateJoinTransformation(
+            input_domain=input_domain,
+            left_key=left_key,
+            right_key=right_key,
+            left_truncation_strategy=left_truncation_strategy,
+            right_truncation_strategy=right_truncation_strategy,
+            left_truncation_threshold=left_truncation_threshold,
+            right_truncation_threshold=right_truncation_threshold,
+            join_cols=join_cols,
+            join_on_nulls=join_on_nulls,
+        )
+
     def visit_join_private(self, expr: JoinPrivateExpr) -> Output:
         """Create a transformation from a JoinPrivate query expression."""
         left_transformation, left_ref, left_constraints = expr.child.accept(self)
-        right_visitor = TransformationVisitor(
-            left_transformation.output_domain,
-            left_transformation.output_metric,
-            self.mechanism,
-            self.public_sources,
-            self.table_constraints,
-        )
+        right_visitor = self._new_visitor_after_transformation(left_transformation)
         (
             right_transformation,
             right_ref,
             right_constraints,
         ) = expr.right_operand_expr.accept(right_visitor)
 
         if left_ref.parent != right_ref.parent:
@@ -782,15 +848,15 @@
                 [left_ref.identifier, right_ref.identifier],
             )
             if not isinstance(subset.output_domain, DictDomain):
                 raise AssertionError(
                     "Unrecognized input domain. This is probably a bug; "
                     "please let us know about it so we can fix it!"
                 )
-            join = PrivateJoinTransformation(
+            join = self.build_private_join_transformation(
                 input_domain=subset.output_domain,
                 left_key=left_ref.identifier,
                 right_key=right_ref.identifier,
                 left_truncation_strategy=l_trunc_strat,
                 right_truncation_strategy=r_trunc_strat,
                 left_truncation_threshold=l_trunc_threshold,
                 right_truncation_threshold=r_trunc_threshold,
@@ -1378,14 +1444,15 @@
         return self.Output(
             *generate_nested_transformation(
                 child_transformation, child_ref.parent, transformation_generators
             ),
             simplify_constraints(propagate_unmodified(expr, child_constraints)),
         )
 
+    # override in new subclass, if constraints aren't enforced
     def visit_enforce_constraint(self, expr: EnforceConstraint) -> Output:
         """Create a transformation from an EnforceConstraint query expression."""
         # Note: at present, enforcing one constraint can never invalidate
         # another constraint, so just adding the new constraint to the list of
         # constraints is perfectly fine. If a new constraint is added that can
         # invalidate other constraints, this will have to be broken out into
         # per-constraint-type logic.
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_schema.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Schema management for private and public tables.
 
 The schema represents the column types of the underlying table. This allows
 for seamless transitions of the data representation type.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from collections.abc import Mapping
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Iterator, List
 from typing import Mapping as MappingType
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_table_identifier.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_identifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Objects for representing tables."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from dataclasses import dataclass
 
 
 class Identifier:
     """Base class for tables, which are each an Identifier type."""
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_table_reference.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_table_reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Object to reference Tables."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from dataclasses import dataclass
 from typing import List, Optional, Union
 
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.metrics import (
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/_transformation_utils.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/_transformation_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Useful functions to be used with transfomations."""
+"""Useful functions to be used with transformations."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 # pylint: disable=unused-argument
 
 from typing import Callable, Dict, Optional, Tuple, Type, cast
 
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
@@ -56,15 +56,15 @@
 
     Args:
         base_transformation: Transformation to be used as a starting point.
         parent_reference: The parent TableReference of base_transformation's associated
          TableReference.
         generator_dict: a dictionary of the form { Metric : generator() },
           where generator() is a function which takes the associated domain and metric
-          of the parent_reference and generates a transormation using the
+          of the parent_reference and generates a transformation using the
           Metric, e.g. generator(parent_domain, parent_metric, target_identifier)
         table_identifier: identifier for new table in case of rename and original
           table in case of delete/persist/unpersist
     """
     parent_domain = lookup_domain(base_transformation.output_domain, parent_reference)
     parent_metric = lookup_metric(base_transformation.output_metric, parent_reference)
 
@@ -127,16 +127,16 @@
             ),
             hint=lambda d_in, _: d_in,
         )
 
     def gen_transformation_ark(pd, pm, tgt):
         assert isinstance(pd, DictDomain)
         assert isinstance(pm, AddRemoveKeys)
-        # Note: No dataframe column is getting renamed here, RenameValue
-        # is used to rename tables
+        # Note: No dataframe column is getting renamed here;
+        # RenameValueTransformation is used to rename tables
         return RenameValueTransformation(pd, pm, base_ref.identifier, tgt, {})
 
     transformation_generators: Dict[Type[Metric], Callable] = {
         DictMetric: gen_transformation_dictmetric,
         AddRemoveKeys: gen_transformation_ark,
     }
     new_transformation, new_ref = generate_nested_transformation(
@@ -149,16 +149,30 @@
     base_transformation: Transformation, base_ref: TableReference
 ) -> Transformation:
     """Deletes tables."""
 
     def gen_transformation(pd, pm, tgt):
         assert isinstance(pd, DictDomain)
         assert isinstance(pm, (DictMetric, AddRemoveKeys))
+        # having temp tables around can cause problems,
+        # so remove them along with the target table
         return SubsetTransformation(
-            pd, pm, list(set(pd.key_to_domain.keys()) - {base_ref.identifier})
+            pd,
+            pm,
+            list(
+                set(pd.key_to_domain.keys())
+                - set(
+                    (
+                        table
+                        for table in pd.key_to_domain.keys()
+                        if isinstance(table, TemporaryTable)
+                    )
+                )
+                - {base_ref.identifier}
+            ),
         )
 
     transformation_generators: Dict[Type[Metric], Callable] = {
         DictMetric: gen_transformation,
         AddRemoveKeys: gen_transformation,
     }
     new_transformation, _ = generate_nested_transformation(
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/binning_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A BinningSpec defines a binning operation on a column."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import bisect
 import datetime
 import math
 from typing import Any, Generic, List, Optional, Sequence, TypeVar, Union, cast
 
 from tmlt.core.utils.type_utils import get_element_type
@@ -39,15 +39,15 @@
         for bin_name in all_bin_names
     )
     allow_inf = any(
         bin_name in [float("inf"), float("-inf")] for bin_name in all_bin_names
     )
     allow_null = True
 
-    # nan_bin type is checked in the __init__.
+    # nan_bin type is checked in the __init__ method.
     column_type = ColumnType(get_element_type(bin_names, allow_none=False))
     return ColumnDescriptor(column_type, allow_null, allow_nan, allow_inf)
 
 
 def _edges_as_str(bin_edges: List[BinT]) -> List[str]:
     """Format the bin edges as strings."""
     if isinstance(bin_edges[0], float):
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/constraints/_base.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Defines the base :class:`Constraint` class."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from tmlt.core.transformations.base import Transformation
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/constraints/_simplify.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_simplify.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Tools for simplifying constraints."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from typing import List
 
 from ._base import Constraint
 from ._truncation import simplify_truncation_constraints
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/constraints/_truncation.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/constraints/_truncation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 These constraints all in some way limit how many distinct values or repetitions
 of the same value may appear in a column, often in relation to some other
 column.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from dataclasses import dataclass
 from typing import Dict, List, Tuple, Union
 
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.metrics import (
     AddRemoveKeys,
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/keyset.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/keyset.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and the values ``[0, 1, 2, 3]`` for column B.
 
 Currently, KeySets are used as a simpler way to specify domains for groupby
 transformations.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from __future__ import annotations
 
 import datetime
 from typing import Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Type, Union
 
 from pyspark.sql import Column, DataFrame
@@ -266,31 +266,31 @@
             True
             >>> different_keyset = KeySet.from_dict({"B": ["a1", "a2"]})
             >>> keyset1 == different_keyset
             False
         """
         if not isinstance(other, KeySet):
             return False
-        # TODO(#2107): Fix typing once Pandas has working type stubs
-        self_df = self.dataframe().toPandas()
-        other_df = other.dataframe().toPandas()
-        if sorted(self_df.columns) != sorted(other_df.columns):  # type: ignore
+        self_df = self.dataframe()
+        other_df = other.dataframe()
+        if sorted(self_df.columns) != sorted(other_df.columns):
             return False
-        if self_df.empty and other_df.empty:  # type: ignore
-            return True
-        sorted_columns = sorted(self_df.columns)  # type: ignore
-        self_df_sorted = (
-            self_df.set_index(sorted_columns).sort_index().reset_index()  # type: ignore
-        )
-        other_df_sorted = (
-            other_df.set_index(sorted_columns)  # type: ignore
-            .sort_index()
-            .reset_index()
-        )
-        return self_df_sorted.equals(other_df_sorted)
+        # Re-select the columns so that both dataframes have columns
+        # in the same order
+        self_df = self_df.select(sorted(self_df.columns))
+        other_df = other_df.select(sorted(other_df.columns))
+        if self_df.schema != other_df.schema:
+            return False
+        # other_df should contain all rows in self_df
+        if self_df.exceptAll(other_df).count() != 0:
+            return False
+        # and vice versa
+        if other_df.exceptAll(self_df).count() != 0:
+            return False
+        return True
 
     def schema(self) -> Schema:
         # pylint: disable=line-too-long
         """Returns a Schema based on the KeySet.
 
         Example:
             >>> domains = {
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/privacy_budget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Classes for specifying privacy budgets.
 
 For a full introduction to privacy budgets, see the
 :ref:`privacy budget topic guide<Privacy budget fundamentals>`.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import math
 from abc import ABC, abstractmethod
 from typing import Tuple, Union
 
 import sympy as sp
 from tmlt.core.utils.exact_number import ExactNumber
@@ -60,14 +60,19 @@
     """
 
     @property
     @abstractmethod
     def value(self) -> Union[ExactNumber, Tuple[ExactNumber, ExactNumber]]:
         """Return the value of the privacy budget."""
 
+    @property
+    @abstractmethod
+    def is_infinite(self) -> bool:
+        """Returns true if the privacy budget is infinite."""
+
 
 class PureDPBudget(PrivacyBudget):
     """A privacy budget under pure differential privacy.
 
     This privacy definition is also known as epsilon-differential privacy, and the
     associated value is the epsilon privacy parameter. The privacy definition can
     be found `here <https://en.wikipedia.org/wiki/Differential_privacy#Definition_of_%CE%B5-differential_privacy>`__.
@@ -105,14 +110,19 @@
         """Returns the value of epsilon as an int or float.
 
         This is helpful for human readability. If you need to use the epsilon value in
         a computation, you should use self.value instead.
         """
         return _to_int_or_float(self._epsilon)
 
+    @property
+    def is_infinite(self) -> bool:
+        """Returns true if epsilon is float('inf')."""
+        return self._epsilon == float("inf")
+
     def __repr__(self) -> str:
         """Returns string representation of this PureDPBudget."""
         return f"PureDPBudget(epsilon={self.epsilon})"
 
     def __eq__(self, other) -> bool:
         """Returns whether or not a PureDPBudget is equivalent to another PrivacyBudget.
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/protected_change.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Types for programmatically specifying what changes in input tables are protected."""
 
-# Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 from abc import ABC
 from dataclasses import dataclass
-from typing import Union
 
 from typeguard import check_type
 
 
 class ProtectedChange(ABC):
     """A description of the largest change in a dataset that is protected under DP.
 
@@ -83,22 +82,22 @@
     of the analysis.
     """
 
     grouping_column: str
     """The name of the column specifying the group."""
     max_groups: int
     """The maximum number of groups that may differ."""
-    max_rows_per_group: Union[int, float]
+    max_rows_per_group: int
     """The maximum number of rows which may be added to or removed from each group."""
 
     def __post_init__(self):
         """Validate attributes."""
         check_type("column", self.grouping_column, str)
         check_type("max_groups", self.max_groups, int)
-        check_type("max_rows_per_group", self.max_rows_per_group, Union[int, float])
+        check_type("max_rows_per_group", self.max_rows_per_group, int)
         if self.max_groups < 1:
             raise ValueError("max_groups must be positive")
         if self.max_rows_per_group < 1:
             raise ValueError("max_rows_per_group must be positive")
 
 
 @dataclass(frozen=True)
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/query_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 :meth:`~tmlt.analytics.query_builder.QueryBuilder.groupby`, yielding a
 :class:`~tmlt.analytics.query_expr.QueryExpr` object. This QueryExpr can then be
 passed to :func:`~tmlt.analytics.session.Session.evaluate` to obtain
 differentially private results to the query.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 import warnings
 from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 from pyspark.sql import DataFrame
 
@@ -87,16 +87,16 @@
     """High-level interface for specifying DP queries.
 
     Each instance corresponds to applying a transformation.
     The full graph of QueryBuilder objects can be traversed from root to a node.
 
     ..
         >>> from tmlt.analytics.privacy_budget import PureDPBudget
-        >>> import tmlt.analytics.session
         >>> from tmlt.analytics.protected_change import AddOneRow
+        >>> import tmlt.analytics.session
         >>> import pandas as pd
         >>> from pyspark.sql import SparkSession
         >>> spark = SparkSession.builder.getOrCreate()
         >>> my_private_data = spark.createDataFrame(
         ...     pd.DataFrame(
         ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
         ...     )
@@ -180,18 +180,23 @@
 
         Every row within a join group (i.e., every row that shares values in the join
         columns) from the private table will be joined with every row from that same
         group in the public table. For example, if a group has :math:`X` rows in the
         private table and :math:`Y` rows in the public table, then the output table
         will contain :math:`X*Y` rows for this group.
 
+        .. note::
+            Tables with a :class:`~tmlt.analytics.protected_change.ProtectedChange` of
+            :class:`~tmlt.analytics.protected_change.AddRowsWithID` must include the
+            *privacy ID* column in the join columns.
+
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -299,18 +304,23 @@
 
         In contrast, operations on tables with a
         :class:`~tmlt.analytics.protected_change.AddRowsWithID`
         :class:`~tmlt.analytics.protected_change.ProtectedChange` do not require a
         :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`, as no
         truncation is necessary while performing the join.
 
+        .. note::
+            Tables with a :class:`~tmlt.analytics.protected_change.ProtectedChange` of
+            :class:`~tmlt.analytics.protected_change.AddRowsWithID` must include the
+            *privacy ID* column in the join columns.
+
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -421,16 +431,16 @@
 
         .. warning::
             If null values are replaced in a column, then Analytics will raise
             an error if you use a KeySet with a null value for that column.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [[None, 0, 0.0], ["1", None, 1.1], ["2", 2, None]],
             ...         columns=["A", "B", "X"],
@@ -497,16 +507,16 @@
     def replace_infinity(
         self, replace_with: Optional[Dict[str, Tuple[float, float]]] = None
     ) -> "QueryBuilder":
         """Updates the current query to replace +inf and -inf values in some columns.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [
             ...             ["a1", 0, 0.0],
@@ -584,16 +594,16 @@
         .. warning::
             If null and NaN values are dropped from a column, then Analytics will
             raise an error if you use a :class:`~tmlt.analytics.keyset.KeySet`
             that contains a null value for that column.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> from pyspark.sql.types import (
             ...     DoubleType,
             ...     LongType,
             ...     StringType,
             ...     StructField,
@@ -674,16 +684,16 @@
         return self
 
     def drop_infinity(self, columns: Optional[List[str]]) -> "QueryBuilder":
         """Updates the current query to drop rows containing infinite values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> from pyspark.sql.types import (
             ...     DoubleType,
             ...     LongType,
             ...     StringType,
             ...     StructField,
@@ -763,16 +773,16 @@
         return self
 
     def rename(self, column_mapper: Dict[str, str]) -> "QueryBuilder":
         """Updates the current query to rename the columns.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -834,16 +844,16 @@
         * ``LENGTH(name) > 17``
         * ``favorite_color IN ('blue', 'red')``
         * ``date = '2022-03-14'``
         * ``time < '2022-01-01T12:45:00'``
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -851,14 +861,15 @@
 
         Example:
             >>> budget = PureDPBudget(float("inf"))
             >>> sess = tmlt.analytics.session.Session.from_dataframe(
             ...     privacy_budget=budget,
             ...     source_id="my_private_data",
             ...     dataframe=my_private_data,
+            ...     protected_change=AddOneRow(),
             ... )
             >>> my_private_data.toPandas()
                A  B  X
             0  0  1  0
             1  1  0  1
             2  1  2  1
             >>> sess.private_sources
@@ -889,18 +900,18 @@
         return self
 
     def select(self, columns: Sequence[str]) -> "QueryBuilder":
         """Updates the current query to select certain columns.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
+            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> # Typeguard doesn't like implicit doctest imports
             >>> from tmlt.analytics.query_builder import QueryBuilder
             >>> import tmlt.analytics.session
-            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -952,16 +963,16 @@
 
         If you provide only a ColumnType for the new column types, Analytics
         assumes that all new columns created may contain null values (and that
         DECIMAL columns may contain NaN or infinite values).
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -969,14 +980,15 @@
 
         Example:
             >>> budget = PureDPBudget(float("inf"))
             >>> sess = tmlt.analytics.session.Session.from_dataframe(
             ...     privacy_budget=budget,
             ...     source_id="my_private_data",
             ...     dataframe=my_private_data,
+            ...     protected_change=AddOneRow(),
             ... )
             >>> my_private_data.toPandas()
                A  B  X
             0  0  1  0
             1  1  0  1
             2  1  2  1
             >>> sess.private_sources
@@ -1057,16 +1069,16 @@
         :class:`~tmlt.analytics.protected_change.AddRowsWithID`
         :class:`~tmlt.analytics.protected_change.ProtectedChange` do not require a
         ``max_rows`` argument, since it is not necessary to impose a limit on
         the number of new rows.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.keyset import KeySet
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1], ["1", 3, 1]],
@@ -1125,15 +1137,17 @@
                 The function's input is a dictionary matching a column name to
                 its value for that row.
                 This function should return a list of dictionaries.
                 Those dictionaries should always
                 have the same keys regardless of input, and the values in those
                 dictionaries should match the column type specified in
                 ``new_column_types``. The function should not have any side effects
-                (in particular, ``f`` must not raise exceptions).
+                (in particular, ``f`` must not raise exceptions), and must be
+                deterministic (running it multiple times on a fixed input should
+                always return the same output).
             new_column_types: Mapping from column names to types, for new columns
                 produced by ``f``. Using
                 :class:`~tmlt.analytics.query_builder.ColumnDescriptor`
                 is preferred.
             augment: If True, add new columns to the existing dataframe (so new
                      schema = old schema + schema_new_columns).
                      If False, make the new dataframe with schema = schema_new_columns
@@ -1187,16 +1201,16 @@
         self, column: str, spec: BinningSpec, name: Optional[str] = None
     ) -> "QueryBuilder":
         """Create a new column by assigning the values in a given column to bins.
 
         ..
             >>> from tmlt.analytics.query_builder import QueryBuilder
             >>> from tmlt.analytics.session import Session
-            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
+            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> from tmlt.analytics.keyset import KeySet
             >>> from pyspark.sql import SparkSession
             >>> import pandas as pd
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         {
@@ -1283,16 +1297,16 @@
         name: Optional[str] = None,
     ) -> "QueryExpr":
         """Returns a count query containing the frequency of values in specified column.
 
         ..
             >>> from tmlt.analytics.query_builder import QueryBuilder
             >>> from tmlt.analytics.session import Session
-            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
+            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> from tmlt.analytics.keyset import KeySet
             >>> from pyspark.sql import SparkSession
             >>> import pandas as pd
             >>> spark = SparkSession.builder.getOrCreate()
 
         Example:
             >>> from tmlt.analytics.binning_spec import BinningSpec
@@ -1415,14 +1429,15 @@
         .. note::
             Because this uses differential privacy, it won't include all of the values
             in the input dataset columns, and may even return no results at all on
             datasets that have few values for each set of group keys.
 
         ..
             >>> from tmlt.analytics.privacy_budget import ApproxDPBudget
+            >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
 
         Example:
             >>> my_private_data = spark.createDataFrame(
@@ -1432,14 +1447,15 @@
             ...         columns=["A", "B", "X"],
             ...     )
             ... )
             >>> sess = tmlt.analytics.session.Session.from_dataframe(
             ...     privacy_budget=ApproxDPBudget(1, 1e-5),
             ...     source_id="my_private_data",
             ...     dataframe=my_private_data,
+            ...     protected_change=AddOneRow(),
             ... )
             >>> # Building a get_groups query
             >>> query = (
             ...     QueryBuilder("my_private_data")
             ...     .get_groups()
             ... )
             >>> # Answering the query with infinite privacy budget
@@ -1450,26 +1466,29 @@
             >>> answer.toPandas()
                A  B  X
             0  0  1  0
             1  1  2  1
 
         Args:
             columns: Name of the column used to assign bins. If empty or none
-                are provided, will use all of the columns in the table.
+                are provided, all of the columns in the table will be used, excluding
+                any column marked as a *privacy ID* in a table with a
+                :class:`~tmlt.analytics.protected_change.ProtectedChange` of
+                :class:`~tmlt.analytics.protected_change.AddRowsWithID`.
         """
         query_expr = GetGroups(child=self._query_expr, columns=columns)
         return query_expr
 
     def groupby(self, keys: KeySet) -> "GroupedQueryBuilder":
         """Groups the query by the given set of keys, returning a GroupedQueryBuilder.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -1606,16 +1625,16 @@
         .. note::
             Differentially private counts may return values that are not
             possible for a non-DP query - including negative values. You can enforce
             non-negativity once the query returns its results; see the example below.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -1681,16 +1700,16 @@
         .. note::
             Differentially private counts may returns values that are not
             possible for a non-DP query - including negative values. You can enforce
             non-negativity once the query returns its results; see the example below.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["0", 1, 0], ["1", 0, 1], ["1", 2, 1]],
             ...         columns=["A", "B", "X"],
@@ -1769,16 +1788,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~drop_null_and_nan` query will be performed first. If the
             column being measured contains infinite values, a
             :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -1840,16 +1859,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~drop_null_and_nan` query will be performed first. If the
             column being measured contains infinite values, a
             :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -1909,16 +1928,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~drop_null_and_nan` query will be performed first. If the
             column being measured contains infinite values, a
             :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -1978,16 +1997,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~drop_null_and_nan` query will be performed first. If the
             column being measured contains infinite values, a
             :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2063,16 +2082,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2147,16 +2166,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2231,16 +2250,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2315,16 +2334,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2402,16 +2421,16 @@
         name: Optional[str] = None,
         mechanism: CountMechanism = CountMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a count query that is ready to be evaluated.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2472,16 +2491,16 @@
         mechanism: CountDistinctMechanism = CountDistinctMechanism.DEFAULT,
         cols: Optional[List[str]] = None,
     ) -> QueryExpr:
         """Returns a count_distinct query that is ready to be evaluated.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["0", 1, 0], ["1", 0, 1], ["1", 2, 1]],
             ...         columns=["A", "B", "X"],
@@ -2574,16 +2593,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
             first. If the column being measured contains infinite values, a
             :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2656,16 +2675,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
             first. If the column being measured contains infinite values, a
             :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2731,16 +2750,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
             first. If the column being measured contains infinite values, a
             :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2806,16 +2825,16 @@
             If the column being measured contains NaN or null values, a
             :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
             first. If the column being measured contains infinite values, a
             :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2893,16 +2912,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -2988,16 +3007,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -3083,16 +3102,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
@@ -3178,16 +3197,16 @@
             #. The narrower the range, the less noise. Larger bounds mean more data \
                 is kept, but more noise needs to be added to the result.
             #. The clamping bounds are assumed to be public information. Avoid using \
                 the private data to set these values.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
-            >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
+            >>> import tmlt.analytics.session
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
             >>> my_private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
             ...     )
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/query_expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 :class:`tmlt.analytics.query_builder.QueryBuilder` to create them and
 :class:`tmlt.analytics.session.Session` to consume them provide more
 user-friendly features.
 """
 # TODO: Known typeguard issue: https://github.com/agronholm/typeguard/issues/65
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 import datetime
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Union
 
@@ -46,15 +46,15 @@
     LAPLACE = auto()
     """Double-sided geometric noise is used."""
     GAUSSIAN = auto()
     """The discrete Gaussian mechanism is used. Not compatible with pure DP."""
 
 
 class CountDistinctMechanism(Enum):
-    """Enumerating the possible mechanims used for the count_distinct aggregation.
+    """Enumerating the possible mechanisms used for the count_distinct aggregation.
 
     Currently, the
     :meth:`~tmlt.analytics.query_builder.GroupedQueryBuilder.count_distinct`
     aggregation uses an additive noise mechanism to achieve differential privacy.
     """
 
     DEFAULT = auto()
@@ -371,15 +371,15 @@
         check_type("child", self.child, QueryExpr)
         check_type("f", self.f, Callable[[Row], List[Row]])
         check_type("max_rows", self.max_rows, Optional[int])
         check_type("schema_new_columns", self.schema_new_columns, Schema)
         check_type("augment", self.augment, bool)
         if self.max_rows and self.max_rows < 0:
             raise ValueError(
-                f"Limit on number of rows '{self.max_rows}' must be nonnegative."
+                f"Limit on number of rows '{self.max_rows}' must be non-negative."
             )
         if (
             self.schema_new_columns.grouping_column
             and len(self.schema_new_columns) != 1
         ):
             raise ValueError(
                 "schema_new_columns contains "
@@ -542,15 +542,15 @@
     """The default value used for VARCHARs (the empty string)."""
     DATE = datetime.date.fromtimestamp(0)
     """The default value used for dates (``datetime.date.fromtimestamp(0)``).
 
     See :meth:`~.datetime.date.fromtimestamp`.
     """
     TIMESTAMP = datetime.datetime.fromtimestamp(0)
-    """The defauLt value used for timestamps (``datetime.datetime.fromtimestamp(0)``).
+    """The default value used for timestamps (``datetime.datetime.fromtimestamp(0)``).
 
     See :meth:`~.datetime.datetime.fromtimestamp`.
     """
 
 
 @dataclass
 class ReplaceNullAndNan(QueryExpr):
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/session.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 each of the private tables, provided that the private data is not used elsewhere
 in the computation of the queries.
 
 More details on the exact privacy promise provided by :class:`Session` can be
 found in the :ref:`Privacy promise topic guide <Privacy promise>`.
 """
 
-# Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 from operator import xor
-from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 from warnings import warn
 
 import pandas as pd  # pylint: disable=unused-import
 import sympy as sp
 from pyspark.sql import SparkSession  # pylint: disable=unused-import
 from pyspark.sql import DataFrame
 from tmlt.core.domains.collections import DictDomain
@@ -37,15 +37,14 @@
     InactiveAccountantError,
     InsufficientBudgetError,
     PrivacyAccountant,
     PrivacyAccountantState,
     SequentialComposition,
 )
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
-from tmlt.core.metrics import AddRemoveKeys as AddRemoveKeysMetric
 from tmlt.core.metrics import (
     DictMetric,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -54,29 +53,35 @@
 from tmlt.core.transformations.identity import Identity
 from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
 from tmlt.core.utils.configuration import SparkConfigError, check_java11
 from tmlt.core.utils.exact_number import ExactNumber
 from tmlt.core.utils.type_utils import assert_never
 from typeguard import check_type, typechecked
 
+from tmlt.analytics._base_builder import (
+    BaseBuilder,
+    DataFrameMixin,
+    PrivacyBudgetMixin,
+    PrivateDataFrame,
+)
 from tmlt.analytics._catalog import Catalog, PrivateTable, PublicTable
 from tmlt.analytics._coerce_spark_schema import (
     SUPPORTED_SPARK_TYPES,
     TYPE_COERCION_MAP,
     coerce_spark_schema_or_fail,
 )
 from tmlt.analytics._neighboring_relation import (
     AddRemoveKeys,
     AddRemoveRows,
     AddRemoveRowsAcrossGroups,
     Conjunction,
     NeighboringRelation,
 )
 from tmlt.analytics._neighboring_relation_visitor import NeighboringRelationCoreVisitor
-from tmlt.analytics._noise_info import _noise_from_measurement
+from tmlt.analytics._noise_info import NoiseInfo
 from tmlt.analytics._privacy_budget_rounding_helper import get_adjusted_budget
 from tmlt.analytics._query_expr_compiler import QueryExprCompiler
 from tmlt.analytics._schema import (
     Schema,
     spark_dataframe_domain_to_analytics_columns,
     spark_schema_to_analytics_columns,
 )
@@ -92,56 +97,42 @@
     delete_table,
     get_table_from_ref,
     persist_table,
     rename_table,
     unpersist_table,
 )
 from tmlt.analytics._type_checking import is_exact_number_tuple
+from tmlt.analytics._utils import assert_is_identifier
 from tmlt.analytics.constraints import Constraint, MaxGroupsPerID
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
     PrivacyBudget,
     PureDPBudget,
     RhoZCDPBudget,
 )
-from tmlt.analytics.protected_change import (
+from tmlt.analytics.protected_change import (  # pylint: disable=unused-import
     AddMaxRows,
     AddMaxRowsInMaxGroups,
     AddOneRow,
     AddRowsWithID,
     ProtectedChange,
 )
 from tmlt.analytics.query_builder import ColumnType, GroupedQueryBuilder, QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
 
 __all__ = ["Session", "SUPPORTED_SPARK_TYPES", "TYPE_COERCION_MAP"]
 
 
-class _PrivateSourceTuple(NamedTuple):
-    """Named tuple of private Dataframe, domain and protected change."""
-
-    dataframe: DataFrame
-    """Private DataFrame."""
-
-    protected_change: ProtectedChange
-    """Protected change for this private source."""
-
-    domain: SparkDataFrameDomain
-    """Domain of private DataFrame."""
-
-
-def _generate_neighboring_relation(
-    sources: Dict[str, _PrivateSourceTuple]
-) -> Conjunction:
+def _generate_neighboring_relation(sources: Dict[str, PrivateDataFrame]) -> Conjunction:
     """Convert a collection of private source tuples into a neighboring relation."""
     relations: List[NeighboringRelation] = []
     # this is used only for AddRemoveKeys.
     protected_ids_dict: Dict[str, Dict[str, str]] = {}
 
-    for name, (_, protected_change, _) in sources.items():
+    for name, (_, protected_change) in sources.items():
         if isinstance(protected_change, AddMaxRows):
             relations.append(AddRemoveRows(name, protected_change.max_rows))
         elif isinstance(protected_change, AddMaxRowsInMaxGroups):
             relations.append(
                 AddRemoveRowsAcrossGroups(
                     name,
                     protected_change.grouping_column,
@@ -160,95 +151,88 @@
                 f"Unsupported ProtectedChange type: {type(protected_change)}"
             )
     for identifier, table_to_key_column in protected_ids_dict.items():
         relations.append(AddRemoveKeys(identifier, table_to_key_column))
     return Conjunction(relations)
 
 
-# TODO(2476): Uncomment this once we allow consuming delta, and remove the part
-# that only reports epsilon (immediately after the commented section).
 def _format_insufficient_budget_msg(
     requested_budget: Union[ExactNumber, Tuple[ExactNumber, ExactNumber]],
     remaining_budget: Union[ExactNumber, Tuple[ExactNumber, ExactNumber]],
     privacy_budget: PrivacyBudget,
 ) -> str:
     """Format message for InsufficientBudgetError."""
     output = ""
+    format_threshold = 0.1
 
     if isinstance(privacy_budget, ApproxDPBudget):
         if is_exact_number_tuple(requested_budget) and is_exact_number_tuple(
             remaining_budget
         ):
             assert isinstance(requested_budget, tuple)
             assert isinstance(remaining_budget, tuple)
             remaining_epsilon = remaining_budget[0].to_float(round_up=True)
             requested_epsilon = requested_budget[0].to_float(round_up=True)
-            #   requested_delta = requested_budget[1].to_float(round_up=True)
-            #   remaining_delta = remaining_budget[1].to_float(round_up=True)
-            #   output += f"\nRequested: ε={requested_epsilon:.3f},"
-            #   output += f" δ={requested_delta:.3f}"
-            #   output += f"\nRemaining: ε={remaining_epsilon:.3f},"
-            #   output += f" δ={remaining_delta:.3f}"
-            #   output += "\nDifference: "
-            #   lacks_epsilon = remaining_epsilon < requested_epsilon
-            #   lacks_delta = remaining_delta < requested_delta
-            #   if lacks_epsilon and lacks_delta:
-            #       eps_diff = abs(remaining_epsilon - requested_epsilon)
-            #       delta_diff = abs(remaining_delta - requested_delta)
-            #       if eps_diff >= 0.1 and delta_diff >= 0.1:
-            #           output += f"ε={eps_diff:.3f}, δ={delta_diff:.3f}"
-            #       elif eps_diff < 0.1:
-            #           output += f"ε={eps_diff:.3e}, δ={delta_diff:.3f}"
-            #       elif delta_diff < 0.1:
-            #           output += f"ε={eps_diff:.3f}, δ={delta_diff:.3e}"
-            #   elif lacks_epsilon:
-            #       eps_diff = abs(remaining_epsilon - requested_epsilon)
-            #       if eps_diff >= 0.1:
-            #           output += f"ε={eps_diff:.3f}"
-            #       else:
-            #           output += f"ε={eps_diff:.3e}"
-            #   elif lacks_delta:
-            #       delta_diff = abs(remaining_delta - requested_delta)
-            #       if delta_diff >= 0.1:
-            #           output += f"δ={delta_diff:.3f}"
-            #       else:
-            #           output += f"δ={delta_diff:.3e}"
-            approx_diff = abs(remaining_epsilon - requested_epsilon)
-            output += f"\nRequested: ε={requested_epsilon:.3f}"
-            output += f"\nRemaining: ε={remaining_epsilon:.3f}"
-            if approx_diff >= 0.1:
-                output += f"\nDifference: ε={approx_diff:.3f}"
-            else:
-                output += f"\nDifference: ε={approx_diff:.3e}"
+            requested_delta = requested_budget[1].to_float(round_up=True)
+            remaining_delta = remaining_budget[1].to_float(round_up=True)
+            output += f"\nRequested: ε={requested_epsilon:.3f},"
+            output += f" δ={requested_delta:.3f}"
+            output += f"\nRemaining: ε={remaining_epsilon:.3f},"
+            output += f" δ={remaining_delta:.3f}"
+            output += "\nDifference: "
+            lacks_epsilon = remaining_epsilon < requested_epsilon
+            lacks_delta = remaining_delta < requested_delta
+            if lacks_epsilon and lacks_delta:
+                eps_diff = round(abs(remaining_epsilon - requested_epsilon), 3)
+                delta_diff = round(abs(remaining_delta - requested_delta), 3)
+                if eps_diff >= format_threshold and delta_diff >= format_threshold:
+                    output += f"ε={eps_diff:.3f}, δ={delta_diff:.3f}"
+                elif eps_diff < format_threshold:
+                    output += f"ε={eps_diff:.3e}, δ={delta_diff:.3f}"
+                elif delta_diff < format_threshold:
+                    output += f"ε={eps_diff:.3f}, δ={delta_diff:.3e}"
+            elif lacks_epsilon:
+                eps_diff = round(abs(remaining_epsilon - requested_epsilon), 3)
+                if eps_diff >= format_threshold:
+                    output += f"ε={eps_diff:.3f}"
+                else:
+                    output += f"ε={eps_diff:.3e}"
+            elif lacks_delta:
+                delta_diff = round(abs(remaining_delta - requested_delta), 3)
+                if delta_diff >= format_threshold:
+                    output += f"δ={delta_diff:.3f}"
+                else:
+                    output += f"δ={delta_diff:.3e}"
+
         else:
             raise AssertionError(
                 "Unable to convert privacy budget of type"
                 f" {type(privacy_budget)} to float or floats. This is"
                 " probably a bug; please let us know about it so we can fix it!"
             )
     elif isinstance(privacy_budget, (PureDPBudget, RhoZCDPBudget)):
         assert isinstance(requested_budget, ExactNumber)
         assert isinstance(remaining_budget, ExactNumber)
         if isinstance(privacy_budget, PureDPBudget):
             remaining_epsilon = remaining_budget.to_float(round_up=True)
             requested_epsilon = requested_budget.to_float(round_up=True)
-            approx_diff = abs(remaining_epsilon - requested_epsilon)
+            approx_diff = round(abs(remaining_epsilon - requested_epsilon), 3)
             output += f"\nRequested: ε={requested_epsilon:.3f}"
             output += f"\nRemaining: ε={remaining_epsilon:.3f}"
-            if approx_diff >= 0.1:
+            if approx_diff >= format_threshold:
                 output += f"\nDifference: ε={approx_diff:.3f}"
             else:
                 output += f"\nDifference: ε={approx_diff:.3e}"
         elif isinstance(privacy_budget, RhoZCDPBudget):
             remaining_rho = remaining_budget.to_float(round_up=True)
             requested_rho = requested_budget.to_float(round_up=True)
-            approx_diff = abs(remaining_rho - requested_rho)
+            approx_diff = round(abs(remaining_rho - requested_rho), 3)
             output += f"\nRequested: 𝝆={requested_rho:.3f}"
             output += f"\nRemaining: 𝝆={remaining_rho:.3f}"
-            if approx_diff >= 0.1:
+            if approx_diff >= format_threshold:
                 output += f"\nDifference: 𝝆={approx_diff:.3f}"
             else:
                 output += f"\nDifference: 𝝆={approx_diff:.3e}"
     else:
         raise AssertionError(
             f"Unsupported budget types: {type(requested_budget)},"
             f" {type(remaining_budget)}. This is probably a bug, please let us know"
@@ -260,233 +244,67 @@
 class Session:
     """Allows differentially private query evaluation on sensitive data.
 
     Sessions should not be directly constructed. Instead, they should be created
     using :meth:`from_dataframe` or with a :class:`Builder`.
     """
 
-    class Builder:
+    class Builder(DataFrameMixin, PrivacyBudgetMixin, BaseBuilder):
         """Builder for :class:`Session`."""
 
-        def __init__(self):
-            """Constructor."""
-            self._privacy_budget: Optional[PrivacyBudget] = None
-            self._private_sources: Dict[str, _PrivateSourceTuple] = {}
-            self._public_sources: Dict[str, DataFrame] = {}
-            self._id_spaces: List[str] = []
-
         def build(self) -> "Session":
             """Builds Session with specified configuration."""
             if self._privacy_budget is None:
                 raise ValueError("Privacy budget must be specified.")
-            if not self._private_sources:
-                raise ValueError("At least one private source must be provided.")
-            neighboring_relation = _generate_neighboring_relation(self._private_sources)
+            if not self._private_dataframes:
+                raise ValueError("At least one private dataframe must be specified")
+            neighboring_relation = _generate_neighboring_relation(
+                self._private_dataframes
+            )
             tables = {
-                source_id: source_tuple.dataframe
-                for source_id, source_tuple in self._private_sources.items()
+                source_id: dataframe
+                for source_id, (dataframe, _) in self._private_dataframes.items()
             }
             sess = (
                 Session._from_neighboring_relation(  # pylint: disable=protected-access
                     self._privacy_budget, tables, neighboring_relation
                 )
             )
-            # check list of ARK identifiers agains session's ID spaces
+            # check list of ARK identifiers against session's ID spaces
             assert isinstance(neighboring_relation, Conjunction)
             for child in neighboring_relation.children:
                 if isinstance(child, AddRemoveKeys):
                     if child.id_space not in self._id_spaces:
                         raise ValueError(
                             "An AddRowsWithID protected change was specified without "
                             "an associated identifier space for the session.\n"
                             f"AddRowsWithID identifier provided: {child.id_space}\n"
                             f"Identifier spaces for the session: {self._id_spaces}"
                         )
             # add public sources
-            for source_id, dataframe in self._public_sources.items():
+            for source_id, dataframe in self._public_dataframes.items():
                 sess.add_public_dataframe(source_id, dataframe)
 
             return sess
 
-        def with_privacy_budget(
-            self, privacy_budget: PrivacyBudget
-        ) -> "Session.Builder":
-            """Sets the privacy budget for the Session to be built.
-
-            Args:
-                privacy_budget: Privacy Budget to be allocated to Session.
-            """
-            if self._privacy_budget is not None:
-                raise ValueError("This Builder already has a privacy budget")
-            self._privacy_budget = privacy_budget
-            return self
-
-        def with_private_dataframe(
-            self,
-            source_id: str,
-            dataframe: DataFrame,
-            stability: Optional[Union[int, float]] = None,
-            grouping_column: Optional[str] = None,
-            protected_change: Optional[ProtectedChange] = None,
-        ) -> "Session.Builder":
-            """Adds a Spark DataFrame as a private source.
-
-            Not all Spark column types are supported in private sources; see
-            :data:`SUPPORTED_SPARK_TYPES` for information about which types are
-            supported.
-
-            Args:
-                source_id: Source id for the private source dataframe.
-                dataframe: Private source dataframe to perform queries on,
-                    corresponding to the ``source_id``.
-                stability: Deprecated: use ``protected_change`` instead, see
-                    :ref:`changelog<changelog#protected-change>`.
-                grouping_column: Deprecated: use ``protected_change`` instead, see
-                    :ref:`changelog<changelog#protected-change>`.
-                protected_change: A
-                    :class:`~tmlt.analytics.protected_change.ProtectedChange`
-                    specifying what changes to the input data the resulting
-                    :class:`Session` should protect.
-            """
-            _assert_is_identifier(source_id)
-            if source_id in self._private_sources or source_id in self._public_sources:
-                raise ValueError(f"Duplicate source id: '{source_id}'")
-
-            dataframe = coerce_spark_schema_or_fail(dataframe)
-            domain = SparkDataFrameDomain.from_spark_schema(dataframe.schema)
-
-            if protected_change is not None:
-                if stability is not None:
-                    raise ValueError(
-                        "stability must not be specified when using protected_change."
-                    )
-                if grouping_column is not None:
-                    raise ValueError(
-                        "grouping_column must not be specified when using"
-                        " protected_change."
-                    )
-                self._private_sources[source_id] = _PrivateSourceTuple(
-                    dataframe, protected_change, domain
-                )
-                return self
-
-            if stability is None:
-                warn(
-                    (
-                        "Using a default for protected_change is deprecated. Future"
-                        " code should explicitly specify protected_change=AddOneRow()"
-                    ),
-                    DeprecationWarning,
-                )
-                if grouping_column is None:
-                    protected_change = AddOneRow()
-                else:
-                    warn(
-                        (
-                            "Providing a grouping_column parameter instead of a"
-                            " protected_change parameter is deprecated"
-                        ),
-                        DeprecationWarning,
-                    )
-                    protected_change = AddMaxRowsInMaxGroups(grouping_column, 1, 1)
-                    grouping_column = None
-            else:
-                warn(
-                    "Providing a stability instead of a protected_change is deprecated",
-                    DeprecationWarning,
-                )
-                if stability < 1:
-                    raise ValueError("Stability must be a positive integer.")
-
-                if grouping_column is None:
-                    if not isinstance(stability, int):
-                        raise ValueError(
-                            "stability must be an integer when no grouping column is"
-                            " specified"
-                        )
-                    protected_change = AddMaxRows(stability)
-                else:
-                    warn(
-                        (
-                            "Providing a grouping_column parameter instead of a"
-                            " protected_change parameter is deprecated"
-                        ),
-                        DeprecationWarning,
-                    )
-                    if not isinstance(stability, (int, float)):
-                        raise ValueError("stability must be a numeric value")
-                    protected_change = AddMaxRowsInMaxGroups(
-                        grouping_column, max_groups=1, max_rows_per_group=stability
-                    )
-                    grouping_column = None
-
-            self._private_sources[source_id] = _PrivateSourceTuple(
-                dataframe, protected_change, domain
-            )
-            return self
-
-        def with_public_dataframe(
-            self, source_id: str, dataframe: DataFrame
-        ) -> "Session.Builder":
-            """Adds a Spark DataFrame as a public source.
-
-            Not all Spark column types are supported in public sources; see
-            :data:`SUPPORTED_SPARK_TYPES` for information about which types are
-            supported.
-
-            Args:
-                source_id: Source id for the public data source.
-                dataframe: Public DataFrame corresponding to the source id.
-            """
-            _assert_is_identifier(source_id)
-            if source_id in self._private_sources or source_id in self._public_sources:
-                raise ValueError(f"Duplicate source id: '{source_id}'")
-            dataframe = coerce_spark_schema_or_fail(dataframe)
-            self._public_sources[source_id] = dataframe
-            return self
-
-        def with_id_space(self, id_space: str) -> "Session.Builder":
-            """Creates an identifier space for the session.
-
-            This defines a space of identifiers that map 1-to-1 to the
-            identifiers being protected by a table with the
-            :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected
-            change. Any table with such a protected change must be a member of
-            some identifier space.
-
-            Args:
-                id_space: The name of the identifier space.
-            """
-            _assert_is_identifier(id_space)
-            if id_space in self._id_spaces:
-                raise ValueError(
-                    f"This Builder already has an ID space of the name: {id_space}."
-                )
-            self._id_spaces.append(id_space)
-            return self
-
     def __init__(
-        self,
-        accountant: PrivacyAccountant,
-        public_sources: Dict[str, DataFrame],
-        compiler: Optional[QueryExprCompiler] = None,
+        self, accountant: PrivacyAccountant, public_sources: Dict[str, DataFrame]
     ) -> None:
         """Initializes a DP session from a queryable.
 
-        This constructor is not intended to be used directly. Use
-        :class:`Session.Builder` or ``from_`` constructors instead.
+        .. warning::
+            This constructor is not intended to be used directly. Use
+            :class:`Session.Builder` or ``from_`` constructors instead.
         """
         # pylint: disable=pointless-string-statement
         """
         Args documented for internal use.
             accountant: A PrivacyAccountant.
             public_sources: The public data for the queries.
                 Provided as a dictionary {source_id: dataframe}
-            compiler: Compiles queries into Measurements,
-                which the queryable uses for evaluation.
         """
         # ensure the session is created with java 11
         try:
             check_java11()
         except SparkConfigError as exc:
             raise RuntimeError(
                 """It looks like the configuration of your Spark session is
@@ -496,49 +314,37 @@
              these options if you import it before you build your Spark session. For
              troubleshooting information, see our Spark topic guide:
              https://docs.tmlt.dev/analytics/latest/topic-guides/spark.html """
             ) from exc
 
         check_type("accountant", accountant, PrivacyAccountant)
         check_type("public_sources", public_sources, Dict[str, DataFrame])
-        check_type("compiler", compiler, Optional[QueryExprCompiler])
 
         self._accountant = accountant
 
         if not isinstance(self._accountant.output_measure, (PureDP, ApproxDP, RhoZCDP)):
             raise ValueError("Accountant is not using PureDP, ApproxDP, or RhoZCDP.")
         if not isinstance(self._accountant.input_metric, DictMetric):
             raise ValueError("The input metric to a session must be a DictMetric.")
         if not isinstance(self._accountant.input_domain, DictDomain):
             raise ValueError("The input domain to a session must be a DictDomain.")
         self._public_sources = public_sources
-        if compiler is None:
-            compiler = QueryExprCompiler(output_measure=self._accountant.output_measure)
-        if self._accountant.output_measure != compiler.output_measure:
-            raise ValueError(
-                "PrivacyAccountant's output measure is"
-                f" {self._accountant.output_measure}, but compiler output measure is"
-                f" {compiler.output_measure}."
-            )
-        self._compiler = compiler
         self._table_constraints: Dict[Identifier, List[Constraint]] = {
             NamedTable(t): [] for t in self.private_sources
         }
 
     # pylint: disable=line-too-long
     @classmethod
     @typechecked
     def from_dataframe(
         cls,
         privacy_budget: PrivacyBudget,
         source_id: str,
         dataframe: DataFrame,
-        stability: Optional[Union[int, float]] = None,
-        grouping_column: Optional[str] = None,
-        protected_change: Optional[ProtectedChange] = None,
+        protected_change: ProtectedChange,
     ) -> "Session":
         """Initializes a DP session from a Spark dataframe.
 
         Only one private data source is supported with this initialization
         method; if you need multiple data sources, use
         :class:`~tmlt.analytics.session.Session.Builder`.
 
@@ -576,32 +382,26 @@
             {'A': 'VARCHAR', 'B': 'INTEGER', 'X': 'INTEGER'}
 
         Args:
             privacy_budget: The total privacy budget allocated to this session.
             source_id: The source id for the private source dataframe.
             dataframe: The private source dataframe to perform queries on,
                 corresponding to the `source_id`.
-            stability: Deprecated: use ``protected_change`` instead, see
-                :ref:`changelog<changelog#protected-change>`
-            grouping_column: Deprecated: use ``protected_change`` instead, see
-                :ref:`changelog<changelog#protected-change>`
             protected_change: A
                 :class:`~tmlt.analytics.protected_change.ProtectedChange`
                 specifying what changes to the input data the resulting
                 :class:`Session` should protect.
         """
         # pylint: enable=line-too-long
         session_builder = (
             Session.Builder()
             .with_privacy_budget(privacy_budget=privacy_budget)
             .with_private_dataframe(
                 source_id=source_id,
                 dataframe=dataframe,
-                stability=stability,
-                grouping_column=grouping_column,
                 protected_change=protected_change,
             )
         )
         if isinstance(protected_change, AddRowsWithID):
             session_builder.with_id_space(protected_change.id_space)
         return session_builder.build()
 
@@ -614,44 +414,31 @@
         relation: NeighboringRelation,
     ) -> "Session":
         """Initializes a DP session using the provided :class:`NeighboringRelation`.
 
         Args:
             privacy_budget: The total privacy budget allocated to this session.
             private_sources: The private data to be used in the session.
-                Provided as a dictionary {source_id: Dataframe}.
+                Provided as a dictionary {source_id: DataFrame}.
             relation: the :class:`NeighboringRelation` to be used in the session.
         """
         # pylint: disable=protected-access
         output_measure: Union[PureDP, ApproxDP, RhoZCDP]
         sympy_budget: sp.Expr
         if isinstance(privacy_budget, PureDPBudget):
             output_measure = PureDP()
             sympy_budget = privacy_budget._epsilon.expr
         elif isinstance(privacy_budget, ApproxDPBudget):
             output_measure = ApproxDP()
             if privacy_budget.is_infinite:
-                warn(
-                    (
-                        "The use of ApproxDP is not yet fully supported. Because you"
-                        " selected an infinite ApproxDP budget, your session will be"
-                        " initialized with PureDP using an infinite epsilon budget."
-                    ),
-                    UserWarning,
-                )
                 sympy_budget = (
                     ExactNumber.from_float(float("inf"), round_up=False).expr,
-                    0,
+                    1,
                 )
             else:
-                warn(
-                    "The use of ApproxDP is not yet fully supported. Your session"
-                    " will be initialized with PureDP using the epsilon provided.",
-                    UserWarning,
-                )
                 sympy_budget = (
                     privacy_budget._epsilon.expr,
                     privacy_budget._delta.expr,
                 )
         elif isinstance(privacy_budget, RhoZCDPBudget):
             output_measure = RhoZCDP()
             sympy_budget = privacy_budget._rho.expr
@@ -666,44 +453,42 @@
 
         # Wrap relation in a Conjunction so that output is appropriate for
         # PrivacyAccountant
         domain, metric, distance, dataframes = Conjunction(relation).accept(
             NeighboringRelationCoreVisitor(private_sources, output_measure)
         )
 
-        compiler = QueryExprCompiler(output_measure=output_measure)
-
         measurement = SequentialComposition(
             input_domain=domain,
             input_metric=metric,
             d_in=distance,
             privacy_budget=sympy_budget,
             output_measure=output_measure,
         )
         accountant = PrivacyAccountant.launch(measurement, dataframes)
-        return Session(accountant=accountant, public_sources={}, compiler=compiler)
+        return Session(accountant=accountant, public_sources={})
 
     @property
     def private_sources(self) -> List[str]:
-        """Returns the ids of the private sources."""
+        """Returns the IDs of the private sources."""
         table_refs = find_named_tables(self._input_domain)
         return [
             t.identifier.name
             for t in table_refs
             if isinstance(t.identifier, NamedTable)
         ]
 
     @property
     def public_sources(self) -> List[str]:
-        """Returns the ids of the public sources."""
+        """Returns the IDs of the public sources."""
         return list(self._public_sources)
 
     @property
     def public_source_dataframes(self) -> Dict[str, DataFrame]:
-        """Returns a dictionary of public source dataframes."""
+        """Returns a dictionary of public source DataFrames."""
         return self._public_sources
 
     @property
     def remaining_privacy_budget(self) -> PrivacyBudget:
         """Returns the remaining privacy_budget left in the session.
 
         The type of the budget (e.g., PureDP or rho-zCDP) will be the same as
@@ -742,19 +527,24 @@
             raise AssertionError(
                 "Session accountant's input metric has an incorrect type. This is "
                 "probably a bug; please let us know about it so we can "
                 "fix it!"
             )
         return self._accountant.input_metric
 
+    @property
+    def _output_measure(self) -> Union[PureDP, ApproxDP, RhoZCDP]:
+        """Returns the output measure of the underlying accountant."""
+        return self._accountant.output_measure
+
     def describe(
         self,
         obj: Optional[Union[QueryExpr, QueryBuilder, GroupedQueryBuilder, str]] = None,
     ) -> None:
-        """Describe a Session, table, or query.
+        """Describes this session, or one of its tables, or the result of a query.
 
         If ``obj`` is not specified, ``session.describe()`` will describe the
         Session and all of the tables it contains.
 
         If ``obj`` is a :class:`~tmlt.analytics.query_builder.QueryBuilder` or
         :class:`~tmlt.analytics.query_expr.QueryExpr`, ``session.describe(obj)``
         will describe the table that would result from that query if it were
@@ -816,15 +606,15 @@
             print(self._describe_query_obj(obj.query_expr))
         elif isinstance(obj, str):
             print(self._describe_query_obj(QueryBuilder(obj).query_expr))
         else:
             assert_never(obj)
 
     def _describe_self(self) -> str:
-        """Describe the current state of this session."""
+        """Describes the current state of this session."""
         out = []
         state = self._accountant.state
         if state == PrivacyAccountantState.ACTIVE:
             # Don't add anything to output if the session is active
             pass
         elif state == PrivacyAccountantState.RETIRED:
             out.append("This session has been stopped, and can no longer be used.")
@@ -897,19 +687,20 @@
         self, query_obj: Union[QueryExpr, GroupedQueryBuilder]
     ) -> str:
         """Build a description of a query object."""
         if isinstance(query_obj, GroupedQueryBuilder):
             expr = query_obj._query_expr  # pylint: disable=protected-access
         else:
             expr = query_obj
-        schema = self._compiler.query_schema(expr, self._catalog)
+        compiler = QueryExprCompiler(self._output_measure)
+        schema = compiler.query_schema(expr, self._catalog)
         schema_desc = _describe_schema(schema)
         constraints: Optional[List[Constraint]] = None
         try:
-            constraints = self._compiler.build_transformation(
+            constraints = compiler.build_transformation(
                 query=expr,
                 input_domain=self._input_domain,
                 input_metric=self._input_metric,
                 public_sources=self._public_sources,
                 catalog=self._catalog,
                 table_constraints=self._table_constraints,
             )[2]
@@ -1086,15 +877,15 @@
 
     # pylint: disable=line-too-long
     @typechecked
     def add_public_dataframe(self, source_id: str, dataframe: DataFrame):
         """Adds a public data source to the session.
 
         Not all Spark column types are supported in public sources; see
-        :data:`SUPPORTED_SPARK_TYPES` for information about which types are
+        :data:`~.session.SUPPORTED_SPARK_TYPES` for information about which types are
         supported.
 
         ..
             >>> # Get data
             >>> spark = SparkSession.builder.getOrCreate()
             >>> private_data = spark.createDataFrame(
             ...     pd.DataFrame(
@@ -1131,50 +922,50 @@
             {'A': 'VARCHAR', 'C': 'INTEGER'}
 
         Args:
             source_id: The name of the public data source.
             dataframe: The public data source corresponding to the ``source_id``.
         """
         # pylint: enable=line-too-long
-        _assert_is_identifier(source_id)
+        assert_is_identifier(source_id)
         if source_id in self.public_sources or source_id in self.private_sources:
             raise ValueError(f"This session already has a table named '{source_id}'.")
         dataframe = coerce_spark_schema_or_fail(dataframe)
         self._public_sources[source_id] = dataframe
 
-    def _compile_and_get_budget(
+    def _compile_and_get_info(
         self, query_expr: QueryExpr, privacy_budget: PrivacyBudget
-    ) -> Tuple[Measurement, PrivacyBudget]:
+    ) -> Tuple[Measurement, PrivacyBudget, NoiseInfo]:
         """Pre-processing needed for evaluate() and _noise_info()."""
         check_type("query_expr", query_expr, QueryExpr)
         check_type("privacy_budget", privacy_budget, PrivacyBudget)
 
         is_approxDP_session = self._accountant.output_measure == ApproxDP()
 
-        # If pureDP session, and approxDP budget, let Core handle the error.
+        # If PureDP session, and ApproxDP budget, let Core handle the error.
         if is_approxDP_session and isinstance(privacy_budget, PureDPBudget):
             privacy_budget = ApproxDPBudget(privacy_budget.value, 0)
 
         self._validate_budget_type_matches_session(privacy_budget)
         if privacy_budget in [PureDPBudget(0), ApproxDPBudget(0, 0), RhoZCDPBudget(0)]:
             raise ValueError("You need a non-zero privacy budget to evaluate a query.")
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
 
-        measurement = self._compiler(
+        measurement, noise_info = QueryExprCompiler(self._output_measure)(
             queries=[query_expr],
             privacy_budget=adjusted_budget,
             stability=self._accountant.d_in,
             input_domain=self._input_domain,
             input_metric=self._input_metric,
             public_sources=self._public_sources,
             catalog=self._catalog,
             table_constraints=self._table_constraints,
         )
-        return (measurement, adjusted_budget)
+        return measurement, adjusted_budget, noise_info
 
     def _noise_info(
         self, query_expr: QueryExpr, privacy_budget: PrivacyBudget
     ) -> List[Dict[str, Any]]:
         """Get noise information about a query.
 
         ..
@@ -1205,25 +996,25 @@
             >>> count_info = sess._noise_info(
             ...     query_expr=count_query,
             ...     privacy_budget=PureDPBudget(0.5),
             ... )
             >>> count_info # doctest: +NORMALIZE_WHITESPACE
             [{'noise_mechanism': <_NoiseMechanism.GEOMETRIC: 2>, 'noise_parameter': 2}]
         """
-        measurement, _ = self._compile_and_get_budget(query_expr, privacy_budget)
-        return _noise_from_measurement(measurement)
+        _, _, noise_info = self._compile_and_get_info(query_expr, privacy_budget)
+        return list(iter(noise_info))
 
     # pylint: disable=line-too-long
     def evaluate(
         self, query_expr: QueryExpr, privacy_budget: PrivacyBudget
     ) -> DataFrame:
         """Answers a query within the given privacy budget and returns a Spark dataframe.
 
         The type of privacy budget that you use must match the type your Session was
-        initialized with (i.e., you cannot evaluate a query using rho-zCDPBudget if
+        initialized with (i.e., you cannot evaluate a query using RhoZCDPBudget if
         the Session was initialized with a PureDPBudget, and vice versa).
 
         ..
             >>> from tmlt.analytics.keyset import KeySet
             >>> # Get data
             >>> spark = SparkSession.builder.getOrCreate()
             >>> data = spark.createDataFrame(
@@ -1264,20 +1055,19 @@
             DataFrame[B_sum: bigint]
 
         Args:
             query_expr: One query expression to answer.
             privacy_budget: The privacy budget used for the query.
         """
         # pylint: enable=line-too-long
-        measurement, adjusted_budget = self._compile_and_get_budget(
+        measurement, adjusted_budget, _ = self._compile_and_get_info(
             query_expr, privacy_budget
         )
         self._activate_accountant()
 
-        # check if type of self._accountant.privacy_budget matches adjusted_budget value
         if xor(
             isinstance(self._accountant.privacy_budget, tuple),
             isinstance(adjusted_budget.value, tuple),
         ):
             raise ValueError(
                 "Expected type of adjusted_budget to match type of accountant's privacy"
                 f" budget ({type(self._accountant.privacy_budget)}), but instead"
@@ -1324,15 +1114,15 @@
             ) from e
 
     # pylint: disable=line-too-long
     @typechecked
     def create_view(
         self, query_expr: Union[QueryExpr, QueryBuilder], source_id: str, cache: bool
     ):
-        """Create a new view from a transformation and possibly cache it.
+        """Creates a new view from a transformation and possibly cache it.
 
         ..
             >>> # Get data
             >>> spark = SparkSession.builder.getOrCreate()
             >>> private_data = spark.createDataFrame(
             ...     pd.DataFrame(
             ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
@@ -1385,25 +1175,28 @@
 
         Args:
             query_expr: A query that performs a transformation.
             source_id: The name, or unique identifier, of the view.
             cache: Whether or not to cache the view.
         """
         # pylint: enable=line-too-long
-        _assert_is_identifier(source_id)
+        assert_is_identifier(source_id)
         self._activate_accountant()
         if source_id in self.private_sources or source_id in self.public_sources:
             raise ValueError(f"Table '{source_id}' already exists.")
 
         if isinstance(query_expr, QueryBuilder):
             query_expr = query_expr.query_expr
 
         if not isinstance(query_expr, QueryExpr):
             raise ValueError("query_expr must be of type QueryBuilder or QueryExpr.")
-        transformation, ref, constraints = self._compiler.build_transformation(
+
+        transformation, ref, constraints = QueryExprCompiler(
+            self._output_measure
+        ).build_transformation(
             query=query_expr,
             input_domain=self._input_domain,
             input_metric=self._input_metric,
             public_sources=self._public_sources,
             catalog=self._catalog,
             table_constraints=self._table_constraints,
         )
@@ -1452,22 +1245,178 @@
 
         transformation = delete_table(
             base_transformation=unpersist_source, base_ref=ref
         )
         self._accountant.transform_in_place(transformation)
         self._table_constraints.pop(ref.identifier, None)
 
+    def _create_partition_constraint(
+        self,
+        constraint: MaxGroupsPerID,
+        child_transformation: Transformation,
+        child_ref: TableReference,
+    ) -> Tuple[Transformation, TableReference]:
+        """Creates the constraint needed for partitioning on an id column.
+
+        This is a helper method for :meth:`~._create_partition_transformation`.
+
+        It is pulled out to make it easier to override in subclasses which change the
+        behavior of constraints, not for code maintainability.
+        """
+        return constraint._enforce(  # pylint: disable=protected-access
+            child_transformation=child_transformation,
+            child_ref=child_ref,
+            update_metric=True,
+            use_l2=isinstance(self._output_measure, RhoZCDP),
+        )
+
+    def _create_partition_transformation(
+        self,
+        source_id: str,
+        column: str,
+        splits: Union[Dict[str, str], Dict[str, int]],
+    ) -> Transformation:
+        """Creates a transformation for partitioning a table.
+
+        Helper method for :meth:`~.partition_and_create`.
+
+        ..
+            >>> # Get data
+            >>> spark = SparkSession.builder.getOrCreate()
+            >>> data = spark.createDataFrame(
+            ...     pd.DataFrame(
+            ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
+            ...     )
+            ... )
+            >>> # Create Session
+            >>> sess = Session.from_dataframe(
+            ...     privacy_budget=PureDPBudget(1),
+            ...     source_id="my_private_data",
+            ...     dataframe=data,
+            ...     protected_change=AddOneRow(),
+            ... )
+
+        Example:
+            >>> sess.private_sources
+            ['my_private_data']
+            >>> sess.get_schema("my_private_data").column_types # doctest: +NORMALIZE_WHITESPACE
+            {'A': 'VARCHAR', 'B': 'INTEGER', 'X': 'INTEGER'}
+            >>> sess.remaining_privacy_budget
+            PureDPBudget(epsilon=1)
+            >>> # Partition the Session
+            >>> transformation = sess._create_partition_transformation(
+            ...     "my_private_data",
+            ...     column="A",
+            ...     splits={"part0":"0", "part1":"1"}
+            ... )
+            >>> transformation.input_domain == sess._input_domain
+            True
+            >>> transformation.input_metric == sess._input_metric
+            True
+            >>> transformation.output_domain
+            ListDomain(element_domain=SparkDataFrameDomain(schema={'A': SparkStringColumnDescriptor(allow_null=True), 'B': SparkIntegerColumnDescriptor(allow_null=True, size=64), 'X': SparkIntegerColumnDescriptor(allow_null=True, size=64)}), length=2)
+            >>> transformation.output_metric
+            SumOf(inner_metric=SymmetricDifference())
+
+        Args:
+            source_id: The private source to partition
+            column: The name of the column partitioning on.
+            splits: Mapping of split name to value of partition.
+                Split name is ``source_id`` in new session.
+        """
+        # First we need to check whether the table can be partitioned
+        table_ref = find_reference(source_id, self._input_domain)
+        if table_ref is None:
+            if source_id in self.public_sources:
+                raise ValueError(
+                    f"Table '{source_id}' is a public table, "
+                    "and you cannot partition_and_create on a public table."
+                )
+            raise KeyError(
+                f"Private table '{source_id}' does not exist. "
+                f"Available private tables are: {', '.join(self.private_sources)}"
+            )
+        # Next we need to check if the table has ID columns. If so, it requires
+        # a MaxGroupsPerID constraint.
+        metric = lookup_metric(self._input_metric, table_ref)
+        has_id_column = isinstance(metric, IfGroupedBy) and isinstance(
+            metric.inner_metric, SymmetricDifference
+        )
+        transformation: Transformation = Identity(
+            domain=self._input_domain, metric=self._input_metric
+        )
+        if has_id_column:
+            # look for the expected constraint
+            constraint = next(
+                (
+                    c
+                    for c in self._table_constraints.get(table_ref.identifier, [])
+                    if isinstance(c, MaxGroupsPerID) and c.grouping_column == column
+                ),
+                None,
+            )
+            if constraint is None:
+                raise ValueError(
+                    "You must create a MaxGroupsPerID constraint before using"
+                    " partition_and_create on tables with the AddRowsWithID"
+                    " protected change."
+                )
+            # if found, create the transformation enforcing it
+            transformation, table_ref = self._create_partition_constraint(
+                constraint, transformation, table_ref
+            )
+        # Get the table we will split on from the dictionary
+        transformation = get_table_from_ref(transformation, table_ref)
+        if not isinstance(
+            transformation.output_metric, (IfGroupedBy, SymmetricDifference)
+        ):
+            raise AssertionError(
+                "Transformation has an unexpected output metric. This is "
+                "probably a bug; please let us know about it so we can fix it!"
+            )
+        transformation_domain = cast(SparkDataFrameDomain, transformation.output_domain)
+
+        try:
+            attr_type = transformation_domain.schema[column]
+        except KeyError as e:
+            raise KeyError(
+                f"'{column}' not present in transformed DataFrame's columns; "
+                "schema of transformed DataFrame is "
+                f"{spark_dataframe_domain_to_analytics_columns(transformation_domain)}"
+            ) from e
+
+        # Actual type is Union[List[Tuple[str, ...]], List[Tuple[int, ...]]]
+        # but mypy doesn't like that.
+        split_vals: List[Tuple[Union[str, int], ...]] = []
+        for split_val in splits.values():
+            if not attr_type.valid_py_value(split_val):
+                raise TypeError(
+                    f"'{column}' column is of type '{attr_type.data_type}'; "
+                    f"'{attr_type.data_type}' column not compatible with splits "
+                    f"value type '{type(split_val).__name__}'"
+                )
+            split_vals.append((split_val,))
+
+        transformation |= PartitionByKeys(
+            input_domain=transformation_domain,
+            input_metric=transformation.output_metric,
+            use_l2=isinstance(self._output_measure, RhoZCDP),
+            keys=[column],
+            list_values=split_vals,
+        )
+        return transformation
+
     # pylint: disable=line-too-long
     @typechecked
     def partition_and_create(
         self,
         source_id: str,
         privacy_budget: PrivacyBudget,
-        column: Optional[str] = None,
-        splits: Optional[Union[Dict[str, str], Dict[str, int]]] = None,
+        column: str,
+        splits: Union[Dict[str, str], Dict[str, int]],
     ) -> Dict[str, "Session"]:
         """Returns new sessions from a partition mapped to split name/``source_id``.
 
         The type of privacy budget that you use must match the type your Session
         was initialized with (i.e., you cannot use a
         :class:`~tmlt.analytics.privacy_budget.RhoZCDPBudget` to partition your
         Session if the Session was created using a
@@ -1547,26 +1496,15 @@
             source_id: The private source to partition.
             privacy_budget: Amount of privacy budget to pass to each new session.
             column: The name of the column partitioning on.
             splits: Mapping of split name to value of partition.
                 Split name is ``source_id`` in new session.
         """
         # pylint: enable=line-too-long
-        if splits is None:
-            raise ValueError(
-                "You must provide a dictionary mapping split names (new source_ids) to"
-                " values on which to partition"
-            )
         # If you remove this if-block, mypy will complain
-        if column is None:
-            raise AssertionError(
-                "column is None, even though either column or attr_name were provided."
-                " This is probably a bug; please let us know about it so we can fix it!"
-            )
-
         if not (
             isinstance(self._accountant.privacy_budget, ExactNumber)
             or is_exact_number_tuple(self._accountant.privacy_budget)
         ):
             raise AssertionError(
                 "Unable to convert privacy budget of type"
                 f" {type(self._accountant.privacy_budget)} to float or floats. This is"
@@ -1574,147 +1512,37 @@
             )
 
         is_approxDP_session = isinstance(self._accountant.output_measure, ApproxDP)
         if is_approxDP_session and isinstance(privacy_budget, PureDPBudget):
             privacy_budget = ApproxDPBudget(privacy_budget.value, 0)
 
         self._validate_budget_type_matches_session(privacy_budget)
-        self._activate_accountant()
-
-        transformation: Transformation = Identity(
-            domain=self._input_domain, metric=self._input_metric
-        )
-        table_ref = find_reference(source_id, self._input_domain)
-        if table_ref is None:
-            if source_id in self.public_sources:
-                raise ValueError(
-                    f"Table '{source_id}' is a public table, which cannot have an "
-                    "ID space."
-                )
-            raise KeyError(
-                f"Private table '{source_id}' does not exist. "
-                f"Available private tables are: {', '.join(self.private_sources)}"
-            )
-
-        # Either DictMetric or AddRemoveKeys
-        parent_metric = lookup_metric(self._input_metric, table_ref.parent)
-        table_has_ids: bool = isinstance(parent_metric, AddRemoveKeysMetric)
-        if table_has_ids:
-            parent_last_element = table_ref.parent.identifier
-            constraints = self._table_constraints.get(NamedTable(source_id))
-            if constraints is None:
-                raise AssertionError(
-                    f"Table '{source_id}' has no constraints. This is probably a"
-                    " bug; please let us know about it so we can fix it!"
-                )
-
-            constraint = next(
-                (
-                    c
-                    for c in constraints
-                    if (isinstance(c, MaxGroupsPerID) and c.grouping_column == column)
-                ),
-                None,
-            )
-
-            if constraint is None:
-                raise ValueError(
-                    "You must create MaxGroupsPerID constraint before using"
-                    " partition_and_create on tables with the AddRowsWithID"
-                    " protected change."
-                )
-
-            (
-                transformation,
-                table_ref,
-            ) = constraint._enforce(  # pylint: disable=protected-access
-                child_transformation=transformation,
-                child_ref=table_ref,
-                update_metric=True,
-                use_l2=isinstance(self._compiler.output_measure, RhoZCDP),
-            )
-        transformation = get_table_from_ref(transformation, table_ref)
-        if not isinstance(
-            transformation.output_metric, (IfGroupedBy, SymmetricDifference)
-        ):
-            raise AssertionError(
-                "Transformation has an unrecognized output metric. This is "
-                "probably a bug; please let us know about it so we can fix it!"
-            )
-        transformation_domain = cast(SparkDataFrameDomain, transformation.output_domain)
-
-        try:
-            attr_type = transformation_domain.schema[column]
-        except KeyError as e:
-            raise KeyError(
-                f"'{column}' not present in transformed dataframe's columns; "
-                "schema of transformed dataframe is "
-                f"{spark_dataframe_domain_to_analytics_columns(transformation_domain)}"
-            ) from e
 
+        # Check that new source names will be valid before using any budget
         new_sources = []
-        # Actual type is Union[List[Tuple[str, ...]], List[Tuple[int, ...]]]
-        # but mypy doesn't like that.
-        split_vals: List[Tuple[Union[str, int], ...]] = []
-        for split_name, split_val in splits.items():
+        for split_name in splits:
             if not split_name.isidentifier():
                 raise ValueError(
                     "The string passed as split name must be a valid Python identifier:"
                     " it can only contain alphanumeric letters (a-z) and (0-9), or"
                     " underscores (_), and it cannot start with a number, or contain"
                     " any spaces."
                 )
-            if not attr_type.valid_py_value(split_val):
-                raise TypeError(
-                    f"'{column}' column is of type '{attr_type.data_type}'; "
-                    f"'{attr_type.data_type}' column not compatible with splits "
-                    f"value type '{type(split_val).__name__}'"
-                )
             new_sources.append(split_name)
-            split_vals.append((split_val,))
-
-        element_metric: Union[IfGroupedBy, SymmetricDifference]
-        if isinstance(transformation.output_metric, SymmetricDifference) or (
-            isinstance(transformation.output_metric, IfGroupedBy)
-            and column != transformation.output_metric.column
-        ):
-            element_metric = transformation.output_metric
-        elif (
-            isinstance(transformation.output_metric, IfGroupedBy)
-            and column == transformation.output_metric.column
-        ):
-            assert isinstance(
-                transformation.output_metric.inner_metric,
-                (IfGroupedBy, RootSumOfSquared, SumOf),
-            )
-            assert isinstance(
-                transformation.output_metric.inner_metric.inner_metric,
-                (IfGroupedBy, SymmetricDifference),
-            )
-            element_metric = transformation.output_metric.inner_metric.inner_metric
-        else:
-            raise AssertionError(
-                "Transformation has an unrecognized output metric. This is "
-                "probably a bug; please let us know about it so  we can fix it!"
-            )
-
-        partition_transformation = PartitionByKeys(
-            input_domain=transformation_domain,
-            input_metric=transformation.output_metric,
-            use_l2=isinstance(self._compiler.output_measure, RhoZCDP),
-            keys=[column],
-            list_values=split_vals,
-        )
-        chained_partition = transformation | partition_transformation
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
+        partition_transformation = self._create_partition_transformation(
+            source_id=source_id, column=column, splits=splits
+        )
 
+        # Split the accountants
+        self._activate_accountant()
         try:
             new_accountants = self._accountant.split(
-                chained_partition, privacy_budget=adjusted_budget.value
+                partition_transformation, privacy_budget=adjusted_budget.value
             )
         except InactiveAccountantError as e:
             raise RuntimeError(
                 "This session is no longer active. Either it was manually stopped"
                 "with session.stop(), or it was stopped indirectly by the "
                 "activity of other sessions. See partition_and_create "
                 "for more information."
@@ -1724,43 +1552,44 @@
                 err.requested_budget, err.remaining_budget, privacy_budget
             )
             raise RuntimeError(
                 "Cannot perform this partition without exceeding "
                 "the Session privacy budget." + msg
             ) from err
 
-        for i, source in enumerate(new_sources):
-            if table_has_ids:
-                create_dict = CreateDictFromValue(
-                    input_domain=transformation_domain,
-                    input_metric=element_metric,
+        # We now have split accountants, and names for each.
+        # The only remaining steps are to:
+        # 1. Update the accountants to have the standard nested dictionary format
+        # 2. Return new sessions from the accountants
+        new_sessions = {}
+        for accountant, source in zip(new_accountants, new_sources):
+            id_space = self.get_id_space(source_id)
+            if id_space is not None:
+                # Create the inner dictionary for the id space
+                nested_dict_transformation: Transformation = CreateDictFromValue(
+                    input_domain=accountant.input_domain,
+                    input_metric=accountant.input_metric,
                     key=NamedTable(source),
                     use_add_remove_keys=True,
                 )
-                dict_transformation_wrapper = create_dict | CreateDictFromValue(
-                    input_domain=create_dict.output_domain,
-                    input_metric=create_dict.output_metric,
-                    key=parent_last_element,
+                # Create the outer dictionary
+                nested_dict_transformation |= CreateDictFromValue(
+                    input_domain=nested_dict_transformation.output_domain,
+                    input_metric=nested_dict_transformation.output_metric,
+                    key=TableCollection(id_space),
                 )
             else:
-                dict_transformation_wrapper = CreateDictFromValue(
-                    input_domain=transformation_domain,
-                    input_metric=element_metric,
+                # Only has the outer dictionary
+                nested_dict_transformation = CreateDictFromValue(
+                    input_domain=accountant.input_domain,
+                    input_metric=accountant.input_metric,
                     key=NamedTable(source),
                 )
-
-            new_accountants[i].queue_transformation(
-                transformation=dict_transformation_wrapper
-            )
-
-        new_sessions = {}
-        for new_accountant, source in zip(new_accountants, new_sources):
-            new_sessions[source] = Session(
-                new_accountant, self._public_sources, self._compiler
-            )
+            accountant.queue_transformation(nested_dict_transformation)
+            new_sessions[source] = Session(accountant, self._public_sources)
         return new_sessions
 
     def _process_requested_budget(self, privacy_budget: PrivacyBudget) -> PrivacyBudget:
         """Process the requested budget to accommodate floating point imprecision.
 
         Args:
             privacy_budget: The requested budget.
@@ -1855,32 +1684,18 @@
                 "Activating a session that is waiting for its children "
                 "(created with partition_and_create) to finish "
                 "may cause unexpected behavior."
             )
         self._accountant.force_activate()
 
     def stop(self) -> None:
-        """Close out this session, allowing other sessions to become active."""
+        """Closes out this session, allowing other sessions to become active."""
         self._accountant.retire()
 
 
-def _assert_is_identifier(source_id: str):
-    """Checks that the ``source_id`` is a valid Python identifier.
-
-    Args:
-        source_id: The name of the dataframe or transformation.
-    """
-    if not source_id.isidentifier():
-        raise ValueError(
-            "The string passed as source_id must be a valid Python identifier: it can"
-            " only contain alphanumeric letters (a-z) and (0-9), or underscores (_),"
-            " and it cannot start with a number, or contain any spaces."
-        )
-
-
 def _describe_schema(schema: Schema) -> List[str]:
     """Get a list of strings to print that describe columns of a schema.
 
     This is a list so that it's easy to append tabs to each line.
     """
     description = ["Columns:"]
     # We actually care about the maximum length of the column name
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/truncation_strategy.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/truncation_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Defines strategies for performing truncation in private joins."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2023
+# Copyright Tumult Labs 2024
 
 from abc import ABC
 from dataclasses import dataclass
 
 from typeguard import check_type
 
 
@@ -23,15 +23,15 @@
       - :math:`T_{left}` and :math:`T_{right}` are the truncation thresholds for the
         left and right truncation strategies, respectively. This value is 1 for
         ``DropNonUnique``.
       - :math:`S_{left}` and :math:`S_{right}` are the stability of the left and right
         truncation strategies, respectively. This value is 2 for ``DropExcess`` and 1
         for ``DropNonUnique``.
       - :math:`M_{left}` and :math:`M_{right}` are the ``max_rows`` parameters of the
-        ``AddMaxRows`` protected changes of the the left and right tables, respectively.
+        ``AddMaxRows`` protected changes of the left and right tables, respectively.
 
     """
 
     class Type(ABC):
         """Type of TruncationStrategy variants."""
 
     @dataclass(frozen=True)
```

### Comparing `tmlt_analytics-0.8.3/tmlt/analytics/utils.py` & `tmlt_analytics-0.9.0rc5/tmlt/analytics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Utility functions."""
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2024
 
 import atexit
 from textwrap import dedent
 
 import pandas as pd
 from pyspark.sql import SparkSession
 from tmlt.core.utils import cleanup as core_cleanup
 from tmlt.core.utils import configuration
 
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget
+from tmlt.analytics.protected_change import AddOneRow
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.session import Session
 
 
 def cleanup():
     """Clean up the temporary table currently in use.
 
@@ -84,15 +87,18 @@
 
         print("Converting to Spark dataframe... ", end="")
         sdf = spark.createDataFrame(pdf)
         print(" OK")
 
         print("Creating Tumult Analytics session... ", end="")
         session = Session.from_dataframe(
-            privacy_budget=PureDPBudget(1), source_id="private_data", dataframe=sdf
+            privacy_budget=PureDPBudget(1),
+            source_id="private_data",
+            dataframe=sdf,
+            protected_change=AddOneRow(),
         )
         print(" OK")
 
         print("Creating query...", end="")
         query = (
             QueryBuilder("private_data")
             .groupby(KeySet.from_dict({"A": ["a0", "a1", "a2"]}))
```

### Comparing `tmlt_analytics-0.8.3/setup.py` & `tmlt_analytics-0.9.0rc5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,32 +8,32 @@
  'tmlt.analytics.constraints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['sympy>=1.8,<1.10',
- 'tmlt.core>=0.11.5,<0.13.0',
+ 'tmlt.core>=0.12.0,<0.13.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=4.1.0,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['pandas>=1.2.0,<1.4.0',
                              'pyspark[sql]>=3.0.0,<3.4.0'],
  ':python_version >= "3.10" and python_version < "3.11"': ['pandas>=1.4.0,<2.0.0'],
  ':python_version >= "3.11"': ['pandas>=1.5.0,<2.0.0',
                                'pyspark[sql]>=3.4.0,<3.6.0'],
  ':python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.2.0,<2.0.0'],
  ':python_version >= "3.8" and python_version < "3.11"': ['pyspark[sql]>=3.0.0,<3.6.0']}
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.8.3',
+    'version': '0.9.0rc5',
     'description': "Tumult's differential privacy analytics API",
-    'long_description': "[![PyPI - Version](https://img.shields.io/pypi/v/tmlt-analytics?color=006dad)](https://pypi.org/project/tmlt-analytics/) |\n[![Documentation - Latest](https://img.shields.io/badge/documentation-latest-cc3d56)](https://docs.tmlt.dev/analytics/latest/) |\n[![Join our Slack!](https://img.shields.io/badge/Join%20our%20Slack!-634ad3?logo=slack)](https://tmlt.dev/slack)\n\n# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Demo video\n\nWant to see Tumult Analytics in action? Check out this video introducing the\ninterface fundamentals:\n\n[![Screenshot of the demo video](https://img.youtube.com/vi/SNfbYOp0CEs/0.jpg)](https://www.youtube.com/watch?v=SNfbYOp0CEs)\n\nA selection of more advanced features is shown on the second part of this demo,\nin a [separate video](https://www.youtube.com/watch?v=BRUPlfwzHHo).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions, feedback, or feature requests, please reach out to us on [Slack](https://tmlt.dev/slack).\n\n## Contributing\n\nWe do not yet have a process in place to accept external contributions, but we are open to collaboration opportunities.\nIf you are interested in contributing, please let us know [via Slack](https://tmlt.dev/slack).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nTumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nTumult Analytics' documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n",
+    'long_description': "[![PyPI - Version](https://img.shields.io/pypi/v/tmlt-analytics?color=006dad)](https://pypi.org/project/tmlt-analytics/) |\n[![Documentation - Latest](https://img.shields.io/badge/documentation-latest-cc3d56)](https://docs.tmlt.dev/analytics/latest/) |\n[![Join our Slack!](https://img.shields.io/badge/Join%20our%20Slack!-634ad3?logo=slack)](https://tmlt.dev/slack)\n\n# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Demo video\n\nWant to see Tumult Analytics in action? Check out this video introducing the\ninterface fundamentals:\n\n[![Screenshot of the demo video](https://img.youtube.com/vi/SNfbYOp0CEs/0.jpg)](https://www.youtube.com/watch?v=SNfbYOp0CEs)\n\nA selection of more advanced features is shown on the second part of this demo,\nin a [separate video](https://www.youtube.com/watch?v=BRUPlfwzHHo).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions, feedback, or feature requests, please reach out to us on [Slack](https://tmlt.dev/slack).\n\n## Contributing\n\nWe do not yet have a process in place to accept external contributions, but we are open to collaboration opportunities.\nIf you are interested in contributing, please let us know [via Slack](https://tmlt.dev/slack).\n\nSee [CONTRIBUTING.md](https://gitlab.com/tumult-labs/analytics/-/blob/dev/CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nTumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nTumult Analytics' documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tmlt_analytics-0.8.3/PKG-INFO` & `tmlt_analytics-0.9.0rc5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-analytics
-Version: 0.8.3
+Version: 0.9.0rc5
 Summary: Tumult's differential privacy analytics API
 Home-page: https://www.tmlt.dev/
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.12.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -24,15 +24,15 @@
 Requires-Dist: pandas (>=1.2.0,<2.0.0); python_version >= "3.8" and python_version < "3.10"
 Requires-Dist: pandas (>=1.4.0,<2.0.0); python_version >= "3.10" and python_version < "3.11"
 Requires-Dist: pandas (>=1.5.0,<2.0.0); python_version >= "3.11"
 Requires-Dist: pyspark[sql] (>=3.0.0,<3.4.0); python_version < "3.8"
 Requires-Dist: pyspark[sql] (>=3.0.0,<3.6.0); python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: pyspark[sql] (>=3.4.0,<3.6.0); python_version >= "3.11"
 Requires-Dist: sympy (>=1.8,<1.10)
-Requires-Dist: tmlt.core (>=0.11.5,<0.13.0)
+Requires-Dist: tmlt.core (>=0.12.0,<0.13.0)
 Requires-Dist: typeguard (>=2.12.1,<2.13.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Project-URL: Documentation, https://docs.tmlt.dev/analytics/latest
 Project-URL: Repository, https://gitlab.com/tumult-labs/analytics
 Description-Content-Type: text/markdown
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tmlt-analytics?color=006dad)](https://pypi.org/project/tmlt-analytics/) |
@@ -75,15 +75,15 @@
 If you have any questions, feedback, or feature requests, please reach out to us on [Slack](https://tmlt.dev/slack).
 
 ## Contributing
 
 We do not yet have a process in place to accept external contributions, but we are open to collaboration opportunities.
 If you are interested in contributing, please let us know [via Slack](https://tmlt.dev/slack).
 
-See [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.
+See [CONTRIBUTING.md](https://gitlab.com/tumult-labs/analytics/-/blob/dev/CONTRIBUTING.md) for information about installing our development dependencies and running tests.
 
 ## Citing Tumult Analytics
 
 If you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.
 
 ```
 @software{tumultanalyticssoftware,
```

