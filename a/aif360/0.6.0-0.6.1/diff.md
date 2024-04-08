# Comparing `tmp/aif360-0.6.0.tar.gz` & `tmp/aif360-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aif360-0.6.0.tar", last modified: Fri Feb 23 14:40:39 2024, max compression
+gzip compressed data, was "aif360-0.6.1.tar", last modified: Mon Apr  8 19:57:05 2024, max compression
```

## Comparing `aif360-0.6.0.tar` & `aif360-0.6.1.tar`

### file list

```diff
@@ -1,272 +1,297 @@
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.084579 aif360-0.6.0/
--rw-r--r--   0 shoffman   (501) staff       (20)    11372 2024-02-23 14:36:04.000000 aif360-0.6.0/LICENSE
--rw-r--r--   0 shoffman   (501) staff       (20)      210 2024-02-23 14:36:04.000000 aif360-0.6.0/MANIFEST.in
--rw-r--r--   0 shoffman   (501) staff       (20)     4650 2024-02-23 14:40:39.083873 aif360-0.6.0/PKG-INFO
--rw-r--r--   0 shoffman   (501) staff       (20)    10003 2024-02-23 14:36:04.000000 aif360-0.6.0/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.959072 aif360-0.6.0/aif360/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/README.md
--rw-r--r--   0 shoffman   (501) staff       (20)       82 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/__init__.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.962939 aif360-0.6.0/aif360/algorithms/
--rw-r--r--   0 shoffman   (501) staff       (20)       67 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/__init__.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.966899 aif360-0.6.0/aif360/algorithms/inprocessing/
--rw-r--r--   0 shoffman   (501) staff       (20)      594 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    13771 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/adversarial_debiasing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2066 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/art_classifier.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.968716 aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/
--rw-r--r--   0 shoffman   (501) staff       (20)     2422 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/FalseDiscovery.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3910 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/General.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2331 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/StatisticalRate.py
--rw-r--r--   0 shoffman   (501) staff       (20)      168 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     5083 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/exponentiated_gradient_reduction.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.972106 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/
--rwxr-xr-x   0 shoffman   (501) staff       (20)      462 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/__init__.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)    11192 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/auditor.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     1042 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/classifier_history.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     5709 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/clean.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     1708 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/fairness_plots.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     4131 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/heatmap.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     2648 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/learner.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     1913 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/reg_oracle_class.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)    12449 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair_classifier.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6598 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/grid_search_reduction.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.973661 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/__init__.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.974330 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/
--rw-r--r--   0 shoffman   (501) staff       (20)     2511 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/__init__.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.975598 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/
--rw-r--r--   0 shoffman   (501) staff       (20)      441 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    15703 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/pr.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.977027 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/
--rw-r--r--   0 shoffman   (501) staff       (20)      257 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4058 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/_base.py
--rw-r--r--   0 shoffman   (501) staff       (20)     8554 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/predict_lr.py
--rw-r--r--   0 shoffman   (501) staff       (20)     9860 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/train_pr.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3313 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/meta_fair_classifier.py
--rw-r--r--   0 shoffman   (501) staff       (20)     9370 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/inprocessing/prejudice_remover.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.980519 aif360-0.6.0/aif360/algorithms/postprocessing/
--rw-r--r--   0 shoffman   (501) staff       (20)      391 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/postprocessing/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     9905 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/postprocessing/calibrated_eq_odds_postprocessing.py
--rw-r--r--   0 shoffman   (501) staff       (20)    10983 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/postprocessing/deterministic_reranking.py
--rw-r--r--   0 shoffman   (501) staff       (20)    11870 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/postprocessing/eq_odds_postprocessing.py
--rw-r--r--   0 shoffman   (501) staff       (20)    11255 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/postprocessing/reject_option_classification.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.983621 aif360-0.6.0/aif360/algorithms/preprocessing/
--rw-r--r--   0 shoffman   (501) staff       (20)      281 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2594 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/disparate_impact_remover.py
--rw-r--r--   0 shoffman   (501) staff       (20)     7969 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/lfr.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.984719 aif360-0.6.0/aif360/algorithms/preprocessing/lfr_helpers/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/lfr_helpers/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1802 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/lfr_helpers/helpers.py
--rw-r--r--   0 shoffman   (501) staff       (20)    11530 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.986575 aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    11395 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/data_preproc_functions.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6595 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/distortion_functions.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)    18812 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/opt_tools.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)     4913 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/preprocessing/reweighing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4026 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/algorithms/transformer.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.987034 aif360-0.6.0/aif360/data/
--rw-r--r--   0 shoffman   (501) staff       (20)     1431 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.987424 aif360-0.6.0/aif360/data/raw/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.987739 aif360-0.6.0/aif360/data/raw/adult/
--rw-r--r--   0 shoffman   (501) staff       (20)     1097 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/adult/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.988136 aif360-0.6.0/aif360/data/raw/bank/
--rw-r--r--   0 shoffman   (501) staff       (20)     1044 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/bank/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.988534 aif360-0.6.0/aif360/data/raw/compas/
--rw-r--r--   0 shoffman   (501) staff       (20)      754 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/compas/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.989079 aif360-0.6.0/aif360/data/raw/german/
--rw-r--r--   0 shoffman   (501) staff       (20)      685 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/german/README.md
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.989985 aif360-0.6.0/aif360/data/raw/meps/
--rw-r--r--   0 shoffman   (501) staff       (20)     4611 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/meps/README.md
--rwxr-xr-x   0 shoffman   (501) staff       (20)     1877 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/data/raw/meps/generate_data.R
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.997539 aif360-0.6.0/aif360/datasets/
--rw-r--r--   0 shoffman   (501) staff       (20)      806 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     5467 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/adult_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2623 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/bank_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2023 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/binary_label_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3865 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/compas_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2419 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4663 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/german_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1439 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/law_school_gpa_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     7022 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/lime_encoder.py
--rw-r--r--   0 shoffman   (501) staff       (20)     5803 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/meps_dataset_panel19_fy2015.py
--rw-r--r--   0 shoffman   (501) staff       (20)     5841 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/meps_dataset_panel20_fy2015.py
--rw-r--r--   0 shoffman   (501) staff       (20)     5840 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/meps_dataset_panel21_fy2016.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2327 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/multiclass_label_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4924 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/regression_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     7470 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/standard_dataset.py
--rwxr-xr-x   0 shoffman   (501) staff       (20)    25740 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/datasets/structured_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)      995 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/decorating_metaclass.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.998444 aif360-0.6.0/aif360/detectors/
--rw-r--r--   0 shoffman   (501) staff       (20)       96 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/__init__.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:38.999623 aif360-0.6.0/aif360/detectors/mdss/
--rw-r--r--   0 shoffman   (501) staff       (20)    18354 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/MDSS.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.002473 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/
--rw-r--r--   0 shoffman   (501) staff       (20)     4057 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/BerkJones.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3656 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/Bernoulli.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3228 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/Gaussian.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3411 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/Poisson.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2289 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/ScoringFunction.py
--rw-r--r--   0 shoffman   (501) staff       (20)      361 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3965 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/optim.py
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1657 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss/generator.py
--rw-r--r--   0 shoffman   (501) staff       (20)     7557 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/detectors/mdss_detector.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.004122 aif360-0.6.0/aif360/explainers/
--rw-r--r--   0 shoffman   (501) staff       (20)      194 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/explainers/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)      155 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/explainers/explainer.py
--rw-r--r--   0 shoffman   (501) staff       (20)    38003 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/explainers/metric_json_explainer.py
--rw-r--r--   0 shoffman   (501) staff       (20)    15878 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/explainers/metric_text_explainer.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.008340 aif360-0.6.0/aif360/metrics/
--rw-r--r--   0 shoffman   (501) staff       (20)      471 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    11349 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/binary_label_dataset_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)    40379 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/classification_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4493 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/dataset_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4905 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/mdss_classification_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1553 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)    10995 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/ot_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4376 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/regression_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6772 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/sample_distortion_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     8113 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/metrics/utils.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.009611 aif360-0.6.0/aif360/sklearn/
--rw-r--r--   0 shoffman   (501) staff       (20)     2307 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/README.md
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/__init__.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.012840 aif360-0.6.0/aif360/sklearn/datasets/
--rw-r--r--   0 shoffman   (501) staff       (20)      770 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/datasets/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4851 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/datasets/compas_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4030 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/datasets/lawschool_dataset.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6334 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/datasets/meps_datasets.py
--rw-r--r--   0 shoffman   (501) staff       (20)    10796 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/datasets/openml_datasets.py
--rw-r--r--   0 shoffman   (501) staff       (20)     5456 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/datasets/utils.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.013940 aif360-0.6.0/aif360/sklearn/detectors/
--rw-r--r--   0 shoffman   (501) staff       (20)      167 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/detectors/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3533 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/detectors/detectors.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.016171 aif360-0.6.0/aif360/sklearn/inprocessing/
--rw-r--r--   0 shoffman   (501) staff       (20)      551 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/inprocessing/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    15593 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/inprocessing/adversarial_debiasing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6304 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/inprocessing/exponentiated_gradient_reduction.py
--rw-r--r--   0 shoffman   (501) staff       (20)     8519 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/inprocessing/grid_search_reduction.py
--rw-r--r--   0 shoffman   (501) staff       (20)    15963 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/inprocessing/infairness.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.017441 aif360-0.6.0/aif360/sklearn/metrics/
--rw-r--r--   0 shoffman   (501) staff       (20)      291 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/metrics/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    53001 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/metrics/metrics.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.018762 aif360-0.6.0/aif360/sklearn/postprocessing/
--rw-r--r--   0 shoffman   (501) staff       (20)     9808 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/postprocessing/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)    10331 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/postprocessing/calibrated_equalized_odds.py
--rw-r--r--   0 shoffman   (501) staff       (20)    16570 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/postprocessing/reject_option_classification.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.020937 aif360-0.6.0/aif360/sklearn/preprocessing/
--rw-r--r--   0 shoffman   (501) staff       (20)      419 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/preprocessing/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)      944 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/preprocessing/fairadapt.R
--rw-r--r--   0 shoffman   (501) staff       (20)     4623 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/preprocessing/fairadapt.py
--rw-r--r--   0 shoffman   (501) staff       (20)     8809 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/preprocessing/learning_fair_representations.py
--rw-r--r--   0 shoffman   (501) staff       (20)     8003 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/preprocessing/reweighing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4409 2024-02-23 14:36:04.000000 aif360-0.6.0/aif360/sklearn/utils.py
--rw-r--r--   0 shoffman   (501) staff       (20)       42 2024-02-23 14:40:38.000000 aif360-0.6.0/aif360/version.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.075670 aif360-0.6.0/aif360.egg-info/
--rw-r--r--   0 shoffman   (501) staff       (20)     4650 2024-02-23 14:40:38.000000 aif360-0.6.0/aif360.egg-info/PKG-INFO
--rw-r--r--   0 shoffman   (501) staff       (20)     9220 2024-02-23 14:40:38.000000 aif360-0.6.0/aif360.egg-info/SOURCES.txt
--rw-r--r--   0 shoffman   (501) staff       (20)        1 2024-02-23 14:40:38.000000 aif360-0.6.0/aif360.egg-info/dependency_links.txt
--rw-r--r--   0 shoffman   (501) staff       (20)        1 2024-02-23 14:38:51.000000 aif360-0.6.0/aif360.egg-info/not-zip-safe
--rw-r--r--   0 shoffman   (501) staff       (20)     1001 2024-02-23 14:40:38.000000 aif360-0.6.0/aif360.egg-info/requires.txt
--rw-r--r--   0 shoffman   (501) staff       (20)        7 2024-02-23 14:40:38.000000 aif360-0.6.0/aif360.egg-info/top_level.txt
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.022449 aif360-0.6.0/docs/
--rw-r--r--   0 shoffman   (501) staff       (20)      681 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/Makefile
--rw-r--r--   0 shoffman   (501) staff       (20)      211 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/README.md
--rw-r--r--   0 shoffman   (501) staff       (20)      808 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/make.bat
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.024700 aif360-0.6.0/docs/source/
--rw-r--r--   0 shoffman   (501) staff       (20)       35 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/CONTRIBUTING.rst
--rw-r--r--   0 shoffman   (501) staff       (20)     8760 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/Getting Started.rst
--rw-r--r--   0 shoffman   (501) staff       (20)     8159 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/conf.py
--rw-r--r--   0 shoffman   (501) staff       (20)      634 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/index.rst
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.027704 aif360-0.6.0/docs/source/modules/
--rw-r--r--   0 shoffman   (501) staff       (20)     1791 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/modules/algorithms.rst
--rw-r--r--   0 shoffman   (501) staff       (20)      749 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/modules/datasets.rst
--rw-r--r--   0 shoffman   (501) staff       (20)      325 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/modules/explainers.rst
--rw-r--r--   0 shoffman   (501) staff       (20)      897 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/modules/metrics.rst
--rw-r--r--   0 shoffman   (501) staff       (20)     5631 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/modules/sklearn.rst
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.028363 aif360-0.6.0/docs/source/static/
--rw-r--r--   0 shoffman   (501) staff       (20)      254 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/static/style.css
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.029583 aif360-0.6.0/docs/source/templates/
--rw-r--r--   0 shoffman   (501) staff       (20)      137 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/templates/base.rst
--rw-r--r--   0 shoffman   (501) staff       (20)      616 2024-02-23 14:36:04.000000 aif360-0.6.0/docs/source/templates/class.rst
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.046084 aif360-0.6.0/examples/
--rw-r--r--   0 shoffman   (501) staff       (20)     3693 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/README.md
--rw-r--r--   0 shoffman   (501) staff       (20)     1340 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/common_utils.py
--rw-r--r--   0 shoffman   (501) staff       (20)    39796 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_adversarial_debiasing.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   214634 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_calibrated_eqodds_postprocessing.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    26257 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_deterministic_reranking.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    63477 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_disparate_impact_remover.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    15263 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_exponentiated_gradient_reduction.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   188457 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_gerryfair.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)     6286 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_json_explainers.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    16449 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_lfr.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   285909 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_lime.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    40509 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_mdss_classifier_metric.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    51506 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_mdss_detector.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   110507 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_meta_classifier.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    25603 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_optim_data_preproc.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    16460 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_optim_preproc_adult.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   193408 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_ot_metric.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    26518 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_reject_option_classification.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   223703 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_reweighing_preproc.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)     6170 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/demo_short_gerryfair_test.ipynb
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.048330 aif360-0.6.0/examples/images/
--rw-r--r--   0 shoffman   (501) staff       (20)    13957 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/images/Complex_NoProc_V3.jpg
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.055464 aif360-0.6.0/examples/sklearn/
--rw-r--r--   0 shoffman   (501) staff       (20)    30746 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_exponentiated_gradient_reduction_sklearn.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    61788 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_fairadapt_sklearn.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    48010 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_grid_search_reduction_classification_sklearn.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    17193 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_grid_search_reduction_regression_sklearn.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   261090 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_learning_fair_representations.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)   148207 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_mdss_bias_scan.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    28506 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_mdss_classifier_metric_sklearn.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    77885 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_new_features.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    93944 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_reject_option_classification.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    37114 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/demo_sensei_infairness.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    54521 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/sklearn/monthly_bee_datasets_metrics.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    49025 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/tutorial_bias_advertising.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)    15240 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/tutorial_credit_scoring.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)  1296286 2024-02-23 14:36:04.000000 aif360-0.6.0/examples/tutorial_medical_expenditure.ipynb
--rw-r--r--   0 shoffman   (501) staff       (20)       38 2024-02-23 14:40:39.084750 aif360-0.6.0/setup.cfg
--rw-r--r--   0 shoffman   (501) staff       (20)     2711 2024-02-23 14:36:04.000000 aif360-0.6.0/setup.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.068676 aif360-0.6.0/tests/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/README.md
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1145 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/notebook_runner.py
-drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-02-23 14:40:39.075123 aif360-0.6.0/tests/sklearn/
--rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/__init__.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1366 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/conftest.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3404 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_adversarial_debiasing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     4167 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_calibrated_equalized_odds.py
--rw-r--r--   0 shoffman   (501) staff       (20)    11977 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_datasets.py
--rw-r--r--   0 shoffman   (501) staff       (20)      487 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_demo_exp_grad_red_sklearn.py
--rw-r--r--   0 shoffman   (501) staff       (20)      934 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_demo_grid_search_red_sklearn.py
--rw-r--r--   0 shoffman   (501) staff       (20)      487 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_demo_mdss_classifier_metric_sklearn.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2264 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_fairadapt.py
--rw-r--r--   0 shoffman   (501) staff       (20)     7100 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_infairness.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3696 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_learning_fair_representations.py
--rw-r--r--   0 shoffman   (501) staff       (20)     9200 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_metrics.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6899 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_reject_option_classification.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2005 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/sklearn/test_reweighing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     7083 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_classification_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)      530 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_adversarial_debiasing.py
--rw-r--r--   0 shoffman   (501) staff       (20)      546 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_calibrated_eqodds_postprocessing.py
--rw-r--r--   0 shoffman   (501) staff       (20)      453 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_exp_grad_red.py
--rw-r--r--   0 shoffman   (501) staff       (20)      494 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_lfr.py
--rw-r--r--   0 shoffman   (501) staff       (20)      453 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_mdss_classifier_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)      514 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_optim_data_preproc.py
--rw-r--r--   0 shoffman   (501) staff       (20)      539 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_reject_option_classification.py
--rw-r--r--   0 shoffman   (501) staff       (20)      519 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_demo_reweighing_preproc.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2954 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_deterministic_reranking.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3200 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_differential_fairness.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2779 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_disparate_impact_remover.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1982 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_eq_odds_postprocessing.py
--rw-r--r--   0 shoffman   (501) staff       (20)      434 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_gerryfair.py
--rw-r--r--   0 shoffman   (501) staff       (20)     3819 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_lfr.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2371 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_meta_classifier.py
--rw-r--r--   0 shoffman   (501) staff       (20)     6417 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_ot_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1234 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_regression_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)      581 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_reweighing.py
--rw-r--r--   0 shoffman   (501) staff       (20)     1976 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_sample_distortion_metric.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2565 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_standard_datasets.py
--rw-r--r--   0 shoffman   (501) staff       (20)     2060 2024-02-23 14:36:04.000000 aif360-0.6.0/tests/test_structured_dataset.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.431653 aif360-0.6.1/
+-rw-r--r--   0 shoffman   (501) staff       (20)    11372 2024-04-08 19:48:56.000000 aif360-0.6.1/LICENSE
+-rw-r--r--   0 shoffman   (501) staff       (20)      210 2024-04-08 19:48:56.000000 aif360-0.6.1/MANIFEST.in
+-rw-r--r--   0 shoffman   (501) staff       (20)     4993 2024-04-08 19:57:05.431087 aif360-0.6.1/PKG-INFO
+-rw-r--r--   0 shoffman   (501) staff       (20)    10003 2024-04-08 19:48:56.000000 aif360-0.6.1/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.290718 aif360-0.6.1/aif360/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/README.md
+-rw-r--r--   0 shoffman   (501) staff       (20)       82 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/__init__.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.294467 aif360-0.6.1/aif360/algorithms/
+-rw-r--r--   0 shoffman   (501) staff       (20)       67 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/__init__.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.298299 aif360-0.6.1/aif360/algorithms/inprocessing/
+-rw-r--r--   0 shoffman   (501) staff       (20)      594 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    13771 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/adversarial_debiasing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2066 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/art_classifier.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.300096 aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/
+-rw-r--r--   0 shoffman   (501) staff       (20)     2422 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/FalseDiscovery.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3910 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/General.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2331 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/StatisticalRate.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      168 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5083 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/exponentiated_gradient_reduction.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.304067 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/
+-rwxr-xr-x   0 shoffman   (501) staff       (20)      462 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/__init__.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)    11192 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/auditor.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     1042 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/classifier_history.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     5709 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/clean.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     1708 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/fairness_plots.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     4131 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/heatmap.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     2648 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/learner.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     1913 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/reg_oracle_class.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)    12449 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair_classifier.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6598 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/grid_search_reduction.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.305613 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/__init__.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.306343 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/
+-rw-r--r--   0 shoffman   (501) staff       (20)     2511 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/__init__.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.307678 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/
+-rw-r--r--   0 shoffman   (501) staff       (20)      441 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    15691 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/pr.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.309115 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/
+-rw-r--r--   0 shoffman   (501) staff       (20)      257 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4058 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/_base.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     8554 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/predict_lr.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     9860 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/train_pr.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3313 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/meta_fair_classifier.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     9370 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/inprocessing/prejudice_remover.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.312555 aif360-0.6.1/aif360/algorithms/postprocessing/
+-rw-r--r--   0 shoffman   (501) staff       (20)      391 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/postprocessing/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     9905 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/postprocessing/calibrated_eq_odds_postprocessing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    10983 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/postprocessing/deterministic_reranking.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11870 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/postprocessing/eq_odds_postprocessing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11255 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/postprocessing/reject_option_classification.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.315982 aif360-0.6.1/aif360/algorithms/preprocessing/
+-rw-r--r--   0 shoffman   (501) staff       (20)      281 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2594 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/disparate_impact_remover.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7969 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/lfr.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.317130 aif360-0.6.1/aif360/algorithms/preprocessing/lfr_helpers/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/lfr_helpers/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1802 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/lfr_helpers/helpers.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11530 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.319576 aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11395 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/data_preproc_functions.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6595 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/distortion_functions.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)    18812 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/opt_tools.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     4913 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/preprocessing/reweighing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4026 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/algorithms/transformer.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.320088 aif360-0.6.1/aif360/data/
+-rw-r--r--   0 shoffman   (501) staff       (20)     1431 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.320517 aif360-0.6.1/aif360/data/raw/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.321143 aif360-0.6.1/aif360/data/raw/adult/
+-rw-r--r--   0 shoffman   (501) staff       (20)     1097 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/adult/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.322053 aif360-0.6.1/aif360/data/raw/bank/
+-rw-r--r--   0 shoffman   (501) staff       (20)     1044 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/bank/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.322855 aif360-0.6.1/aif360/data/raw/compas/
+-rw-r--r--   0 shoffman   (501) staff       (20)      754 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/compas/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.323509 aif360-0.6.1/aif360/data/raw/german/
+-rw-r--r--   0 shoffman   (501) staff       (20)      685 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/german/README.md
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.324640 aif360-0.6.1/aif360/data/raw/meps/
+-rw-r--r--   0 shoffman   (501) staff       (20)     4611 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/meps/README.md
+-rwxr-xr-x   0 shoffman   (501) staff       (20)     1877 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/data/raw/meps/generate_data.R
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.332621 aif360-0.6.1/aif360/datasets/
+-rw-r--r--   0 shoffman   (501) staff       (20)      806 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5467 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/adult_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2623 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/bank_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2023 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/binary_label_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3865 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/compas_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2419 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4663 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/german_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1439 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/law_school_gpa_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7022 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/lime_encoder.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5803 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/meps_dataset_panel19_fy2015.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5841 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/meps_dataset_panel20_fy2015.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5840 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/meps_dataset_panel21_fy2016.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2327 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/multiclass_label_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4924 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/regression_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7470 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/standard_dataset.py
+-rwxr-xr-x   0 shoffman   (501) staff       (20)    25740 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/datasets/structured_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      995 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/decorating_metaclass.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.333478 aif360-0.6.1/aif360/detectors/
+-rw-r--r--   0 shoffman   (501) staff       (20)       96 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/__init__.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.334724 aif360-0.6.1/aif360/detectors/mdss/
+-rw-r--r--   0 shoffman   (501) staff       (20)    18354 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/MDSS.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.337606 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/
+-rw-r--r--   0 shoffman   (501) staff       (20)     4057 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/BerkJones.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3656 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/Bernoulli.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3228 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/Gaussian.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3411 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/Poisson.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2289 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/ScoringFunction.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      361 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3965 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/optim.py
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1657 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss/generator.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7557 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/detectors/mdss_detector.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.339244 aif360-0.6.1/aif360/explainers/
+-rw-r--r--   0 shoffman   (501) staff       (20)      194 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/explainers/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      155 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/explainers/explainer.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    38003 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/explainers/metric_json_explainer.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    15878 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/explainers/metric_text_explainer.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.344047 aif360-0.6.1/aif360/metrics/
+-rw-r--r--   0 shoffman   (501) staff       (20)      471 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11349 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/binary_label_dataset_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    40379 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/classification_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4493 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/dataset_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4905 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/mdss_classification_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1553 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    10995 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/ot_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4376 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/regression_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6772 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/sample_distortion_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     8113 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/metrics/utils.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.345463 aif360-0.6.1/aif360/sklearn/
+-rw-r--r--   0 shoffman   (501) staff       (20)     2307 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/README.md
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/__init__.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.348280 aif360-0.6.1/aif360/sklearn/datasets/
+-rw-r--r--   0 shoffman   (501) staff       (20)      770 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/datasets/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4851 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/datasets/compas_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4030 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/datasets/lawschool_dataset.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6334 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/datasets/meps_datasets.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    10796 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/datasets/openml_datasets.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5456 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/datasets/utils.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.349094 aif360-0.6.1/aif360/sklearn/detectors/
+-rw-r--r--   0 shoffman   (501) staff       (20)      335 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3538 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/detectors.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.354648 aif360-0.6.1/aif360/sklearn/detectors/facts/
+-rw-r--r--   0 shoffman   (501) staff       (20)    27037 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5250 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/clean.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    15775 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/formatting.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3071 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/frequent_itemsets.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7991 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/metrics.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    26701 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/misc.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5327 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/optimization.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6459 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/parameters.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     8181 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/predicate.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11290 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/rule_filters.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4845 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/detectors/facts/utils.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.357835 aif360-0.6.1/aif360/sklearn/inprocessing/
+-rw-r--r--   0 shoffman   (501) staff       (20)      551 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/inprocessing/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    15593 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/inprocessing/adversarial_debiasing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6304 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/inprocessing/exponentiated_gradient_reduction.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     8519 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/inprocessing/grid_search_reduction.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    15963 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/inprocessing/infairness.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.359212 aif360-0.6.1/aif360/sklearn/metrics/
+-rw-r--r--   0 shoffman   (501) staff       (20)      291 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/metrics/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    53001 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/metrics/metrics.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.361395 aif360-0.6.1/aif360/sklearn/postprocessing/
+-rw-r--r--   0 shoffman   (501) staff       (20)     9808 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/postprocessing/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    10331 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/postprocessing/calibrated_equalized_odds.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    16570 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/postprocessing/reject_option_classification.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.364639 aif360-0.6.1/aif360/sklearn/preprocessing/
+-rw-r--r--   0 shoffman   (501) staff       (20)      419 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/preprocessing/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      944 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/preprocessing/fairadapt.R
+-rw-r--r--   0 shoffman   (501) staff       (20)     4623 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/preprocessing/fairadapt.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     8809 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/preprocessing/learning_fair_representations.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     8003 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/preprocessing/reweighing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4409 2024-04-08 19:48:56.000000 aif360-0.6.1/aif360/sklearn/utils.py
+-rw-r--r--   0 shoffman   (501) staff       (20)       42 2024-04-08 19:57:05.000000 aif360-0.6.1/aif360/version.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.423395 aif360-0.6.1/aif360.egg-info/
+-rw-r--r--   0 shoffman   (501) staff       (20)     4993 2024-04-08 19:57:05.000000 aif360-0.6.1/aif360.egg-info/PKG-INFO
+-rw-r--r--   0 shoffman   (501) staff       (20)    10143 2024-04-08 19:57:05.000000 aif360-0.6.1/aif360.egg-info/SOURCES.txt
+-rw-r--r--   0 shoffman   (501) staff       (20)        1 2024-04-08 19:57:05.000000 aif360-0.6.1/aif360.egg-info/dependency_links.txt
+-rw-r--r--   0 shoffman   (501) staff       (20)        1 2024-04-08 19:56:21.000000 aif360-0.6.1/aif360.egg-info/not-zip-safe
+-rw-r--r--   0 shoffman   (501) staff       (20)     1066 2024-04-08 19:57:05.000000 aif360-0.6.1/aif360.egg-info/requires.txt
+-rw-r--r--   0 shoffman   (501) staff       (20)        7 2024-04-08 19:57:05.000000 aif360-0.6.1/aif360.egg-info/top_level.txt
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.366361 aif360-0.6.1/docs/
+-rw-r--r--   0 shoffman   (501) staff       (20)      681 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/Makefile
+-rw-r--r--   0 shoffman   (501) staff       (20)      305 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/README.md
+-rw-r--r--   0 shoffman   (501) staff       (20)      808 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/make.bat
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.368781 aif360-0.6.1/docs/source/
+-rw-r--r--   0 shoffman   (501) staff       (20)       35 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/CONTRIBUTING.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)     8760 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/Getting Started.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)     8159 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/conf.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      634 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/index.rst
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.372466 aif360-0.6.1/docs/source/modules/
+-rw-r--r--   0 shoffman   (501) staff       (20)     1791 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/modules/algorithms.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)      749 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/modules/datasets.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)      325 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/modules/explainers.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)      897 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/modules/metrics.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)     5751 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/modules/sklearn.rst
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.373032 aif360-0.6.1/docs/source/static/
+-rw-r--r--   0 shoffman   (501) staff       (20)      254 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/static/style.css
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.373771 aif360-0.6.1/docs/source/templates/
+-rw-r--r--   0 shoffman   (501) staff       (20)      137 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/templates/base.rst
+-rw-r--r--   0 shoffman   (501) staff       (20)      616 2024-04-08 19:48:56.000000 aif360-0.6.1/docs/source/templates/class.rst
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.387938 aif360-0.6.1/examples/
+-rw-r--r--   0 shoffman   (501) staff       (20)     3693 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/README.md
+-rw-r--r--   0 shoffman   (501) staff       (20)     1340 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/common_utils.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    37904 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_FACTS.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    39796 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_adversarial_debiasing.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   214634 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_calibrated_eqodds_postprocessing.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    26257 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_deterministic_reranking.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    63477 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_disparate_impact_remover.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    15263 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_exponentiated_gradient_reduction.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   188457 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_gerryfair.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)     6286 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_json_explainers.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    16449 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_lfr.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   285909 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_lime.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    40509 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_mdss_classifier_metric.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    51506 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_mdss_detector.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   110507 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_meta_classifier.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    25603 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_optim_data_preproc.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    16460 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_optim_preproc_adult.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   193408 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_ot_metric.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    26518 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_reject_option_classification.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   223703 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_reweighing_preproc.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)     6170 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/demo_short_gerryfair_test.ipynb
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.389880 aif360-0.6.1/examples/images/
+-rw-r--r--   0 shoffman   (501) staff       (20)    13957 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/images/Complex_NoProc_V3.jpg
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.396887 aif360-0.6.1/examples/sklearn/
+-rw-r--r--   0 shoffman   (501) staff       (20)    30746 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_exponentiated_gradient_reduction_sklearn.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    61788 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_fairadapt_sklearn.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    48010 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_grid_search_reduction_classification_sklearn.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    17193 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_grid_search_reduction_regression_sklearn.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   261090 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_learning_fair_representations.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)   148207 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_mdss_bias_scan.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    28506 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_mdss_classifier_metric_sklearn.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    77885 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_new_features.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    93944 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_reject_option_classification.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    37114 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/demo_sensei_infairness.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    54521 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/sklearn/monthly_bee_datasets_metrics.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    49025 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/tutorial_bias_advertising.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)    15240 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/tutorial_credit_scoring.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)  1296286 2024-04-08 19:48:56.000000 aif360-0.6.1/examples/tutorial_medical_expenditure.ipynb
+-rw-r--r--   0 shoffman   (501) staff       (20)       38 2024-04-08 19:57:05.431773 aif360-0.6.1/setup.cfg
+-rw-r--r--   0 shoffman   (501) staff       (20)     2757 2024-04-08 19:48:56.000000 aif360-0.6.1/setup.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.408106 aif360-0.6.1/tests/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/README.md
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1145 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/notebook_runner.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.417217 aif360-0.6.1/tests/sklearn/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1366 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/conftest.py
+drwxr-xr-x   0 shoffman   (501) staff       (20)        0 2024-04-08 19:57:05.422689 aif360-0.6.1/tests/sklearn/facts/
+-rw-r--r--   0 shoffman   (501) staff       (20)        0 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/__init__.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4132 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_clean.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4423 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_formatting.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      905 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_frequent_itemsets.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7636 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_metrics.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    17696 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_misc.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    18782 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_optimization.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     5169 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_parameters.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7719 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_predicate.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    13163 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_rule_filters.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1922 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/facts/test_utils.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3404 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_adversarial_debiasing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     4167 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_calibrated_equalized_odds.py
+-rw-r--r--   0 shoffman   (501) staff       (20)    11977 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_datasets.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      487 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_demo_exp_grad_red_sklearn.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      934 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_demo_grid_search_red_sklearn.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      487 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_demo_mdss_classifier_metric_sklearn.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2264 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_fairadapt.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7100 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_infairness.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3696 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_learning_fair_representations.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     9200 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_metrics.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6899 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_reject_option_classification.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2005 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/sklearn/test_reweighing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     7083 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_classification_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      530 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_adversarial_debiasing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      546 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_calibrated_eqodds_postprocessing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      453 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_exp_grad_red.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      494 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_lfr.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      453 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_mdss_classifier_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      514 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_optim_data_preproc.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      539 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_reject_option_classification.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      519 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_demo_reweighing_preproc.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2954 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_deterministic_reranking.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3200 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_differential_fairness.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2779 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_disparate_impact_remover.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1982 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_eq_odds_postprocessing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      434 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_gerryfair.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     3819 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_lfr.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2371 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_meta_classifier.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     6417 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_ot_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1234 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_regression_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)      581 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_reweighing.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     1976 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_sample_distortion_metric.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2565 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_standard_datasets.py
+-rw-r--r--   0 shoffman   (501) staff       (20)     2060 2024-04-08 19:48:56.000000 aif360-0.6.1/tests/test_structured_dataset.py
```

### Comparing `aif360-0.6.0/LICENSE` & `aif360-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/PKG-INFO` & `aif360-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aif360
-Version: 0.6.0
+Version: 0.6.1
 Summary: IBM AI Fairness 360
 Home-page: https://github.com/Trusted-AI/AIF360
 Author: aif360 developers
 Author-email: aif360@us.ibm.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -48,14 +48,18 @@
 Requires-Dist: tqdm; extra == "notebooks"
 Requires-Dist: igraph[plotting]; extra == "notebooks"
 Requires-Dist: lightgbm; extra == "notebooks"
 Requires-Dist: seaborn; extra == "notebooks"
 Requires-Dist: ipympl; extra == "notebooks"
 Provides-Extra: optimaltransport
 Requires-Dist: pot; extra == "optimaltransport"
+Provides-Extra: facts
+Requires-Dist: mlxtend; extra == "facts"
+Requires-Dist: colorama; extra == "facts"
+Requires-Dist: tqdm; extra == "facts"
 Provides-Extra: tests
 Requires-Dist: cvxpy>=1.0; extra == "tests"
 Requires-Dist: tensorflow>=1.13.1; extra == "tests"
 Requires-Dist: BlackBoxAuditing; extra == "tests"
 Requires-Dist: torch; extra == "tests"
 Requires-Dist: lime; extra == "tests"
 Requires-Dist: adversarial-robustness-toolbox>=1.0.0; extra == "tests"
@@ -66,44 +70,49 @@
 Requires-Dist: jupyter; extra == "tests"
 Requires-Dist: tqdm; extra == "tests"
 Requires-Dist: igraph[plotting]; extra == "tests"
 Requires-Dist: lightgbm; extra == "tests"
 Requires-Dist: seaborn; extra == "tests"
 Requires-Dist: ipympl; extra == "tests"
 Requires-Dist: pot; extra == "tests"
+Requires-Dist: mlxtend; extra == "tests"
+Requires-Dist: colorama; extra == "tests"
+Requires-Dist: tqdm; extra == "tests"
 Requires-Dist: pytest>=3.5; extra == "tests"
 Requires-Dist: pytest-cov>=2.8.1; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: jinja2>3.1.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: fairlearn~=0.7; extra == "docs"
 Provides-Extra: all
-Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: fairlearn~=0.7; extra == "all"
-Requires-Dist: jupyter; extra == "all"
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: lightgbm; extra == "all"
-Requires-Dist: pot; extra == "all"
-Requires-Dist: pytest>=3.5; extra == "all"
-Requires-Dist: rpy2; extra == "all"
-Requires-Dist: jinja2>3.1.0; extra == "all"
 Requires-Dist: tqdm; extra == "all"
+Requires-Dist: adversarial-robustness-toolbox>=1.0.0; extra == "all"
+Requires-Dist: mlxtend; extra == "all"
+Requires-Dist: pytest>=3.5; extra == "all"
+Requires-Dist: igraph[plotting]; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: inFairness>=0.2.2; extra == "all"
 Requires-Dist: pytest-cov>=2.8.1; extra == "all"
 Requires-Dist: skorch; extra == "all"
 Requires-Dist: BlackBoxAuditing; extra == "all"
+Requires-Dist: fairlearn~=0.7; extra == "all"
+Requires-Dist: lightgbm; extra == "all"
+Requires-Dist: cvxpy>=1.0; extra == "all"
+Requires-Dist: rpy2; extra == "all"
+Requires-Dist: sphinx; extra == "all"
+Requires-Dist: pot; extra == "all"
+Requires-Dist: colorama; extra == "all"
+Requires-Dist: jinja2>3.1.0; extra == "all"
+Requires-Dist: jupyter; extra == "all"
 Requires-Dist: tensorflow>=1.13.1; extra == "all"
+Requires-Dist: sphinx_rtd_theme; extra == "all"
 Requires-Dist: lime; extra == "all"
-Requires-Dist: torch; extra == "all"
-Requires-Dist: igraph[plotting]; extra == "all"
-Requires-Dist: inFairness>=0.2.2; extra == "all"
 Requires-Dist: ipympl; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: adversarial-robustness-toolbox>=1.0.0; extra == "all"
-Requires-Dist: cvxpy>=1.0; extra == "all"
+Requires-Dist: torch; extra == "all"
 
 The AI Fairness 360 toolkit is an open-source library to help detect and mitigate bias in machine
 learning models. The AI Fairness 360 Python package includes a comprehensive set of metrics for datasets and models to
 test for biases, explanations for these metrics, and algorithms to mitigate bias in datasets and models.
 
 We have developed the package with extensibility in mind. This library is still in development. We encourage the
 contribution of your datasets, metrics, explainers, and debiasing algorithms.
```

### Comparing `aif360-0.6.0/README.md` & `aif360-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/__init__.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/adversarial_debiasing.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/adversarial_debiasing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/art_classifier.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/art_classifier.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/FalseDiscovery.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/FalseDiscovery.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/General.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/General.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/celisMeta/StatisticalRate.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/celisMeta/StatisticalRate.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/exponentiated_gradient_reduction.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/exponentiated_gradient_reduction.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/auditor.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/auditor.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/classifier_history.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/classifier_history.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/clean.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/clean.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/fairness_plots.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/fairness_plots.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/heatmap.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/heatmap.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/learner.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/learner.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair/reg_oracle_class.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair/reg_oracle_class.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/gerryfair_classifier.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/gerryfair_classifier.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/grid_search_reduction.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/grid_search_reduction.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/__init__.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/__init__.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/pr.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/lr/pr.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,34 +209,34 @@
         s : array, shape=(n_samples)
             values of sensitive features
         """
 
         if itype == 0:
             # clear by zeros
             self.coef_ = np.zeros(self.n_sfv_ * self.n_features_,
-                                  dtype=np.float)
+                                  dtype=float)
         elif itype == 1:
             # at random
             self.coef_ = np.random.randn(self.n_sfv_ * self.n_features_)
 
         elif itype == 2:
             # learned by standard LR
             self.coef_ = np.empty(self.n_sfv_ * self.n_features_,
-                                  dtype=np.float)
+                                  dtype=float)
             coef = self.coef_.reshape(self.n_sfv_, self.n_features_)
 
             clr = LogisticRegression(C=self.C, penalty='l2',
                                      fit_intercept=False)
             clr.fit(X, y)
 
             coef[:, :] = clr.coef_
         elif itype == 3:
             # learned by standard LR
             self.coef_ = np.empty(self.n_sfv_ * self.n_features_,
-                                  dtype=np.float)
+                                  dtype=float)
             coef = self.coef_.reshape(self.n_sfv_, self.n_features_)
 
             for i in range(self.n_sfv_):
                 clr = LogisticRegression(C=self.C, penalty='l2', max_iter=1000,
                                          fit_intercept=False)
                 clr.fit(X[s == i, :], y[s == i])
                 coef[i, :] = clr.coef_
@@ -272,15 +272,15 @@
             kwargs['disp'] = False
         if not 'maxiter' in kwargs:
             kwargs['maxiter'] = 100
 
         # set instance variables
         self.n_s_ = ns
         self.n_sfv_ = np.max(s) + 1
-        self.c_s_ = np.array([np.sum(s == si).astype(np.float)
+        self.c_s_ = np.array([np.sum(s == si).astype(float)
                               for si in range(self.n_sfv_)])
         self.n_features_ = X.shape[1]
         self.n_samples_ = X.shape[0]
 
         # optimization
         self.init_coef(itype, X, y, s)
         self.coef_ = fmin_cg(self.loss,
```

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/_base.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/fadm/util/_base.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/predict_lr.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/predict_lr.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/train_pr.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/kamfadm-2012ecmlpkdd/train_pr.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/meta_fair_classifier.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/meta_fair_classifier.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/inprocessing/prejudice_remover.py` & `aif360-0.6.1/aif360/algorithms/inprocessing/prejudice_remover.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/postprocessing/calibrated_eq_odds_postprocessing.py` & `aif360-0.6.1/aif360/algorithms/postprocessing/calibrated_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/postprocessing/deterministic_reranking.py` & `aif360-0.6.1/aif360/algorithms/postprocessing/deterministic_reranking.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/postprocessing/eq_odds_postprocessing.py` & `aif360-0.6.1/aif360/algorithms/postprocessing/eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/postprocessing/reject_option_classification.py` & `aif360-0.6.1/aif360/algorithms/postprocessing/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/disparate_impact_remover.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/disparate_impact_remover.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/lfr.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/lfr.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/lfr_helpers/helpers.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/lfr_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/data_preproc_functions.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/data_preproc_functions.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/distortion_functions.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/distortion_functions.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/optim_preproc_helpers/opt_tools.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/optim_preproc_helpers/opt_tools.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/preprocessing/reweighing.py` & `aif360-0.6.1/aif360/algorithms/preprocessing/reweighing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/algorithms/transformer.py` & `aif360-0.6.1/aif360/algorithms/transformer.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/README.md` & `aif360-0.6.1/aif360/data/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/raw/adult/README.md` & `aif360-0.6.1/aif360/data/raw/adult/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/raw/bank/README.md` & `aif360-0.6.1/aif360/data/raw/bank/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/raw/compas/README.md` & `aif360-0.6.1/aif360/data/raw/compas/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/raw/german/README.md` & `aif360-0.6.1/aif360/data/raw/german/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/raw/meps/README.md` & `aif360-0.6.1/aif360/data/raw/meps/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/data/raw/meps/generate_data.R` & `aif360-0.6.1/aif360/data/raw/meps/generate_data.R`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/__init__.py` & `aif360-0.6.1/aif360/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/adult_dataset.py` & `aif360-0.6.1/aif360/datasets/adult_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/bank_dataset.py` & `aif360-0.6.1/aif360/datasets/bank_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/binary_label_dataset.py` & `aif360-0.6.1/aif360/datasets/binary_label_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/compas_dataset.py` & `aif360-0.6.1/aif360/datasets/compas_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/dataset.py` & `aif360-0.6.1/aif360/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/german_dataset.py` & `aif360-0.6.1/aif360/datasets/german_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/law_school_gpa_dataset.py` & `aif360-0.6.1/aif360/datasets/law_school_gpa_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/lime_encoder.py` & `aif360-0.6.1/aif360/datasets/lime_encoder.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/meps_dataset_panel19_fy2015.py` & `aif360-0.6.1/aif360/datasets/meps_dataset_panel19_fy2015.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/meps_dataset_panel20_fy2015.py` & `aif360-0.6.1/aif360/datasets/meps_dataset_panel20_fy2015.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/meps_dataset_panel21_fy2016.py` & `aif360-0.6.1/aif360/datasets/meps_dataset_panel21_fy2016.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/multiclass_label_dataset.py` & `aif360-0.6.1/aif360/datasets/multiclass_label_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/regression_dataset.py` & `aif360-0.6.1/aif360/datasets/regression_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/standard_dataset.py` & `aif360-0.6.1/aif360/datasets/standard_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/datasets/structured_dataset.py` & `aif360-0.6.1/aif360/datasets/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/decorating_metaclass.py` & `aif360-0.6.1/aif360/decorating_metaclass.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/MDSS.py` & `aif360-0.6.1/aif360/detectors/mdss/MDSS.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/BerkJones.py` & `aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/BerkJones.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/Bernoulli.py` & `aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/Bernoulli.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/Gaussian.py` & `aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/Gaussian.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/Poisson.py` & `aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/Poisson.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/ScoringFunction.py` & `aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/ScoringFunction.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/ScoringFunctions/optim.py` & `aif360-0.6.1/aif360/detectors/mdss/ScoringFunctions/optim.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss/generator.py` & `aif360-0.6.1/aif360/detectors/mdss/generator.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/detectors/mdss_detector.py` & `aif360-0.6.1/aif360/detectors/mdss_detector.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/explainers/metric_json_explainer.py` & `aif360-0.6.1/aif360/explainers/metric_json_explainer.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/explainers/metric_text_explainer.py` & `aif360-0.6.1/aif360/explainers/metric_text_explainer.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/binary_label_dataset_metric.py` & `aif360-0.6.1/aif360/metrics/binary_label_dataset_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/classification_metric.py` & `aif360-0.6.1/aif360/metrics/classification_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/dataset_metric.py` & `aif360-0.6.1/aif360/metrics/dataset_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/mdss_classification_metric.py` & `aif360-0.6.1/aif360/metrics/mdss_classification_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/metric.py` & `aif360-0.6.1/aif360/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/ot_metric.py` & `aif360-0.6.1/aif360/metrics/ot_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/regression_metric.py` & `aif360-0.6.1/aif360/metrics/regression_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/sample_distortion_metric.py` & `aif360-0.6.1/aif360/metrics/sample_distortion_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/metrics/utils.py` & `aif360-0.6.1/aif360/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/README.md` & `aif360-0.6.1/aif360/sklearn/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/datasets/__init__.py` & `aif360-0.6.1/aif360/sklearn/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/datasets/compas_dataset.py` & `aif360-0.6.1/aif360/sklearn/datasets/compas_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/datasets/lawschool_dataset.py` & `aif360-0.6.1/aif360/sklearn/datasets/lawschool_dataset.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/datasets/meps_datasets.py` & `aif360-0.6.1/aif360/sklearn/datasets/meps_datasets.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/datasets/openml_datasets.py` & `aif360-0.6.1/aif360/sklearn/datasets/openml_datasets.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/datasets/utils.py` & `aif360-0.6.1/aif360/sklearn/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/detectors/detectors.py` & `aif360-0.6.1/aif360/sklearn/detectors/detectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from aif360.detectors import bias_scan as _bias_scan
 from aif360.detectors.mdss.ScoringFunctions import ScoringFunction
 
 import pandas as pd
 
 
-def bias_scan(
+def MDSS_bias_scan(
     X: pd.DataFrame,
     y_true: pd.Series,
     y_pred: Union[pd.Series, pd.DataFrame] = None,
     pos_label: Union[str, float] = None,
     overpredicted: bool = True,
     scoring: Union[str, ScoringFunction] = "Bernoulli",
     num_iters: int = 10,
```

### Comparing `aif360-0.6.0/aif360/sklearn/inprocessing/__init__.py` & `aif360-0.6.1/aif360/sklearn/inprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/inprocessing/adversarial_debiasing.py` & `aif360-0.6.1/aif360/sklearn/inprocessing/adversarial_debiasing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/inprocessing/exponentiated_gradient_reduction.py` & `aif360-0.6.1/aif360/sklearn/inprocessing/exponentiated_gradient_reduction.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/inprocessing/grid_search_reduction.py` & `aif360-0.6.1/aif360/sklearn/inprocessing/grid_search_reduction.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/inprocessing/infairness.py` & `aif360-0.6.1/aif360/sklearn/inprocessing/infairness.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/metrics/metrics.py` & `aif360-0.6.1/aif360/sklearn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/postprocessing/__init__.py` & `aif360-0.6.1/aif360/sklearn/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/postprocessing/calibrated_equalized_odds.py` & `aif360-0.6.1/aif360/sklearn/postprocessing/calibrated_equalized_odds.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/postprocessing/reject_option_classification.py` & `aif360-0.6.1/aif360/sklearn/postprocessing/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/preprocessing/fairadapt.R` & `aif360-0.6.1/aif360/sklearn/preprocessing/fairadapt.R`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/preprocessing/fairadapt.py` & `aif360-0.6.1/aif360/sklearn/preprocessing/fairadapt.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/preprocessing/learning_fair_representations.py` & `aif360-0.6.1/aif360/sklearn/preprocessing/learning_fair_representations.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/preprocessing/reweighing.py` & `aif360-0.6.1/aif360/sklearn/preprocessing/reweighing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360/sklearn/utils.py` & `aif360-0.6.1/aif360/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/aif360.egg-info/PKG-INFO` & `aif360-0.6.1/aif360.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aif360
-Version: 0.6.0
+Version: 0.6.1
 Summary: IBM AI Fairness 360
 Home-page: https://github.com/Trusted-AI/AIF360
 Author: aif360 developers
 Author-email: aif360@us.ibm.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -48,14 +48,18 @@
 Requires-Dist: tqdm; extra == "notebooks"
 Requires-Dist: igraph[plotting]; extra == "notebooks"
 Requires-Dist: lightgbm; extra == "notebooks"
 Requires-Dist: seaborn; extra == "notebooks"
 Requires-Dist: ipympl; extra == "notebooks"
 Provides-Extra: optimaltransport
 Requires-Dist: pot; extra == "optimaltransport"
+Provides-Extra: facts
+Requires-Dist: mlxtend; extra == "facts"
+Requires-Dist: colorama; extra == "facts"
+Requires-Dist: tqdm; extra == "facts"
 Provides-Extra: tests
 Requires-Dist: cvxpy>=1.0; extra == "tests"
 Requires-Dist: tensorflow>=1.13.1; extra == "tests"
 Requires-Dist: BlackBoxAuditing; extra == "tests"
 Requires-Dist: torch; extra == "tests"
 Requires-Dist: lime; extra == "tests"
 Requires-Dist: adversarial-robustness-toolbox>=1.0.0; extra == "tests"
@@ -66,44 +70,49 @@
 Requires-Dist: jupyter; extra == "tests"
 Requires-Dist: tqdm; extra == "tests"
 Requires-Dist: igraph[plotting]; extra == "tests"
 Requires-Dist: lightgbm; extra == "tests"
 Requires-Dist: seaborn; extra == "tests"
 Requires-Dist: ipympl; extra == "tests"
 Requires-Dist: pot; extra == "tests"
+Requires-Dist: mlxtend; extra == "tests"
+Requires-Dist: colorama; extra == "tests"
+Requires-Dist: tqdm; extra == "tests"
 Requires-Dist: pytest>=3.5; extra == "tests"
 Requires-Dist: pytest-cov>=2.8.1; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: jinja2>3.1.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: fairlearn~=0.7; extra == "docs"
 Provides-Extra: all
-Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: fairlearn~=0.7; extra == "all"
-Requires-Dist: jupyter; extra == "all"
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: lightgbm; extra == "all"
-Requires-Dist: pot; extra == "all"
-Requires-Dist: pytest>=3.5; extra == "all"
-Requires-Dist: rpy2; extra == "all"
-Requires-Dist: jinja2>3.1.0; extra == "all"
 Requires-Dist: tqdm; extra == "all"
+Requires-Dist: adversarial-robustness-toolbox>=1.0.0; extra == "all"
+Requires-Dist: mlxtend; extra == "all"
+Requires-Dist: pytest>=3.5; extra == "all"
+Requires-Dist: igraph[plotting]; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: inFairness>=0.2.2; extra == "all"
 Requires-Dist: pytest-cov>=2.8.1; extra == "all"
 Requires-Dist: skorch; extra == "all"
 Requires-Dist: BlackBoxAuditing; extra == "all"
+Requires-Dist: fairlearn~=0.7; extra == "all"
+Requires-Dist: lightgbm; extra == "all"
+Requires-Dist: cvxpy>=1.0; extra == "all"
+Requires-Dist: rpy2; extra == "all"
+Requires-Dist: sphinx; extra == "all"
+Requires-Dist: pot; extra == "all"
+Requires-Dist: colorama; extra == "all"
+Requires-Dist: jinja2>3.1.0; extra == "all"
+Requires-Dist: jupyter; extra == "all"
 Requires-Dist: tensorflow>=1.13.1; extra == "all"
+Requires-Dist: sphinx_rtd_theme; extra == "all"
 Requires-Dist: lime; extra == "all"
-Requires-Dist: torch; extra == "all"
-Requires-Dist: igraph[plotting]; extra == "all"
-Requires-Dist: inFairness>=0.2.2; extra == "all"
 Requires-Dist: ipympl; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: adversarial-robustness-toolbox>=1.0.0; extra == "all"
-Requires-Dist: cvxpy>=1.0; extra == "all"
+Requires-Dist: torch; extra == "all"
 
 The AI Fairness 360 toolkit is an open-source library to help detect and mitigate bias in machine
 learning models. The AI Fairness 360 Python package includes a comprehensive set of metrics for datasets and models to
 test for biases, explanations for these metrics, and algorithms to mitigate bias in datasets and models.
 
 We have developed the package with extensibility in mind. This library is still in development. We encourage the
 contribution of your datasets, metrics, explainers, and debiasing algorithms.
```

### Comparing `aif360-0.6.0/aif360.egg-info/SOURCES.txt` & `aif360-0.6.1/aif360.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,25 @@
 aif360/sklearn/datasets/compas_dataset.py
 aif360/sklearn/datasets/lawschool_dataset.py
 aif360/sklearn/datasets/meps_datasets.py
 aif360/sklearn/datasets/openml_datasets.py
 aif360/sklearn/datasets/utils.py
 aif360/sklearn/detectors/__init__.py
 aif360/sklearn/detectors/detectors.py
+aif360/sklearn/detectors/facts/__init__.py
+aif360/sklearn/detectors/facts/clean.py
+aif360/sklearn/detectors/facts/formatting.py
+aif360/sklearn/detectors/facts/frequent_itemsets.py
+aif360/sklearn/detectors/facts/metrics.py
+aif360/sklearn/detectors/facts/misc.py
+aif360/sklearn/detectors/facts/optimization.py
+aif360/sklearn/detectors/facts/parameters.py
+aif360/sklearn/detectors/facts/predicate.py
+aif360/sklearn/detectors/facts/rule_filters.py
+aif360/sklearn/detectors/facts/utils.py
 aif360/sklearn/inprocessing/__init__.py
 aif360/sklearn/inprocessing/adversarial_debiasing.py
 aif360/sklearn/inprocessing/exponentiated_gradient_reduction.py
 aif360/sklearn/inprocessing/grid_search_reduction.py
 aif360/sklearn/inprocessing/infairness.py
 aif360/sklearn/metrics/__init__.py
 aif360/sklearn/metrics/metrics.py
@@ -147,14 +158,15 @@
 docs/source/modules/metrics.rst
 docs/source/modules/sklearn.rst
 docs/source/static/style.css
 docs/source/templates/base.rst
 docs/source/templates/class.rst
 examples/README.md
 examples/common_utils.py
+examples/demo_FACTS.ipynb
 examples/demo_adversarial_debiasing.ipynb
 examples/demo_calibrated_eqodds_postprocessing.ipynb
 examples/demo_deterministic_reranking.ipynb
 examples/demo_disparate_impact_remover.ipynb
 examples/demo_exponentiated_gradient_reduction.ipynb
 examples/demo_gerryfair.ipynb
 examples/demo_json_explainers.ipynb
@@ -218,8 +230,19 @@
 tests/sklearn/test_demo_grid_search_red_sklearn.py
 tests/sklearn/test_demo_mdss_classifier_metric_sklearn.py
 tests/sklearn/test_fairadapt.py
 tests/sklearn/test_infairness.py
 tests/sklearn/test_learning_fair_representations.py
 tests/sklearn/test_metrics.py
 tests/sklearn/test_reject_option_classification.py
-tests/sklearn/test_reweighing.py
+tests/sklearn/test_reweighing.py
+tests/sklearn/facts/__init__.py
+tests/sklearn/facts/test_clean.py
+tests/sklearn/facts/test_formatting.py
+tests/sklearn/facts/test_frequent_itemsets.py
+tests/sklearn/facts/test_metrics.py
+tests/sklearn/facts/test_misc.py
+tests/sklearn/facts/test_optimization.py
+tests/sklearn/facts/test_parameters.py
+tests/sklearn/facts/test_predicate.py
+tests/sklearn/facts/test_rule_filters.py
+tests/sklearn/facts/test_utils.py
```

### Comparing `aif360-0.6.0/aif360.egg-info/requires.txt` & `aif360-0.6.1/aif360.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 [AdversarialDebiasing]
 tensorflow>=1.13.1
 
 [DisparateImpactRemover]
 BlackBoxAuditing
 
+[FACTS]
+mlxtend
+colorama
+tqdm
+
 [FairAdapt]
 rpy2
 
 [LFR]
 torch
 
 [LIME]
@@ -28,36 +33,38 @@
 [OptimalTransport]
 pot
 
 [Reductions]
 fairlearn~=0.7
 
 [all]
-sphinx_rtd_theme
-fairlearn~=0.7
-jupyter
-sphinx
-lightgbm
-pot
-pytest>=3.5
-rpy2
-jinja2>3.1.0
 tqdm
+adversarial-robustness-toolbox>=1.0.0
+mlxtend
+pytest>=3.5
+igraph[plotting]
+seaborn
+inFairness>=0.2.2
 pytest-cov>=2.8.1
 skorch
 BlackBoxAuditing
+fairlearn~=0.7
+lightgbm
+cvxpy>=1.0
+rpy2
+sphinx
+pot
+colorama
+jinja2>3.1.0
+jupyter
 tensorflow>=1.13.1
+sphinx_rtd_theme
 lime
-torch
-igraph[plotting]
-inFairness>=0.2.2
 ipympl
-seaborn
-adversarial-robustness-toolbox>=1.0.0
-cvxpy>=1.0
+torch
 
 [docs]
 sphinx
 jinja2>3.1.0
 sphinx_rtd_theme
 fairlearn~=0.7
 
@@ -87,9 +94,11 @@
 jupyter
 tqdm
 igraph[plotting]
 lightgbm
 seaborn
 ipympl
 pot
+mlxtend
+colorama
 pytest>=3.5
 pytest-cov>=2.8.1
```

### Comparing `aif360-0.6.0/docs/Makefile` & `aif360-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/make.bat` & `aif360-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/Getting Started.rst` & `aif360-0.6.1/docs/source/Getting Started.rst`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/conf.py` & `aif360-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/index.rst` & `aif360-0.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/modules/algorithms.rst` & `aif360-0.6.1/docs/source/modules/algorithms.rst`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/modules/datasets.rst` & `aif360-0.6.1/docs/source/modules/datasets.rst`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/modules/metrics.rst` & `aif360-0.6.1/docs/source/modules/metrics.rst`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/docs/source/modules/sklearn.rst` & `aif360-0.6.1/docs/source/modules/sklearn.rst`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,22 @@
 ---------
 .. currentmodule:: aif360.sklearn
 
 .. autosummary::
    :toctree: generated/
    :template: base.rst
 
-   detectors.bias_scan
+   detectors.MDSS_bias_scan
+   detectors.FACTS_bias_scan
+
+.. autosummary::
+   :toctree: generated/
+   :template: class.rst
+
+   detectors.FACTS
 
 :mod:`aif360.sklearn.preprocessing`: Pre-processing algorithms
 ==============================================================
 
 .. automodule:: aif360.sklearn.preprocessing
     :no-members:
     :no-inherited-members:
```

### Comparing `aif360-0.6.0/docs/source/templates/class.rst` & `aif360-0.6.1/docs/source/templates/class.rst`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/README.md` & `aif360-0.6.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/common_utils.py` & `aif360-0.6.1/examples/common_utils.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_adversarial_debiasing.ipynb` & `aif360-0.6.1/examples/demo_adversarial_debiasing.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_calibrated_eqodds_postprocessing.ipynb` & `aif360-0.6.1/examples/demo_calibrated_eqodds_postprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_deterministic_reranking.ipynb` & `aif360-0.6.1/examples/demo_deterministic_reranking.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_disparate_impact_remover.ipynb` & `aif360-0.6.1/examples/demo_disparate_impact_remover.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_exponentiated_gradient_reduction.ipynb` & `aif360-0.6.1/examples/demo_exponentiated_gradient_reduction.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_gerryfair.ipynb` & `aif360-0.6.1/examples/demo_gerryfair.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_json_explainers.ipynb` & `aif360-0.6.1/examples/demo_json_explainers.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_lfr.ipynb` & `aif360-0.6.1/examples/demo_lfr.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_lime.ipynb` & `aif360-0.6.1/examples/demo_lime.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_mdss_classifier_metric.ipynb` & `aif360-0.6.1/examples/demo_mdss_classifier_metric.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_mdss_detector.ipynb` & `aif360-0.6.1/examples/demo_mdss_detector.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_meta_classifier.ipynb` & `aif360-0.6.1/examples/demo_meta_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_optim_data_preproc.ipynb` & `aif360-0.6.1/examples/demo_optim_data_preproc.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_optim_preproc_adult.ipynb` & `aif360-0.6.1/examples/demo_optim_preproc_adult.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_ot_metric.ipynb` & `aif360-0.6.1/examples/demo_ot_metric.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_reject_option_classification.ipynb` & `aif360-0.6.1/examples/demo_reject_option_classification.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_reweighing_preproc.ipynb` & `aif360-0.6.1/examples/demo_reweighing_preproc.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/demo_short_gerryfair_test.ipynb` & `aif360-0.6.1/examples/demo_short_gerryfair_test.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/images/Complex_NoProc_V3.jpg` & `aif360-0.6.1/examples/images/Complex_NoProc_V3.jpg`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_exponentiated_gradient_reduction_sklearn.ipynb` & `aif360-0.6.1/examples/sklearn/demo_exponentiated_gradient_reduction_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_fairadapt_sklearn.ipynb` & `aif360-0.6.1/examples/sklearn/demo_fairadapt_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_grid_search_reduction_classification_sklearn.ipynb` & `aif360-0.6.1/examples/sklearn/demo_grid_search_reduction_classification_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_grid_search_reduction_regression_sklearn.ipynb` & `aif360-0.6.1/examples/sklearn/demo_grid_search_reduction_regression_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_learning_fair_representations.ipynb` & `aif360-0.6.1/examples/sklearn/demo_learning_fair_representations.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_mdss_bias_scan.ipynb` & `aif360-0.6.1/examples/sklearn/demo_mdss_bias_scan.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_mdss_classifier_metric_sklearn.ipynb` & `aif360-0.6.1/examples/sklearn/demo_mdss_classifier_metric_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_new_features.ipynb` & `aif360-0.6.1/examples/sklearn/demo_new_features.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_reject_option_classification.ipynb` & `aif360-0.6.1/examples/sklearn/demo_reject_option_classification.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/demo_sensei_infairness.ipynb` & `aif360-0.6.1/examples/sklearn/demo_sensei_infairness.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/sklearn/monthly_bee_datasets_metrics.ipynb` & `aif360-0.6.1/examples/sklearn/monthly_bee_datasets_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/tutorial_bias_advertising.ipynb` & `aif360-0.6.1/examples/tutorial_bias_advertising.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/tutorial_credit_scoring.ipynb` & `aif360-0.6.1/examples/tutorial_credit_scoring.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/examples/tutorial_medical_expenditure.ipynb` & `aif360-0.6.1/examples/tutorial_medical_expenditure.ipynb`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/setup.py` & `aif360-0.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = """The AI Fairness 360 toolkit is an open-source library to help detect and mitigate bias in machine
 learning models. The AI Fairness 360 Python package includes a comprehensive set of metrics for datasets and models to
 test for biases, explanations for these metrics, and algorithms to mitigate bias in datasets and models.
 
 We have developed the package with extensibility in mind. This library is still in development. We encourage the
 contribution of your datasets, metrics, explainers, and debiasing algorithms."""
-version = '0.6.0'
+version = '0.6.1'
 
 with open("aif360/version.py", 'w') as f:
     f.write('# generated by setup.py\nversion = "{}"\n'.format(version))
 
 extras = {
     'OptimPreproc': ['cvxpy>=1.0'],
     'AdversarialDebiasing': ['tensorflow>=1.13.1'],
@@ -20,14 +20,15 @@
     'LIME': ['lime'],
     'ART': ['adversarial-robustness-toolbox>=1.0.0'],
     'Reductions': ['fairlearn~=0.7'],
     'FairAdapt': ['rpy2'],
     'inFairness': ['skorch', 'inFairness>=0.2.2'],
     'notebooks': ['jupyter', 'tqdm', 'igraph[plotting]', 'lightgbm', 'seaborn', 'ipympl'],
     'OptimalTransport': ['pot'],
+    'FACTS': ['mlxtend', 'colorama', 'tqdm'],
 }
 extras['tests'] = list(chain(*extras.values(), ['pytest>=3.5', 'pytest-cov>=2.8.1']))
 extras['docs'] = ['sphinx', 'jinja2>3.1.0', 'sphinx_rtd_theme'] + extras['Reductions']
 extras['all'] = list(set(chain(*extras.values())))
 
 setup(name='aif360',
       version=version,
```

### Comparing `aif360-0.6.0/tests/notebook_runner.py` & `aif360-0.6.1/tests/notebook_runner.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/conftest.py` & `aif360-0.6.1/tests/sklearn/conftest.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_adversarial_debiasing.py` & `aif360-0.6.1/tests/sklearn/test_adversarial_debiasing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_calibrated_equalized_odds.py` & `aif360-0.6.1/tests/sklearn/test_calibrated_equalized_odds.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_datasets.py` & `aif360-0.6.1/tests/sklearn/test_datasets.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_demo_grid_search_red_sklearn.py` & `aif360-0.6.1/tests/sklearn/test_demo_grid_search_red_sklearn.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_fairadapt.py` & `aif360-0.6.1/tests/sklearn/test_fairadapt.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_infairness.py` & `aif360-0.6.1/tests/sklearn/test_infairness.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_learning_fair_representations.py` & `aif360-0.6.1/tests/sklearn/test_learning_fair_representations.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_metrics.py` & `aif360-0.6.1/tests/sklearn/test_metrics.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_reject_option_classification.py` & `aif360-0.6.1/tests/sklearn/test_reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/sklearn/test_reweighing.py` & `aif360-0.6.1/tests/sklearn/test_reweighing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_classification_metric.py` & `aif360-0.6.1/tests/test_classification_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_demo_adversarial_debiasing.py` & `aif360-0.6.1/tests/test_demo_adversarial_debiasing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_demo_calibrated_eqodds_postprocessing.py` & `aif360-0.6.1/tests/test_demo_calibrated_eqodds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_demo_optim_data_preproc.py` & `aif360-0.6.1/tests/test_demo_optim_data_preproc.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_demo_reject_option_classification.py` & `aif360-0.6.1/tests/test_demo_reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_demo_reweighing_preproc.py` & `aif360-0.6.1/tests/test_demo_reweighing_preproc.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_deterministic_reranking.py` & `aif360-0.6.1/tests/test_deterministic_reranking.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_differential_fairness.py` & `aif360-0.6.1/tests/test_differential_fairness.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_disparate_impact_remover.py` & `aif360-0.6.1/tests/test_disparate_impact_remover.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_eq_odds_postprocessing.py` & `aif360-0.6.1/tests/test_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_lfr.py` & `aif360-0.6.1/tests/test_lfr.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_meta_classifier.py` & `aif360-0.6.1/tests/test_meta_classifier.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_ot_metric.py` & `aif360-0.6.1/tests/test_ot_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_regression_metric.py` & `aif360-0.6.1/tests/test_regression_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_reweighing.py` & `aif360-0.6.1/tests/test_reweighing.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_sample_distortion_metric.py` & `aif360-0.6.1/tests/test_sample_distortion_metric.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_standard_datasets.py` & `aif360-0.6.1/tests/test_standard_datasets.py`

 * *Files identical despite different names*

### Comparing `aif360-0.6.0/tests/test_structured_dataset.py` & `aif360-0.6.1/tests/test_structured_dataset.py`

 * *Files identical despite different names*

