# Comparing `tmp/google-vizier-0.1.8.tar.gz` & `tmp/google-vizier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-vizier-0.1.8.tar", last modified: Thu Aug 17 21:38:52 2023, max compression
+gzip compressed data, was "google-vizier-0.1.9.tar", last modified: Fri Sep  1 01:04:45 2023, max compression
```

## Comparing `google-vizier-0.1.8.tar` & `google-vizier-0.1.9.tar`

### file list

```diff
@@ -1,364 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.953462 google-vizier-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-17 21:38:28.000000 google-vizier-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-08-17 21:38:52.953462 google-vizier-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-17 21:38:28.000000 google-vizier-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.877461 google-vizier-0.1.8/google_vizier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-08-17 21:38:52.000000 google-vizier-0.1.8/google_vizier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-08-17 21:38:52.000000 google-vizier-0.1.8/google_vizier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 21:38:52.000000 google-vizier-0.1.8/google_vizier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 21:38:52.000000 google-vizier-0.1.8/google_vizier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-17 21:38:52.000000 google-vizier-0.1.8/google_vizier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-17 21:38:52.000000 google-vizier-0.1.8/google_vizier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 21:38:52.953462 google-vizier-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-08-17 21:38:28.000000 google-vizier-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.877461 google-vizier-0.1.8/vizier/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.877461 google-vizier-0.1.8/vizier/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.877461 google-vizier-0.1.8/vizier/_src/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.877461 google-vizier-0.1.8/vizier/_src/algorithms/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/classification/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/classification/classifiers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.881461 google-vizier-0.1.8/vizier/_src/algorithms/core/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/core/abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.881461 google-vizier-0.1.8/vizier/_src/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/bocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/bocs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/cmaes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/cmaes_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.885461 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20732 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/emukit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/emukit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.885461 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/acquisitions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/gp_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/gp_models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/output_warpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/output_warpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/transfer_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/transfer_learning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/yjt.py
--rw-r--r--   0 runner    (1001) docker     (123)    21253 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/gp_bandit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/grid_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/harmonica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/harmonica_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/quasi_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/quasi_random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarizing_designer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarizing_designer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.885461 google-vizier-0.1.8/vizier/_src/algorithms/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_design.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_design_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_designer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_designer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.885461 google-vizier-0.1.8/vizier/_src/algorithms/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/evolution/numpy_populations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/evolution/numpy_populations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/evolution/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.889461 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/designer_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    39427 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22618 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/vectorized_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/optimizers/vectorized_base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.889461 google-vizier-0.1.8/vizier/_src/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/designer_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/designer_policy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/random_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/random_policy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/trial_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/policies/trial_caches_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.889461 google-vizier-0.1.8/vizier/_src/algorithms/random/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/random/random_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/random/random_sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.889461 google-vizier-0.1.8/vizier/_src/algorithms/regression/
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/regression/trial_regression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/regression/trial_regression_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.893462 google-vizier-0.1.8/vizier/_src/algorithms/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/testing/comparator_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/testing/comparator_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/testing/optimizer_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/algorithms/testing/test_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.873461 google-vizier-0.1.8/vizier/_src/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.893462 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)    25977 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/convergence_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/simple_regret_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/state_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.897462 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.897462 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo/
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/experimenter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.897462 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob/
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/switch_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.897462 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.897462 google-vizier-0.1.8/vizier/_src/benchmarks/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_state_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.901462 google-vizier-0.1.8/vizier/_src/jax/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/gp_bandit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.901462 google-vizier-0.1.8/vizier/_src/jax/models/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/continuous_only_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/gaussian_process_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/gaussian_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/hebo_gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/hebo_gp_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/mask_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/mask_features_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/tuned_gp_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/models/tuned_gp_models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.905462 google-vizier-0.1.8/vizier/_src/jax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/jaxopt_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/optax_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/optax_wrappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.905462 google-vizier-0.1.8/vizier/_src/jax/optimizers/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/optimizers/testing/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/predictive_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/predictive_fns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    37178 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/stochastic_process_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23884 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/stochastic_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/types_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/xla_pareto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/jax/xla_pareto_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.909462 google-vizier-0.1.8/vizier/_src/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/oss_vizier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/oss_vizier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/pythia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/pythia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyglove/vizier_test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.909462 google-vizier-0.1.8/vizier/_src/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pythia/local_policy_supporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pythia/local_policy_supporters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pythia/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pythia/policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pythia/pythia_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.873461 google-vizier-0.1.8/vizier/_src/pyvizier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.913462 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/hypervolume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/pareto_optimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/safety_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.917462 google-vizier-0.1.8/vizier/_src/pyvizier/oss/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/automated_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/automated_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/metadata_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33067 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/proto_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/proto_converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/study_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/oss/study_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.917462 google-vizier-0.1.8/vizier/_src/pyvizier/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/pythia/study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.921462 google-vizier-0.1.8/vizier/_src/pyvizier/shared/
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/base_study_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/base_study_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/context_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    47697 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_iterators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/study.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/pyvizier/shared/trial_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.925462 google-vizier-0.1.8/vizier/_src/raytune/
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/raytune/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/raytune/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/raytune/run_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/raytune/run_tune_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/raytune/vizier_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/raytune/vizier_search_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.933462 google-vizier-0.1.8/vizier/_src/service/
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/clients_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/datastore_test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/grpc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/policy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/pythia_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/pythia_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/ram_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/ram_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/service_policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/service_policy_supporter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/sql_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/sql_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/stubs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/stubs_util_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.933462 google-vizier-0.1.8/vizier/_src/service/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/vizier_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/vizier_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/vizier_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    36429 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/vizier_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/_src/service/vizier_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/algorithms/designers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/algorithms/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/benchmarks/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/benchmarks/experimenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/benchmarks/experimenters/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/benchmarks/experimenters/hpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/benchmarks/experimenters/nas/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/benchmarks/experimenters/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/benchmarks/experimenters/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/benchmarks/experimenters/rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.937462 google-vizier-0.1.8/vizier/client/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/client/client_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15824 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/client/client_abc_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.941462 google-vizier-0.1.8/vizier/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/interfaces/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.941462 google-vizier-0.1.8/vizier/jax/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/jax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/jax/optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.941462 google-vizier-0.1.8/vizier/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyglove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pythia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.941462 google-vizier-0.1.8/vizier/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.945462 google-vizier-0.1.8/vizier/pyvizier/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45402 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    44675 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/embedder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/feature_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/feature_mapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/input_warping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/input_warping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/jnp_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/jnp_converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/spatio_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/converters/spatio_temporal_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/pyvizier/multimetric/xla_pareto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/raytune/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/raytune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/service/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/service/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/service/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/service/protos/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/service/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/service/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/service/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/service/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/service/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.949462 google-vizier-0.1.8/vizier/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/testing/numpy_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/testing/test_studies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 21:38:52.953462 google-vizier-0.1.8/vizier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/utils/attrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/utils/attrs_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/utils/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-17 21:38:28.000000 google-vizier-0.1.8/vizier/utils/profiler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (999)    11358 2023-09-01 01:04:23.000000 google-vizier-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     7890 2023-09-01 01:04:45.792961 google-vizier-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     6776 2023-09-01 01:04:23.000000 google-vizier-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/google_vizier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     7890 2023-09-01 01:04:45.000000 google-vizier-0.1.9/google_vizier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    14379 2023-09-01 01:04:45.000000 google-vizier-0.1.9/google_vizier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 01:04:45.000000 google-vizier-0.1.9/google_vizier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 01:04:45.000000 google-vizier-0.1.9/google_vizier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (999)      945 2023-09-01 01:04:45.000000 google-vizier-0.1.9/google_vizier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        7 2023-09-01 01:04:45.000000 google-vizier-0.1.9/google_vizier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 01:04:45.792961 google-vizier-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     4280 2023-09-01 01:04:23.000000 google-vizier-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/vizier/
+-rw-r--r--   0 runner    (1001) docker     (999)      831 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/vizier/_src/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/vizier/_src/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/vizier/_src/algorithms/classification/
+-rw-r--r--   0 runner    (1001) docker     (999)     4179 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/classification/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5456 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/classification/classifiers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/vizier/_src/algorithms/core/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6716 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/core/abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.768960 google-vizier-0.1.9/vizier/_src/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19486 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/bocs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1633 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/bocs_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4513 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1644 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/cmaes_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.768960 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/
+-rw-r--r--   0 runner    (1001) docker     (999)     2764 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19573 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8892 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20732 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16393 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4517 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2545 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5349 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8562 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/emukit.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2001 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/emukit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.768960 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/
+-rw-r--r--   0 runner    (1001) docker     (999)    18920 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11483 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/acquisitions_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11473 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11923 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/gp_models_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    25608 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/output_warpers.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16195 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/output_warpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5417 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2387 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/transfer_learning_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3483 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/yjt.py
+-rw-r--r--   0 runner    (1001) docker     (999)    21253 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16322 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/gp_bandit_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7297 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/grid.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5136 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/grid_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11889 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/harmonica.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1419 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/harmonica_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12751 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/quasi_random.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6590 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/quasi_random_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3146 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/random.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3231 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3452 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2053 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarization_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4645 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarizing_designer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4421 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarizing_designer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.768960 google-vizier-0.1.9/vizier/_src/algorithms/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (999)     9407 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_design.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3109 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_design_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7475 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_designer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3444 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_designer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.768960 google-vizier-0.1.9/vizier/_src/algorithms/evolution/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8259 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7626 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13712 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/evolution/numpy_populations.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2697 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/evolution/numpy_populations_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6399 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/evolution/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.772960 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (999)      747 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5205 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3340 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/designer_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1833 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4346 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    39427 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20678 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7297 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3959 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4555 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2027 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22618 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/vectorized_base.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13562 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/optimizers/vectorized_base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.772960 google-vizier-0.1.9/vizier/_src/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (999)      613 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13538 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/designer_policy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7809 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/designer_policy_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2512 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/random_policy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2968 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/random_policy_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4648 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/trial_caches.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2561 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/policies/trial_caches_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.772960 google-vizier-0.1.9/vizier/_src/algorithms/random/
+-rw-r--r--   0 runner    (1001) docker     (999)     4155 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/random/random_sample.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5082 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/random/random_sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.772960 google-vizier-0.1.9/vizier/_src/algorithms/regression/
+-rw-r--r--   0 runner    (1001) docker     (999)    18505 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/regression/trial_regression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12026 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/regression/trial_regression_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.772960 google-vizier-0.1.9/vizier/_src/algorithms/testing/
+-rw-r--r--   0 runner    (1001) docker     (999)      624 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10508 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/testing/comparator_runner.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11791 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/testing/comparator_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2660 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/testing/optimizer_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5501 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/algorithms/testing/test_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.760960 google-vizier-0.1.9/vizier/_src/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.772960 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (999)    27452 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/convergence_curve.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18350 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7952 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3448 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/plot_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2549 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/simple_regret_score.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3612 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9646 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/state_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6321 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (999)     6861 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2239 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo/
+-rw-r--r--   0 runner    (1001) docker     (999)     5148 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo/common.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16909 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2557 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8060 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5840 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2167 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7426 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/experimenter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5843 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob/
+-rw-r--r--   0 runner    (1001) docker     (999)    11646 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob/handler.py
+-rw-r--r--   0 runner    (1001) docker     (999)    25640 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3070 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3344 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2915 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3573 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2479 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3982 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1959 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3202 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1957 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7332 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5875 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3714 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2655 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3955 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3488 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4599 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6267 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2650 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2879 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6015 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4851 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2083 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2356 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2792 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/switch_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1749 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (999)    17411 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2023 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/branin.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1550 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/branin_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3440 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/hartmann.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2497 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/hartmann_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/benchmarks/runners/
+-rw-r--r--   0 runner    (1001) docker     (999)     6538 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_runner.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5760 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5720 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2903 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_state_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/benchmarks/testing/
+-rw-r--r--   0 runner    (1001) docker     (999)     1638 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/benchmarks/testing/experimenter_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.776960 google-vizier-0.1.9/vizier/_src/jax/
+-rw-r--r--   0 runner    (1001) docker     (999)     1738 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/gp_bandit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.780960 google-vizier-0.1.9/vizier/_src/jax/models/
+-rw-r--r--   0 runner    (1001) docker     (999)      630 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4963 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/continuous_only_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6506 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/gaussian_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3114 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/gaussian_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4664 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/hebo_gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3850 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/hebo_gp_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3034 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/mask_features.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2751 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/mask_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13414 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/multitask_tuned_gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7146 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/multitask_tuned_gp_models_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14954 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/tuned_gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10585 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/models/tuned_gp_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.780960 google-vizier-0.1.9/vizier/_src/jax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (999)     4116 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/core.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1738 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9350 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/jaxopt_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1668 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5096 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/optax_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1484 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/optax_wrappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.780960 google-vizier-0.1.9/vizier/_src/jax/optimizers/testing/
+-rw-r--r--   0 runner    (1001) docker     (999)     3340 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/optimizers/testing/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3713 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/predictive_fns.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4178 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/predictive_fns_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    37178 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/stochastic_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (999)    23884 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/stochastic_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6435 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3063 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/types_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6865 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/xla_pareto.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2139 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/jax/xla_pareto_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.780960 google-vizier-0.1.9/vizier/_src/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (999)     2659 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12231 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/backend.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3758 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/client.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1371 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19354 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/converters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8974 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12146 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/core.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1355 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10262 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/oss_vizier.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1699 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/oss_vizier_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2402 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6891 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/pythia.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3754 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/pythia_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19643 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyglove/vizier_test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.780960 google-vizier-0.1.9/vizier/_src/pythia/
+-rw-r--r--   0 runner    (1001) docker     (999)     9982 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pythia/local_policy_supporters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7211 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pythia/local_policy_supporters_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8983 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pythia/policy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4834 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pythia/policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2845 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pythia/pythia_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.764960 google-vizier-0.1.9/vizier/_src/pyvizier/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.780960 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (999)     6783 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2288 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/hypervolume_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9182 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/pareto_optimal.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3382 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2994 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/safety.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3714 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/safety_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.784960 google-vizier-0.1.9/vizier/_src/pyvizier/oss/
+-rw-r--r--   0 runner    (1001) docker     (999)     1628 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/automated_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1164 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/automated_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1145 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/compare.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8836 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2187 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/metadata_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    33067 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/proto_converters.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14759 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/proto_converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17314 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/study_config.py
+-rw-r--r--   0 runner    (1001) docker     (999)    36459 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/oss/study_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.784960 google-vizier-0.1.9/vizier/_src/pyvizier/pythia/
+-rw-r--r--   0 runner    (1001) docker     (999)     1651 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/pythia/study.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.784960 google-vizier-0.1.9/vizier/_src/pyvizier/shared/
+-rw-r--r--   0 runner    (1001) docker     (999)    13397 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/base_study_config.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4221 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/base_study_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    24485 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/common.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15254 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2234 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/context.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1105 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    47697 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_config.py
+-rw-r--r--   0 runner    (1001) docker     (999)    24044 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3779 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2384 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_iterators_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1205 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/study.py
+-rw-r--r--   0 runner    (1001) docker     (999)    23413 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/trial.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13055 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/pyvizier/shared/trial_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.784960 google-vizier-0.1.9/vizier/_src/raytune/
+-rw-r--r--   0 runner    (1001) docker     (999)     4580 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/raytune/converters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4163 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/raytune/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4309 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/raytune/run_tune.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2018 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/raytune/run_tune_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7805 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/raytune/vizier_search.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3243 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/raytune/vizier_search_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/_src/service/
+-rw-r--r--   0 runner    (1001) docker     (999)     7820 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/clients.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3454 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/clients_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1371 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1068 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7024 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12366 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/datastore_test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2898 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/grpc_util.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3108 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4140 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/policy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4734 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/pythia_service.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2607 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/pythia_util.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15795 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/ram_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2521 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/ram_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7442 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/resources.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4178 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3405 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/service_policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3705 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/service_policy_supporter_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22481 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/sql_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3498 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/sql_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2629 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/stubs_util.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1243 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/stubs_util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/_src/service/testing/
+-rw-r--r--   0 runner    (1001) docker     (999)     5071 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1212 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17489 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/vizier_client.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12307 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/vizier_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4986 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/vizier_server.py
+-rw-r--r--   0 runner    (1001) docker     (999)    36429 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/vizier_service.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17256 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/_src/service/vizier_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (999)     1545 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (999)     1781 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/algorithms/designers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (999)      707 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/algorithms/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (999)     1708 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1818 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/benchmarks/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (999)     2725 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/benchmarks/experimenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/benchmarks/experimenters/hpo/
+-rw-r--r--   0 runner    (1001) docker     (999)      726 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/benchmarks/experimenters/hpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/benchmarks/experimenters/nas/
+-rw-r--r--   0 runner    (1001) docker     (999)      885 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/benchmarks/experimenters/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/benchmarks/experimenters/rl/
+-rw-r--r--   0 runner    (1001) docker     (999)      759 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/benchmarks/experimenters/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/client/
+-rw-r--r--   0 runner    (1001) docker     (999)      693 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9515 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/client/client_abc.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15824 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/client/client_abc_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (999)      678 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3557 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/interfaces/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/jax/
+-rw-r--r--   0 runner    (1001) docker     (999)      690 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1348 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/jax/models.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1477 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/jax/optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (999)      866 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyglove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2007 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pythia.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.788960 google-vizier-0.1.9/vizier/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (999)     3478 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/pyvizier/converters/
+-rw-r--r--   0 runner    (1001) docker     (999)     2053 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    45402 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/core.py
+-rw-r--r--   0 runner    (1001) docker     (999)    44675 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6127 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6145 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/embedder_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7088 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/feature_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7675 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/feature_mapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3060 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/input_warping.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2546 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/input_warping_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15140 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/jnp_converters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6788 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/jnp_converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2980 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/padding.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2054 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20179 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/spatio_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9955 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/converters/spatio_temporal_test.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (999)      963 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      839 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/pyvizier/multimetric/xla_pareto.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/raytune/
+-rw-r--r--   0 runner    (1001) docker     (999)      816 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/raytune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/service/
+-rw-r--r--   0 runner    (1001) docker     (999)      887 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/service/clients/
+-rw-r--r--   0 runner    (1001) docker     (999)      842 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/service/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/service/protos/
+-rw-r--r--   0 runner    (1001) docker     (999)      887 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/service/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/service/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (999)     4097 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/service/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/service/servers/
+-rw-r--r--   0 runner    (1001) docker     (999)      792 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/service/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/testing/
+-rw-r--r--   0 runner    (1001) docker     (999)      612 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1250 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/testing/numpy_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4489 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/testing/test_studies.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 01:04:45.792961 google-vizier-0.1.9/vizier/utils/
+-rw-r--r--   0 runner    (1001) docker     (999)     3329 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/utils/attrs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3100 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/utils/attrs_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1894 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1285 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/utils/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9176 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2748 2023-09-01 01:04:23.000000 google-vizier-0.1.9/vizier/utils/profiler_test.py
```

### Comparing `google-vizier-0.1.8/LICENSE` & `google-vizier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/PKG-INFO` & `google-vizier-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `google-vizier-0.1.8/README.md` & `google-vizier-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/google_vizier.egg-info/PKG-INFO` & `google-vizier-0.1.9/google_vizier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `google-vizier-0.1.8/google_vizier.egg-info/SOURCES.txt` & `google-vizier-0.1.9/google_vizier.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,16 @@
 vizier/_src/algorithms/testing/__init__.py
 vizier/_src/algorithms/testing/comparator_runner.py
 vizier/_src/algorithms/testing/comparator_runner_test.py
 vizier/_src/algorithms/testing/optimizer_test_utils.py
 vizier/_src/algorithms/testing/test_runners.py
 vizier/_src/benchmarks/analyzers/convergence_curve.py
 vizier/_src/benchmarks/analyzers/convergence_curve_test.py
+vizier/_src/benchmarks/analyzers/plot_utils.py
+vizier/_src/benchmarks/analyzers/plot_utils_test.py
 vizier/_src/benchmarks/analyzers/simple_regret_score.py
 vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
 vizier/_src/benchmarks/analyzers/state_analyzer.py
 vizier/_src/benchmarks/analyzers/state_analyzer_test.py
 vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
 vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
 vizier/_src/benchmarks/experimenters/combo_experimenter.py
@@ -132,18 +134,23 @@
 vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
 vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
 vizier/_src/benchmarks/experimenters/switch_experimenter.py
 vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
 vizier/_src/benchmarks/experimenters/combo/common.py
 vizier/_src/benchmarks/experimenters/hpob/handler.py
 vizier/_src/benchmarks/experimenters/synthetic/bbob.py
+vizier/_src/benchmarks/experimenters/synthetic/branin.py
+vizier/_src/benchmarks/experimenters/synthetic/branin_test.py
+vizier/_src/benchmarks/experimenters/synthetic/hartmann.py
+vizier/_src/benchmarks/experimenters/synthetic/hartmann_test.py
 vizier/_src/benchmarks/runners/benchmark_runner.py
 vizier/_src/benchmarks/runners/benchmark_runner_test.py
 vizier/_src/benchmarks/runners/benchmark_state.py
 vizier/_src/benchmarks/runners/benchmark_state_test.py
+vizier/_src/benchmarks/testing/experimenter_testing.py
 vizier/_src/jax/gp_bandit_utils.py
 vizier/_src/jax/predictive_fns.py
 vizier/_src/jax/predictive_fns_test.py
 vizier/_src/jax/stochastic_process_model.py
 vizier/_src/jax/stochastic_process_model_test.py
 vizier/_src/jax/types.py
 vizier/_src/jax/types_test.py
@@ -153,14 +160,16 @@
 vizier/_src/jax/models/continuous_only_kernel.py
 vizier/_src/jax/models/gaussian_process_model.py
 vizier/_src/jax/models/gaussian_process_model_test.py
 vizier/_src/jax/models/hebo_gp_model.py
 vizier/_src/jax/models/hebo_gp_model_test.py
 vizier/_src/jax/models/mask_features.py
 vizier/_src/jax/models/mask_features_test.py
+vizier/_src/jax/models/multitask_tuned_gp_models.py
+vizier/_src/jax/models/multitask_tuned_gp_models_test.py
 vizier/_src/jax/models/tuned_gp_models.py
 vizier/_src/jax/models/tuned_gp_models_test.py
 vizier/_src/jax/optimizers/core.py
 vizier/_src/jax/optimizers/core_test.py
 vizier/_src/jax/optimizers/jaxopt_wrappers.py
 vizier/_src/jax/optimizers/jaxopt_wrappers_test.py
 vizier/_src/jax/optimizers/optax_wrappers.py
```

### Comparing `google-vizier-0.1.8/google_vizier.egg-info/requires.txt` & `google-vizier-0.1.9/google_vizier.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 absl-py>=1.0.0
 numpy>=1.21.5
 protobuf>=3.6
 portpicker>=1.3.1
 grpcio>=1.35.0
 grpcio-tools>=1.35.0
 googleapis-common-protos>=1.56.4
-sqlalchemy==1.4
+sqlalchemy<=1.4.20,>=1.4
 
 [algorithms]
 emukit==0.4.9
 scipy<1.8.0,>1.2.3
 cvxpy==1.2.1
 cvxopt==1.3.0
 scikit-learn==1.1.2
```

### Comparing `google-vizier-0.1.8/setup.py` & `google-vizier-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/__init__.py` & `google-vizier-0.1.9/vizier/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 import sys
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 PROTO_ROOT = os.path.realpath(os.path.join(THIS_DIR, "_src", "service"))
 
 sys.path.append(PROTO_ROOT)
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `google-vizier-0.1.8/vizier/_src/__init__.py` & `google-vizier-0.1.9/vizier/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/classification/classifiers.py` & `google-vizier-0.1.9/vizier/_src/algorithms/classification/classifiers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/classification/classifiers_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/classification/classifiers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/core/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/core/abstractions.py` & `google-vizier-0.1.9/vizier/_src/algorithms/core/abstractions.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/bocs.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/bocs.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/bocs_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/bocs_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/cmaes.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/cmaes.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/cmaes_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/cmaes_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/serialization.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/serialization.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/eagle_strategy/testing.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/eagle_strategy/testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/emukit.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/emukit.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/emukit_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/emukit_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/acquisitions.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/acquisitions.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/acquisitions_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/acquisitions_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/gp_models.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/gp_models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/gp_models_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/gp_models_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/output_warpers.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/output_warpers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/output_warpers_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/output_warpers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/transfer_learning.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/transfer_learning_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/transfer_learning_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp/yjt.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp/yjt.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp_bandit.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp_bandit.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/gp_bandit_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/gp_bandit_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/grid.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/grid.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/grid_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/grid_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/harmonica.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/harmonica.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/harmonica_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/harmonica_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/quasi_random.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/quasi_random.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/quasi_random_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/quasi_random_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/random.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/random.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/random_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/random_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarization.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarization.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarization_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarization_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarizing_designer.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarizing_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/designers/scalarizing_designer_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/designers/scalarizing_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_design.py` & `google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_design.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_design_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_design_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_designer.py` & `google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/ensemble/ensemble_designer_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/ensemble/ensemble_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/evolution/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/evolution/nsga2.py` & `google-vizier-0.1.9/vizier/_src/algorithms/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/evolution/nsga2_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/evolution/numpy_populations.py` & `google-vizier-0.1.9/vizier/_src/algorithms/evolution/numpy_populations.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/evolution/numpy_populations_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/evolution/numpy_populations_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/evolution/templates.py` & `google-vizier-0.1.9/vizier/_src/algorithms/evolution/templates.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/base.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/designer_optimizer.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/designer_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/designer_optimizer_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/designer_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/eagle_strategy.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/eagle_strategy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/eagle_strategy_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/eagle_strategy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/vectorized_base.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/vectorized_base.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/optimizers/vectorized_base_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/optimizers/vectorized_base_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/designer_policy.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/designer_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/designer_policy_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/designer_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/random_policy.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/random_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/random_policy_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/random_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/trial_caches.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/trial_caches.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,17 @@
   _include_intermediate_measurements: bool = attrs.field(
       kw_only=True, default=False
   )
 
   def __attrs_post_init__(self):
     logging.info('Initialized %s', self)
 
+  def num_incorporated_trials(self) -> int:
+    return len(self._incorporated_completed_trial_ids)
+
   def clear(self) -> None:
     """Make the next call to get_newly_completed_trials() return all trials."""
     self._incorporated_completed_trial_ids = set()
 
   def get_active_trials(self) -> Sequence[vz.Trial]:
     """Returns all active trials."""
     trials = self._supporter.GetTrials(
```

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/policies/trial_caches_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/policies/trial_caches_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,39 +36,39 @@
     cache = trial_caches.IdDeduplicatingTrialLoader(supporter)
 
     ################## PHASE 1 ################
     active_trial = new_active()
     supporter.AddTrials([new_completed(), active_trial, new_completed()])
 
     self.assertLen(cache.get_newly_completed_trials(3), 2)
-    self.assertLen(cache._incorporated_completed_trial_ids, 2)
+    self.assertEqual(cache.num_incorporated_trials(), 2)
 
     # dump and load should restore the state.
     dump = cache.dump()
     cache = trial_caches.IdDeduplicatingTrialLoader(supporter)
     cache.load(dump)
     self.assertEmpty(cache.get_newly_completed_trials(3))
-    self.assertLen(cache._incorporated_completed_trial_ids, 2)
+    self.assertEqual(cache.num_incorporated_trials(), 2)
 
     ################## PHASE 2 ################
 
     # Trial 2 completed
     active_trial.complete(vz.Measurement())
     # Trial 4 added as pending. 5 added as completed
     supporter.AddTrials([new_active(), new_completed()])
     self.assertLen(cache.get_newly_completed_trials(5), 2)
     self.assertLen(cache.get_active_trials(), 1)
-    self.assertLen(cache._incorporated_completed_trial_ids, 4)
+    self.assertEqual(cache.num_incorporated_trials(), 4)
 
     # dump and load should restore the state.
     dump = cache.dump()
     cache = trial_caches.IdDeduplicatingTrialLoader(supporter)
     cache.load(dump)
     self.assertEmpty(cache.get_newly_completed_trials(5))
-    self.assertLen(cache._incorporated_completed_trial_ids, 4)
+    self.assertEqual(cache.num_incorporated_trials(), 4)
 
     # clear should reset.
     cache.clear()
     self.assertEmpty(cache._incorporated_completed_trial_ids)
     self.assertLen(cache.get_newly_completed_trials(5), 4)
```

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/random/random_sample.py` & `google-vizier-0.1.9/vizier/_src/algorithms/random/random_sample.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/random/random_sample_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/random/random_sample_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/regression/trial_regression_utils.py` & `google-vizier-0.1.9/vizier/_src/algorithms/regression/trial_regression_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/regression/trial_regression_utils_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/regression/trial_regression_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/testing/__init__.py` & `google-vizier-0.1.9/vizier/_src/algorithms/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/testing/comparator_runner.py` & `google-vizier-0.1.9/vizier/_src/algorithms/testing/comparator_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/testing/comparator_runner_test.py` & `google-vizier-0.1.9/vizier/_src/algorithms/testing/comparator_runner_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/testing/optimizer_test_utils.py` & `google-vizier-0.1.9/vizier/_src/algorithms/testing/optimizer_test_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/algorithms/testing/test_runners.py` & `google-vizier-0.1.9/vizier/_src/algorithms/testing/test_runners.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/convergence_curve.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/convergence_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """Converters and comparators for convergence curves."""
 
 import abc
 import bisect
 import enum
 import logging
-from typing import Callable, List, Optional, Sequence
+from typing import Callable, List, Optional, Protocol, Sequence
 
 import attr
 import numpy as np
 from vizier import pyvizier
 from vizier.pyvizier import converters
 from vizier.pyvizier import multimetric
 from vizier.pyvizier.multimetric import xla_pareto
@@ -377,15 +377,15 @@
         ys=np.asarray(hv_curve).reshape([1, -1]),
         trend=ConvergenceCurve.YTrend.INCREASING,
         ylabel='hypervolume',
     )
 
 
 @attr.define
-class ConvergenceComparatorBase(abc.ABC):
+class ConvergenceComparator(abc.ABC):
   """Base class for convergence curve compartors.
 
   Attributes:
     baseline_curve: The baseline ConvergenceCurve.
     compared_curve: The compared ConvergenceCurve.
     baseline_quantile: Quantile in [0, 1] of the batched baseline curve to use
       for efficiency comparison. The higher the quantile, the better the quality
@@ -487,38 +487,62 @@
         baseline_ys = baseline_ys[baseline_cutoff_ind[0] :]
         compared_ys = compared_ys[compared_cutoff_ind[0] :]
 
     return baseline_ys, compared_ys
 
   @abc.abstractmethod
   def score(self) -> float:
+    """Returns a summary score for the comparison between base and compared.
+
+    Usually, higher positive numbers mean the compared curve is better than the
+    baseline and vice versa.
+    """
+    pass
+
+  @abc.abstractmethod
+  def curve(self) -> ConvergenceCurve:
+    """Returns a score curve for each xs."""
+    pass
+
+
+class ConvergenceComparatorFactory(Protocol):
+  """ConvergenceComparator factory interface."""
+
+  def __call__(
+      self,
+      baseline_curve: ConvergenceCurve,
+      compared_curve: ConvergenceCurve,
+      baseline_quantile: float = 0.5,
+      compared_quantile: float = 0.5,
+      **kwargs,
+  ) -> ConvergenceComparator:
     ...
 
 
 @attr.define
-class LogEfficiencyConvergenceCurveComparator(ConvergenceComparatorBase):
+class LogEfficiencyConvergenceCurveComparator(ConvergenceComparator):
   """Comparator methods for ConvergenceCurves.
 
   Methods in this class generally return comparison metrics for a compared curve
   against a baseline curve. Only works for curves with INCREASING or DECREASING
   trend.
 
   Example usage:
     baseline_curve = ConvergenceCurve(...)
     comparator = LogEfficiencyConvergenceCurveComparator(baseline_curve)
-    comparator.log_efficiency_curve(compared_curve)
+    comparator.curve(compared_curve)
   """
   max_score: float = attr.field(
       default=1.0, validator=[attr.validators.ge(0)], kw_only=True
   )
   summary_function: Callable[[np.ndarray], float] = attr.field(
       default=np.median
   )
 
-  def log_efficiency_curve(self) -> ConvergenceCurve:
+  def curve(self) -> ConvergenceCurve:
     """Builds the log sample efficiency curve.
 
     The compared curve should approximately use exp(-relative efficiency)% less
     Trials than the baseline curve. Note that a positive relative effiency
     demonstrates that the compared curve is better than the baseline. Also,
     the relative efficiency CURVES are not fully symmetric due to differences
     in drops in objective values.
@@ -547,16 +571,20 @@
         np.nanquantile(
             self._sign * self._compared_curve.ys,
             self._compared_quantile,
             axis=0,
         ),
     )
 
-    ys = np.log(1 + np.asarray(baseline_index_curve)) - np.log(
-        1 + np.asarray(other_index_curve))
+    ys = np.clip(
+        np.log(1 + np.asarray(baseline_index_curve))
+        - np.log(1 + np.asarray(other_index_curve)),
+        a_min=-self.max_score,
+        a_max=self.max_score,
+    )
     return ConvergenceCurve(
         xs=self._baseline_curve.xs, ys=ys.reshape(1, len(ys)))
 
   def score(self) -> float:
     """Gets a finalized log efficiency score.
 
     The compared curve should approximately use exp(-score)% Trials compared to
@@ -589,33 +617,33 @@
         compared_curve, extend_steps
     )
     baseline_comparator = LogEfficiencyConvergenceCurveComparator(
         baseline_curve=combined_curve,
         compared_curve=extended_baseline,
         compared_quantile=self._baseline_quantile,
     )
-    efficiency_baseline = baseline_comparator.log_efficiency_curve()
+    efficiency_baseline = baseline_comparator.curve()
     compared_comparator = LogEfficiencyConvergenceCurveComparator(
         baseline_curve=combined_curve,
         compared_curve=extended_compared,
         compared_quantile=self._compared_quantile,
     )
-    efficiency_compared = compared_comparator.log_efficiency_curve()
+    efficiency_compared = compared_comparator.curve()
 
     # Clip log efficiency and return median log efficiency in last half.
     diff = np.clip(
         efficiency_compared.ys, a_min=-self.max_score, a_max=self.max_score
     ) - np.clip(
         efficiency_baseline.ys, a_min=-self.max_score, a_max=self.max_score
     )
     return self.summary_function(diff)
 
 
 @attr.define
-class SimpleConvergenceCurveComparator(ConvergenceComparatorBase):
+class SimpleConvergenceCurveComparator(ConvergenceComparator):
   """Comparator method based on simple comparison.
 
   Attributes:
     burn_cutoff: The cutoff below which values not included in score.
   """
 
   _xs_cutoff: Optional[float] = None
@@ -634,17 +662,20 @@
       ValueError: If curve trends are not INCREASING or DECREASING, or not
       equal.
     """
     baseline_ys, compared_ys = self._standardize_curves(self._xs_cutoff)
     # Compute mean indices that compared is better than baseline.
     return np.mean(baseline_ys < compared_ys)
 
+  def curve(self) -> ConvergenceCurve:
+    raise NotImplementedError('Curve not yet implemented.')
+
 
 @attr.define
-class PercentageBetterConvergenceCurveComparator(ConvergenceComparatorBase):
+class PercentageBetterConvergenceCurveComparator(ConvergenceComparator):
   """Comparator method based on percentage better.
 
   Attributes:
     burn_cutoff: The cutoff below which values not included in score.
   """
 
   _xs_cutoff: Optional[float] = None
@@ -708,14 +739,37 @@
         baseline_ys, compared_ys
     )
     compared_baseline_score = self._compute_directional_score(
         compared_ys, baseline_ys
     )
     return baseline_compared_score - compared_baseline_score
 
+  def curve(self) -> ConvergenceCurve:
+    raise NotImplementedError('Curve not yet implemented.')
+
+
+class PercentageBetterConvergenceCurveComparatorFactory(
+    ConvergenceComparatorFactory
+):
+  """Factory class for PercentageBetterConvergenceCurveComparator."""
+
+  def __call__(
+      self,
+      baseline_curve: ConvergenceCurve,
+      compared_curve: ConvergenceCurve,
+      baseline_quantile: float = 0.5,
+      compared_quantile: float = 0.5,
+  ) -> ConvergenceComparator:
+    return PercentageBetterConvergenceCurveComparator(
+        baseline_curve=baseline_curve,
+        compared_curve=compared_curve,
+        baseline_quantile=baseline_quantile,
+        compared_quantile=compared_quantile,
+    )
+
 
 def build_convergence_curve(
     baseline_curve: Sequence[float], compared_curve: Sequence[float]
 ) -> List[float]:
   """Builds a relative convergence curve (see returns for definition).
 
   Finds the smallest index j for each element i in 'baseline_curve'
```

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/convergence_curve_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/convergence_curve_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,20 +317,20 @@
         ys=np.exp(np.array([-1.5, -1.8, -2.0]).reshape(3, 1) * xs_t),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
 
   def test_get_relative_efficiency_curve(self):
     baseline_length = len(self._baseline_curve.xs)
     rel_effiency = convergence.LogEfficiencyConvergenceCurveComparator(
         baseline_curve=self._baseline_curve, compared_curve=self._better_curves
-    ).log_efficiency_curve()
+    ).curve()
     higher_quantile = convergence.LogEfficiencyConvergenceCurveComparator(
         baseline_curve=self._baseline_curve,
         compared_curve=self._better_curves,
         compared_quantile=0.9,
-    ).log_efficiency_curve()
+    ).curve()
 
     self.assertEqual(rel_effiency.ys.shape, (1, baseline_length))
     self.assertEqual(higher_quantile.ys.shape, (1, baseline_length))
     # Better curves should have positive efficiency.
     self.assertTrue((rel_effiency.ys >= 0.0).all())
     # Higher quantile means better efficiency which means more positive scores.
     self.assertTrue((higher_quantile.ys >= rel_effiency.ys).all())
@@ -338,30 +338,33 @@
   def test_get_relative_efficiency_flat(self):
     flat_curve = convergence.ConvergenceCurve(
         xs=np.array(range(0, 20)),
         ys=np.array([4.0, 3.0, 2.0] + [1.5] * 17).reshape(1, 20),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     self_eff = convergence.LogEfficiencyConvergenceCurveComparator(
         baseline_curve=flat_curve, compared_curve=flat_curve
-    ).log_efficiency_curve()
+    ).curve()
     # Relative efficiency of a curve on itself is close to 0.
     self.assertAlmostEqual(np.linalg.norm(self_eff.ys), 0.0, delta=0.1)
 
   def test_get_relative_efficiency_short_curve(self):
     baseline_length = len(self._baseline_curve.xs)
     short_length = round(baseline_length / 2)
     short_curve = convergence.ConvergenceCurve(
         xs=self._baseline_curve.xs[:short_length],
         ys=self._baseline_curve.ys[:, :short_length],
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
+    max_score = 10.3
     short_efficiency = convergence.LogEfficiencyConvergenceCurveComparator(
-        baseline_curve=self._baseline_curve, compared_curve=short_curve
-    ).log_efficiency_curve()
+        baseline_curve=self._baseline_curve,
+        compared_curve=short_curve,
+        max_score=max_score,
+    ).curve()
     self.assertEqual(short_efficiency.ys.shape, (1, baseline_length))
-    self.assertEqual(float(short_efficiency.ys[:, -1]), -float('inf'))
+    self.assertEqual(float(short_efficiency.ys[:, -1]), -max_score)
 
   def test_get_efficiency_score(self):
     # Higher compared quantile should increase score. Higher baseline
     # quantile should decrease score.
     median_score = convergence.LogEfficiencyConvergenceCurveComparator(
         baseline_curve=self._baseline_curve, compared_curve=self._better_curves
     ).score()
```

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/simple_regret_score.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/simple_regret_score.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/analyzers/state_analyzer_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_state_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,79 +10,75 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from vizier import algorithms as vza
+from vizier import pythia
 from vizier import pyvizier as vz
 from vizier._src.algorithms.designers import random
-from vizier._src.benchmarks.analyzers import state_analyzer
-from vizier._src.benchmarks.experimenters import experimenter_factory
-from vizier._src.benchmarks.runners import benchmark_runner
 from vizier._src.benchmarks.runners import benchmark_state
 
 from absl.testing import absltest
 
 
-class StateAnalyzerTest(absltest.TestCase):
+class BenchmarkStateTest(absltest.TestCase):
 
-  def test_curve_conversion(self):
-    dim = 10
-    experimenter = experimenter_factory.BBOBExperimenterFactory('Sphere', dim)()
-
-    def _designer_factory(config: vz.ProblemStatement, seed: int):
-      return random.RandomDesigner(config.search_space, seed=seed)
-
-    benchmark_state_factory = benchmark_state.DesignerBenchmarkStateFactory(
-        designer_factory=_designer_factory, experimenter=experimenter
+  def test_policy_suggester_active_trials_with_init(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('x', 0.0, 1.0)
+    problem.search_space.root.add_float_param('y', 0.0, 1.0)
+    problem.metric_information.append(
+        vz.MetricInformation(
+            name='maximize_metric', goal=vz.ObjectiveMetricGoal.MAXIMIZE
+        )
     )
-    num_trials = 20
-    runner = benchmark_runner.BenchmarkRunner(
-        benchmark_subroutines=[benchmark_runner.GenerateAndEvaluate()],
-        num_repeats=num_trials,
-    )
-
-    states = []
-    num_repeats = 3
-    for i in range(num_repeats):
-      bench_state = benchmark_state_factory(seed=i)
-      runner.run(bench_state)
-      states.append(bench_state)
-
-    curve = state_analyzer.BenchmarkStateAnalyzer.to_curve(states)
-    self.assertEqual(curve.ys.shape, (num_repeats, num_trials))
-
-  def test_empty_curve_error(self):
-    with self.assertRaisesRegex(ValueError, 'Empty'):
-      state_analyzer.BenchmarkStateAnalyzer.to_curve([])
-
-  def test_different_curve_error(self):
-    exp1 = experimenter_factory.BBOBExperimenterFactory('Sphere', dim=2)()
-    exp2 = experimenter_factory.BBOBExperimenterFactory('Sphere', dim=3)()
 
-    def _designer_factory(config: vz.ProblemStatement, seed: int):
-      return random.RandomDesigner(config.search_space, seed=seed)
-
-    state1_factory = benchmark_state.DesignerBenchmarkStateFactory(
-        designer_factory=_designer_factory, experimenter=exp1
-    )
-    state2_factory = benchmark_state.DesignerBenchmarkStateFactory(
-        designer_factory=_designer_factory, experimenter=exp2
+    # Set up policy supporter with one Active and Completed Trial.
+    policy_supporter = pythia.InRamPolicySupporter(problem)
+    trials = [
+        vz.Trial(parameters={'x': 0.5, 'y': 0.6}).complete(
+            vz.Measurement(metrics={'maximize_metric': 0.3})
+        ),
+        vz.Trial(parameters={'x': 0.1, 'y': 0.2}),
+    ]
+    # The Completed and Active Trials should be updated in Designer.
+    policy_supporter.AddTrials(trials)
+
+    class DummyDesigner(vza.Designer):
+
+      def __init__(self, problem_statement):
+        self._designer = random.RandomDesigner(problem_statement.search_space)
+        self.completed = []
+        self.all_active = []
+
+      def suggest(self, count):
+        return self._designer.suggest(count)
+
+      def update(self, completed, all_active):
+        self.completed.extend(completed.trials)
+        self.all_active = all_active.trials
+
+    designer = DummyDesigner(problem)
+    suggester = benchmark_state.PolicySuggester.from_designer_factory(
+        problem, lambda _, **kwargs: designer, supporter=policy_supporter
     )
 
-    runner = benchmark_runner.BenchmarkRunner(
-        benchmark_subroutines=[benchmark_runner.GenerateAndEvaluate()],
-        num_repeats=10,
+    suggestions = list(suggester.suggest(batch_size=5))
+    self.assertLen(designer.completed, 1)
+    self.assertLen(designer.all_active, 1)
+    self.assertLen(suggestions, 5)
+
+    # Report COMPLETED Trial back to supporter directly.
+    completed_trial = suggestions[0].complete(
+        vz.Measurement(metrics={'maximize_metric': 0.4})
     )
-
-    state1 = state1_factory()
-    state2 = state2_factory()
-    runner.run(state1)
-    runner.run(state2)
-
-    with self.assertRaisesRegex(ValueError, 'must have same problem'):
-      state_analyzer.BenchmarkStateAnalyzer.to_curve([state1, state2])
+    suggester.supporter.AddTrials([completed_trial])
+    suggester.suggest(1)
+    self.assertLen(designer.completed, 2)
+    self.assertLen(designer.all_active, 5)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo/common.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/experimenter_factory.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/experimenter_factory.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob/handler.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob/handler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/noisy_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/noisy_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/numpy_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/numpy_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/shifting_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/shifting_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sparse_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sparse_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/switch_experimenter.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/switch_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/experimenters/synthetic/bbob.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/experimenters/synthetic/bbob.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_runner.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_runner_test.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_runner_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/benchmarks/runners/benchmark_state.py` & `google-vizier-0.1.9/vizier/_src/benchmarks/runners/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/gp_bandit_utils.py` & `google-vizier-0.1.9/vizier/_src/jax/gp_bandit_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/__init__.py` & `google-vizier-0.1.9/vizier/_src/jax/models/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/continuous_only_kernel.py` & `google-vizier-0.1.9/vizier/_src/jax/models/continuous_only_kernel.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/gaussian_process_model.py` & `google-vizier-0.1.9/vizier/_src/jax/models/gaussian_process_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 """Coroutine for a trainable Gaussian process with an ARD kernel."""
 
 from typing import Any, Generator, Optional, Type, Union
 
+import jax
 from jax import numpy as jnp
 from tensorflow_probability.substrates import jax as tfp
 from vizier._src.jax import stochastic_process_model as sp_model
 from vizier._src.jax import types
 
 Array = Any
 tfd = tfp.distributions
@@ -86,14 +87,19 @@
         be expensive and should be used only during development/debugging.
       dtype: Float dtype.
     """
     self.dimension = dimension
     self._kernel_class = kernel_class
     self._use_tfp_runtime_validation = use_tfp_runtime_validation
     self.dtype = dtype
+    if dtype == jnp.float64 and not jax.config.read('jax_enable_x64'):
+      raise ValueError(
+          "x64 is not enabled for jax. Add jax_config.update('jax_enable_x64',"
+          ' True) to your main'
+      )
 
   def __call__(
       self, inputs: Optional[types.ModelInput] = None
   ) -> Generator[sp_model.ModelParameter, Array, tfd.GaussianProcess]:
     # TODO: Remove the following line when the linter bug is fixed.
     # pylint: disable=g-doc-return-or-yield
     """The coroutine that specifies the GP model.
```

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/gaussian_process_model_test.py` & `google-vizier-0.1.9/vizier/_src/jax/models/gaussian_process_model_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for gaussian_process_model."""
 
+import jax
 from jax import random
 import numpy as np
 from tensorflow_probability.substrates import jax as tfp
 from vizier._src.jax import types
 from vizier._src.jax.models import gaussian_process_model as gp_model
 from absl.testing import absltest
 
@@ -89,8 +90,9 @@
       param_vals[param.name] = v
       param = g.send(v)
   except StopIteration as e:
     return e.value, param_vals
 
 
 if __name__ == '__main__':
+  jax.config.update('jax_enable_x64', True)
   absltest.main()
```

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/hebo_gp_model.py` & `google-vizier-0.1.9/vizier/_src/jax/models/hebo_gp_model.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/hebo_gp_model_test.py` & `google-vizier-0.1.9/vizier/_src/jax/models/hebo_gp_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/mask_features.py` & `google-vizier-0.1.9/vizier/_src/jax/models/mask_features.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/mask_features_test.py` & `google-vizier-0.1.9/vizier/_src/jax/models/mask_features_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/tuned_gp_models.py` & `google-vizier-0.1.9/vizier/_src/jax/models/tuned_gp_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,16 @@
     kernel = tfpke.FeatureScaledWithCategorical(
         kernel,
         scale_diag=tfpke.ContinuousAndCategoricalValues(
             jnp.sqrt(continuous_length_scale_squared),
             jnp.sqrt(categorical_length_scale_squared),
         ),
     )
-    # TODO: Tune priors and add in shift/bias_amplitudes.
+
+    # We do not need to tune bias here because we are tuning mean_fn.
     slopes = yield sp.ModelParameter(
         init_fn=_log_uniform_init(*amplitude_bounds),
         constraint=sp.Constraint(
             amplitude_bounds,
             tfb.SoftClip(*amplitude_bounds, hinge_softness=1e-2),
         ),
         regularizer=lambda x: 0.01 * jnp.log(x / 0.039) ** 2,
```

### Comparing `google-vizier-0.1.8/vizier/_src/jax/models/tuned_gp_models_test.py` & `google-vizier-0.1.9/vizier/_src/jax/models/tuned_gp_models_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/core.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/core_test.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/core_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/jaxopt_wrappers.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/jaxopt_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/optax_wrappers.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/optax_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/optax_wrappers_test.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/optax_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/optimizers/testing/sinusoidal.py` & `google-vizier-0.1.9/vizier/_src/jax/optimizers/testing/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/predictive_fns.py` & `google-vizier-0.1.9/vizier/_src/jax/predictive_fns.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/predictive_fns_test.py` & `google-vizier-0.1.9/vizier/_src/jax/predictive_fns_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/stochastic_process_model.py` & `google-vizier-0.1.9/vizier/_src/jax/stochastic_process_model.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/stochastic_process_model_test.py` & `google-vizier-0.1.9/vizier/_src/jax/stochastic_process_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/types.py` & `google-vizier-0.1.9/vizier/_src/jax/types.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/types_test.py` & `google-vizier-0.1.9/vizier/_src/jax/types_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/xla_pareto.py` & `google-vizier-0.1.9/vizier/_src/jax/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/jax/xla_pareto_test.py` & `google-vizier-0.1.9/vizier/_src/jax/xla_pareto_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/algorithms.py` & `google-vizier-0.1.9/vizier/_src/pyglove/algorithms.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/backend.py` & `google-vizier-0.1.9/vizier/_src/pyglove/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,20 @@
         mode = TunerMode.PRIMARY  # We will make this a chief
         problem = self._converter.problem_or_dummy
         local_tuner_id = self._tuner.get_tuner_id(self._algorithm)
         problem.metadata.ns(constants.METADATA_NAMESPACE)[
             constants.STUDY_METADATA_KEY_TUNER_ID
         ] = local_tuner_id
         self._study = self._tuner.create_study(
-            problem, self._converter, study_owner, name, self._algorithm
+            problem,
+            self._converter,
+            study_owner,
+            name,
+            self._algorithm,
+            early_stopping_policy,
         )
         if local_tuner_id == self._get_chief_tuner_id():
           # For multi-thread scenario, `local_tuner_id` will be the same for
           # all the worker threads, therefore there is a chance that multiple
           # worker threads consider themselves as PRIMARY. This does not matter
           # since there is only one Pythia service shared across them.
           mode = TunerMode.PRIMARY  # We will make this a chief
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/client.py` & `google-vizier-0.1.9/vizier/_src/pyglove/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 """Abstraction for Vizier Tuner."""
 
 import abc
 import threading
-from typing import Dict, NewType, Union
+from typing import Dict, NewType, Optional, Union
 
 import attrs
 import pyglove as pg
 from vizier import pythia
 from vizier import pyvizier as vz
 from vizier._src.pyglove import converters
 from vizier._src.pyglove import pythia as pg_pythia
@@ -85,14 +85,15 @@
   def create_study(
       self,
       problem: vz.ProblemStatement,
       converter: converters.VizierConverter,
       owner: str,
       name: str,
       algorithm: pg.DNAGenerator,
+      stopping_policy: Optional[pg.tuning.EarlyStoppingPolicy] = None,
   ) -> client_abc.StudyInterface:
     """Creates a new study."""
 
   @abc.abstractmethod
   def get_group_id(self, group_id: Union[None, int, str] = None) -> str:
     """Get worker ID."""
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/constants.py` & `google-vizier-0.1.9/vizier/_src/pyglove/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/converters.py` & `google-vizier-0.1.9/vizier/_src/pyglove/converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/converters_test.py` & `google-vizier-0.1.9/vizier/_src/pyglove/converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/core.py` & `google-vizier-0.1.9/vizier/_src/pyglove/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/e2e_test.py` & `google-vizier-0.1.9/vizier/_src/pyglove/e2e_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/oss_vizier.py` & `google-vizier-0.1.9/vizier/_src/pyglove/oss_vizier.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
   def create_study(
       self,
       problem: vz.ProblemStatement,
       converter: converters.VizierConverter,
       owner: str,
       name: str,
       algorithm: pg.DNAGenerator,
+      stopping_policy: Optional[pg.tuning.EarlyStoppingPolicy] = None,
   ) -> client_abc.StudyInterface:
     """See parent class."""
     study_config = svz.StudyConfig.from_problem(problem)
     if converter.vizier_conversion_error:
       study_config.observation_noise = svz.ObservationNoise.HIGH
     self._configure_algorithm(study_config, algorithm)
     logging.info(
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/oss_vizier_test.py` & `google-vizier-0.1.9/vizier/_src/pyglove/oss_vizier_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for pyglove.tuner.vizier2.oss_vizier_test."""
+import datetime
 import os
-from absl import logging
 
+from absl import logging
 from vizier._src.pyglove import oss_vizier as vizier
 from vizier._src.pyglove import vizier_test_lib
 from vizier._src.service import constants
 from vizier._src.service import vizier_server
 
 from absl.testing import absltest
 
 
 class OSSVizierSampleTest(vizier_test_lib.SampleTest):
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
     server = vizier_server.DefaultVizierServer(
-        host=os.uname()[1], database_url=constants.SQL_MEMORY_URL
+        host=os.uname()[1],
+        database_url=constants.SQL_MEMORY_URL,
+        early_stop_recycle_period=datetime.timedelta(seconds=0.0),
     )
     logging.info(server.endpoint)
     vizier._services.reset_for_testing()
     vizier.init(vizier_endpoint=server.endpoint)
     cls.server = server
     logging.info('Vizier service has been set up!')
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/performance_test.py` & `google-vizier-0.1.9/vizier/_src/pyglove/performance_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/pythia.py` & `google-vizier-0.1.9/vizier/_src/pyglove/pythia.py`

 * *Files 15% similar despite different names*

```diff
@@ -103,20 +103,20 @@
 
     new_trials = []
     count = request.count or 1
 
     logging.info(
         (
             'The algorithm is updated with %s new trials out of %s newly'
-            ' completed trials.It has seen %s trials total. Now generating %s'
+            ' completed trials. It has seen %s trials total. Now generating %s'
             ' new suggestions.'
         ),
         n_trials_updated,
         len(newly_completed_trials),
-        str(self._suggestion_cache),
+        self._suggestion_cache.num_incorporated_trials,
         count,
     )
     for _ in range(request.count or 1):
       dna = self.algorithm.propose()
       if dna.spec is None:
         dna.use_spec(self._converter.dna_spec)
       trial = self._converter.to_trial(dna, fallback='return_dummy')
@@ -160,7 +160,36 @@
           pythia.EarlyStopDecision(
               vizier_trial.id,
               should_stop=should_stop,
               reason='Pyglove stopping policy stopped the trial.',
           )
       )
     return decisions
+
+
+def create_policy(
+    supporter: pythia.PolicySupporter,
+    problem_statement: vz.ProblemStatement,
+    algorithm: pg.geno.DNAGenerator,
+    early_stopping_policy: Optional[pg.tuning.EarlyStoppingPolicy] = None,
+    prior_trials: Optional[Sequence[vz.Trial]] = None,
+) -> pythia.Policy:
+  """Creates a Pythia policy that uses PyGlove algorithms."""
+  converter = converters.VizierConverter.from_problem(problem_statement)
+
+  # Bind the algorithm with the search space before usage.
+  algorithm.setup(converter.dna_spec)
+
+  # Warm up algorithm if prior trials are present.
+  if prior_trials:
+
+    def get_trial_history():
+      for trial in prior_trials:
+        tuner_trial = core.VizierTrial(converter, trial)
+        reward = tuner_trial.get_reward_for_feedback(
+            converter.metrics_to_optimize
+        )
+        yield (tuner_trial.dna, reward)
+
+    algorithm.recover(get_trial_history())
+
+  return TunerPolicy(supporter, converter, algorithm, early_stopping_policy)
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/pythia_test.py` & `google-vizier-0.1.9/vizier/_src/pyglove/pythia_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,33 +25,32 @@
 from vizier._src.algorithms.testing import test_runners
 from vizier._src.pyglove import converters
 from vizier._src.pyglove import pythia as pg_pythia
 from vizier._src.pyglove import vizier_test_lib
 
 from absl.testing import absltest
 
-_RandomAlgorithm = vizier_test_lib.DummyAlgorithm
+_RandomAlgorithm = vizier_test_lib.RandomAlgorithm
 
 
 class TunerPolicyTest(absltest.TestCase):
 
   def test_stopping_policy(self):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('x', 0.0, 1.0)
     problem.metric_information.append(
         vz.MetricInformation(name='r', goal=vz.ObjectiveMetricGoal.MAXIMIZE)
     )
 
-    converter = converters.VizierConverter.from_problem(problem)
     supporter = pythia.InRamPolicySupporter(problem)
 
     m = mock.create_autospec(pg.tuning.EarlyStoppingPolicy, instance=True)
-    policy = pg_pythia.TunerPolicy(
+    policy = pg_pythia.create_policy(
         supporter,
-        converter,
+        problem,
         algorithm=_RandomAlgorithm(),
         early_stopping_policy=m,
     )
 
     supporter.AddTrials([
         vz.Trial(
             parameters={'x': 0.0},
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyglove/vizier_test_lib.py` & `google-vizier-0.1.9/vizier/_src/pyglove/vizier_test_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,52 +12,84 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Libraries for testing different Tuners on the shared backend."""
 # pylint:disable=protected-access
+# pylint:disable=invalid-name
 import inspect
 from typing import Type
+
 from absl import flags
 from absl import logging
 import pyglove as pg
 from vizier._src.pyglove import backend
 
 from absl.testing import absltest
 
 FLAGS = flags.FLAGS
 
 
-class DummyAlgorithm(pg.DNAGenerator):
+class RandomAlgorithm(pg.DNAGenerator):
   """Dummy algorithm for testing."""
 
   def setup(self, dna_spec: pg.DNASpec):
     super().setup(dna_spec)
     self._random = pg.geno.Random(seed=1)
     self._random.setup(dna_spec)
 
   def _propose(self) -> pg.DNA:
     return self._random.propose()
 
 
+@pg.members([
+    ('max_trial_id', pg.typing.Int()),
+    ('max_step', pg.typing.Int()),
+])
+class SizeLimitingStoppingPolicy(pg.tuning.EarlyStoppingPolicy):
+  """Policy that stops trials when either ID or step is larger."""
+
+  def _on_bound(self):
+    super()._on_bound()
+    self.requested_trial_steps = []
+    self.stopped_trial_steps = []
+
+  def should_stop_early(self, trial: pg.tuning.Trial) -> bool:
+    if trial.status == 'COMPLETED':
+      return False
+
+    measurement = trial.measurements[-1]
+    self.requested_trial_steps.append((trial.id, measurement.step))
+    should_stop = (
+        trial.id > self.max_trial_id or measurement.step > self.max_step
+    )
+    if should_stop:
+      self.stopped_trial_steps.append((trial.id, measurement.step))
+    return should_stop
+
+
 class VizierTest(absltest.TestCase):
   """Base class for Vizier-based tests."""
 
   def __init__(
       self,
       backend_class: Type[backend.VizierBackend], *args, **kwargs
   ):
     self._backend_class = backend_class
     super().__init__(*args, **kwargs)
 
 
 class SampleTest(VizierTest):
   """Tests for PyGlove sampling with Vizier backend."""
 
+  def setUp(self):
+    super().setUp()
+    self._backend_class.use_study_prefix(self.id())
+
   def __init__(
       self,
       backend_class: Type[backend.VizierBackend],
       *args,
       builtin_multiobjective_algorithm_to_test: str,
       **kwargs):
     self._builtin_multiobjective_algorithm_to_test = (
@@ -65,15 +97,15 @@
     super().__init__(backend_class, *args, **kwargs)
 
   def testSample(self):
     """Test `pg.sample` with Vizier backend."""
     self._backend_class.use_study_prefix('distributed_sampling')
 
     rewards_a = []
-    algorithm = DummyAlgorithm()
+    algorithm = RandomAlgorithm()
     for a, fa in pg.sample(
         pg.Dict(x=pg.oneof([1, 2, 3])),  # Outer search space.
         algorithm=algorithm,
         num_examples=2,
         name='a',
     ):
       rs = []
@@ -424,14 +456,51 @@
                 t.measurements[0].elapse_secs,
                 t.created_time,
                 t.completed_time,
             )
         ),
     )
 
+  def testSampleWithEarlyStopping(self):
+    """Test sample with early stopping."""
+    # Stop trial early if either the trial id or trial-step is greater than 1.
+    early_stopping_policy = SizeLimitingStoppingPolicy(
+        max_trial_id=1, max_step=1
+    )
+    actually_stopped = []
+    for x, f in pg.sample(
+        pg.oneof([1, 2, 3]),
+        algorithm=RandomAlgorithm(),
+        early_stopping_policy=early_stopping_policy,
+        num_examples=2,
+    ):
+      skipped = False
+      for i in range(4):
+        f.add_measurement(x, step=i)
+        # Add a minimal sleep to ensure that the measurement is added to DB.
+        if f.should_stop_early():
+          f.skip()
+          skipped = True
+          actually_stopped.append((f.id, i))
+          break
+      if not skipped:
+        f.done()
+
+    self.assertEqual(
+        early_stopping_policy.requested_trial_steps,
+        [(1, 0), (1, 1), (1, 2), (2, 0)],
+    )
+    self.assertEqual(
+        early_stopping_policy.stopped_trial_steps, actually_stopped
+    )
+
+    self.assertEqual(
+        early_stopping_policy.stopped_trial_steps, [(1, 2), (2, 0)]
+    )
+
   def testSampleWithMultipleWorkers(self):
     """Test `pg.sample` with multiple workers."""
     self._backend_class.use_study_prefix(None)
 
     hyper_value = pg.Dict(x=pg.oneof([1, 2, 3]))
 
     # Create a new study for sample using Random.
@@ -461,34 +530,34 @@
         group=0,
     )
 
     # Make sure sampling with different worker IDs get different trial IDs.
     _, f1 = next(sample1)
     self.assertEqual(f1.id, 1)
     f1.set_metadata('x', 1)
-    f1.set_metadata('y', DummyAlgorithm(), per_trial=False)
+    f1.set_metadata('y', RandomAlgorithm(), per_trial=False)
 
     # X is not serializable via `pg.to_json_str()`.
     class X:
       pass
 
     with self.assertRaisesRegex(
         ValueError, 'Cannot convert local class .* to JSON'
     ):
       f1.set_metadata('z', X)
 
     _, f2 = next(sample2)
     self.assertEqual(f2.id, 2)
     self.assertIsNone(f2.get_metadata('x'))
-    self.assertEqual(f2.get_metadata('y', per_trial=False), DummyAlgorithm())
+    self.assertEqual(f2.get_metadata('y', per_trial=False), RandomAlgorithm())
 
     _, f3 = next(sample3)
     self.assertEqual(f3.id, 1)
     self.assertEqual(f3.get_metadata('x'), 1)
-    self.assertEqual(f3.get_metadata('y', per_trial=False), DummyAlgorithm())
+    self.assertEqual(f3.get_metadata('y', per_trial=False), RandomAlgorithm())
     # Update the value of 'x'.
     f3.set_metadata('x', 2)
     f3.set_metadata('z', 'foo')
     f3.add_measurement(0.1, step=1)
 
     # Make sure sampling within the same worker get the same trial IDs before
     # feedback.
```

### Comparing `google-vizier-0.1.8/vizier/_src/pythia/local_policy_supporters.py` & `google-vizier-0.1.9/vizier/_src/pythia/local_policy_supporters.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 """Policy supporters that keep data in RAM."""
 
 import datetime
 from typing import Iterable, List, Optional, Sequence
+import uuid
 
 from absl import logging
 import attr
 import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.pythia import policy
 from vizier._src.pythia import policy_supporter
@@ -46,15 +47,15 @@
         break
       for t in trials:
         t.complete(vz.Measurement(
             {'my_objective': my_objective(t)}, inplace=True))
 
   Attributes:
     study_config: Study config.
-    study_guid: Unique identifier for the study.
+    study_guid: Unique identifier for the current study.
   """
 
   study_config: vz.ProblemStatement = attr.ib(
       init=True,
       validator=attr.validators.instance_of(vz.ProblemStatement),
       on_setattr=attr.setters.frozen,
   )
@@ -64,14 +65,18 @@
       default='',
       converter=str,
       on_setattr=attr.setters.frozen,
   )
   _trials: dict[int, vz.Trial] = attr.ib(
       init=False, factory=dict, on_setattr=attr.setters.frozen
   )
+  # Dictionary of study_guid to ProblemAndTrials.
+  prior_studies: dict[str, vz.ProblemAndTrials] = attr.ib(
+      init=False, factory=dict
+  )
 
   def __str__(self) -> str:
     return (
         f'InRamPolicySupporter(study_guid={self.study_guid},'
         f' num_trials={len(self.trials)})'
     )
 
@@ -104,25 +109,34 @@
       min_trial_id: Optional[int] = None,
       max_trial_id: Optional[int] = None,
       status_matches: Optional[vz.TrialStatus] = None,
       include_intermediate_measurements: bool = True,
   ) -> List[vz.Trial]:
     """Returns trials by reference to allow changing their status and attributes."""
     self.CheckCancelled('GetTrials')
+    if study_guid is not None and study_guid != self.study_guid:
+      if study_guid not in self.prior_studies:
+        raise KeyError(f'Study Guid does not exist {study_guid}')
+
+      candidate_trials = self.prior_studies[study_guid].trials
+    else:
+      candidate_trials = self.trials
+
+    trial_id_set = None
     if trial_ids is not None:
       trial_id_set = set(trial_ids)
     output: List[vz.Trial] = []
-    for t in self.trials:
+    for t in candidate_trials:
       if status_matches is not None and t.status != status_matches:
         continue
       if min_trial_id is not None and t.id < min_trial_id:
         continue
       if max_trial_id is not None and t.id > max_trial_id:
         continue
-      if trial_ids is not None and t.id not in trial_id_set:
+      if trial_id_set is not None and t.id not in trial_id_set:
         continue
       # NOTE: we ignore include_intermediate_measurements and always enclude
       # them.  That should be safe, and avoids a nasty conflict with the
       # pass-by-reference philosophy for Trials (you can't delete the
       # intermediate measurements without deleting them everywhere, and you
       # can't copy the trial without breaking desired reference connections).
       output.append(t)
@@ -187,14 +201,29 @@
     else:
       algorithm = multimetric.FastParetoOptimalAlgorithm()
       is_optimal = algorithm.is_pareto_optimal(
           points=converter.to_labels(self.trials)
       )
       return list(np.asarray(self.trials)[is_optimal][:count])
 
+  def SetPriorStudy(
+      self, study: vz.ProblemAndTrials, study_guid: Optional[str] = None
+  ) -> str:
+    if study_guid is None:
+      # Assign study_guid using unique identifier.
+      study_guid = f'prior_{uuid.uuid1()}'
+      if study_guid in self.prior_studies:
+        raise RuntimeError(f'Cannot set unique id: {study_guid}')
+
+    if study_guid in self.prior_studies:
+      logging.warning('Prior study already exists with guid %s ', study_guid)
+
+    self.prior_studies[study_guid] = study
+    return study_guid
+
   def AddTrials(self, trials: Sequence[vz.Trial]) -> None:
     """Assigns ids to the trials and add them to the supporter (by reference).
 
     New IDs are always assigned in increasing order from the max id unless:
       * If an incoming Trial has an ID that matches an ACTIVE Trial, the ACTIVE
     Trial is replaced and the COMPLETED Trial keeps its ID.
       * If an incoming Trial has an ID that matches an COMPLETE Trial, no
```

### Comparing `google-vizier-0.1.8/vizier/_src/pythia/local_policy_supporters_test.py` & `google-vizier-0.1.9/vizier/_src/pythia/local_policy_supporters_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for vizier.pythia.base.local_policy_supporters."""
 
 import numpy as np
-
 from vizier import pyvizier as vz
 from vizier._src.pythia import local_policy_supporters
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 InRamPolicySupporter = local_policy_supporters.InRamPolicySupporter
@@ -69,14 +68,61 @@
     # The 10 trials are assigned ids 1 through 10 automatically.
     self.assertSequenceEqual([t.id for t in trials], range(1, 11))
     self.assertEqual(trials[0].infeasibility_reason, 'test')
 
     trials = runner.GetTrials(status_matches=vz.TrialStatus.ACTIVE)
     self.assertLen(trials, 9)
 
+  def test_prior_studies(self):
+    runner = _runner_with_10trials()
+
+    # Add a PriorStudy with study guid 1 and 10 completed Trials.
+    prior_runner = _runner_with_10trials()
+    completed_trials = []
+    for t in prior_runner.GetTrials():
+      t.complete(vz.Measurement())
+      completed_trials.append(t)
+    study = vz.ProblemAndTrials(
+        problem=vz.ProblemStatement(), trials=completed_trials
+    )
+    study_guid = runner.SetPriorStudy(study, study_guid='1')
+    self.assertEqual(study_guid, '1')
+
+    # Add another PriorStudy with generated study guid and it has
+    # 5 active and completed Trials
+    prior_runner = _runner_with_10trials()
+    trials = []
+    for idx, t in enumerate(prior_runner.GetTrials()):
+      if idx > 4:
+        t.complete(vz.Measurement())
+      trials.append(t)
+    study = vz.ProblemAndTrials(problem=vz.ProblemStatement(), trials=trials)
+    generated_study_guid = runner.SetPriorStudy(study)
+
+    active_trials = runner.GetTrials(
+        study_guid=study_guid, status_matches=vz.TrialStatus.ACTIVE
+    )
+    self.assertEmpty(active_trials)
+    completed_trials = runner.GetTrials(
+        study_guid=study_guid, status_matches=vz.TrialStatus.COMPLETED
+    )
+    self.assertLen(completed_trials, 10)
+
+    active_trials = runner.GetTrials(
+        study_guid=generated_study_guid, status_matches=vz.TrialStatus.ACTIVE
+    )
+    self.assertLen(active_trials, 5)
+    completed_trials = runner.GetTrials(
+        study_guid=generated_study_guid, status_matches=vz.TrialStatus.COMPLETED
+    )
+    self.assertLen(completed_trials, 5)
+
+    with self.assertRaises(KeyError):
+      runner.GetTrials(study_guid='2')
+
   def test_push_metadata(self):
     runner = _runner_with_10trials()
     trial1 = runner.GetTrials(min_trial_id=1, max_trial_id=1)[0]
 
     mu = vz.MetadataDelta()
     mu.assign('ns', 'key', 'value')
     mu.assign('ns', 'key', 'value', trial_id=1)
```

### Comparing `google-vizier-0.1.8/vizier/_src/pythia/policy.py` & `google-vizier-0.1.9/vizier/_src/pythia/policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pythia/policy_supporter.py` & `google-vizier-0.1.9/vizier/_src/pythia/policy_supporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,19 @@
       VizierDatabaseError: If the database operation raises an error, e.g. if
         $study_guid refers to a nonexistent or inaccessible study.
 
     NOTE: if $trial_ids is set, $min_trial_id, $max_trial_id, and
       $status_matches will be ignored.
     """
 
+  @property
+  @abc.abstractmethod
+  def study_guid(self) -> str:
+    """Default study GUID."""
+
   def CheckCancelled(self, note: Optional[str] = None) -> None:
     """Throws a CancelComputeError on timeout or if Vizier cancels.
 
     This should be called occasionally by any long-running computation.
     Raises an exception if the interaction has been cancelled by the Vizier
     side of the protocol; the exception shuts down the Pythia server.
```

### Comparing `google-vizier-0.1.8/vizier/_src/pythia/pythia_errors.py` & `google-vizier-0.1.9/vizier/_src/pythia/pythia_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/hypervolume.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/hypervolume.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/hypervolume_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/hypervolume_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/pareto_optimal.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/pareto_optimal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/safety.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/safety.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/multimetric/safety_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/multimetric/safety_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/automated_stopping.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/automated_stopping.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/automated_stopping_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/automated_stopping_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/compare.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/compare.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/metadata_util.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/metadata_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/metadata_util_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/metadata_util_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/proto_converters.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/proto_converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/proto_converters_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/proto_converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/study_config.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/study_config.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/oss/study_config_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/oss/study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/pythia/study.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/pythia/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/base_study_config.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/base_study_config.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/base_study_config_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/base_study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/common.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/common_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/common_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/context.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/context.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/context_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/context_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_config.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_config.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_config_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_iterators.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_iterators.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/parameter_iterators_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/parameter_iterators_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/study.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/trial.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -611,14 +611,20 @@
       self.completion_time = _to_local_time(datetime.datetime.now())
       return self
     else:
       clone = copy.deepcopy(self)
       return clone.complete(
           measurement, inplace=True, infeasibility_reason=infeasibility_reason)
 
+  @property
+  def final_measurement_or_die(self) -> Measurement:
+    if self.final_measurement is None:
+      raise ValueError('Trial is missing final_measurement.')
+    return self.final_measurement
+
 
 # Define aliases.
 CompletedTrial = Trial
 PendingTrial = Trial
 CompletedTrialWithMeasurements = Trial
 PendingTrialWithMeasurements = Trial
```

### Comparing `google-vizier-0.1.8/vizier/_src/pyvizier/shared/trial_test.py` & `google-vizier-0.1.9/vizier/_src/pyvizier/shared/trial_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/raytune/converters.py` & `google-vizier-0.1.9/vizier/_src/raytune/converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/raytune/converters_test.py` & `google-vizier-0.1.9/vizier/_src/raytune/converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/raytune/run_tune.py` & `google-vizier-0.1.9/vizier/_src/raytune/run_tune.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/raytune/run_tune_test.py` & `google-vizier-0.1.9/vizier/_src/raytune/run_tune_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/raytune/vizier_search.py` & `google-vizier-0.1.9/vizier/_src/raytune/vizier_search.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/raytune/vizier_search_test.py` & `google-vizier-0.1.9/vizier/_src/raytune/vizier_search_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/clients.py` & `google-vizier-0.1.9/vizier/_src/service/clients.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/clients_test.py` & `google-vizier-0.1.9/vizier/_src/service/clients_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/constants.py` & `google-vizier-0.1.9/vizier/_src/service/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/custom_errors.py` & `google-vizier-0.1.9/vizier/_src/service/custom_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/datastore.py` & `google-vizier-0.1.9/vizier/_src/service/datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/datastore_test_lib.py` & `google-vizier-0.1.9/vizier/_src/service/datastore_test_lib.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/grpc_util.py` & `google-vizier-0.1.9/vizier/_src/service/grpc_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/performance_test.py` & `google-vizier-0.1.9/vizier/_src/service/performance_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/policy_factory.py` & `google-vizier-0.1.9/vizier/_src/service/policy_factory.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/pythia_service.py` & `google-vizier-0.1.9/vizier/_src/service/pythia_service.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/pythia_util.py` & `google-vizier-0.1.9/vizier/_src/service/pythia_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/ram_datastore.py` & `google-vizier-0.1.9/vizier/_src/service/ram_datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/ram_datastore_test.py` & `google-vizier-0.1.9/vizier/_src/service/ram_datastore_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/resources.py` & `google-vizier-0.1.9/vizier/_src/service/resources.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/resources_test.py` & `google-vizier-0.1.9/vizier/_src/service/resources_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/service_policy_supporter.py` & `google-vizier-0.1.9/vizier/_src/service/service_policy_supporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,18 @@
       study_guid: A default study_name; the name of this study.
       vizier_service: Vizier Service, in the form of a GRPC stub or actual
         class.
     """
     self._study_guid = study_guid
     self._vizier_service = vizier_service
 
+  @property
+  def study_guid(self) -> str:
+    return self._study_guid
+
   def GetStudyConfig(self, study_guid: str) -> vz.ProblemStatement:
     request = vizier_service_pb2.GetStudyRequest(name=study_guid)
     study = self._vizier_service.GetStudy(request)
     return pyvizier.StudyConfig.from_proto(study.study_spec).to_problem()
 
   # TODO: Support filters in ListTrialsRequest.
   def GetTrials(
```

### Comparing `google-vizier-0.1.8/vizier/_src/service/service_policy_supporter_test.py` & `google-vizier-0.1.9/vizier/_src/service/service_policy_supporter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/sql_datastore.py` & `google-vizier-0.1.9/vizier/_src/service/sql_datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/sql_datastore_test.py` & `google-vizier-0.1.9/vizier/_src/service/sql_datastore_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/stubs_util.py` & `google-vizier-0.1.9/vizier/_src/service/stubs_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/stubs_util_test.py` & `google-vizier-0.1.9/vizier/_src/service/stubs_util_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/testing/util.py` & `google-vizier-0.1.9/vizier/_src/service/testing/util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/types.py` & `google-vizier-0.1.9/vizier/_src/service/types.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/vizier_client.py` & `google-vizier-0.1.9/vizier/_src/service/vizier_client.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/vizier_client_test.py` & `google-vizier-0.1.9/vizier/_src/service/vizier_client_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/vizier_server.py` & `google-vizier-0.1.9/vizier/_src/service/vizier_server.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/vizier_service.py` & `google-vizier-0.1.9/vizier/_src/service/vizier_service.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/_src/service/vizier_service_test.py` & `google-vizier-0.1.9/vizier/_src/service/vizier_service_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/algorithms/__init__.py` & `google-vizier-0.1.9/vizier/algorithms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,7 @@
 from vizier._src.algorithms.core.abstractions import Predictor
 from vizier._src.algorithms.core.abstractions import SerializableDesigner
 from vizier._src.algorithms.optimizers.base import BatchTrialScoreFunction
 from vizier._src.algorithms.optimizers.base import BranchSelection
 from vizier._src.algorithms.optimizers.base import BranchSelector
 from vizier._src.algorithms.optimizers.base import BranchThenOptimizer
 from vizier._src.algorithms.optimizers.base import GradientFreeOptimizer
-from vizier._src.algorithms.optimizers.designer_optimizer import DesignerAsOptimizer
```

### Comparing `google-vizier-0.1.8/vizier/algorithms/designers/__init__.py` & `google-vizier-0.1.9/vizier/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/algorithms/policies/__init__.py` & `google-vizier-0.1.9/vizier/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/benchmarks/__init__.py` & `google-vizier-0.1.9/vizier/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/benchmarks/analyzers.py` & `google-vizier-0.1.9/vizier/benchmarks/analyzers.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Curve Analysis utilities for benchmarking and metalearning."""
 # pylint: disable=unused-import
 
-from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceComparatorBase
+from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceComparator
+from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceComparatorFactory
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurve
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurveConverter
 from vizier._src.benchmarks.analyzers.convergence_curve import HypervolumeCurveConverter
 from vizier._src.benchmarks.analyzers.convergence_curve import LogEfficiencyConvergenceCurveComparator
 from vizier._src.benchmarks.analyzers.convergence_curve import PercentageBetterConvergenceCurveComparator
+from vizier._src.benchmarks.analyzers.plot_utils import plot_from_records
+from vizier._src.benchmarks.analyzers.plot_utils import plot_mean_convergence
+from vizier._src.benchmarks.analyzers.plot_utils import plot_median_convergence
+from vizier._src.benchmarks.analyzers.state_analyzer import BenchmarkRecord
 from vizier._src.benchmarks.analyzers.state_analyzer import BenchmarkStateAnalyzer
+from vizier._src.benchmarks.analyzers.state_analyzer import PlotElement
```

### Comparing `google-vizier-0.1.8/vizier/benchmarks/experimenters/__init__.py` & `google-vizier-0.1.9/vizier/benchmarks/experimenters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/benchmarks/experimenters/hpo/__init__.py` & `google-vizier-0.1.9/vizier/benchmarks/experimenters/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/benchmarks/experimenters/nas/__init__.py` & `google-vizier-0.1.9/vizier/benchmarks/experimenters/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/benchmarks/experimenters/rl/__init__.py` & `google-vizier-0.1.9/vizier/benchmarks/experimenters/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/client/__init__.py` & `google-vizier-0.1.9/vizier/client/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/client/client_abc.py` & `google-vizier-0.1.9/vizier/client/client_abc.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/client/client_abc_testing.py` & `google-vizier-0.1.9/vizier/client/client_abc_testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/interfaces/__init__.py` & `google-vizier-0.1.9/vizier/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/interfaces/serializable.py` & `google-vizier-0.1.9/vizier/interfaces/serializable.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/jax/__init__.py` & `google-vizier-0.1.9/vizier/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/jax/models.py` & `google-vizier-0.1.9/vizier/jax/models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/jax/optimizers.py` & `google-vizier-0.1.9/vizier/jax/optimizers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyglove/__init__.py` & `google-vizier-0.1.9/vizier/service/clients/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Vizier backend for PyGlove."""
-from vizier._src.pyglove.algorithms import BuiltinAlgorithm
-from vizier._src.pyglove.converters import VizierConverter
-from vizier._src.pyglove.oss_vizier import init
+"""OSS Client API."""
+from vizier._src.service.clients import environment_variables
+from vizier._src.service.clients import Study
+from vizier._src.service.clients import Trial
+from vizier._src.service.clients import TrialIterable
```

### Comparing `google-vizier-0.1.8/vizier/pythia.py` & `google-vizier-0.1.9/vizier/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/__init__.py` & `google-vizier-0.1.9/vizier/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/__init__.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/core.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/core_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/core_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/embedder.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/embedder.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/embedder_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/embedder_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/feature_mapper.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/feature_mapper.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/feature_mapper_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/feature_mapper_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/input_warping.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/input_warping.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/input_warping_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/input_warping_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/jnp_converters.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/jnp_converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/jnp_converters_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/jnp_converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/padding.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/padding.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/padding_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/padding_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/spatio_temporal.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/spatio_temporal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/converters/spatio_temporal_test.py` & `google-vizier-0.1.9/vizier/pyvizier/converters/spatio_temporal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/multimetric/__init__.py` & `google-vizier-0.1.9/vizier/pyvizier/multimetric/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/pyvizier/multimetric/xla_pareto.py` & `google-vizier-0.1.9/vizier/pyvizier/multimetric/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/raytune/__init__.py` & `google-vizier-0.1.9/vizier/raytune/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/service/__init__.py` & `google-vizier-0.1.9/vizier/service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/service/clients/__init__.py` & `google-vizier-0.1.9/vizier/service/protos/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""OSS Client API."""
-from vizier._src.service.clients import environment_variables
-from vizier._src.service.clients import Study
-from vizier._src.service.clients import Trial
-from vizier._src.service.clients import TrialIterable
+"""All protos used in the service."""
+from vizier._src.service import key_value_pb2
+from vizier._src.service import pythia_service_pb2
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_oss_pb2
+from vizier._src.service import vizier_service_pb2
```

### Comparing `google-vizier-0.1.8/vizier/service/pyvizier/__init__.py` & `google-vizier-0.1.9/vizier/service/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/service/servers/__init__.py` & `google-vizier-0.1.9/vizier/service/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/testing/__init__.py` & `google-vizier-0.1.9/vizier/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/testing/numpy_assertions.py` & `google-vizier-0.1.9/vizier/testing/numpy_assertions.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/testing/test_studies.py` & `google-vizier-0.1.9/vizier/testing/test_studies.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/utils/attrs_utils.py` & `google-vizier-0.1.9/vizier/utils/attrs_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/utils/attrs_utils_test.py` & `google-vizier-0.1.9/vizier/utils/attrs_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/utils/json_utils.py` & `google-vizier-0.1.9/vizier/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/utils/json_utils_test.py` & `google-vizier-0.1.9/vizier/utils/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/utils/profiler.py` & `google-vizier-0.1.9/vizier/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.8/vizier/utils/profiler_test.py` & `google-vizier-0.1.9/vizier/utils/profiler_test.py`

 * *Files identical despite different names*

