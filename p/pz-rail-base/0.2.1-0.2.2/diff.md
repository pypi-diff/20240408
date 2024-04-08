# Comparing `tmp/pz-rail-base-0.2.1.tar.gz` & `tmp/pz-rail-base-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.2.1.tar", last modified: Wed Apr  3 18:11:15 2024, max compression
+gzip compressed data, was "pz-rail-base-0.2.2.tar", last modified: Mon Apr  8 16:32:47 2024, max compression
```

## Comparing `pz-rail-base-0.2.1.tar` & `pz-rail-base-0.2.2.tar`

### file list

```diff
@@ -1,152 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.542290 pz-rail-base-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/point_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/util_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/equal_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/uniform_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/stats_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.542290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.542290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.570290 pz-rail-base-0.2.1/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.570290 pz-rail-base-0.2.1/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/cli/hello_world.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/cli/single_number.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_point_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/creation/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/creation/test_degraders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/estimation/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.057174 pz-rail-base-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-08 16:32:47.057174 pz-rail-base-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:32:47.057174 pz-rail-base-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.021174 pz-rail-base-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-08 16:32:47.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25183 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/point_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/util_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/creation/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/dist_to_dist_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/dist_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/point_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/single_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/stats_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.021174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.037174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.037174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.037174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.045174 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/cli/hello_world.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/cli/single_number.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_point_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/creation/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.github/pull_request_template.md` & `pz-rail-base-0.2.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.github/workflows/linting.yml` & `pz-rail-base-0.2.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.2.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.github/workflows/smoke-test.yml` & `pz-rail-base-0.2.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.2.2/.github/workflows/testing-and-coverage.yml`

 * *Files 12% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
-        python -m pytest tests --cov=core --cov-report=xml
+        python -m pytest tests --cov=rail --cov-report=xml
     - name: Upload coverage report to codecov
       uses: codecov/codecov-action@v3
```

### Comparing `pz-rail-base-0.2.1/.gitignore` & `pz-rail-base-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/.pre-commit-config.yaml` & `pz-rail-base-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/LICENSE` & `pz-rail-base-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/PKG-INFO` & `pz-rail-base-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.1
+Version: 0.2.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.1/README.md` & `pz-rail-base-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/pyproject.toml` & `pz-rail-base-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ]
 
 [tool.pylint]
 disable = [
     "abstract-method",
     "invalid-name",
     "too-many-statements",
+    "too-many-arguments",
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "too-few-public-methods",
     "duplicate-code",
     "use-dict-literal",
     "broad-exception-caught",
```

### Comparing `pz-rail-base-0.2.1/src/pz_rail_base.egg-info/PKG-INFO` & `pz-rail-base-0.2.2/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.1
+Version: 0.2.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.1/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.2.2/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,19 @@
 src/rail/estimation/algos/equal_count.py
 src/rail/estimation/algos/naive_stack.py
 src/rail/estimation/algos/point_est_hist.py
 src/rail/estimation/algos/random_gauss.py
 src/rail/estimation/algos/train_z.py
 src/rail/estimation/algos/uniform_binning.py
 src/rail/estimation/algos/var_inf.py
+src/rail/evaluation/dist_to_dist_evaluator.py
+src/rail/evaluation/dist_to_point_evaluator.py
 src/rail/evaluation/evaluator.py
+src/rail/evaluation/point_to_point_evaluator.py
+src/rail/evaluation/single_evaluator.py
 src/rail/evaluation/stats_groups.py
 src/rail/evaluation/metrics/base.py
 src/rail/evaluation/metrics/cdeloss.py
 src/rail/evaluation/metrics/pointestimates.py
 src/rail/examples_data/.gitignore
 src/rail/examples_data/creation_data/configs/flowModeler.yaml
 src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
```

### Comparing `pz-rail-base-0.2.1/src/rail/cli/commands.py` & `pz-rail-base-0.2.2/src/rail/cli/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,58 +7,58 @@
 @click.group()
 @click.version_option(__version__)
 def cli() -> None:
     """RAIL utility scripts"""
 
 
 @cli.command()
-@options.outdir(default='docs')
+@options.outdir(default="docs")
 @options.clear_output()
 @options.dry_run()
 @options.inputs()
 @options.skip()
-def render_nb(outdir, clear_output, dry_run, inputs, skip, **kwargs):
+def render_nb(outdir, clear_output, dry_run, inputs, skip, **_kwargs):
     """Render jupyter notebooks"""
     return scripts.render_nb(outdir, clear_output, dry_run, inputs, skip)
 
 
 @cli.command()
-@options.outdir(default='..')
+@options.outdir(default="..")
 @options.git_mode()
 @options.dry_run()
 @options.package_file()
-def clone_source(outdir, git_mode, dry_run, package_file, **kwargs):
+def clone_source(outdir, git_mode, dry_run, package_file, **_kwargs):
     """Install packages from source"""
     scripts.clone_source(outdir, git_mode, dry_run, package_file)
     return 0
-   
-    
+
+
 @cli.command()
-@options.outdir(default='..')
+@options.outdir(default="..")
 @options.dry_run()
 @options.package_file()
-def update_source(outdir, dry_run, package_file, **kwargs):
+def update_source(outdir, dry_run, package_file, **_kwargs):
     """Update packages from source"""
     scripts.update_source(outdir, dry_run, package_file)
     return 0
-    
-    
+
+
 @cli.command()
-@options.outdir(default='..')
+@options.outdir(default="..")
 @options.dry_run()
 @options.from_source()
 @options.package_file()
-def install(outdir, dry_run, from_source, package_file, **kwargs):
+def install(outdir, dry_run, from_source, package_file, **_kwargs):
     """Install rail packages one by one, to be fault tolerant"""
     scripts.install(outdir, from_source, dry_run, package_file)
     return 0
-    
+
 
 @cli.command()
-@options.outdir(default='..')
+@options.outdir(default="..")
 @options.print_all()
 @options.print_packages()
 @options.print_namespaces()
 @options.print_modules()
 @options.print_tree()
 @options.print_stages()
 def info(**kwargs):
```

### Comparing `pz-rail-base-0.2.1/src/rail/cli/options.py` & `pz-rail-base-0.2.2/src/rail/cli/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
-from functools import partial, wraps
-from typing import Any, Callable, Type, TypeVar, cast
+from functools import partial
+from typing import Any, Type, TypeVar
 
 import click
 
 __all__ = [
     "clear_output",
     "bpz_demo_data",
     "dry_run",
@@ -16,57 +16,62 @@
     "print_namespaces",
     "print_modules",
     "print_tree",
     "print_stages",
     "package_file",
     "skip",
     "inputs",
-    "verbose_download"
+    "verbose_download",
 ]
 
 
 class GitMode(enum.Enum):
     """Choose git clone mode"""
+
     ssh = 0
     https = 1
     cli = 2
 
 
 EnumType_co = TypeVar("EnumType_co", bound=Type[enum.Enum], covariant=True)
 
 
 class EnumChoice(click.Choice):
     """A version of click.Choice specialized for enum types"""
 
-    def __init__(self, enum: EnumType_co, case_sensitive: bool = True) -> None:
-        self._enum = enum
-        super().__init__(list(enum.__members__.keys()), case_sensitive=case_sensitive)
+    def __init__(self, the_enum: EnumType_co, case_sensitive: bool = True) -> None:
+        self._enum = the_enum
+        super().__init__(list(the_enum.__members__.keys()), case_sensitive=case_sensitive)
 
-    def convert(self, value: Any, param, ctx) -> EnumType_co:
+    def convert(self, value: Any, param, ctx) -> EnumType_co:  # pragma: no cover
         converted_str = super().convert(value, param, ctx)
         return self._enum.__members__[converted_str]
 
 
 class PartialOption:
     """Wraps click.option with partial arguments for convenient reuse"""
 
     def __init__(self, *param_decls: Any, **kwargs: Any) -> None:
-        self._partial = partial(click.option, *param_decls, cls=partial(click.Option), **kwargs)
+        self._partial = partial(
+            click.option, *param_decls, cls=partial(click.Option), **kwargs
+        )
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:  # pragma: no cover
         return self._partial(*args, **kwargs)
 
 
 class PartialArgument:
     """Wraps click.argument with partial arguments for convenient reuse"""
 
     def __init__(self, *param_decls: Any, **kwargs: Any) -> None:
-        self._partial = partial(click.argument, *param_decls, cls=partial(click.Argument), **kwargs)
+        self._partial = partial(
+            click.argument, *param_decls, cls=partial(click.Argument), **kwargs
+        )
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:  # pragma: no cover
         return self._partial(*args, **kwargs)
 
 
 clear_output = PartialOption(
     "--clear-output",
     help="Clear Notebook output",
     is_flag=True,
@@ -90,15 +95,15 @@
     default=None,
     help="Output directory.",
 )
 
 git_mode = PartialOption(
     "--git-mode",
     type=EnumChoice(GitMode),
-    default='ssh',
+    default="ssh",
     help="Git Clone mode",
 )
 
 print_all = PartialOption(
     "--print-all",
     help="Print all RAIL information",
     is_flag=True,
@@ -144,24 +149,19 @@
 skip = PartialOption(
     "--skip",
     type=click.Path(),
     multiple=True,
     help="Skip files",
 )
 
-inputs = PartialArgument(
-    "inputs",
-    nargs=-1
-)
+inputs = PartialArgument("inputs", nargs=-1)
 
 verbose_download = PartialOption(
-    "-v",
-    "--verbose",
-    help="Verbose output when downloading",
-    is_flag=True
+    "-v", "--verbose", help="Verbose output when downloading", is_flag=True
 )
 
 bpz_demo_data = PartialOption(
     "--bpz-demo-data",
-    help="Download data that is explicitly only for use in the bpz demo and nowhere else (it is dummy data that will not make sense)",
-    is_flag=True
+    help="Download data that is explicitly only for use in the bpz demo and nowhere else"
+    "(it is dummy data that will not make sense)",
+    is_flag=True,
 )
```

### Comparing `pz-rail-base-0.2.1/src/rail/cli/scripts.py` & `pz-rail-base-0.2.2/src/rail/cli/scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-import sys
 import os
-import glob
 import yaml
 
 import rail.stages
 from rail.core import RailEnv
 from rail.cli.options import GitMode
 from rail.core.utils import RAILDIR
 
 
-def render_nb(outdir, clear_output, dry_run, inputs, skip, **kwargs):
-
+def render_nb(outdir, clear_output, dry_run, inputs, skip, **_kwargs):
     command = "jupyter nbconvert"
     options = "--to html"
 
     status = {}
 
     for nb_file in inputs:
         if nb_file in skip:
             continue
-        subdir = os.path.dirname(nb_file).split('/')[-1]
+        subdir = os.path.dirname(nb_file).split("/")[-1]
         basename = os.path.splitext(os.path.basename(nb_file))[0]
-        outfile = os.path.join('..', '..', outdir, f"{subdir}/{basename}.html")
-        relpath = os.path.join(outdir, f'{subdir}')
+        outfile = os.path.join("..", "..", outdir, f"{subdir}/{basename}.html")
+        relpath = os.path.join(outdir, f"{subdir}")
 
         try:
             print(relpath)
             os.makedirs(relpath)
         except FileExistsError:
             pass
 
@@ -41,108 +38,103 @@
         else:
             render = os.system(comline)
         status[nb_file] = render
 
     failed_notebooks = []
     for key, val in status.items():
         print(f"{key} {val}")
-        if val != 0:
+        if val != 0:  # pragma: no cover
             failed_notebooks.append(key)
 
-    if failed_notebooks:
+    if failed_notebooks:  # pragma: no cover
         raise ValueError(f"The following notebooks failed {str(failed_notebooks)}")
-        
 
-def clone_source(outdir, git_mode, dry_run, package_file):
 
-    with open(package_file) as pfile:
+def clone_source(outdir, git_mode, dry_run, package_file):  # pragma: no cover
+    with open(package_file, encoding="utf-8") as pfile:
         package_dict = yaml.safe_load(pfile)
 
-    for key, val in package_dict.items():
+    for key, _val in package_dict.items():
         if os.path.exists(f"{outdir}/{key}"):
             print(f"Skipping existing {outdir}/{key}")
             continue
-            
+
         if git_mode == GitMode.ssh:
             com_line = f"git clone https://github.com/LSSTDESC/{key}.git {outdir}/{key}"
         elif git_mode == GitMode.https:
             com_line = f"git clone git@github.com:LSSTDESC/{key}.git {outdir}/{key}"
         elif git_mode == GitMode.cli:
             com_line = f"gh repo clone LSSTDESC/{key} {outdir}/{key}"
 
         if dry_run:
             print(com_line)
         else:
             os.system(com_line)
 
-            
-def update_source(outdir, dry_run, package_file):
 
-    with open(package_file) as pfile:
+def update_source(outdir, dry_run, package_file):
+    with open(package_file, encoding="utf-8") as pfile:
         package_dict = yaml.safe_load(pfile)
 
-    currentpath = os.path.abspath('.')    
-    for key, val in package_dict.items():
+    currentpath = os.path.abspath(".")
+    for key, _val in package_dict.items():
         abspath = os.path.abspath(f"{outdir}/{key}")
 
-        if os.path.exists(f"{outdir}/{key}") is not True:
+        if os.path.exists(f"{outdir}/{key}") is not True:  # pragma: no cover
             print(f"Package {outdir}/{key} does not exist!")
-            continue            
-                
+            continue
+
         com_line = f"cd {abspath} && git pull && cd {currentpath}"
 
         if dry_run:
             print(com_line)
-        else:
+        else:  # pragma: no cover
             os.system(com_line)
-            
 
-def install(outdir, from_source, dry_run, package_file):
 
-    with open(package_file) as pfile:
+def install(outdir, from_source, dry_run, package_file):
+    with open(package_file, encoding="utf-8") as pfile:
         package_dict = yaml.safe_load(pfile)
 
     for key, val in package_dict.items():
-
         if not from_source:
             com_line = f"pip install {val}"
-        else:            
-            if not os.path.exists(f"{outdir}/{key}"):
+        else:
+            if not os.path.exists(f"{outdir}/{key}"):  # pragma: no cover
                 print(f"Skipping missing {outdir}/{key}")
                 continue
             com_line = f"pip install -e {outdir}/{key}"
-        
+
         if dry_run:
             print(com_line)
-        else:
+        else:  # pragma: no cover
             os.system(com_line)
 
 
 def info(**kwargs):
-    
     rail.stages.import_and_attach_all()
 
-    print_all = kwargs.get('print_all', False)
-    if kwargs.get('print_packages') or print_all:
+    print_all = kwargs.get("print_all", False)
+    if kwargs.get("print_packages") or print_all:
         print("======= Printing RAIL packages ==============")
         RailEnv.print_rail_packages()
         print("\n\n")
-    if kwargs.get('print_namespaces') or print_all:
+    if kwargs.get("print_namespaces") or print_all:
         print("======= Printing RAIL namespaces ==============")
         RailEnv.print_rail_namespaces()
         print("\n\n")
-    if kwargs.get('print_modules') or print_all:
+    if kwargs.get("print_modules") or print_all:
         print("======= Printing RAIL modules ==============")
         RailEnv.print_rail_modules()
         print("\n\n")
-    if kwargs.get('print_tree') or print_all:
+    if kwargs.get("print_tree") or print_all:
         print("======= Printing RAIL source tree ==============")
         RailEnv.print_rail_namespace_tree()
         print("\n\n")
-    if kwargs.get('print_stages') or print_all:
+    if kwargs.get("print_stages") or print_all:
         print("======= Printing RAIL stages ==============")
         RailEnv.print_rail_stage_dict()
         print("\n\n")
 
 
 def get_data(verbose, **kwargs):  # pragma: no cover
     standard_data_files = [
@@ -157,22 +149,22 @@
             "remote_path": "https://portal.nersc.gov/cfs/lsst/PZ/nonphysical_dc2_templates.tar",
         },
         {
             "local_path": "rail/examples_data/estimation_data/data/test_dc2_training_9816_broadtypes.hdf5",
             "remote_path": "https://portal.nersc.gov/cfs/lsst/PZ/test_dc2_training_9816_broadtypes.hdf5",
         },
         {
-            "local_path": "rail/examples_data/estimation_data/data/test_dc2_train_customtemp_broadttypes.hdf5",
+            "local_path": "rail/examples_data/estimation_data/data/test_dc2_train_customtemp_broadttypes.hdf5",  # pylint: disable=line-too-long
             "remote_path": "https://portal.nersc.gov/cfs/lsst/PZ/test_dc2_train_customtemp_broadttypes.hdf5",
         }
     ]
 
     data_files = standard_data_files
     if kwargs.get("bpz_demo_data"):
-        # The bpz demo data is quarantined into its own flag, as it contains some 
+        # The bpz demo data is quarantined into its own flag, as it contains some
         # non-physical features that would add systematics if run on any real data.
         # This data should NOT be used for any science with real data!
         data_files = bpz_data_files
         print("Downloading BPZ demo data...")
         print("(Note: you can run get-data without the bpz-demo-data flag to download standard data.)")
 
     for data_file in data_files:
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/algo_utils.py` & `pz-rail-base-0.2.2/src/rail/core/algo_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,82 @@
 """Utility functions to test alogrithms"""
 import os
+import scipy.special
 from rail.core.stage import RailStage
 from rail.core.utils import RAILDIR
 from rail.core.data import TableHandle
-import scipy.special
-sci_ver_str = scipy.__version__.split('.')
 
 
-traindata = os.path.join(RAILDIR, 'rail/examples_data/testdata/training_100gal.hdf5')
-validdata = os.path.join(RAILDIR, 'rail/examples_data/testdata/validation_10gal.hdf5')
+traindata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
+validdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
-def one_algo(key, single_trainer, single_estimator, train_kwargs, estim_kwargs, is_classifier=False):
+def one_algo(
+    key,
+    single_trainer,
+    single_estimator,
+    train_kwargs,
+    estim_kwargs,
+    is_classifier=False,
+):
     """
     A basic test of running an estimator subclass.
     Run inform, write temporary trained model to
     'tempmodelfile.tmp', run photo-z algorithm.
     Then, load tempmodelfile.tmp and re-run, return
     both datasets.
     """
     DS.clear()
-    training_data = DS.read_file('training_data', TableHandle, traindata)
-    validation_data = DS.read_file('validation_data', TableHandle, validdata)
+    training_data = DS.read_file("training_data", TableHandle, traindata)
+    validation_data = DS.read_file("validation_data", TableHandle, validdata)
 
     if single_trainer is not None:
         train_pz = single_trainer.make_stage(**train_kwargs)
         train_pz.inform(training_data)
 
     pz = single_estimator.make_stage(name=key, **estim_kwargs)
-    if is_classifier==False:
+    if not is_classifier:
         estim = pz.estimate(validation_data)
-    elif is_classifier==True: #pragma: no cover
+    elif is_classifier:  # pragma: no cover
         estim = pz.classify(validation_data)
     pz_2 = None
     estim_2 = estim
     pz_3 = None
     estim_3 = estim
 
     copy_estim_kwargs = estim_kwargs.copy()
-    model_file = copy_estim_kwargs.pop('model', 'None')
+    model_file = copy_estim_kwargs.pop("model", "None")
 
-    if model_file != 'None':
-        copy_estim_kwargs['model'] = model_file
+    if model_file != "None":
+        copy_estim_kwargs["model"] = model_file
         pz_2 = single_estimator.make_stage(name=f"{pz.name}_copy", **copy_estim_kwargs)
-        if is_classifier==False:
+        if not is_classifier:
             estim_2 = pz_2.estimate(validation_data)
-        elif is_classifier==True: #pragma: no cover
+        elif is_classifier:  # pragma: no cover
             estim_2 = pz_2.classify(validation_data)
 
-    if single_trainer is not None and 'model' in single_trainer.output_tags():
+    if single_trainer is not None and "model" in single_trainer.output_tags():
         copy3_estim_kwargs = estim_kwargs.copy()
-        copy3_estim_kwargs['model'] = train_pz.get_handle('model')
-        pz_3 = single_estimator.make_stage(name=f"{pz.name}_copy3", **copy3_estim_kwargs)
-        if is_classifier==False:
+        copy3_estim_kwargs["model"] = train_pz.get_handle("model")
+        pz_3 = single_estimator.make_stage(
+            name=f"{pz.name}_copy3", **copy3_estim_kwargs
+        )
+        if not is_classifier:
             estim_3 = pz_3.estimate(validation_data)
-        elif is_classifier==True: #pragma: no cover
+        elif is_classifier:  # pragma: no cover
             estim_3 = pz_3.classify(validation_data)
 
-    os.remove(pz.get_output(pz.get_aliased_tag('output'), final_name=True))
+    os.remove(pz.get_output(pz.get_aliased_tag("output"), final_name=True))
     if pz_2 is not None:
-        os.remove(pz_2.get_output(pz_2.get_aliased_tag('output'), final_name=True))
+        os.remove(pz_2.get_output(pz_2.get_aliased_tag("output"), final_name=True))
 
     if pz_3 is not None:
-        os.remove(pz_3.get_output(pz_3.get_aliased_tag('output'), final_name=True))
-    model_file = estim_kwargs.get('model', 'None')
-    if model_file != 'None':
+        os.remove(pz_3.get_output(pz_3.get_aliased_tag("output"), final_name=True))
+    model_file = estim_kwargs.get("model", "None")
+    if model_file != "None":
         try:
             os.remove(model_file)
-        except FileNotFoundError:  #pragma: no cover
+        except FileNotFoundError:  # pragma: no cover
             pass
     return estim.data, estim_2.data, estim_3.data
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/common_params.py` & `pz-rail-base-0.2.2/src/rail/core/common_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 """ Parameters that are shared between stages """
 
 from ceci.config import StageParameter as Param
 from ceci.config import StageConfig
 
-lsst_bands = 'ugrizy'
-lsst_mag_cols = [f'mag_{band}_lsst' for band in lsst_bands]
-lsst_mag_err_cols = [f'mag_err_{band}_lsst' for band in lsst_bands]
+lsst_bands = "ugrizy"
+lsst_mag_cols = [f"mag_{band}_lsst" for band in lsst_bands]
+lsst_mag_err_cols = [f"mag_err_{band}_lsst" for band in lsst_bands]
 lsst_def_maglims = dict(
     mag_u_lsst=27.79,
     mag_g_lsst=29.04,
     mag_r_lsst=29.06,
     mag_i_lsst=28.62,
     mag_z_lsst=27.98,
-    mag_y_lsst=27.05
+    mag_y_lsst=27.05,
 )
 
 
 SHARED_PARAMS = StageConfig(
-    hdf5_groupname=Param(str, "photometry", msg="name of hdf5 group for data, if None, then set to ''"),
+    hdf5_groupname=Param(
+        str, "photometry", msg="name of hdf5 group for data, if None, then set to ''"
+    ),
     zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
     zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
     nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
     dz=Param(float, 0.01, msg="delta z in grid"),
-    nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
-    bands=Param(list, lsst_mag_cols, msg="Names of columns for magnitgude by filter band"),
-    err_bands=Param(list, lsst_mag_err_cols, msg="Names of columns for magnitgude errors by filter band"),
+    nondetect_val=Param(
+        float, 99.0, msg="value to be replaced with magnitude limit for non detects"
+    ),
+    bands=Param(
+        list, lsst_mag_cols, msg="Names of columns for magnitgude by filter band"
+    ),
+    err_bands=Param(
+        list,
+        lsst_mag_err_cols,
+        msg="Names of columns for magnitgude errors by filter band",
+    ),
     mag_limits=Param(dict, lsst_def_maglims, msg="Limiting magnitdues by filter"),
     ref_band=Param(str, "mag_i_lsst", msg="band to use in addition to colors"),
-    redshift_col=Param(str, 'redshift', msg="name of redshift column"),
-    calculated_point_estimates=Param(dtype=list, default=[],
-                                     msg="List of strings defining which point estimates to automatically calculate using `qp.Ensemble`. Options include, 'mean', 'mode', 'median'.")
+    redshift_col=Param(str, "redshift", msg="name of redshift column"),
+    calculated_point_estimates=Param(
+        dtype=list,
+        default=[],
+        msg="List of strings defining which point estimates to automatically calculate using `qp.Ensemble`."
+        "Options include, 'mean', 'mode', 'median'.",
+    ),
 )
 
 
 def copy_param(param_name):
     """Return a copy of one of the shared parameters"""
     return SHARED_PARAMS.get(param_name).copy()
 
 
 def set_param_default(param_name, default_value):
     """Change the default value of one of the shared parameters"""
     try:
         SHARED_PARAMS.get(param_name).set_default(default_value)
     except AttributeError as msg:  # pragma: no cover
-        raise KeyError(f"No shared parameter {param_name} in SHARED_PARAMS")
+        raise KeyError(f"No shared parameter {param_name} in SHARED_PARAMS") from msg
+
 
 def set_param_defaults(**kwargs):  # pragma: no cover
     """Change the default value of several of the shared parameters"""
     for key, val in kwargs.items():
         set_param_default(key, val)
-
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/data.py` & `pz-rail-base-0.2.2/src/rail/core/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 """Rail-specific data management"""
 
 import os
-import tables_io
 import pickle
+import enum
+import tables_io
 import qp
 
 
-
-class DataHandle:
+class DataHandle:  # pylint: disable=too-many-instance-attributes
     """Class to act as a handle for a bit of data.  Associating it with a file and
     providing tools to read & write it to that file
 
     Parameters
     ----------
     tag : str
         The tag under which this data handle can be found in the store
     data : any or None
         The associated data
     path : str or None
         The path to the associated file
     creator : str or None
         The name of the stage that created this data handle
     """
-    suffix = ''
+
+    suffix = ""
 
     # This is to keep track of all the sub-types
     data_handle_type_dict = {}
 
     def __init__(self, tag, data=None, path=None, creator=None):
-        """Constructor """
+        """Constructor"""
         self.tag = tag
         if data is not None:
             self._validate_data(data)
         self.data = data
         self.path = path
         self.creator = creator
         self.fileObj = None
         self.groups = None
         self.partial = False
         self.length = None
-        
+
     def __init_subclass__(cls, **kwargs):
         """Register the subclass with the dict"""
         cls.data_handle_type_dict[cls.__name__] = cls
 
     @classmethod
     def get_sub_class(cls, class_name):
         """Get a particular subclass by name"""
         return cls.data_handle_type_dict[class_name]
 
     @classmethod
     def print_sub_classes(cls):
         """Print the list of all the subclasses"""
         for key, val in cls.data_handle_type_dict.items():
-            print(f"{key}: {val}")    
+            print(f"{key}: {val}")
 
     def open(self, **kwargs):
         """Open and return the associated file
 
         Notes
         -----
         This will simply open the file and return a file-like object to the caller.
@@ -66,128 +67,159 @@
         if self.path is None:
             raise ValueError("DataHandle.open() called but path has not been specified")
         self.fileObj = self._open(os.path.expandvars(self.path), **kwargs)
         return self.fileObj
 
     @classmethod
     def _open(cls, path, **kwargs):
-        raise NotImplementedError("DataHandle._open")  #pragma: no cover
+        raise NotImplementedError("DataHandle._open")  # pragma: no cover
 
-    def close(self, **kwargs):  #pylint: disable=unused-argument
-        """Close """
+    def close(self, **kwargs):  # pylint: disable=unused-argument
+        """Close"""
         self.fileObj = None
 
     def read(self, force=False, **kwargs):
-        """Read and return the data from the associated file """
+        """Read and return the data from the associated file"""
         if self.data is not None and not force:
             return self.data
         self.set_data(self._read(os.path.expandvars(self.path), **kwargs))
         return self.data
 
     def __call__(self, **kwargs):
         """Return the data, re-reading the fill if needed"""
         if self.has_data and not self.partial:
             return self.data
         return self.read(force=True, **kwargs)
 
     @classmethod
     def _read(cls, path, **kwargs):
-        raise NotImplementedError("DataHandle._read")  #pragma: no cover
+        raise NotImplementedError("DataHandle._read")  # pragma: no cover
 
     def write(self, **kwargs):
-        """Write the data to the associated file """
+        """Write the data to the associated file"""
         if self.path is None:
-            raise ValueError("TableHandle.write() called but path has not been specified")
+            raise ValueError(
+                "TableHandle.write() called but path has not been specified"
+            )
         if self.data is None:
-            raise ValueError(f"TableHandle.write() called for path {self.path} with no data")
+            raise ValueError(
+                f"TableHandle.write() called for path {self.path} with no data"
+            )
         outdir = os.path.dirname(os.path.abspath(os.path.expandvars(self.path)))
-        if not os.path.exists(outdir):  #pragma: no cover
+        if not os.path.exists(outdir):  # pragma: no cover
             os.makedirs(outdir, exist_ok=True)
         return self._write(self.data, os.path.expandvars(self.path), **kwargs)
 
     @classmethod
     def _write(cls, data, path, **kwargs):
-        raise NotImplementedError("DataHandle._write")  #pragma: no cover
+        raise NotImplementedError("DataHandle._write")  # pragma: no cover
 
     def initialize_write(self, data_length, **kwargs):
         """Initialize file to be written by chunks"""
-        if self.path is None:  #pragma: no cover
-            raise ValueError("TableHandle.write() called but path has not been specified")
-        self.groups, self.fileObj = self._initialize_write(self.data, os.path.expandvars(self.path), data_length, **kwargs)
+        if self.path is None:  # pragma: no cover
+            raise ValueError(
+                "TableHandle.write() called but path has not been specified"
+            )
+        self.groups, self.fileObj = self._initialize_write(
+            self.data, os.path.expandvars(self.path), data_length, **kwargs
+        )
 
     @classmethod
     def _initialize_write(cls, data, path, data_length, **kwargs):
-        raise NotImplementedError("DataHandle._initialize_write") #pragma: no cover
+        raise NotImplementedError("DataHandle._initialize_write")  # pragma: no cover
 
     def write_chunk(self, start, end, **kwargs):
-        """Write the data to the associated file """
+        """Write the data to the associated file"""
         if self.data is None:
-            raise ValueError(f"TableHandle.write_chunk() called for path {self.path} with no data")
+            raise ValueError(
+                f"TableHandle.write_chunk() called for path {self.path} with no data"
+            )
         if self.fileObj is None:
-            raise ValueError(f"TableHandle.write_chunk() called before open for {self.tag} : {self.path}")
-        return self._write_chunk(self.data, self.fileObj, self.groups, start, end, **kwargs)
-
+            raise ValueError(
+                f"TableHandle.write_chunk() called before open for {self.tag} : {self.path}"
+            )
+        return self._write_chunk(
+            self.data, self.fileObj, self.groups, start, end, **kwargs
+        )
 
     @classmethod
     def _write_chunk(cls, data, fileObj, groups, start, end, **kwargs):
-        raise NotImplementedError("DataHandle._write_chunk")  #pragma: no cover
+        raise NotImplementedError("DataHandle._write_chunk")  # pragma: no cover
 
     def finalize_write(self, **kwargs):
         """Finalize and close file written by chunks"""
-        if self.fileObj is None:  #pragma: no cover
-            raise ValueError(f"TableHandle.finalize_wite() called before open for {self.tag} : {self.path}")
+        if self.fileObj is None:  # pragma: no cover
+            raise ValueError(
+                f"TableHandle.finalize_wite() called before open for {self.tag} : {self.path}"
+            )
         self._finalize_write(self.data, self.fileObj, **kwargs)
 
     @classmethod
     def _finalize_write(cls, data, fileObj, **kwargs):
-        raise NotImplementedError("DataHandle._finalize_write")  #pragma: no cover
+        raise NotImplementedError("DataHandle._finalize_write")  # pragma: no cover
 
     def iterator(self, **kwargs):
         """Iterator over the data"""
-        #if self.data is not None:
-        #    for i in range(1):
-        #        yield i, -1, self.data
+        if self.data is not None and self.partial is False:
+            return self._in_memory_iterator(**kwargs)
         return self._iterator(self.path, **kwargs)
 
     def set_data(self, data, partial=False):
         """Set the data for a chunk, and set the partial flag to true"""
         self._validate_data(data)
         self.data = data
         self.partial = partial
 
     @classmethod
-    def _validate_data(cls, data):
+    def _validate_data(cls, data):  # pylint: disable=unused-argument
         """Make sure that the right type of data is being passed in"""
         return
 
     def size(self, **kwargs):
         """Return the size of the data associated to this handle"""
+        if self.partial:
+            if self.length is not None:  # pragma: no cover
+                return self.length
+            return self._size(self.path, **kwargs)
+        if self.data is not None:
+            return self.data_size(**kwargs)
         return self._size(self.path, **kwargs)
 
-    @classmethod
-    def _size(cls, path, **kwargs):
-        raise NotImplementedError("DataHandle._size")  #pragma: no cover
+    def _size(self, path, **kwargs):
+        raise NotImplementedError("DataHandle._size")  # pragma: no cover
+
+    def data_size(self, **kwargs):
+        """Return the size of the in memorry data"""
+        if self.data is None:  # pragma: no cover
+            return 0
+        return self._data_size(self.data, **kwargs)
+
+    def _data_size(self, data, **kwargs):
+        raise NotImplementedError("DataHandle._data_size")  # pragma: no cover
+
+    def _in_memory_iterator(self, **kwargs):
+        raise NotImplementedError("DataHandle._in_memory_iterator")  # pragma: no cover
 
     @classmethod
     def _iterator(cls, path, **kwargs):
-        raise NotImplementedError("DataHandle._iterator")  #pragma: no cover
+        raise NotImplementedError("DataHandle._iterator")  # pragma: no cover
 
     @property
     def has_data(self):
-        """Return true if the data for this handle are loaded """
+        """Return true if the data for this handle are loaded"""
         return self.data is not None
 
     @property
     def has_path(self):
-        """Return true if the path for the associated file is defined """
+        """Return true if the path for the associated file is defined"""
         return self.path is not None
 
     @property
     def is_written(self):
-        """Return true if the associated file has been written """
+        """Return true if the associated file has been written"""
         if self.path is None:
             return False
         return os.path.exists(os.path.expandvars(self.path))
 
     def __str__(self):
         s = f"{type(self)} "
         if self.has_path:
@@ -199,326 +231,526 @@
         if self.has_data:
             s += "d"
         s += ")"
         return s
 
     @classmethod
     def make_name(cls, tag):
-        """Construct and return file name for a particular data tag """
+        """Construct and return file name for a particular data tag"""
         if cls.suffix:
             return f"{tag}.{cls.suffix}"
-        else:
-            return tag  #pragma: no cover
+        return tag  # pragma: no cover
 
 
 class TableHandle(DataHandle):
-    """DataHandle for single tables of data
-    """
+    """DataHandle for single tables of data"""
+
     suffix = None
 
+    def set_data(self, data, partial=False):
+        """Set the data for a chunk, and set the partial flag to true"""
+        self._validate_data(data)
+        self.data = data
+        self.partial = partial
+
+    @classmethod
+    def _validate_data(cls, data):  # pylint: disable=unused-argument
+        """Make sure that the right type of data is being passed in"""
+        return
+
     @classmethod
     def _open(cls, path, **kwargs):
         """Open and return the associated file
 
         Notes
         -----
         This will simply open the file and return a file-like object to the caller.
         It will not read or cache the data
         """
-        return tables_io.io.io_open(path, **kwargs)  #pylint: disable=no-member
+        return tables_io.io.io_open(path, **kwargs)  # pylint: disable=no-member
 
     @classmethod
     def _read(cls, path, **kwargs):
-        """Read and return the data from the associated file """
+        """Read and return the data from the associated file"""
         return tables_io.read(path, **kwargs)
 
     @classmethod
     def _write(cls, data, path, **kwargs):
-        """Write the data to the associated file """
+        """Write the data to the associated file"""
         return tables_io.write(data, path, **kwargs)
 
-    @classmethod
-    def _size(cls, path, **kwargs):
-        return tables_io.io.getInputDataLengthHdf5(path, **kwargs)
+    def _size(self, path, **kwargs):
+        if path in [None, 'none', 'None']:  # pragma: no cover
+            return 0
+        try:
+            return tables_io.io.getInputDataLengthHdf5(path, **kwargs)
+        except Exception:
+            return 0
+
+    def _data_size(self, data, **kwargs):
+        group_name = kwargs.get('groupname', None)
+        if group_name:
+            try:
+                data = data[group_name]
+            except KeyError:  # pragma: no cover
+                pass
+        max_l = 0
+        for _k, v in data.items():
+            max_l = max(max_l, len(v))
+        return max_l
+
+    def _in_memory_iterator(self, **kwargs):
+        nrows = self.data_size(**kwargs)
+        groupname = kwargs.get('groupname', None)
+        if isinstance(self.data, dict) and groupname:
+            try:
+                table = self.data[groupname]
+            except KeyError:   # pragma: no cover
+                table = self.data
+        else:
+            table = self.data
+        for start, end in tables_io.ioUtils.data_ranges_by_rank(
+                nrows, kwargs.get('chunk_size', 100000), 1, 0
+            ):
+            if isinstance(self.data, dict):
+                yield start, end, tables_io.arrayUtils.sliceDict(table, slice(start, end))
+            else:  # pragma: no cover
+                yield start, end, table[start:end]
 
     @classmethod
     def _iterator(cls, path, **kwargs):
         """Iterate over the data"""
         return tables_io.iteratorNative(path, **kwargs)
 
 
 class Hdf5Handle(TableHandle):  # pragma: no cover
     """DataHandle for a table written to HDF5"""
-    suffix = 'hdf5'
+
+    suffix = "hdf5"
 
     @classmethod
     def _initialize_write(cls, data, path, data_length, **kwargs):
         initial_dict = cls._get_allocation_kwds(data, data_length)
-        comm = kwargs.get('communicator', None)
-        group, fout = tables_io.io.initializeHdf5WriteSingle(path, groupname=None, comm=comm, **initial_dict)
+        comm = kwargs.get("communicator", None)
+        group, fout = tables_io.io.initializeHdf5WriteSingle(
+            path, groupname=None, comm=comm, **initial_dict
+        )
         return group, fout
 
     @classmethod
     def _get_allocation_kwds(cls, data, data_length):
         keywords = {}
         for key, array in data.items():
             shape = list(array.shape)
+            if not shape:
+                continue
             shape[0] = data_length
             keywords[key] = (shape, array.dtype)
         return keywords
 
     @classmethod
     def _write_chunk(cls, data, fileObj, groups, start, end, **kwargs):
         tables_io.io.writeDictToHdf5ChunkSingle(fileObj, data, start, end, **kwargs)
 
     @classmethod
     def _finalize_write(cls, data, fileObj, **kwargs):
         return tables_io.io.finalizeHdf5Write(fileObj, **kwargs)
 
+
 class FitsHandle(TableHandle):
     """DataHandle for a table written to fits"""
-    suffix = 'fits'
+
+    suffix = "fits"
 
 
 class PqHandle(TableHandle):
     """DataHandle for a parquet table"""
-    suffix = 'pq'
+
+    suffix = "pq"
 
 
 class QPHandle(DataHandle):
-    """DataHandle for qp ensembles
-    """
-    suffix = 'hdf5'
+    """DataHandle for qp ensembles"""
+
+    suffix = "hdf5"
 
     @classmethod
     def _open(cls, path, **kwargs):
         """Open and return the associated file
 
         Notes
         -----
         This will simply open the file and return a file-like object to the caller.
         It will not read or cache the data
         """
-        return tables_io.io.io_open(path, **kwargs)  #pylint: disable=no-member
+        return tables_io.io.io_open(path, **kwargs)  # pylint: disable=no-member
 
     @classmethod
     def _read(cls, path, **kwargs):
-        """Read and return the data from the associated file """
+        """Read and return the data from the associated file"""
         return qp.read(path)
 
     @classmethod
     def _write(cls, data, path, **kwargs):
-        """Write the data to the associated file """
+        """Write the data to the associated file"""
         return data.write_to(path)
 
     @classmethod
     def _initialize_write(cls, data, path, data_length, **kwargs):
-        comm = kwargs.get('communicator', None)
+        comm = kwargs.get("communicator", None)
         return data.initializeHdf5Write(path, data_length, comm)
 
     @classmethod
     def _write_chunk(cls, data, fileObj, groups, start, end, **kwargs):
         return data.writeHdf5Chunk(fileObj, start, end)
 
     @classmethod
     def _finalize_write(cls, data, fileObj, **kwargs):
         return data.finalizeHdf5Write(fileObj)
 
     @classmethod
     def _validate_data(cls, data):
         if not isinstance(data, qp.Ensemble):
-            raise TypeError(f"Expected `data` to be a `qp.Ensemble`, but {type(data)} was provided. Perhaps you meant to use `TableHandle`?")
-
-    # @classmethod
-    def _size(cls, path, **kwargs):
-        if path == 'None':
-            return cls.data.npdf
-        return tables_io.io.getInputDataLengthHdf5(path, groupname='data')
+            raise TypeError(
+                f"Expected `data` to be a `qp.Ensemble`, but {type(data)} was provided."
+                "Perhaps you meant to use `TableHandle`?"
+            )
+
+    def _size(self, path, **kwargs):
+        if self.data is not None and not self.partial:  # pragma: no cover
+            return self._data_size(self.data)
+        if path in [None, 'none', "None"]:  # pragma: no cover
+            return 0
+        return tables_io.io.getInputDataLengthHdf5(path, groupname="data")
+
+    def _data_size(self, data, **kwargs):
+        return self.data.npdf
+
+    def _in_memory_iterator(self, **kwargs):
+        nrows = self.data.npdf
+        for start, end in tables_io.ioUtils.data_ranges_by_rank(
+                nrows, kwargs.get('chunk_size', 100000), 1, 0
+            ):
+            yield start, end, self.data[start:end]
 
     @classmethod
     def _iterator(cls, path, **kwargs):
         """Iterate over the data"""
-        kwargs.pop('groupname','None')
+        kwargs.pop("groupname", "None")
         return qp.iterator(path, **kwargs)
 
+
+class QPDictHandle(DataHandle):
+    """DataHandle for dictionaries of qp ensembles"""
+
+    suffix = "hdf5"
+
+    @classmethod
+    def _open(cls, path, **kwargs):
+        """Open and return the associated file
+
+        Notes
+        -----
+        This will simply open the file and return a file-like object to the caller.
+        It will not read or cache the data
+        """
+        return tables_io.io.io_open(path, **kwargs)  # pylint: disable=no-member
+
+    @classmethod
+    def _read(cls, path, **kwargs):
+        """Read and return the dictionary of qp.Ensembles from the associated file"""
+        return qp.read_dict(path)
+
+    @classmethod
+    def _write(cls, data, path, **kwargs):
+        """Write the data (a dictionary of qp.Ensembles) to the associated file"""
+        return qp.write_dict(path, data)
+
+
+class QPOrTableHandle(QPHandle, Hdf5Handle):
+    """DataHandle that should work with either qp.ensembles or tables
+    """
+    suffix = 'hdf5'
+
+    class PdfOrValue(enum.Enum):
+        unknown = -1
+        distribution = 0
+        point_estimate = 1
+        both = 2
+
+        def has_dist(self):
+            return self.value in [0, 2]
+
+        def has_point(self):
+            return self.value in [1, 2]
+
+    def is_qp(self):
+        """ Check if the associated data or file is a QP ensemble"""
+        if self.path in [None, 'None', 'none']:
+            return isinstance(self.data, qp.Ensemble)
+        return qp.is_qp_file(self.path)
+
+    def check_pdf_or_point(self):
+        """Check the associated file to see if it is a QP pdf, point estimate or both"""
+        if self.is_qp():
+            return self.PdfOrValue.both
+        return self.PdfOrValue.point_estimate
+
+    @classmethod
+    def _open(cls, path, **kwargs):
+        """Open and return the associated file
+
+        Notes
+        -----
+        This will simply open the file and return a file-like object to the caller.
+        It will not read or cache the data
+        """
+        return tables_io.io.io_open(path, **kwargs)  # pylint: disable=no-member
+
+    @classmethod
+    def _read(cls, path, **kwargs):
+        """Read and return the data from the associated file """
+        if qp.is_qp_file(path):
+            return qp.read(path, **kwargs)
+        return tables_io.read(path, **kwargs)
+
+    @classmethod
+    def _write(cls, data, path, **kwargs):
+        """Write the data to the associated file """
+        raise RuntimeError("QPOrTableHandle should be used for input, not output")  # pragma: no cover
+
+    @classmethod
+    def _initialize_write(cls, data, path, data_length, **kwargs):
+        raise RuntimeError("QPOrTableHandle should be used for input, not output")  # pragma: no cover
+
+    @classmethod
+    def _write_chunk(cls, data, fileObj, groups, start, end, **kwargs):
+        raise RuntimeError("QPOrTableHandle should be used for input, not output")  # pragma: no cover
+
+    @classmethod
+    def _finalize_write(cls, data, fileObj, **kwargs):
+        raise RuntimeError("QPOrTableHandle should be used for input, not output")  # pragma: no cover
+
+    @classmethod
+    def _validate_data(cls, data):
+        pass
+
+    def _size(self, path, **kwargs):
+        if self.is_qp():
+            return QPHandle._size(self, path, **kwargs)
+        return Hdf5Handle._size(self, path, **kwargs)
+
+    def _data_size(self, data, **kwargs):
+        if self.is_qp():
+            return self.data.npdf
+        return TableHandle._data_size(self, data, **kwargs)
+
+    def _in_memory_iterator(self, **kwargs):
+        if self.is_qp():
+            return QPHandle._in_memory_iterator(self, **kwargs)
+        return Hdf5Handle._in_memory_iterator(self, **kwargs)
+
+    @classmethod
+    def _iterator(cls, path, **kwargs):
+        """Iterate over the data"""
+        if qp.is_qp_file(path):
+            return QPHandle._iterator(path, **kwargs)
+        return Hdf5Handle._iterator(path, **kwargs)
+
+
 def default_model_read(modelfile):
     """Default function to read model files, simply used pickle.load"""
-    return pickle.load(open(modelfile, 'rb'))
+    return pickle.load(open(modelfile, "rb"))
 
 
 def default_model_write(model, path):
     """Write the model, this default implementation uses pickle"""
-    with open(path, 'wb') as fout:
+    with open(path, "wb") as fout:
         pickle.dump(obj=model, file=fout, protocol=pickle.HIGHEST_PROTOCOL)
 
 
 class ModelDict(dict):
     """
-    A specialized dict to keep track of individual estimation models objects.
-    This is just a dict with these additional features:
+    A specialized dict to keep track of individual estimation models objects:
+    this is just a dict these additional features
 
     1. Keys are paths
     2. There is a read(path, force=False) method that reads a model object and
     inserts it into the dictionary
     3. There is a single static instance of this class
     """
-    def open(self, path, mode, **kwargs):  #pylint: disable=no-self-use
+
+    def open(self, path, mode, **kwargs):
         """Open the file and return the file handle"""
-        return open(path, mode, **kwargs)
+        return open(path, mode, **kwargs)  # pylint: disable=unspecified-encoding
 
-    def read(self, path, force=False, reader=None, **kwargs):  #pylint: disable=unused-argument
+    def read(
+        self, path, force=False, reader=None, **kwargs
+    ):  # pylint: disable=unused-argument
         """Read a model into this dict"""
         if reader is None:
             reader = default_model_read
         if force or path not in self:
             model = reader(path)
-            self.__setitem__(path, model)
+            self[path] = model
             return model
         return self[path]
 
-    def write(self, model, path, force=False, writer=None, **kwargs):  #pylint: disable=unused-argument
+    def write(
+        self, model, path, force=False, writer=None, **kwargs
+    ):  # pylint: disable=unused-argument
         """Write the model, this default implementation uses pickle"""
         if writer is None:
             writer = default_model_write
         if force or path not in self or not os.path.exists(path):
-            self.__setitem__(path, model)
+            self[path] = model
             writer(model, path)
 
 
-
 class ModelHandle(DataHandle):
-    """DataHandle for machine learning models
-    """
-    suffix = 'pkl'
+    """DataHandle for machine learning models"""
+
+    suffix = "pkl"
 
     model_factory = ModelDict()
 
     @classmethod
     def _open(cls, path, **kwargs):
-        """Open and return the associated file
-        """
+        """Open and return the associated file"""
         kwcopy = kwargs.copy()
-        if kwcopy.pop('mode', 'r') == 'w':
-            return cls.model_factory.open(path, mode='wb', **kwcopy)
+        if kwcopy.pop("mode", "r") == "w":
+            return cls.model_factory.open(path, mode="wb", **kwcopy)
         return cls.model_factory.read(path, **kwargs)
 
     @classmethod
     def _read(cls, path, **kwargs):
-        """Read and return the data from the associated file """
+        """Read and return the data from the associated file"""
         return cls.model_factory.read(path, **kwargs)
 
     @classmethod
     def _write(cls, data, path, **kwargs):
-        """Write the data to the associatied file """
+        """Write the data to the associated file"""
         return cls.model_factory.write(data, path, **kwargs)
 
 
 class DataStore(dict):
     """Class to provide a transient data store
 
     This class:
     1) associates data products with keys
     2) provides functions to read and write the various data produces to associated files
     """
+
     allow_overwrite = False
 
     def __init__(self, **kwargs):
-        """ Build from keywords
+        """Build from keywords
 
         Note
         ----
         All of the values must be data handles of this will raise a TypeError
         """
         dict.__init__(self)
         for key, val in kwargs.items():
             self[key] = val
 
     def __str__(self):
-        """ Override __str__ casting to deal with `TableHandle` objects in the map """
+        """Override __str__ casting to deal with `TableHandle` objects in the map"""
         s = "{"
         for key, val in self.items():
             s += f"  {key}:{val}\n"
         s += "}"
         return s
 
     def __repr__(self):
-        """ A custom representation """
+        """A custom representation"""
         s = "DataStore\n"
         s += self.__str__()
         return s
 
     def __setitem__(self, key, value):
         """ Override the __setitem__ to work with ``TableHandle`` """
         if not isinstance(value, DataHandle):
-            raise TypeError(f"Can only add objects of type DataHandle to DataStore, not {type(value)}")
+            raise TypeError(
+                f"Can only add objects of type DataHandle to DataStore, not {type(value)}"
+            )
         check = self.get(key)
         if check is not None and not self.allow_overwrite:
-            raise ValueError(f"DataStore already has an item with key {key}, of type {type(check)}, created by {check.creator}")
+            raise ValueError(
+                f"DataStore already has an item with key {key},"
+                "of type {type(check)}, created by {check.creator}"
+            )
         dict.__setitem__(self, key, value)
         return value
 
     def __getattr__(self, key):
-        """ Allow attribute-like parameter access """
+        """Allow attribute-like parameter access"""
         try:
             return self.__getitem__(key)
         except KeyError as msg:
             # Kludge to get docstrings to work
-            if key in ['__objclass__']:  #pragma: no cover
+            if key in ["__objclass__"]:  # pragma: no cover
                 return None
             raise KeyError from msg
 
     def __setattr__(self, key, value):
-        """ Allow attribute-like parameter setting """
+        """Allow attribute-like parameter setting"""
         return self.__setitem__(key, value)
 
-    def add_data(self, key, data, handle_class, path=None, creator='DataStore'):
-        """ Create a handle for some data, and insert it into the DataStore """
+    def add_data(self, key, data, handle_class, path=None, creator="DataStore"):
+        """Create a handle for some data, and insert it into the DataStore"""
         handle = handle_class(key, path=path, data=data, creator=creator)
         self[key] = handle
         return handle
 
-    def read_file(self, key, handle_class, path, creator='DataStore', **kwargs):
-        """ Create a handle, use it to read a file, and insert it into the DataStore """
+    def add_handle(self, key, handle_class, path, creator="DataStore"):
+        """Create a handle for some data, and insert it into the DataStore"""
+        handle = handle_class(key, path=path, data=None, creator=creator)
+        self[key] = handle
+        return handle
+
+    def read_file(self, key, handle_class, path, creator="DataStore", **kwargs):
+        """Create a handle, use it to read a file, and insert it into the DataStore"""
         handle = handle_class(key, path=path, data=None, creator=creator)
         handle.read(**kwargs)
         self[key] = handle
         return handle
 
     def read(self, key, force=False, **kwargs):
-        """ Read the data associated to a particular key """
+        """Read the data associated to a particular key"""
         try:
             handle = self[key]
         except KeyError as msg:
             raise KeyError(f"Failed to read data {key} because {msg}") from msg
         return handle.read(force, **kwargs)
 
-    def open(self, key, mode='r', **kwargs):
-        """ Open and return the file associated to a particular key """
+    def open(self, key, mode="r", **kwargs):
+        """Open and return the file associated to a particular key"""
         try:
             handle = self[key]
         except KeyError as msg:
             raise KeyError(f"Failed to open data {key} because {msg}") from msg
         return handle.open(mode=mode, **kwargs)
 
     def write(self, key, **kwargs):
-        """ Write the data associated to a particular key """
+        """Write the data associated to a particular key"""
         try:
             handle = self[key]
         except KeyError as msg:
             raise KeyError(f"Failed to write data {key} because {msg}") from msg
         return handle.write(**kwargs)
 
     def write_all(self, force=False, **kwargs):
-        """ Write all the data in this DataStore """
+        """Write all the data in this DataStore"""
         for key, handle in self.items():
             local_kwargs = kwargs.get(key, {})
             if handle.is_written and not force:
                 continue
             handle.write(**local_kwargs)
 
 
-
 _DATA_STORE = DataStore()
 
+
 def DATA_STORE():
     """Return the factory instance"""
     return _DATA_STORE
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/introspection.py` & `pz-rail-base-0.2.2/src/rail/core/introspection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,157 @@
 import pkgutil
-import setuptools
 import os
 import importlib
+import setuptools
 
 import rail
 
 
 class RailEnv:
-
     PACKAGES = {}
     NAMESPACE_PATH_DICT = {}
     NAMESPACE_MODULE_DICT = {}
     MODULE_DICT = {}
     MODULE_PATH_DICT = {}
     TREE = {}
     STAGE_DICT = {}
     BASE_STAGES = []
 
     @classmethod
     def list_rail_packages(cls):
         """List all the packages that are available in the RAIL ecosystem"""
-        cls.PACKAGES = {pkg.name:pkg for pkg in pkgutil.iter_modules(rail.__path__, rail.__name__ + '.')}
+        cls.PACKAGES = {
+            pkg.name: pkg
+            for pkg in pkgutil.iter_modules(rail.__path__, rail.__name__ + ".")
+        }
         return cls.PACKAGES
 
-    
     @classmethod
     def print_rail_packages(cls):
         """Print all the packages that are available in the RAIL ecosystem"""
-        if not cls.PACKAGES:
+        if not cls.PACKAGES:  # pragma: no cover
             cls.list_rail_packages()
         for pkg_name, pkg in cls.PACKAGES.items():
             print(f"{pkg_name} @ {pkg[0].path}")
-        return
 
     @classmethod
     def list_rail_namespaces(cls):
         """List all the namespaces within rail"""
         cls.NAMESPACE_PATH_DICT.clear()
-        
+
         for path_ in rail.__path__:
             namespaces = setuptools.find_namespace_packages(path_)
             for namespace_ in namespaces:
                 # exclude stuff that starts with 'example'
-                if namespace_.find('example') == 0:
+                if namespace_.find("example") == 0:
                     continue
                 if namespace_ in cls.NAMESPACE_PATH_DICT:  # pragma: no cover
                     cls.NAMESPACE_PATH_DICT[namespace_].append(path_)
                 else:
                     cls.NAMESPACE_PATH_DICT[namespace_] = [path_]
 
         return cls.NAMESPACE_PATH_DICT
 
-                    
     @classmethod
     def print_rail_namespaces(cls):
         """Print all the namespaces that are available in the RAIL ecosystem"""
         if not cls.NAMESPACE_PATH_DICT:
             cls.list_rail_namespaces()
         for key, val in cls.NAMESPACE_PATH_DICT.items():
             print(f"Namespace {key}")
             for vv in val:
                 print(f"     {vv}")
-        return
-
 
     @classmethod
     def list_rail_modules(cls):
         """List all modules within rail"""
         cls.MODULE_DICT.clear()
         cls.MODULE_PATH_DICT.clear()
         cls.NAMESPACE_MODULE_DICT.clear()
         if not cls.NAMESPACE_PATH_DICT:  # pragma: no cover
             cls.list_rail_namespaces()
         for key, val in cls.NAMESPACE_PATH_DICT.items():
             cls.NAMESPACE_MODULE_DICT[key] = []
             for vv in val:
-                fullpath = os.path.join(vv, key.replace('.', '/'))
-                modules = [pkg for pkg in pkgutil.iter_modules([fullpath], rail.__name__ + '.' + key + '.')]
+                fullpath = os.path.join(vv, key.replace(".", "/"))
+                modules = list(pkgutil.iter_modules(
+                        [fullpath], rail.__name__ + "." + key + "."
+                    )
+                )
                 for module_ in modules:
                     if module_ in cls.MODULE_DICT:  # pragma: no cover
                         cls.MODULE_DICT[module_.name].append(key)
                     else:
                         cls.MODULE_DICT[module_.name] = [key]
                     cls.NAMESPACE_MODULE_DICT[key].append(module_)
                     cls.MODULE_PATH_DICT[module_.name] = module_[0].path
 
         return cls.MODULE_PATH_DICT
 
-
     @classmethod
     def print_rail_modules(cls):
         """Print all the moduels that are available in the RAIL ecosystem"""
         if not cls.MODULE_DICT:
             cls.list_rail_modules()
-        
+
         for key, val in cls.MODULE_DICT.items():
             print(f"Module {key}")
             for vv in val:
                 print(f"     {vv}")
 
         for key, val in cls.NAMESPACE_MODULE_DICT.items():
             print(f"Namespace {key}")
             for vv in val:
                 print(f"     {vv}")
-        return
-
 
     @classmethod
     def build_rail_namespace_tree(cls):
         """Build a tree of the namespaces and packages in rail"""
         cls.TREE.clear()
         if not cls.NAMESPACE_MODULE_DICT:  # pragma: no cover
             cls.list_rail_modules()
 
         if not cls.PACKAGES:  # pragma: no cover
             cls.list_rail_packages()
 
         level_dict = {}
-        for key in cls.NAMESPACE_MODULE_DICT.keys():
-            count = key.count('.')
+        for key in cls.NAMESPACE_MODULE_DICT:
+            count = key.count(".")
             if count in level_dict:
                 level_dict[count].append(key)
             else:
                 level_dict[count] = [key]
 
         depth = max(level_dict.keys())
-        for current_depth in range(depth+1):
+        for current_depth in range(depth + 1):
             for key in level_dict[current_depth]:
-                nsname = f"rail.{key}"
+                _nsname = f"rail.{key}"
                 if current_depth == 0:
-                    nsname = f"rail.{key}"
+                    _nsname = f"rail.{key}"
                     cls.TREE[key] = cls.NAMESPACE_MODULE_DICT[key]
                 else:
-                    parent_key = '.'.join(key.split('.')[0:current_depth])
+                    parent_key = ".".join(key.split(".")[0:current_depth])
                     if parent_key in cls.TREE:
-                        cls.TREE[parent_key].append({key:cls.NAMESPACE_MODULE_DICT[key]})
+                        cls.TREE[parent_key].append(
+                            {key: cls.NAMESPACE_MODULE_DICT[key]}
+                        )
 
         return cls.TREE
-        
+
     @classmethod
     def pretty_print_tree(cls, the_dict=None, indent=""):
         """Utility function to help print the namespace tree
 
         This can be called recurisvely to walk the tree structure, which has nested dicts
 
         Parameters
         ----------
         the_dict:  dict | None
             Current dictionary to print, if None it will print cls.TREE
-    
+
         indent:  str
             Indentation string prepended to each line
         """
         if the_dict is None:  # pragma: no cover
             the_dict = cls.TREE
         for key, val in the_dict.items():
             nsname = f"rail.{key}"
@@ -160,72 +159,65 @@
                 pkg_type = "Package"
             else:
                 pkg_type = "Namespace"
 
             print(f"{indent}{pkg_type} {nsname}")
             for vv in val:
                 if isinstance(vv, dict):
-                    cls.pretty_print_tree(vv, indent=indent+"    ")
+                    cls.pretty_print_tree(vv, indent=indent + "    ")
                 else:
                     print(f"    {indent}{vv.name}")
-        return
 
-                    
     @classmethod
     def print_rail_namespace_tree(cls):
         """Print the namespace tree in a nice way"""
         if not cls.TREE:
             cls.build_rail_namespace_tree()
         cls.pretty_print_tree(cls.TREE)
-        return
-        
+
     @classmethod
     def do_pkg_api_rst(cls, basedir, key, val):
         """Build the api rst file for a rail package"""
-        
+
         api_pkg_toc = f"rail.{key} package\n"
-        api_pkg_toc += "="*len(api_pkg_toc)
+        api_pkg_toc += "=" * len(api_pkg_toc)
 
-        api_pkg_toc += \
-f"""
+        api_pkg_toc += f"""
 .. automodule:: rail.{key}
     :members:
     :undoc-members:
     :show-inheritance:
 
 Submodules
 ----------
 
 .. toctree::
     :maxdepth: 4
 
 """
-    
+
         for vv in val:
             if isinstance(vv, dict):  # pragma: no cover
-                for k3, v3 in vv.items():
+                for _k3, v3 in vv.items():
                     for v4 in v3:
                         api_pkg_toc += f"    {v4.name}.rst\n"
             else:
-                api_pkg_toc += f"    {vv.name}.rst\n"                        
+                api_pkg_toc += f"    {vv.name}.rst\n"
 
-        with open(os.path.join(basedir, 'api', f"rail.{key}.rst"), 'w') as apitocfile:
+        with open(os.path.join(basedir, "api", f"rail.{key}.rst"), "w", encoding="utf-8") as apitocfile:
             apitocfile.write(api_pkg_toc)
-        return
 
-            
     @classmethod
     def do_namespace_api_rst(cls, basedir, key, val):
         """Build the api rst file for a rail namespace"""
 
         api_pkg_toc = f"{key} namespace\n"
-        api_pkg_toc += "="*len(api_pkg_toc)
+        api_pkg_toc += "=" * len(api_pkg_toc)
 
-        api_pkg_toc += \
-"""
+        api_pkg_toc += """
 
 .. py:module:: rail.estimation
 
 Subpackages
 -----------
 
 .. toctree::
@@ -247,84 +239,80 @@
         for vv in val:
             if isinstance(vv, dict):
                 for k3, v3 in vv.items():
                     cls.do_namespace_api_rst(basedir, k3, v3)
                     sub_packages += f"    rail.{k3}\n"
             else:
                 sub_modules += f"    {vv.name}\n"
-        api_pkg_toc = api_pkg_toc.format(sub_packages=sub_packages, sub_modules=sub_modules)
-            
-        with open(os.path.join(basedir, 'api', f"rail.{key}.rst"), 'w') as apitocfile:
+        api_pkg_toc = api_pkg_toc.format(
+            sub_packages=sub_packages, sub_modules=sub_modules
+        )
+
+        with open(os.path.join(basedir, "api", f"rail.{key}.rst"), "w", encoding="utf-8") as apitocfile:
             apitocfile.write(api_pkg_toc)
-        return
 
-            
     @classmethod
-    def do_api_rst(cls, basedir='.'):
+    def do_api_rst(cls, basedir="."):
         if not cls.TREE:  # pragma: no cover
             cls.build_rail_namespace_tree()
 
-        apitoc = \
-"""API Documentation
+        apitoc = """API Documentation
 =================
 
 Information on specific functions, classes, and methods.
 
 .. toctree::
 
 """
         try:
             os.makedirs(basedir)
-        except:
+        except Exception:
             pass
 
         try:
-            os.makedirs(os.path.join(basedir, 'api'))
-        except:  # pragma: no cover
+            os.makedirs(os.path.join(basedir, "api"))
+        except Exception:  # pragma: no cover
             pass
 
-        for key, val in cls.TREE.items():        
+        for key, val in cls.TREE.items():
             nsname = f"rail.{key}"
-            nsfile = os.path.join('api', f"{nsname}.rst")
+            nsfile = os.path.join("api", f"{nsname}.rst")
             apitoc += f"    {nsfile}\n"
 
             if nsname in cls.PACKAGES:
                 cls.do_pkg_api_rst(basedir, key, val)
             else:
-                cls.do_namespace_api_rst(basedir, key, val) 
+                cls.do_namespace_api_rst(basedir, key, val)
 
-        with open(os.path.join(basedir, 'api.rst'), 'w') as apitocfile:
+        with open(os.path.join(basedir, "api.rst"), "w", encoding="utf-8") as apitocfile:
             apitocfile.write(apitoc)
 
-        return
-
-
     @classmethod
     def import_all_packages(cls):
         """Import all the packages that are available in the RAIL ecosystem"""
         pkgs = cls.list_rail_packages()
-        for pkg in pkgs.keys():
+        for pkg in pkgs:
             try:
-                imported_module = importlib.import_module(pkg)
+                _imported_module = importlib.import_module(pkg)
                 print(f"Imported {pkg}")
             except Exception as msg:
                 print(f"Failed to import {pkg} because: {str(msg)}")
 
-
     @classmethod
     def attach_stages(cls, to_module):
         """Attach all the available stages to this module
-        
+
         This allow you to do 'from rail.stages import *'
         """
-        from rail.core.stage import RailStage
+        from rail.core.stage import RailStage  # pylint: disable=import-outside-toplevel
+
         cls.STAGE_DICT.clear()
-        cls.STAGE_DICT['none'] = []
+        cls.STAGE_DICT["none"] = []
         cls.BASE_STAGES.clear()
-        
+
         n_base_classes = 0
         n_stages = 0
 
         for stage_name, stage_info in RailStage.incomplete_pipeline_stages.items():
             if stage_info[0] in [RailStage]:
                 continue
             cls.BASE_STAGES.append(stage_info[0])
@@ -339,17 +327,17 @@
             baseclass = "none"
             for possible_base in cls.BASE_STAGES:
                 if issubclass(stage_info[0], possible_base):
                     baseclass = possible_base.__name__
                     break
             cls.STAGE_DICT[baseclass].append(stage_name)
 
-        print(f"Attached {n_base_classes} base classes and {n_stages} fully formed stages to rail.stages")
-        return
-
+        print(
+            f"Attached {n_base_classes} base classes and {n_stages} fully formed stages to rail.stages"
+        )
 
     @classmethod
     def print_rail_stage_dict(cls):
         """Print an dict of all the RailSages organized by their base class"""
         for key, val in cls.STAGE_DICT.items():
             print(f"BaseClass {key}")
             for vv in val:
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/point_estimation.py` & `pz-rail-base-0.2.2/src/rail/core/point_estimation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.typing import NDArray
 
-class PointEstimationMixin():
 
+class PointEstimationMixin:
     def calculate_point_estimates(self, qp_dist, grid=None):
         """This function drives the calculation of point estimates for qp.Ensembles.
         It is defined here, and called from the `_process_chunk` method in the
         `CatEstimator` child classes.
 
         Parameters
         ----------
@@ -32,28 +32,28 @@
             - `_calculate_mode_point_estimate`
             - `_calculate_mean_point_estimate`
             - `_calculate_median_point_estimate`
         """
 
         ancil_dict = dict()
         calculated_point_estimates = []
-        if 'calculated_point_estimates' in self.config:
-            calculated_point_estimates = self.config['calculated_point_estimates']
+        if "calculated_point_estimates" in self.config:
+            calculated_point_estimates = self.config["calculated_point_estimates"]
 
-        if 'mode' in calculated_point_estimates:
+        if "mode" in calculated_point_estimates:
             mode_value = self._calculate_mode_point_estimate(qp_dist, grid)
-            ancil_dict.update(mode = mode_value)
+            ancil_dict.update(mode=mode_value)
 
-        if 'mean' in calculated_point_estimates:
+        if "mean" in calculated_point_estimates:
             mean_value = self._calculate_mean_point_estimate(qp_dist)
-            ancil_dict.update(mean = mean_value)
+            ancil_dict.update(mean=mean_value)
 
-        if 'median' in calculated_point_estimates:
+        if "median" in calculated_point_estimates:
             median_value = self._calculate_median_point_estimate(qp_dist)
-            ancil_dict.update(median = median_value)
+            ancil_dict.update(median=median_value)
 
         if calculated_point_estimates:
             if qp_dist.ancil is None:
                 qp_dist.set_ancil(ancil_dict)
             else:
                 qp_dist.add_to_ancil(ancil_dict)
 
@@ -81,18 +81,20 @@
         ------
         KeyError
             If `grid` is not provided, one will be created using stage_config
             `zmin`, `zmax`, and `nzbins` keys. If any of those keys are missing,
             we'll raise a KeyError.
         """
         if grid is None:
-            for key in ['zmin', 'zmax', 'nzbins']:
+            for key in ["zmin", "zmax", "nzbins"]:
                 if key not in self.config:
-                    raise KeyError(f"Expected `{key}` to be defined in stage " \
-                                   "configuration dictionary in order to caluclate mode.")
+                    raise KeyError(
+                        f"Expected `{key}` to be defined in stage "
+                        "configuration dictionary in order to caluclate mode."
+                    )
 
             grid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins)
 
         return qp_dist.mode(grid=grid)
 
     def _calculate_mean_point_estimate(self, qp_dist) -> NDArray:
         """Calculates and returns the mean values for a set of posterior estimates
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/stage.py` & `pz-rail-base-0.2.2/src/rail/core/stage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """ Base class for PipelineStages in Rail """
 
 import os
+from math import ceil
 
 from ceci import PipelineStage, MiniPipeline
 from ceci.config import StageParameter as Param
 from rail.core.data import DATA_STORE, DataHandle
 
-from math import ceil
 
 class StageIO:
     """A small utility class for Stage Input/ Output
 
     This make it possible to get access to stage inputs and outputs
     as attributes rather that by using the get_handle() method.
 
     In short it maps
 
     a_stage.get_handle('input', allow_missing=True) to a_stage.input
 
     This allows users to be more concise when writing pipelines.
     """
+
     def __init__(self, parent):
         self._parent = parent
 
     def __getattr__(self, item):
         return self._parent.get_handle(item, allow_missing=True)
 
 
@@ -38,14 +39,15 @@
     a_pipe.stage_name = StageClass.build(...)
 
     And get a stage named 'stage_name', rather than having to do:
 
     a_stage = StageClass.make_stage(..)
     a_pipe.add_stage(a_stage)
     """
+
     def __init__(self, stage_class, **kwargs):
         self.stage_class = stage_class
         self._kwargs = kwargs
 
     def build(self, name):
         """Actually build the stage, this is called by the pipeline the stage
         belongs to
@@ -72,15 +74,15 @@
     self.stage_1 = Stage1Class.build(...)
     self.stage_2 = Stage2Class.build(connections=dict(input=self.stage1.io.output), ...)
 
     And end up with a fully specified pipeline.
     """
 
     def __init__(self):
-        MiniPipeline.__init__(self, [], dict(name='mini'))
+        MiniPipeline.__init__(self, [], dict(name="mini"))
 
     def __setattr__(self, name, value):
         if isinstance(value, RailStageBuild):
             stage = value.build(name)
             self.add_stage(stage)
             return stage
         return MiniPipeline.__setattr__(self, name, value)
@@ -123,22 +125,23 @@
     under the key "special_pz_input".
 
     And `connect_input()` will do the alias lookup both on the input and output.
     I.e., it is the same as calling
     `self.set_data(inputTag, other.get_handle(outputTag, allow_missing=True), do_read=False)`
     """
 
-    config_options = dict(output_mode=Param(str, 'default',
-                                            msg="What to do with the outputs"))
+    config_options = dict(
+        output_mode=Param(str, "default", msg="What to do with the outputs")
+    )
 
     data_store = DATA_STORE()
 
     def __init__(self, args, comm=None):
-        """ Constructor:
-        Do RailStage specific initialization """
+        """Constructor:
+        Do RailStage specific initialization"""
         PipelineStage.__init__(self, args, comm=comm)
         self._input_length = None
         self.io = StageIO(self)
 
     @classmethod
     def make_and_connect(cls, **kwargs):
         """Make a stage and connects it to other stages
@@ -152,15 +155,15 @@
         The 'connections' keyword is special, it is a dict[str, DataHandle]
         and should define the Input connections for this stage
 
         Returns
         -------
         A stage
         """
-        connections = kwargs.pop('connections', {})
+        connections = kwargs.pop("connections", {})
         stage = cls.make_stage(**kwargs)
         for key, val in connections.items():
             stage.set_data(key, val, do_read=False)
         return stage
 
     @classmethod
     def build(cls, **kwargs):
@@ -184,15 +187,17 @@
         handle : DataHandle
             The handle that give access to the associated data
         """
         aliased_tag = self.get_aliased_tag(tag)
         handle = self.data_store.get(aliased_tag)
         if handle is None:
             if not allow_missing:
-                raise KeyError(f'{self.instance_name} failed to get data by handle {aliased_tag}, associated to {tag}')
+                raise KeyError(
+                    f"{self.instance_name} failed to get data by handle {aliased_tag}, associated to {tag}"
+                )
             handle = self.add_handle(tag, path=path)
         return handle
 
     def add_handle(self, tag, data=None, path=None):
         """Adds a DataHandle associated to a particular tag
 
         Parameters
@@ -214,16 +219,20 @@
             if path is None:
                 path = self.get_input(aliased_tag)
             handle_type = self.get_input_type(tag)
         else:
             if path is None:
                 path = self.get_output(aliased_tag)
             handle_type = self.get_output_type(tag)
-        handle = handle_type(aliased_tag, path=path, data=data, creator=self.instance_name)
-        print(f"Inserting handle into data store.  {aliased_tag}: {handle.path}, {handle.creator}")
+        handle = handle_type(
+            aliased_tag, path=path, data=data, creator=self.instance_name
+        )
+        print(
+            f"Inserting handle into data store.  {aliased_tag}: {handle.path}, {handle.creator}"
+        )
         self.data_store[aliased_tag] = handle
         return handle
 
     def get_data(self, tag, allow_missing=True):
         """Gets the data associated to a particular tag
 
         Notes
@@ -326,48 +335,50 @@
 
         kwargs : dict[str, Any]
             These will be passed to the Handle's iterator method
         """
         handle = self.get_handle(tag, allow_missing=True)
 
         try:
-            self.config.hdf5_groupname
-        except:
-            self.config.hdf5_groupname = None
-
-        if handle.path and handle.path!='None':
-            self._input_length = handle.size(groupname=self.config.hdf5_groupname)
-            total_chunks_needed = ceil(self._input_length/self.config.chunk_size)
+            groupname = kwargs.get('groupname', self.config.hdf5_groupname)
+        except Exception:
+            groupname = None
+
+        if handle.path and handle.path != "None":   # pylint: disable=no-else-return
+            self._input_length = handle.size(groupname=groupname)
+            total_chunks_needed = ceil(self._input_length / self.config.chunk_size)
             # If the number of process is larger than we need, we wemove some of them
-            if total_chunks_needed < self.size:  #pragma: no cover
-                color = self.rank+1 <= total_chunks_needed
-                newcomm = self.comm.Split(color=color,key=self.rank)
+            if total_chunks_needed < self.size:  # pragma: no cover
+                color = self.rank + 1 <= total_chunks_needed
+                newcomm = self.comm.Split(color=color, key=self.rank)
                 if color:
                     self.setup_mpi(newcomm)
                 else:
                     quit()
-            kwcopy = dict(groupname=self.config.hdf5_groupname,
-                          chunk_size=self.config.chunk_size,
-                          rank=self.rank,
-                          parallel_size=self.size)
+            kwcopy = dict(
+                groupname=groupname,
+                chunk_size=self.config.chunk_size,
+                rank=self.rank,
+                parallel_size=self.size,
+            )
             kwcopy.update(**kwargs)
             return handle.iterator(**kwcopy)
+
+
         # If data is in memory and not in a file, it means is small enough to process it
         # in a single chunk.
-        else:  #pragma: no cover
+        else:  # pragma: no cover
             if self.config.hdf5_groupname:
-                test_data = self.get_data('input')[self.config.hdf5_groupname]
+                test_data = self.get_data(tag)[self.config.hdf5_groupname]
+                self._input_length = self.get_handle(tag).data_size(groupname=self.config.hdf5_groupname)
             else:
-                test_data = self.get_data('input')
-            max_l = 0
-            for k, v in test_data.items():
-                max_l = max(max_l, len(v))
-            self._input_length = max_l
+                test_data = self.get_data(tag)
+                self._input_length = self.get_handle(tag).data_size()
             s = 0
-            iterator=[[s, self._input_length, test_data]]
+            iterator = [[s, self._input_length, test_data]]
             return iterator
 
     def connect_input(self, other, inputTag=None, outputTag=None):
         """Connect another stage to this stage as an input
 
         Parameters
         ----------
@@ -379,15 +390,15 @@
              Which output tag of the other stage to connect to.  None -> other.outputs[0]
 
         Returns
         -------
         handle : The input handle for this stage
         """
         if inputTag is None:
-            inputTag = self.inputs[0][0]  #pylint: disable=no-member
+            inputTag = self.inputs[0][0]  # pylint: disable=no-member
         if outputTag is None:
             outputTag = other.outputs[0][0]
         handle = other.get_handle(outputTag, allow_missing=True)
         return self.set_data(inputTag, handle, do_read=False)
 
     def _finalize_tag(self, tag):
         """Finalize the data for a particular tag.
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/util_stages.py` & `pz-rail-base-0.2.2/src/rail/core/util_stages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """ Stages that implement utility functions """
-import os
-import numpy as np
-
 import tables_io
 
 from rail.core.stage import RailStage
 
 from rail.core.data import PqHandle, Hdf5Handle
 
 
@@ -16,29 +13,30 @@
     -----
     1. This operates on pandas dataframs in parquet files.
 
     2. In short, this does:
     `output_data = input_data.rename(columns=self.config.columns, inplace=self.config.inplace)`
 
     """
-    name = 'ColumnMapper'
+
+    name = "ColumnMapper"
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=100_000, columns=dict, inplace=False)
-    inputs = [('input', PqHandle)]
-    outputs = [('output', PqHandle)]
+    inputs = [("input", PqHandle)]
+    outputs = [("output", PqHandle)]
 
     def __init__(self, args, comm=None):
         RailStage.__init__(self, args, comm=comm)
 
     def run(self):
-        data = self.get_data('input', allow_missing=True)
+        data = self.get_data("input", allow_missing=True)
         out_data = data.rename(columns=self.config.columns, inplace=self.config.inplace)
-        if self.config.inplace:  #pragma: no cover
+        if self.config.inplace:  # pragma: no cover
             out_data = data
-        self.add_data('output', out_data)
+        self.add_data("output", out_data)
 
     def __repr__(self):  # pragma: no cover
         printMsg = "Stage that applies remaps the following column names in a pandas DataFrame:\n"
         printMsg += "f{str(self.config.columns)}"
         return printMsg
 
     def __call__(self, data):
@@ -50,44 +48,45 @@
             The data to be renamed
 
         Returns
         -------
         table : Table-like
             The degraded sample
         """
-        self.set_data('input', data)
+        self.set_data("input", data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
 
 
 class RowSelector(RailStage):
     """Utility Stage that sub-selects rows from a table by index
 
     Notes
     -----
     1. This operates on pandas dataframs in parquet files.
 
     2. In short, this does:
     `output_data = input_data[self.config.start:self.config.stop]`
 
     """
-    name = 'RowSelector'
+
+    name = "RowSelector"
     config_options = RailStage.config_options.copy()
     config_options.update(start=int, stop=int)
-    inputs = [('input', PqHandle)]
-    outputs = [('output', PqHandle)]
+    inputs = [("input", PqHandle)]
+    outputs = [("output", PqHandle)]
 
     def __init__(self, args, comm=None):
         RailStage.__init__(self, args, comm=comm)
 
     def run(self):
-        data = self.get_data('input', allow_missing=True)
-        out_data = data.iloc[self.config.start:self.config.stop]
-        self.add_data('output', out_data)
+        data = self.get_data("input", allow_missing=True)
+        out_data = data.iloc[self.config.start : self.config.stop]
+        self.add_data("output", out_data)
 
     def __repr__(self):  # pragma: no cover
         printMsg = "Stage that applies remaps the following column names in a pandas DataFrame:\n"
         printMsg += "f{str(self.config.columns)}"
         return printMsg
 
     def __call__(self, data):
@@ -99,51 +98,52 @@
             The data to be renamed
 
         Returns
         -------
         table : table-like
             The degraded sample
         """
-        self.set_data('input', data)
+        self.set_data("input", data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
 
 
 class TableConverter(RailStage):
     """Utility stage that converts tables from one format to anothe
 
     FIXME, this is hardwired to convert parquet tables to Hdf5Tables.
     It would be nice to have more options here.
     """
-    name = 'TableConverter'
+
+    name = "TableConverter"
     config_options = RailStage.config_options.copy()
     config_options.update(output_format=str)
-    inputs = [('input', PqHandle)]
-    outputs = [('output', Hdf5Handle)]
+    inputs = [("input", PqHandle)]
+    outputs = [("output", Hdf5Handle)]
 
     def __init__(self, args, comm=None):
         RailStage.__init__(self, args, comm=comm)
 
     def run(self):
-        data = self.get_data('input', allow_missing=True)
+        data = self.get_data("input", allow_missing=True)
         out_fmt = tables_io.types.TABULAR_FORMAT_NAMES[self.config.output_format]
         out_data = tables_io.convert(data, out_fmt)
-        self.add_data('output', out_data)
+        self.add_data("output", out_data)
 
     def __call__(self, data):
         """Return a converted table
 
         Parameters
         ----------
         data : table-like
             The data to be converted
 
         Returns
         -------
         out_data : table-like
             The converted version of the table
         """
-        self.set_data('input', data)
+        self.set_data("input", data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
```

### Comparing `pz-rail-base-0.2.1/src/rail/core/utils.py` & `pz-rail-base-0.2.2/src/rail/core/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Utility functions """
 
 import os
 import rail
 import rail.core
 
-RAILDIR = os.path.abspath(os.path.join(os.path.dirname(rail.core.__file__), '..', '..'))
+RAILDIR = os.path.abspath(os.path.join(os.path.dirname(rail.core.__file__), "..", ".."))
 
 
 def find_rail_file(relpath):
     """Find a file somewhere in rail by searching the namespace path
 
     This lets us avoid issues that the paths can be different depending
     on if we have installed things from source or not
```

### Comparing `pz-rail-base-0.2.1/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.2.2/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/creation/degrader.py` & `pz-rail-base-0.2.2/src/rail/creation/degrader.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 The key feature is that the __call__ method takes a pandas DataFrame and a seed,
 and returns a pandas DataFrame, and wraps the run method.
 """
 
 from rail.core.stage import RailStage
 from rail.core.data import PqHandle
 
+
 class Degrader(RailStage):
     """Base class Degraders, which apply various degradations to synthetic 
     photometric data.
 
     Degraders take "input" data in the form of pandas dataframes in Parquet 
     files and provide as "output" another pandas dataframes written to Parquet 
     files.
     """
 
-    name = 'Degrader'
+    name = "Degrader"
     config_options = RailStage.config_options.copy()
     config_options.update(seed=12345)
-    inputs = [('input', PqHandle)]
-    outputs = [('output', PqHandle)]
+    inputs = [("input", PqHandle)]
+    outputs = [("output", PqHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Degrader that can degrade photometric data"""
         RailStage.__init__(self, args, comm=comm)
 
     def __call__(self, sample, seed: int = None):
         """The main interface method for ``Degrader``.
@@ -53,11 +54,11 @@
         Returns
         -------
         output_data : PqHandle
             A handle giving access to a table with degraded sample
         """
         if seed is not None:
             self.config.seed = seed
-        self.set_data('input', sample)
+        self.set_data("input", sample)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
```

### Comparing `pz-rail-base-0.2.1/src/rail/creation/engine.py` & `pz-rail-base-0.2.2/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/equal_count.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/equal_count.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,58 +4,66 @@
 """
 
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.estimation.classifier import PZClassifier
 from rail.core.data import TableHandle
 
+
 class EqualCountClassifier(PZClassifier):
     """Classifier that simply assign tomographic
     bins based on point estimate according to SRD"""
 
-    name = 'EqualCountClassifier'
+    name = "EqualCountClassifier"
     config_options = PZClassifier.config_options.copy()
     config_options.update(
-        id_name=Param(str, "", msg="Column name for the object ID in the input data, if empty the row index is used as the ID."),
-        point_estimate=Param(str, 'zmode', msg="Which point estimate to use"),
+        id_name=Param(
+            str,
+            "",
+            msg="Column name for the object ID in the input data, if empty the row index is used as the ID.",
+        ),
+        point_estimate=Param(str, "zmode", msg="Which point estimate to use"),
         zmin=Param(float, 0.0, msg="Minimum redshift of the sample"),
         zmax=Param(float, 3.0, msg="Maximum redshift of the sample"),
         nbins=Param(int, 5, msg="Number of tomographic bins"),
         no_assign=Param(int, -99, msg="Value for no assignment flag"),
-        )
-    outputs = [('output', TableHandle)]
+    )
+    outputs = [("output", TableHandle)]
 
     def __init__(self, args, comm=None):
         PZClassifier.__init__(self, args, comm=comm)
 
     def run(self):
-        test_data = self.get_data('input')
+        test_data = self.get_data("input")
         npdf = test_data.npdf
-        
+
         try:
             zb = test_data.ancil[self.config.point_estimate]
-        except KeyError:
-            raise KeyError(f"{self.config.point_estimate} is not contained in the data ancil, you will need to compute it explicitly.")
+        except KeyError as msg:
+            raise KeyError(
+                f"{self.config.point_estimate} is not contained in the data ancil, "
+                "you will need to compute it explicitly."
+            ) from msg
 
         # tomographic bins with equal number density
         sortind = np.argsort(zb)
-        cum=np.arange(1,(len(zb)+1))
+        cum = np.arange(1, (len(zb) + 1))
         bin_index = np.zeros(len(zb))
         for ii in range(self.config.nbins):
-            perc1=ii/self.config.nbins
-            perc2=(ii+1)/self.config.nbins
-            ind=(cum/cum[-1]>perc1)&(cum/cum[-1]<=perc2)
-            useind=sortind[ind]
-            bin_index[useind] = int(ii+1)
+            perc1 = ii / self.config.nbins
+            perc2 = (ii + 1) / self.config.nbins
+            ind = (cum / cum[-1] > perc1) & (cum / cum[-1] <= perc2)
+            useind = sortind[ind]
+            bin_index[useind] = int(ii + 1)
 
         if self.config.id_name != "":
             # below is commented out and replaced by a redundant line
             # because the data doesn't have ID yet
             # obj_id = test_data[self.config.id_name]
             obj_id = np.arange(npdf)
         elif self.config.id_name == "":
             # ID set to row index
             obj_id = np.arange(npdf)
-            self.config.id_name="row_index"
-        
+            self.config.id_name = "row_index"
+
         class_id = {self.config.id_name: obj_id, "class_id": bin_index}
-        self.add_data('output', class_id)
+        self.add_data("output", class_id)
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/naive_stack.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/naive_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,76 +8,76 @@
 from ceci.config import StageParameter as Param
 from rail.estimation.summarizer import PZSummarizer
 from rail.estimation.informer import PzInformer
 from rail.core.data import QPHandle
 
 
 class NaiveStackInformer(PzInformer):
-    """Placeholder Informer
-    """
+    """Placeholder Informer"""
 
-    name = 'NaiveStackInformer'
+    name = "NaiveStackInformer"
     config_options = PzInformer.config_options.copy()
 
     def __init__(self, args, comm=None):
         PzInformer.__init__(self, args, comm=comm)
 
     def run(self):
-        self.add_data('model', np.array([None]))
+        self.add_data("model", np.array([None]))
+
 
 class NaiveStackSummarizer(PZSummarizer):
-    """Summarizer which stacks individual P(z)
-    """
+    """Summarizer which stacks individual P(z)"""
 
-    name = 'NaiveStackSummarizer'
+    name = "NaiveStackSummarizer"
     config_options = PZSummarizer.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
-                          zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
-                          nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
-                          seed=Param(int, 87, msg="random seed"),
-                          nsamples=Param(int, 1000, msg="Number of sample distributions to create"))
-    inputs = [('input', QPHandle)]
-    outputs = [('output', QPHandle),
-               ('single_NZ', QPHandle)]
+    config_options.update(
+        zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
+        zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
+        nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
+        seed=Param(int, 87, msg="random seed"),
+        nsamples=Param(int, 1000, msg="Number of sample distributions to create"),
+    )
+    inputs = [("input", QPHandle)]
+    outputs = [("output", QPHandle), ("single_NZ", QPHandle)]
 
     def __init__(self, args, comm=None):
         PZSummarizer.__init__(self, args, comm=comm)
         self.zgrid = None
 
     def run(self):
-        iterator = self.input_iterator('input')
-        self.zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins + 1)
+        iterator = self.input_iterator("input")
+        self.zgrid = np.linspace(
+            self.config.zmin, self.config.zmax, self.config.nzbins + 1
+        )
         # Initiallizing the stacking pdf's
         yvals = np.zeros((1, len(self.zgrid)))
         bvals = np.zeros((self.config.nsamples, len(self.zgrid)))
-        bootstrap_matrix  = self._broadcast_bootstrap_matrix()
+        bootstrap_matrix = self._broadcast_bootstrap_matrix()
 
         first = True
         for s, e, test_data in iterator:
             print(f"Process {self.rank} running estimator on chunk {s} - {e}")
             self._process_chunk(s, e, test_data, first, bootstrap_matrix, yvals, bvals)
             first = False
         if self.comm is not None:  # pragma: no cover
             bvals, yvals = self._join_histograms(bvals, yvals)
 
         if self.rank == 0:
-            sample_ens = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=bvals))
+            sample_ens = qp.Ensemble(
+                qp.interp, data=dict(xvals=self.zgrid, yvals=bvals)
+            )
             qp_d = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=yvals))
-            self.add_data('output', sample_ens)
-            self.add_data('single_NZ', qp_d)
-
+            self.add_data("output", sample_ens)
+            self.add_data("single_NZ", qp_d)
 
-    def  _process_chunk(self, start, end, data, first, bootstrap_matrix, yvals, bvals):
+    def _process_chunk(self, start, end, data, _first, bootstrap_matrix, yvals, bvals):
         pdf_vals = data.pdf(self.zgrid)
-        yvals += np.expand_dims(np.sum(np.where(np.isfinite(pdf_vals), pdf_vals, 0.), axis=0), 0)
+        yvals += np.expand_dims(
+            np.sum(np.where(np.isfinite(pdf_vals), pdf_vals, 0.0), axis=0), 0
+        )
         # qp_d is the normalized probability of the stack, we need to know how many galaxies were
         for i in range(self.config.nsamples):
             bootstrap_draws = bootstrap_matrix[:, i]
             # Neither all of the bootstrap_draws are in this chunk nor the index starts at "start"
-            mask = (bootstrap_draws>=start) & (bootstrap_draws<end)
+            mask = (bootstrap_draws >= start) & (bootstrap_draws < end)
             bootstrap_draws = bootstrap_draws[mask] - start
             bvals[i] += np.sum(pdf_vals[bootstrap_draws], axis=0)
-
-
-
-
-
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/point_est_hist.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/point_est_hist.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,78 +8,83 @@
 from ceci.config import StageParameter as Param
 from rail.estimation.summarizer import PZSummarizer
 from rail.estimation.informer import PzInformer
 from rail.core.data import QPHandle
 
 
 class PointEstHistInformer(PzInformer):
-    """Placeholder Informer
-    """
+    """Placeholder Informer"""
 
-    name = 'PointEstHistInformer'
+    name = "PointEstHistInformer"
     config_options = PzInformer.config_options.copy()
 
     def __init__(self, args, comm=None):
         PzInformer.__init__(self, args, comm=comm)
 
     def run(self):
-        self.add_data('model', np.array([None]))
+        self.add_data("model", np.array([None]))
 
 
 class PointEstHistSummarizer(PZSummarizer):
-    """Summarizer which simply histograms a point estimate
-    """
+    """Summarizer which simply histograms a point estimate"""
 
-    name = 'PointEstHistSummarizer'
+    name = "PointEstHistSummarizer"
     config_options = PZSummarizer.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
-                          zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
-                          nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
-                          seed=Param(int, 87, msg="random seed"),
-                          point_estimate=Param(str, 'zmode', msg="Which point estimate to use"),
-                          nsamples=Param(int, 1000, msg="Number of sample distributions to return"))
-    inputs = [('input', QPHandle)]
-    outputs = [('output', QPHandle),
-               ('single_NZ', QPHandle)]
+    config_options.update(
+        zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
+        zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
+        nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
+        seed=Param(int, 87, msg="random seed"),
+        point_estimate=Param(str, "zmode", msg="Which point estimate to use"),
+        nsamples=Param(int, 1000, msg="Number of sample distributions to return"),
+    )
+    inputs = [("input", QPHandle)]
+    outputs = [("output", QPHandle), ("single_NZ", QPHandle)]
 
     def __init__(self, args, comm=None):
         PZSummarizer.__init__(self, args, comm=comm)
         self.zgrid = None
         self.bincents = None
 
-
     def run(self):
-        iterator = self.input_iterator('input')
-        self.zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins + 1)
+        iterator = self.input_iterator("input")
+        self.zgrid = np.linspace(
+            self.config.zmin, self.config.zmax, self.config.nzbins + 1
+        )
         self.bincents = 0.5 * (self.zgrid[1:] + self.zgrid[:-1])
-        bootstrap_matrix  = self._broadcast_bootstrap_matrix()
+        bootstrap_matrix = self._broadcast_bootstrap_matrix()
         # Initiallizing the histograms
         single_hist = np.zeros(self.config.nzbins)
         hist_vals = np.zeros((self.config.nsamples, self.config.nzbins))
 
         first = True
         for s, e, test_data in iterator:
             print(f"Process {self.rank} running estimator on chunk {s} - {e}")
-            self._process_chunk(s, e, test_data, first, bootstrap_matrix, single_hist, hist_vals)
+            self._process_chunk(
+                s, e, test_data, first, bootstrap_matrix, single_hist, hist_vals
+            )
             first = False
         if self.comm is not None:  # pragma: no cover
             hist_vals, single_hist = self._join_histograms(hist_vals, single_hist)
 
         if self.rank == 0:
-            sample_ens = qp.Ensemble(qp.hist,
-                                 data=dict(bins=self.zgrid, pdfs=np.atleast_2d(hist_vals)))
-            qp_d = qp.Ensemble(qp.hist,
-                           data=dict(bins=self.zgrid, pdfs=np.atleast_2d(single_hist)))
-            self.add_data('output', sample_ens)
-            self.add_data('single_NZ', qp_d)
-
-    def  _process_chunk(self, start, end, test_data, first, bootstrap_matrix, single_hist, hist_vals):
+            sample_ens = qp.Ensemble(
+                qp.hist, data=dict(bins=self.zgrid, pdfs=np.atleast_2d(hist_vals))
+            )
+            qp_d = qp.Ensemble(
+                qp.hist, data=dict(bins=self.zgrid, pdfs=np.atleast_2d(single_hist))
+            )
+            self.add_data("output", sample_ens)
+            self.add_data("single_NZ", qp_d)
+
+    def _process_chunk(
+        self, start, end, test_data, _first, bootstrap_matrix, single_hist, hist_vals
+    ):
         zb = test_data.ancil[self.config.point_estimate]
         single_hist += np.histogram(zb, bins=self.zgrid)[0]
         for i in range(self.config.nsamples):
             bootstrap_indeces = bootstrap_matrix[:, i]
             # Neither all of the bootstrap_draws are in this chunk nor the index starts at "start"
-            mask = (bootstrap_indeces>=start) & (bootstrap_indeces<end)
+            mask = (bootstrap_indeces >= start) & (bootstrap_indeces < end)
             bootstrap_indeces = bootstrap_indeces[mask] - start
             zarr = zb[bootstrap_indeces]
             hist_vals[i] += np.histogram(zarr, bins=self.zgrid)[0]
-
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/random_gauss.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/random_gauss.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,56 +10,66 @@
 from scipy.stats import norm
 from ceci.config import StageParameter as Param
 from rail.estimation.estimator import CatEstimator, CatInformer
 from rail.core.data import TableHandle
 
 
 class RandomGaussInformer(CatInformer):
-    """Placeholder Informer
-    """
+    """Placeholder Informer"""
 
-    name = 'RandomGaussInformer'
+    name = "RandomGaussInformer"
     config_options = CatInformer.config_options.copy()
 
     def __init__(self, args, comm=None):
         CatInformer.__init__(self, args, comm=comm)
 
     def run(self):
-        self.add_data('model', np.array([None]))
+        self.add_data("model", np.array([None]))
 
 
 class RandomGaussEstimator(CatEstimator):
-    """Random CatEstimator
-    """
+    """Random CatEstimator"""
 
-    name = 'RandomGaussEstimator'
-    inputs = [('input', TableHandle)]
+    name = "RandomGaussEstimator"
+    inputs = [("input", TableHandle)]
     config_options = CatEstimator.config_options.copy()
-    config_options.update(rand_width=Param(float, 0.025, "ad hock width of PDF"),
-                          rand_zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
-                          rand_zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
-                          nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
-                          seed=Param(int, 87, msg="random seed"),
-                          column_name=Param(str, "mag_i_lsst",
-                                            msg="name of a column that has the "\
-                                                "correct number of galaxies to find length of"))
+    config_options.update(
+        rand_width=Param(float, 0.025, "ad hock width of PDF"),
+        rand_zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
+        rand_zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
+        nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
+        seed=Param(int, 87, msg="random seed"),
+        column_name=Param(
+            str,
+            "mag_i_lsst",
+            msg="name of a column that has the "
+            "correct number of galaxies to find length of",
+        ),
+    )
 
     def __init__(self, args, comm=None):
-        """ Constructor:
-        Do CatEstimator specific initialization """
+        """Constructor:
+        Do CatEstimator specific initialization"""
         CatEstimator.__init__(self, args, comm=comm)
         self.zgrid = None
 
     def _process_chunk(self, start, end, data, first):
         pdf = []
         # allow for either format for now
         numzs = len(data[self.config.column_name])
         rng = np.random.default_rng(seed=self.config.seed + start)
         zmode = np.round(rng.uniform(0.0, self.config.rand_zmax, numzs), 3)
         widths = self.config.rand_width * (1.0 + zmode)
-        self.zgrid = np.linspace(self.config.rand_zmin, self.config.rand_zmax, self.config.nzbins)
+        self.zgrid = np.linspace(
+            self.config.rand_zmin, self.config.rand_zmax, self.config.nzbins
+        )
         for i in range(numzs):
             pdf.append(norm.pdf(self.zgrid, zmode[i], widths[i]))
-        qp_d = qp.Ensemble(qp.stats.norm, data=dict(loc=np.expand_dims(zmode, -1),  # pylint: disable=no-member
-                                                    scale=np.expand_dims(widths, -1)))
+        qp_d = qp.Ensemble(
+            qp.stats.norm,  # pylint: disable=no-member
+            data=dict(
+                loc=np.expand_dims(zmode, -1),  # pylint: disable=no-member
+                scale=np.expand_dims(widths, -1),
+            ),
+        )
         qp_d.set_ancil(dict(zmode=zmode))
         self._do_chunk_output(qp_d, start, end, first)
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/train_z.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/train_z.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,73 +2,72 @@
 Implementation of the 'pathological photo-z PDF estimator,
 as used in arXiv:2001.03621 (see section 3.3). It assigns each test set galaxy
 a photo-z PDF equal to the normalized redshift distribution
 N (z) of the training set.
 """
 
 import numpy as np
-from ceci.config import StageParameter as Param
-from rail.estimation.estimator import CatEstimator, CatInformer
-from rail.core.common_params import SHARED_PARAMS
 import qp
+from rail.estimation.estimator import CatEstimator
+from rail.estimation.informer import CatInformer
+from rail.core.common_params import SHARED_PARAMS
 
 
 class trainZmodel:
     """
     Temporary class to store the single trainZ pdf for trained model.
     Given how simple this is to compute, this seems like overkill.
     """
+
     def __init__(self, zgrid, pdf, zmode):
         self.zgrid = zgrid
         self.pdf = pdf
         self.zmode = zmode
 
 
 class TrainZInformer(CatInformer):
-    """Train an Estimator which returns a global PDF for all galaxies
-    """
+    """Train an Estimator which returns a global PDF for all galaxies"""
 
-    name = 'TrainZInformer'
+    name = "TrainZInformer"
     config_options = CatInformer.config_options.copy()
-    config_options.update(zmin=SHARED_PARAMS,
-                          zmax=SHARED_PARAMS,
-                          nzbins=SHARED_PARAMS,
-                          redshift_col=SHARED_PARAMS)
+    config_options.update(
+        zmin=SHARED_PARAMS,
+        zmax=SHARED_PARAMS,
+        nzbins=SHARED_PARAMS,
+        redshift_col=SHARED_PARAMS,
+    )
 
     def __init__(self, args, comm=None):
         CatInformer.__init__(self, args, comm=comm)
 
     def run(self):
         if self.config.hdf5_groupname:
-            training_data = self.get_data('input')[self.config.hdf5_groupname]
+            training_data = self.get_data("input")[self.config.hdf5_groupname]
         else:  # pragma: no cover
-            training_data = self.get_data('input')
+            training_data = self.get_data("input")
         zbins = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins + 1)
         speczs = np.sort(training_data[self.config.redshift_col])
         train_pdf, _ = np.histogram(speczs, zbins)
         midpoints = zbins[:-1] + np.diff(zbins) / 2
         zmode = midpoints[np.argmax(train_pdf)]
         cdf = np.cumsum(train_pdf)
         cdf = cdf / cdf[-1]
         norm = cdf[-1] * (zbins[2] - zbins[1])
         train_pdf = train_pdf / norm
         zgrid = midpoints
         self.model = trainZmodel(zgrid, train_pdf, zmode)
-        self.add_data('model', self.model)
+        self.add_data("model", self.model)
 
 
 class TrainZEstimator(CatEstimator):
-    """CatEstimator which returns a global PDF for all galaxies
-    """
+    """CatEstimator which returns a global PDF for all galaxies"""
 
-    name = 'TrainZEstimator'
+    name = "TrainZEstimator"
     config_options = CatEstimator.config_options.copy()
-    config_options.update(zmin=SHARED_PARAMS,
-                          zmax=SHARED_PARAMS,
-                          nzbins=SHARED_PARAMS)
+    config_options.update(zmin=SHARED_PARAMS, zmax=SHARED_PARAMS, nzbins=SHARED_PARAMS)
 
     def __init__(self, args, comm=None):
         self.zgrid = None
         self.train_pdf = None
         self.zmode = None
         CatEstimator.__init__(self, args, comm=comm)
 
@@ -79,11 +78,13 @@
         self.zgrid = self.model.zgrid
         self.train_pdf = self.model.pdf
         self.zmode = self.model.zmode
 
     def _process_chunk(self, start, end, data, first):
         test_size = end - start
         zmode = np.repeat(self.zmode, test_size)
-        qp_d = qp.Ensemble(qp.interp,
-                           data=dict(xvals=self.zgrid, yvals=np.tile(self.train_pdf, (test_size, 1))))
+        qp_d = qp.Ensemble(
+            qp.interp,
+            data=dict(xvals=self.zgrid, yvals=np.tile(self.train_pdf, (test_size, 1))),
+        )
         qp_d.set_ancil(dict(zmode=zmode))
         self._do_chunk_output(qp_d, start, end, first)
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/uniform_binning.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/uniform_binning.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,34 @@
 """
 
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.estimation.classifier import PZClassifier
 from rail.core.data import TableHandle, Hdf5Handle
 
+
 class UniformBinningClassifier(PZClassifier):
     """Classifier that simply assigns tomographic bins based on a point estimate 
     according to SRD.
     """
     name = 'UniformBinningClassifier'
     config_options = PZClassifier.config_options.copy()
     config_options.update(
-        id_name=Param(str, "", msg="Column name for the object ID in the input data, if empty the row index is used as the ID."),
-        point_estimate=Param(str, 'zmode', msg="Which point estimate to use"),
-        zbin_edges=Param(list, [], msg="The tomographic redshift bin edges. If this is given (contains two or more entries), all settings below will be ignored."),
+        id_name=Param(
+            str,
+            "",
+            msg="Column name for the object ID in the input data, if empty the row index is used as the ID.",
+        ),
+        point_estimate=Param(str, "zmode", msg="Which point estimate to use"),
+        zbin_edges=Param(
+            list,
+            [],
+            msg="The tomographic redshift bin edges."
+            "If this is given (contains two or more entries), all settings below will be ignored.",
+        ),
         zmin=Param(float, 0.0, msg="Minimum redshift of the sample"),
         zmax=Param(float, 3.0, msg="Maximum redshift of the sample"),
         nbins=Param(int, 5, msg="Number of tomographic bins"),
         no_assign=Param(int, -99, msg="Value for no assignment flag"),
         )
     outputs = [('output', Hdf5Handle)]
     
@@ -60,24 +70,27 @@
         
         try:
             npdf = test_data.npdf
         except KeyError:
             raise KeyError(f"npdf is not a supported attribute of {type(test_data)}. Are you sure you don't mean to be using a qp ensemble?")
 
         # binning options
-        if len(self.config.zbin_edges)>=2:
+        if len(self.config.zbin_edges) >= 2:
             # this overwrites all other key words
             # linear binning defined by zmin, zmax, and nbins
             bin_index = np.digitize(zb, self.config.zbin_edges)
             # assign -99 to objects not in any bin:
             bin_index[bin_index==0]=self.config.no_assign
             bin_index[bin_index==len(self.config.zbin_edges)]=self.config.no_assign
         else:
             # linear binning defined by zmin, zmax, and nbins
-            bin_index = np.digitize(zb, np.linspace(self.config.zmin, self.config.zmax, self.config.nbins+1))
+            bin_index = np.digitize(
+                zb,
+                np.linspace(self.config.zmin, self.config.zmax, self.config.nbins + 1),
+            )
             # assign -99 to objects not in any bin:
             bin_index[bin_index==0]=self.config.no_assign
             bin_index[bin_index==(self.config.nbins+1)]=self.config.no_assign
         
         if self.config.id_name != "":
             # below is commented out and replaced by a redundant line
             # because the data doesn't have ID yet
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/algos/var_inf.py` & `pz-rail-base-0.2.2/src/rail/estimation/algos/var_inf.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 from scipy.special import digamma
 from scipy.stats import dirichlet
 from ceci.config import StageParameter as Param
 from rail.estimation.summarizer import PZSummarizer
 from rail.estimation.informer import PzInformer
 from rail.core.data import QPHandle
 
-TEENY = 1.e-15
+TEENY = 1.0e-15
 
 
 class VarInfStackInformer(PzInformer):
-    """Placeholder Informer
-    """
+    """Placeholder Informer"""
 
-    name = 'VarInfStackInformer'
+    name = "VarInfStackInformer"
     config_options = PzInformer.config_options.copy()
 
     def __init__(self, args, comm=None):
         PzInformer.__init__(self, args, comm=comm)
 
     def run(self):
-        self.add_data('model', np.array([None]))
+        self.add_data("model", np.array([None]))
 
 
 class VarInfStackSummarizer(PZSummarizer):
     """Variational inference summarizer based on notebook created by Markus Rau
     The summzarizer is appropriate for the likelihoods returned by
     template-based codes, for which the NaiveSummarizer are not appropriate.
 
@@ -43,81 +42,92 @@
       number of bins for redshift grid
     niter: int
       number of iterations to perform in the variational inference
     nsamples: int
       number of samples used in dirichlet to determind error bar
     """
 
-    name = 'VarInfStackSummarizer'
+    name = "VarInfStackSummarizer"
     config_options = PZSummarizer.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
-                          zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
-                          nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
-                          seed=Param(int, 87, msg="random seed"),
-                          niter=Param(int, 100, msg="The number of iterations in the variational inference"),
-                          nsamples=Param(int, 500, msg="The number of samples used in dirichlet uncertainty"))
-    inputs = [('input', QPHandle)]
-    outputs = [('output', QPHandle),
-               ('single_NZ', QPHandle)]
+    config_options.update(
+        zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
+        zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
+        nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
+        seed=Param(int, 87, msg="random seed"),
+        niter=Param(
+            int, 100, msg="The number of iterations in the variational inference"
+        ),
+        nsamples=Param(
+            int, 500, msg="The number of samples used in dirichlet uncertainty"
+        ),
+    )
+    inputs = [("input", QPHandle)]
+    outputs = [("output", QPHandle), ("single_NZ", QPHandle)]
 
     def __init__(self, args, comm=None):
         PZSummarizer.__init__(self, args, comm=comm)
         self.zgrid = None
 
     def run(self):
         # Redefining the chunk size so that all of the data is distributed at once in the
         # nodes. This would fill all the memory if not enough nodes are allocated
 
-        input_data = self.get_handle('input', allow_missing=True)
+        input_data = self.get_handle("input", allow_missing=True)
         try:
             self.config.hdf5_groupname
-        except:
+        except Exception:
             self.config.hdf5_groupname = None
         input_length = input_data.size(groupname=self.config.hdf5_groupname)
-        self.config.chunk_size = np.ceil(input_length/self.size)
-
+        self.config.chunk_size = np.ceil(input_length / self.size)
 
-        iterator = self.input_iterator('input')
+        iterator = self.input_iterator("input")
         self.zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins)
         first = True
         for s, e, test_data in iterator:
             print(f"Process {self.rank} running estimator on chunk {s} - {e}")
             alpha_trace = self._process_chunk(s, e, test_data, first)
             first = False
 
         if self.rank == 0:
             # old way of just spitting out a single distribution
             # qp_d = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=alpha_trace))
             # instead, sample and save the samples
             rng = np.random.default_rng(seed=self.config.seed)
-            sample_pz = dirichlet.rvs(alpha_trace, size=self.config.nsamples, random_state=rng)
-            qp_d = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=alpha_trace))
-
-            sample_ens = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=sample_pz))
-            self.add_data('output', sample_ens)
-            self.add_data('single_NZ', qp_d)
-
-
-    def  _process_chunk(self, start, end, test_data, first):
-        if not first: #pragma: no cover
-            raise ValueError(f"This algorithm needs all data in memory at once, increase nprocess or chunk size.")
+            sample_pz = dirichlet.rvs(
+                alpha_trace, size=self.config.nsamples, random_state=rng
+            )
+            qp_d = qp.Ensemble(
+                qp.interp, data=dict(xvals=self.zgrid, yvals=alpha_trace)
+            )
+
+            sample_ens = qp.Ensemble(
+                qp.interp, data=dict(xvals=self.zgrid, yvals=sample_pz)
+            )
+            self.add_data("output", sample_ens)
+            self.add_data("single_NZ", qp_d)
+
+    def _process_chunk(self, _start, _end, test_data, first):
+        if not first:  # pragma: no cover
+            raise ValueError(
+                "This algorithm needs all data in memory at once, increase nprocess or chunk size."
+            )
 
         # Initiallizing arrays
         alpha_trace = np.ones(len(self.zgrid))
         init_trace = np.ones(len(self.zgrid))
         pdf_vals = test_data.pdf(self.zgrid)
         log_pdf_vals = np.log(np.array(pdf_vals) + TEENY)
         for _ in range(self.config.niter):
-            dig = np.array([digamma(kk) - digamma(np.sum(alpha_trace)) for kk in alpha_trace])
+            dig = np.array(
+                [digamma(kk) - digamma(np.sum(alpha_trace)) for kk in alpha_trace]
+            )
             matrix_grid = np.exp(dig + log_pdf_vals)
             gamma_matrix = np.array([kk / np.sum(kk) for kk in matrix_grid])
             for kk in matrix_grid:
                 break
             nk_partial = np.sum(gamma_matrix, axis=0)
             if self.comm is not None:  # pragma: no cover
                 nk = self.comm.allreduce(nk_partial)
             else:
                 nk = nk_partial
             alpha_trace = nk + init_trace
-        return(alpha_trace)
-
-
+        return alpha_trace
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/classifier.py` & `pz-rail-base-0.2.2/src/rail/estimation/classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,39 @@
 """
 
 import gc
 from rail.core.data import QPHandle, TableHandle, ModelHandle, Hdf5Handle
 from rail.core.stage import RailStage
 
 
-class CatClassifier(RailStage):  #pragma: no cover
+class CatClassifier(RailStage):  # pragma: no cover
     """The base class for assigning classes to catalogue-like table.
 
     Classifier uses a generic "model", the details of which depends on the sub-class.
 
     CatClassifier take as "input" a catalogue-like table, assign each object into
-    a tomographic bin, and provide as "output" a tabular data which can be appended 
+    a tomographic bin, and provide as "output" a tabular data which can be appended
     to the catalogue.
     """
-    
-    name='CatClassifier'
+
+    name = "CatClassifier"
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=10000, hdf5_groupname=str)
-    inputs = [('model', ModelHandle),
-              ('input', TableHandle)]
-    outputs = [('output', TableHandle)]
-    
+    inputs = [("model", ModelHandle), ("input", TableHandle)]
+    outputs = [("output", TableHandle)]
+
     def __init__(self, args, comm=None):
         """Initialize Classifier"""
         RailStage.__init__(self, args, comm=comm)
         self._output_handle = None
         self.model = None
-        if not isinstance(args, dict):  #pragma: no cover
+        if not isinstance(args, dict):  # pragma: no cover
             args = vars(args)
         self.open_model(**args)
-        
-    
+
     def open_model(self, **kwargs):
         """Load the model and/or attach it to this Classifier
 
         Parameters
         ----------
         model : `object`, `str` or `ModelHandle`
             Either an object with a trained model,
@@ -45,29 +43,28 @@
             or a `ModelHandle` providing access to the trained model.
 
         Returns
         -------
         self.model : `object`
             The object encapsulating the trained model.
         """
-        model = kwargs.get('model', None)
-        if model is None or model == 'None':
+        model = kwargs.get("model", None)
+        if model is None or model == "None":
             self.model = None
             return self.model
         if isinstance(model, str):
-            self.model = self.set_data('model', data=None, path=model)
-            self.config['model'] = model
+            self.model = self.set_data("model", data=None, path=model)
+            self.config["model"] = model
             return self.model
         if isinstance(model, ModelHandle):
             if model.has_path:
-                self.config['model'] = model.path
-        self.model = self.set_data('model', model)
+                self.config["model"] = model.path
+        self.model = self.set_data("model", model)
         return self.model
-        
-        
+
     def classify(self, input_data):
         """The main run method for the classifier, should be implemented
         in the specific subclass.
 
         This will attach the input_data to this `CatClassifier`
         (for introspection and provenance tracking).
 
@@ -85,21 +82,20 @@
             A dictionary of all input data
 
         Returns
         -------
         output: `dict`
             Class assignment for each galaxy.
         """
-        self.set_data('input', input_data)
+        self.set_data("input", input_data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
-    
+        return self.get_handle("output")
+
 
-    
 class PZClassifier(RailStage):
     """The base class for assigning classes (tomographic bins) to per-galaxy PZ 
     estimates.
 
     PZClassifier takes as "input" a `qp.Ensemble` with per-galaxy PDFs, and
     provides as "output" tabular data which can be appended to the catalogue.
     """
@@ -151,15 +147,15 @@
 
         Returns
         -------
         output: `dict`
             Class assignment for each galaxy, typically in the form of a 
             dictionary with IDs and class labels.
         """
-        self.set_data('input', input_data)
+        self.set_data("input", input_data)
         self.run()
         self.finalize()
         return self.get_handle('output')
     
 
     def _finalize_run(self):
         """Finalize the classification process after processing all chunks."""
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/estimator.py` & `pz-rail-base-0.2.2/src/rail/estimation/estimator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 """
 import gc
 
 from rail.core.common_params import SHARED_PARAMS
 from rail.core.data import TableHandle, QPHandle, ModelHandle
 from rail.core.stage import RailStage
 
-from rail.estimation.informer import CatInformer
 from rail.core.point_estimation import PointEstimationMixin
-# for backwards compatibility
+
+# for backwards compatibility, to avoid break stuff that imports it from here
+from rail.estimation.informer import CatInformer  # pylint: disable=unused-import
 
 
 class CatEstimator(RailStage, PointEstimationMixin):
     """The base class for making photo-z posterior estimates from catalog-like inputs
     (i.e., tables with fluxes in photometric bands among the set of columns)
 
     Estimators use a generic "model", the details of which depends on the sub-class.
 
     Estimators take as "input" tabular data, apply the photo-z estimation and
     provide as "output" a ``QPEnsemble``, with per-object p(z).
 
     """
 
-    name = 'CatEstimator'
+    name = "CatEstimator"
     config_options = RailStage.config_options.copy()
     config_options.update(
         chunk_size=10000,
-        hdf5_groupname=SHARED_PARAMS['hdf5_groupname'],
-        calculated_point_estimates=SHARED_PARAMS['calculated_point_estimates'])
-    inputs = [('model', ModelHandle),
-              ('input', TableHandle)]
-    outputs = [('output', QPHandle)]
+        hdf5_groupname=SHARED_PARAMS["hdf5_groupname"],
+        calculated_point_estimates=SHARED_PARAMS["calculated_point_estimates"],
+    )
+    inputs = [("model", ModelHandle), ("input", TableHandle)]
+    outputs = [("output", QPHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Estimator"""
         RailStage.__init__(self, args, comm=comm)
         self._output_handle = None
         self.model = None
 
@@ -50,26 +51,26 @@
             providing access to the trained model.
 
         Returns
         -------
         self.model : ``object``
             The object encapsulating the trained model.
         """
-        model = kwargs.get('model', None)
-        if model is None or model == 'None':
+        model = kwargs.get("model", None)
+        if model is None or model == "None":
             self.model = None
             return self.model
         if isinstance(model, str):
-            self.model = self.set_data('model', data=None, path=model)
-            self.config['model'] = model
+            self.model = self.set_data("model", data=None, path=model)
+            self.config["model"] = model
             return self.model
         if isinstance(model, ModelHandle):
             if model.has_path:
-                self.config['model'] = model.path
-        self.model = self.set_data('model', model)
+                self.config["model"] = model.path
+        self.model = self.set_data("model", model)
         return self.model
 
     def estimate(self, input_data):
         """The main interface method for the photo-z estimation
 
         This will attach the input data (defined in ``inputs`` as "input") to this
         ``Estimator`` (for introspection and provenance tracking). Then call the
@@ -88,24 +89,23 @@
             access to the same
 
         Returns
         -------
         output: ``QPHandle``
             Handle providing access to QP ensemble with output data
         """
-        self.set_data('input', input_data)
+        self.set_data("input", input_data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
 
     def run(self):
-
         self.open_model(**self.config)
 
-        iterator = self.input_iterator('input')
+        iterator = self.input_iterator("input")
         first = True
         self._initialize_run()
         self._output_handle = None
         for s, e, test_data in iterator:
             print(f"Process {self.rank} running estimator on chunk {s} - {e}")
             self._process_chunk(s, e, test_data, first)
             first = False
@@ -117,16 +117,20 @@
     def _initialize_run(self):
         self._output_handle = None
 
     def _finalize_run(self):
         self._output_handle.finalize_write()
 
     def _process_chunk(self, start, end, data, first):
-        raise NotImplementedError(f"{self.name}._process_chunk is not implemented")  # pragma: no cover
+        raise NotImplementedError(
+            f"{self.name}._process_chunk is not implemented"
+        )  # pragma: no cover
 
     def _do_chunk_output(self, qp_dstn, start, end, first):
         qp_dstn = self.calculate_point_estimates(qp_dstn)
         if first:
-            self._output_handle = self.add_handle('output', data=qp_dstn)
-            self._output_handle.initialize_write(self._input_length, communicator=self.comm)
+            self._output_handle = self.add_handle("output", data=qp_dstn)
+            self._output_handle.initialize_write(
+                self._input_length, communicator=self.comm
+            )
         self._output_handle.set_data(qp_dstn, partial=True)
         self._output_handle.write_chunk(start, end)
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/informer.py` & `pz-rail-base-0.2.2/src/rail/estimation/informer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 They are distinguished by their input data types, and the models they output can
 be used for their corresponding Estimator, Summarizer, or Classifier stages.
 """
 
 from rail.core.data import TableHandle, QPHandle, ModelHandle
 from rail.core.stage import RailStage
 
+
 class CatInformer(RailStage):
-    """The base class for informing models used to make photo-z data products  
+    """The base class for informing models used to make photo-z data products
     from catalog-like inputs (i.e., tables with fluxes in photometric bands among
     the set of columns).
 
     Estimators use a generic "model", the details of which depends on the sub-class.
     Most estimators will have associated Informer classes, which can be used to inform
     those models.
 
@@ -22,21 +23,21 @@
     are template-based rather than machine learning-based.)
 
     Informer will produce as output a generic "model", the details of which depends on the sub-class.
 
     They take as "input" catalog-like tabular data, which is used to "inform" the model.
     """
 
-    name = 'CatInformer'
+    name = "CatInformer"
     config_options = RailStage.config_options.copy()
-    inputs = [('input', TableHandle)]
-    outputs = [('model', ModelHandle)]
+    inputs = [("input", TableHandle)]
+    outputs = [("model", ModelHandle)]
 
     def __init__(self, args, comm=None):
-        """Initialize Informer that can inform models for redshift estimation """
+        """Initialize Informer that can inform models for redshift estimation"""
         RailStage.__init__(self, args, comm=comm)
         self.model = None
 
     def inform(self, training_data):
         """The main interface method for Informers
 
         This will attach the input_data to this `Informer`
@@ -56,18 +57,19 @@
             dictionary of all input data, or a `TableHandle` providing access to it
 
         Returns
         -------
         model : ModelHandle
             Handle providing access to trained model
         """
-        self.set_data('input', training_data)
+        self.set_data("input", training_data)
         self.run()
         self.finalize()
-        return self.get_handle('model')
+        return self.get_handle("model")
+
 
 class PzInformer(RailStage):
     """The base class for informing models used to make photo-z data products from
     existing ensembles of p(z) distributions.
 
     PzSummarizers can use a generic "model", the details of which depends on the sub-class.
     Some summaer will have associated PzInformer classes, which can be used to inform
@@ -77,21 +79,21 @@
     are template-based rather than machine learning-based.)
 
     PzInformer will produce as output a generic "model", the details of which depends on the sub-class.
 
     They take as "input" a qp.Ensemble of per-galaxy p(z) data, which is used to "inform" the model.
     """
 
-    name = 'PzInformer'
+    name = "PzInformer"
     config_options = RailStage.config_options.copy()
-    inputs = [('input', QPHandle)]
-    outputs = [('model', ModelHandle)]
+    inputs = [("input", QPHandle)]
+    outputs = [("model", ModelHandle)]
 
     def __init__(self, args, comm=None):
-        """Initialize Informer that can inform models for redshift estimation """
+        """Initialize Informer that can inform models for redshift estimation"""
         RailStage.__init__(self, args, comm=comm)
         self.model = None
 
     def inform(self, training_data):
         """The main interface method for Informers
 
         This will attach the input_data to this `Informer`
@@ -111,11 +113,11 @@
             Per-galaxy p(z), and any ancilary data associated with it
 
         Returns
         -------
         model : ModelHandle
             Handle providing access to trained model
         """
-        self.set_data('input', training_data)
+        self.set_data("input", training_data)
         self.run()
         self.finalize()
-        return self.get_handle('model')
+        return self.get_handle("model")
```

### Comparing `pz-rail-base-0.2.1/src/rail/estimation/summarizer.py` & `pz-rail-base-0.2.2/src/rail/estimation/summarizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Abstract base classes defining Summarizers of the redshift distribution of an ensemble of galaxies
 """
+import numpy as np
+
 from rail.core.data import QPHandle, TableHandle, ModelHandle
 from rail.core.stage import RailStage
 
-from rail.estimation.informer import PzInformer
 # for backwards compatibility
 
 
 class CatSummarizer(RailStage):
     """The base class for classes that go from catalog-like tables
     to ensemble NZ estimates.
 
     CatSummarizer take as "input" a catalog-like table.  I.e., a
     table with fluxes in photometric bands among the set of columns.
 
     provide as "output" a QPEnsemble, with per-ensemble n(z).
     """
 
-    name = 'CatSummarizer'
+    name = "CatSummarizer"
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=10000)
-    inputs = [('input', TableHandle)]
-    outputs = [('output', QPHandle)]
+    inputs = [("input", TableHandle)]
+    outputs = [("output", QPHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Summarizer"""
         RailStage.__init__(self, args, comm=comm)
 
     def summarize(self, input_data):
         """The main run method for the summarization, should be implemented
@@ -49,33 +50,32 @@
             Either a dictionary of all input data or a `ModelHandle` providing access to the same
 
         Returns
         -------
         output: `qp.Ensemble`
             Ensemble with n(z), and any ancilary data
         """
-        self.set_data('input', input_data)
+        self.set_data("input", input_data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
 
 
 class PZSummarizer(RailStage):
     """The base class for classes that go from per-galaxy PZ estimates to ensemble NZ estimates
 
     PZSummarizer take as "input" a `qp.Ensemble` with per-galaxy PDFs, and
     provide as "output" a QPEnsemble, with per-ensemble n(z).
     """
 
-    name = 'PZtoNZSummarizer'
+    name = "PZtoNZSummarizer"
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=10000)
-    inputs = [('model', ModelHandle),
-              ('input', QPHandle)]
-    outputs = [('output', QPHandle)]
+    inputs = [("model", ModelHandle), ("input", QPHandle)]
+    outputs = [("output", QPHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Estimator that can sample galaxy data."""
         RailStage.__init__(self, args, comm=comm)
 
     def summarize(self, input_data):
         """The main run method for the summarization, should be implemented
@@ -98,51 +98,55 @@
             Per-galaxy p(z), and any ancilary data associated with it
 
         Returns
         -------
         output: `qp.Ensemble`
             Ensemble with n(z), and any ancilary data
         """
-        self.set_data('input', input_data)
+        self.set_data("input", input_data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
-
+        return self.get_handle("output")
 
     def _broadcast_bootstrap_matrix(self):
-        import numpy as np
         rng = np.random.default_rng(seed=self.config.seed)
         # Only one of the nodes needs to produce the bootstrap indices
         ngal = self._input_length
         if self.rank == 0:
-            bootstrap_matrix = rng.integers(low=0, high=ngal, size=(ngal,self.config.nsamples))
+            bootstrap_matrix = rng.integers(
+                low=0, high=ngal, size=(ngal, self.config.nsamples)
+            )
         else:  # pragma: no cover
             bootstrap_matrix = None
         if self.comm is not None:  # pragma: no cover
             self.comm.Barrier()
-            bootstrap_matrix = self.comm.bcast(bootstrap_matrix, root = 0)
+            bootstrap_matrix = self.comm.bcast(bootstrap_matrix, root=0)
         return bootstrap_matrix
 
-    def _join_histograms(self, bvals, yvals):#pragma: no cover
+    def _join_histograms(self, bvals, yvals):  # pragma: no cover
         bvals_r = self.comm.reduce(bvals)
         yvals_r = self.comm.reduce(yvals)
-        return(bvals_r, yvals_r)
+        return (bvals_r, yvals_r)
+
 
 class SZPZSummarizer(RailStage):
     """The base class for classes that use two sets of data: a photometry sample with
     spec-z values, and a photometry sample with unknown redshifts, e.g. minisom_som and
     outputs a QP Ensemble with bootstrap realization of the N(z) distribution
     """
-    name = 'SZPZtoNZSummarizer'
+
+    name = "SZPZtoNZSummarizer"
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=10000)
-    inputs = [('input', TableHandle),
-              ('spec_input', TableHandle),
-              ('model', ModelHandle)]
-    outputs = [('output', QPHandle)]
+    inputs = [
+        ("input", TableHandle),
+        ("spec_input", TableHandle),
+        ("model", ModelHandle),
+    ]
+    outputs = [("output", QPHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Estimator that can sample galaxy data."""
         RailStage.__init__(self, args, comm=comm)
         self.model = None
         # NOTE: open model removed from init, need to put an
         # `open_model` call explicitly in the run method for
@@ -160,26 +164,26 @@
         can be read to obtain the trained model, or a `ModelHandle` providing access to the trained model.
 
         Returns
         -------
         self.model : `object`
             The object encapsulating the trained model.
         """
-        model = kwargs.get('model', None)
-        if model is None or model == 'None':  # pragma: no cover
+        model = kwargs.get("model", None)
+        if model is None or model == "None":  # pragma: no cover
             self.model = None
             return self.model
         if isinstance(model, str):
-            self.model = self.set_data('model', data=None, path=model)
-            self.config['model'] = model
+            self.model = self.set_data("model", data=None, path=model)
+            self.config["model"] = model
             return self.model
         if isinstance(model, ModelHandle):
             if model.has_path:
-                self.config['model'] = model.path
-        self.model = self.set_data('model', model)
+                self.config["model"] = model.path
+        self.model = self.set_data("model", model)
         return self.model
 
     def summarize(self, input_data, spec_data):
         """The main run method for the summarization, should be implemented
         in the specific subclass.
 
         This will attach the input_data to this `SZandPhottoNZSummarizer`
@@ -199,12 +203,12 @@
             Per-galaxy p(z), and any ancilary data associated with it
 
         Returns
         -------
         output: `qp.Ensemble`
             Ensemble with n(z), and any ancilary data
         """
-        self.set_data('input', input_data)
-        self.set_data('spec_input', spec_data)
+        self.set_data("input", input_data)
+        self.set_data("spec_input", spec_data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
+        return self.get_handle("output")
```

### Comparing `pz-rail-base-0.2.1/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.2.2/src/rail/evaluation/metrics/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 class MetricEvaluator:
-    """ A superclass for metrics evaluations"""
+    """A superclass for metrics evaluations"""
+
     def __init__(self, qp_ens):
         """Class constructor.
         Parameters
         ----------
         qp_ens: qp.Ensemble object
             PDFs as qp.Ensemble
         """
         self._qp_ens = qp_ens
 
-    def evaluate(self):  #pragma: no cover
+    def evaluate(self):  # pragma: no cover
         """
         Evaluates the metric a function of the truth and prediction
 
         Returns
         -------
         metric: dictionary
             value of the metric and statistics thereof
```

### Comparing `pz-rail-base-0.2.1/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.2.2/src/rail/evaluation/metrics/cdeloss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
-from .base import MetricEvaluator
 from rail.evaluation.stats_groups import stat_and_pval
+from .base import MetricEvaluator
 
 
 class CDELoss(MetricEvaluator):
-    """ Conditional density loss """
+    """Conditional density loss"""
+
     def __init__(self, qp_ens, zgrid, ztrue):
         """Class constructor"""
         super().__init__(qp_ens)
 
         self._pdfs = qp_ens.pdf(zgrid)
         self._xvals = zgrid
         self._ztrue = ztrue
@@ -19,14 +20,14 @@
         Izbicki & Lee 2017 (arXiv:1704.08095).
 
         Notes
         -----
         """
 
         # Calculate first term E[\int f*(z | X)^2 dz]
-        term1 = np.mean(np.trapz(self._pdfs ** 2, x=self._xvals))
+        term1 = np.mean(np.trapz(self._pdfs**2, x=self._xvals))
         # z bin closest to ztrue
         nns = [np.argmin(np.abs(self._xvals - z)) for z in self._ztrue]
         # Calculate second term E[f*(Z | X)]
         term2 = np.mean(self._pdfs[range(self._npdf), nns])
         cdeloss = term1 - 2 * term2
         return stat_and_pval(cdeloss, np.nan)
```

### Comparing `pz-rail-base-0.2.1/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.2.2/src/rail/evaluation/metrics/pointestimates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 
 from .base import MetricEvaluator
 
+
 class PointStatsEz(MetricEvaluator):
     """Copied from PZDC1paper repo. Adapted to remove the cut based on
     magnitude."""
 
     def __init__(self, pzvec, szvec):
         """ An object that takes in the vectors of the point photo-z
         the spec-z, and the i-band magnitudes for calculating the
@@ -22,15 +23,15 @@
             Array of the point photo-z values
         szvec : ndarray
             array of the spec-z values
         """
         super().__init__(None)
         self.pzs = pzvec
         self.szs = szvec
-        ez = (pzvec - szvec) / (1. + szvec)
+        ez = (pzvec - szvec) / (1.0 + szvec)
         self.ez = ez
 
     def evaluate(self):
         """Return the ez values"""
         return self.ez
 
 
@@ -41,25 +42,26 @@
         """Calculate the width of the e_z distribution
         using the Interquartile range
 
         Returns
         -------
         ``sigma_IQR`` float. Width of ez distribution for full sample
         """
-        x75, x25 = np.percentile(self.ez, [75., 25.])
+        x75, x25 = np.percentile(self.ez, [75.0, 25.0])
         iqr = x75 - x25
         sigma_iqr = iqr / 1.349
         return sigma_iqr
 
 
 class PointBias(PointStatsEz):
     """calculates the bias of the ez and ez_magcut samples.
 
     In keeping with the Science Book, this is just the median of the ez values
     """
+
     def evaluate(self):
         """
         Returns
         -------
         ``bias`` ndarray. Median of the full ez sample
         """
         return np.median(self.ez)
```

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.hdf5` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.2.2/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/src/rail/stages/__init__.py` & `pz-rail-base-0.2.2/src/rail/stages/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import rail
 from rail.core import RailEnv
 
 from rail.estimation.estimator import *
 from rail.estimation.classifier import *
 from rail.estimation.summarizer import *
 from rail.estimation.algos.naive_stack import *
@@ -16,19 +15,20 @@
 
 from rail.creation.degrader import *
 #from rail.creation.degradation.spectroscopic_degraders import *
 # from rail.creation.degradation.spectroscopic_selections import *
 from rail.creation.degradation.quantityCut import *
 
 from rail.creation.engine import *
-#from rail.creation.engines.flowEngine import *
-#from rail.creation.engines.galaxy_population_components import *
-#from rail.creation.engines.dsps_photometry_creator import *
-#from rail.creation.engines.dsps_sed_modeler import *
 
-from rail.evaluation.evaluator import Evaluator
+# from rail.creation.engines.flowEngine import *
+# from rail.creation.engines.galaxy_population_components import *
+# from rail.creation.engines.dsps_photometry_creator import *
+# from rail.creation.engines.dsps_sed_modeler import *
+
+# from rail.evaluation.evaluator import Evaluator
 
 
 def import_and_attach_all():
     """Import all the packages in the rail ecosystem and attach them to this module"""
     RailEnv.import_all_packages()
     RailEnv.attach_stages(rail.stages)
```

### Comparing `pz-rail-base-0.2.1/tests/cli/hello_world.ipynb` & `pz-rail-base-0.2.2/tests/cli/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/tests/cli/single_number.ipynb` & `pz-rail-base-0.2.2/tests/cli/single_number.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/tests/cli/test_scripts.py` & `pz-rail-base-0.2.2/tests/cli/test_scripts.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,34 @@
 import os
 from rail.cli import scripts
 from rail.cli.options import GitMode
 
 
 def test_render_nb():
     nb_dir = "./tests/cli/"
-    nb_files = glob.glob(os.path.join(nb_dir,'*.ipynb'))
-    scripts.render_nb('docs', False, True, nb_files, skip=[])
-    scripts.render_nb('docs', True, True, nb_files, skip=["./tests/cli/single_number.ipynb"])
-    scripts.render_nb('docs', True, False, nb_files, skip=["./tests/cli/single_number.ipynb"])
+    nb_files = glob.glob(os.path.join(nb_dir, "*.ipynb"))
+    scripts.render_nb("docs", False, True, nb_files, skip=[])
+    scripts.render_nb(
+        "docs", True, True, nb_files, skip=["./tests/cli/single_number.ipynb"]
+    )
+    scripts.render_nb(
+        "docs", True, False, nb_files, skip=["./tests/cli/single_number.ipynb"]
+    )
 
 
 def test_clone_source():
-    scripts.clone_source('..', GitMode.ssh, True, 'rail_packages.yml')
-    scripts.clone_source('..', GitMode.https, True, 'rail_packages.yml')
-    scripts.clone_source('..', GitMode.cli, True, 'rail_packages.yml')
+    scripts.clone_source("..", GitMode.ssh, True, "rail_packages.yml")
+    scripts.clone_source("..", GitMode.https, True, "rail_packages.yml")
+    scripts.clone_source("..", GitMode.cli, True, "rail_packages.yml")
+
 
-    
 def test_update_source():
-    scripts.update_source('..', True, 'rail_packages.yml')
+    scripts.update_source("..", True, "rail_packages.yml")
 
 
 def test_install():
-    scripts.install('..', False, True, 'rail_packages.yml')
-    scripts.install('..', True, True, 'rail_packages.yml')
+    scripts.install("..", False, True, "rail_packages.yml")
+    scripts.install("..", True, True, "rail_packages.yml")
 
 
 def test_info():
     scripts.info(print_all=True)
```

### Comparing `pz-rail-base-0.2.1/tests/core/test_core.py` & `pz-rail-base-0.2.2/tests/core/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,283 @@
 import os
 import pickle
 from types import GeneratorType
 
 import numpy as np
-import pandas as pd
 import pytest
-import tempfile
 
-import rail
-from rail.core.common_params import SHARED_PARAMS, copy_param, set_param_default
+from rail.core.common_params import copy_param, set_param_default
 from rail.core.data import (
     DataHandle,
     DataStore,
     FitsHandle,
     Hdf5Handle,
     ModelHandle,
     PqHandle,
     QPHandle,
+    QPOrTableHandle,
     TableHandle,
 )
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.core.utils import RAILDIR, find_rail_file
 from rail.core.util_stages import (
     ColumnMapper,
     RowSelector,
     TableConverter,
 )
-    
+
 
 # def test_data_file():
 #    with pytest.raises(ValueError) as errinfo:
 #        df = DataFile('dummy', 'x')
 
+def test_find_rail_file():
+    afile = find_rail_file(os.path.join("examples_data", "testdata", "test_dc2_training_9816.pq"))
+    assert afile
+    with pytest.raises(ValueError):
+        _not_a_file = find_rail_file("not_a_file")
+
 
 def test_util_stages():
     DS = RailStage.data_store
     DS.clear()
-    datapath = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq")
-    
-    data = DS.read_file('data', TableHandle, datapath)
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq"
+    )
+
+    data = DS.read_file("data", TableHandle, datapath)
 
     table_conv = TableConverter.make_stage(name="conv", output_format="numpyDict")
     col_map = ColumnMapper.make_stage(name="col_map", columns={})
     row_sel = RowSelector.make_stage(name="row_sel", start=1, stop=15)
 
-    with pytest.raises(KeyError) as errinfo:
+    with pytest.raises(KeyError) as _errinfo:
         table_conv.get_handle("nope", allow_missing=False)
 
-    conv_data = table_conv(data)
+    _conv_data = table_conv(data)
     mapped_data = col_map(data)
-    sel_data = row_sel(mapped_data)
+    _sel_data = row_sel(mapped_data)
 
     row_sel_2 = RowSelector.make_stage(name="row_sel_2", start=1, stop=15)
     row_sel_2.set_data("input", mapped_data.data)
     handle = row_sel_2.get_handle("input")
 
-    row_sel_3 = RowSelector.make_stage(name="row_sel_3", input=handle.path, start=1, stop=15)
+    row_sel_3 = RowSelector.make_stage(
+        name="row_sel_3", input=handle.path, start=1, stop=15
+    )
     row_sel_3.set_data("input", None, do_read=True)
 
-    
+
 def do_data_handle(datapath, handle_class):
-    DS = RailStage.data_store
+    _DS = RailStage.data_store
 
     th = handle_class("data", path=datapath)
 
-    with pytest.raises(ValueError) as errinfo:
+    with pytest.raises(ValueError) as _errinfo:
         th.write()
 
     assert not th.has_data
-    with pytest.raises(ValueError) as errinfo:
+    check_size = th.size()
+    if check_size == 0:
+        print(f"Warning, failed to read size from {datapath}")
+    
+    with pytest.raises(ValueError) as _errinfo:
         th.write_chunk(0, 1)
     assert th.has_path
     assert th.is_written
     data = th.read()
     data2 = th.read()
 
     assert data is data2
     assert th.has_data
     assert th.make_name("data") == f"data.{handle_class.suffix}"
 
     th2 = handle_class("data2", data=data)
     assert th2.has_data
+    assert th2.size() > 0
+    
     assert not th2.has_path
     assert not th2.is_written
-    with pytest.raises(ValueError) as errinfo:
+    with pytest.raises(ValueError) as _errinfo:
         th2.open()
-    with pytest.raises(ValueError) as errinfo:
+    with pytest.raises(ValueError) as _errinfo:
         th2.write()
-    with pytest.raises(ValueError) as errinfo:
+    with pytest.raises(ValueError) as _errinfo:
         th2.write_chunk(0, 1)
 
     assert th2.make_name("data2") == f"data2.{handle_class.suffix}"
     assert str(th)
     assert str(th2)
     return th
 
 
 def test_pq_handle():
-    datapath = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq")
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq"
+    )
     handle = do_data_handle(datapath, PqHandle)
     pqfile = handle.open()
     assert pqfile
     assert handle.fileObj is not None
     handle.close()
     assert handle.fileObj is None
 
 
 def test_qp_handle():
-    datapath = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "output_BPZ_lite.hdf5")
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "output_BPZ_lite.hdf5"
+    )
     handle = do_data_handle(datapath, QPHandle)
     qpfile = handle.open()
     assert qpfile
     assert handle.fileObj is not None
     handle.close()
     assert handle.fileObj is None
 
-    with pytest.raises(TypeError) as errInfo:
-        bad_dh = QPHandle(data="this is not an Ensemble")
+    with pytest.raises(TypeError) as _errInfo:
+        _bad_dh = QPHandle(tag="bad_tag", data="this is not an Ensemble")
+
+
+def test_qp_or_table_handle_qp():
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "output_BPZ_lite.hdf5"
+    )
+    handle = do_data_handle(datapath, QPOrTableHandle)
+    qpfile = handle.open()
+    assert qpfile
+    assert handle.fileObj is not None
+    handle.close()
+    assert handle.fileObj is None
+    
+    x = handle.iterator(chunk_size=100)
+
+    assert isinstance(x, GeneratorType)
+    for i, xx in enumerate(x):
+        assert xx[0] == i * 100
+        assert xx[1] - xx[0] <= 100
+
+
+    handle2 = QPOrTableHandle(tag='qp_or_table_qp_2', path=datapath)
+    
+    x2 = handle2.iterator(chunk_size=100)
+
+    assert isinstance(x2, GeneratorType)
+    for i2, xx2 in enumerate(x2):
+        assert xx2[0] == i2 * 100
+        assert xx2[1] - xx2[0] <= 100
+
+        
+
+def test_qp_or_table_handle_table():
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5"
+    )
+    handle = do_data_handle(datapath, QPOrTableHandle)
+    tablefile = handle.open()
+    assert tablefile
+    assert handle.fileObj is not None
+    handle.close()
+    assert handle.fileObj is None
+    
+    x = handle.iterator(chunk_size=100)
+
+    assert isinstance(x, GeneratorType)
+    for i, xx in enumerate(x):
+        assert xx[0] == i * 100
+        assert xx[1] - xx[0] <= 100
+        
+    handle2 = QPOrTableHandle(tag='qp_or_table_table_2', path=datapath)
+    
+    x2 = handle2.iterator(groupname='photometry', chunk_size=100)
+
+    assert isinstance(x2, GeneratorType)
+    for i2, xx2 in enumerate(x2):
+        assert xx2[0] == i2 * 100
+        assert xx2[1] - xx2[0] <= 100
 
 
 def test_hdf5_handle():
-    datapath = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5")
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5"
+    )
     handle = do_data_handle(datapath, Hdf5Handle)
     with handle.open(mode="r") as f:
         assert f
         assert handle.fileObj is not None
     datapath_chunked = os.path.join(
-      RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816_chunked.hdf5"
+        RAILDIR,
+        "rail",
+        "examples_data",
+        "testdata",
+        "test_dc2_training_9816_chunked.hdf5",
     )
     handle_chunked = Hdf5Handle("chunked", handle.data, path=datapath_chunked)
-    from tables_io.arrayUtils import getGroupInputDataLength, getInitializationForODict, sliceDict
+    from tables_io.arrayUtils import (  # pylint: disable=import-outside-toplevel
+        getInitializationForODict,
+        sliceDict,
+    )
 
     num_rows = len(handle.data["photometry"]["id"])
     check_num_rows = len(handle()["photometry"]["id"])
     assert num_rows == check_num_rows
     chunk_size = 1000
     data = handle.data["photometry"]
     init_dict = getInitializationForODict(data)
     with handle_chunked.open(mode="w") as fout:
         for k, v in init_dict.items():
             fout.create_dataset(k, v[0], v[1])
         for i in range(0, num_rows, chunk_size):
             start = i
             end = i + chunk_size
-            if end > num_rows:
-                end = num_rows
-            handle_chunked.set_data(sliceDict(handle.data["photometry"], slice(start, end)), partial=True)
+            end = min(end, num_rows)
+            handle_chunked.set_data(
+                sliceDict(handle.data["photometry"], slice(start, end)), partial=True
+            )
             handle_chunked.write_chunk(start, end)
     write_size = handle_chunked.size()
     assert len(handle_chunked.data) <= 1000
     data_called = handle_chunked()
     assert len(data_called["id"]) == write_size
     read_chunked = Hdf5Handle("read_chunked", None, path=datapath_chunked)
     data_check = read_chunked.read()
     assert np.allclose(data["id"], data_check["id"])
     assert np.allclose(data_called["id"], data_check["id"])
     os.remove(datapath_chunked)
 
 
 def test_fits_handle():
-    datapath = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "output_BPZ_lite.fits")
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "output_BPZ_lite.fits"
+    )
     handle = do_data_handle(datapath, FitsHandle)
     fitsfile = handle.open()
     assert fitsfile
     assert handle.fileObj is not None
     handle.close()
     assert handle.fileObj is None
 
 
 def test_model_handle():
     DS = RailStage.data_store
     DS.clear()
-    model_path = os.path.join(RAILDIR, "rail", "examples_data", "estimation_data", "data", "CWW_HDFN_prior.pkl")
+    model_path = os.path.join(
+        RAILDIR,
+        "rail",
+        "examples_data",
+        "estimation_data",
+        "data",
+        "CWW_HDFN_prior.pkl",
+    )
     model_path_copy = os.path.join(
-        RAILDIR, "rail", "examples_data", "estimation_data", "data", "CWW_HDFN_prior_copy.pkl"
+        RAILDIR,
+        "rail",
+        "examples_data",
+        "estimation_data",
+        "data",
+        "CWW_HDFN_prior_copy.pkl",
     )
     mh = ModelHandle("model", path=model_path)
     mh2 = ModelHandle("model2", path=model_path)
 
     model1 = mh.read()
     model2 = mh2.read()
 
@@ -191,50 +291,61 @@
         pickle.dump(obj=mh3.data, file=fout, protocol=pickle.HIGHEST_PROTOCOL)
     os.remove(model_path_copy)
 
 
 def test_data_hdf5_iter():
     DS = RailStage.data_store
     DS.clear()
-    
-    datapath = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5")
+
+    datapath = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5"
+    )
 
     # data = DS.read_file('data', TableHandle, datapath)
     th = Hdf5Handle("data", path=datapath)
     x = th.iterator(groupname="photometry", chunk_size=1000)
 
     assert isinstance(x, GeneratorType)
     for i, xx in enumerate(x):
         assert xx[0] == i * 1000
         assert xx[1] - xx[0] <= 1000
 
-    data = DS.read_file("input", TableHandle, datapath)
+    _data = DS.read_file("input", TableHandle, datapath)
     cm = ColumnMapper.make_stage(
-        input=datapath, chunk_size=1000, hdf5_groupname="photometry", columns=dict(id="bob")
+        input=datapath,
+        chunk_size=1000,
+        hdf5_groupname="photometry",
+        columns=dict(id="bob"),
     )
     x = cm.input_iterator("input")
 
     assert isinstance(x, GeneratorType)
 
     for i, xx in enumerate(x):
         assert xx[0] == i * 1000
         assert xx[1] - xx[0] <= 1000
 
 
 def test_data_store():
     DS = RailStage.data_store
     DS.clear()
     DS.__class__.allow_overwrite = False
-    
-    datapath_hdf5 = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5")
-    datapath_pq = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq")
+
+    datapath_hdf5 = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5"
+    )
+    datapath_pq = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq"
+    )
     datapath_hdf5_copy = os.path.join(
         RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816_copy.hdf5"
     )
-    datapath_pq_copy = os.path.join(RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816_copy.pq")
+    datapath_pq_copy = os.path.join(
+        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816_copy.pq"
+    )
 
     DS.add_data("hdf5", None, Hdf5Handle, path=datapath_hdf5)
     DS.add_data("pq", None, PqHandle, path=datapath_pq)
 
     with DS.open("hdf5") as f:
         assert f
 
@@ -242,44 +353,48 @@
     data_hdf5 = DS.read("hdf5")
 
     DS.add_data("pq_copy", data_pq, PqHandle, path=datapath_pq_copy)
     DS.add_data("hdf5_copy", data_hdf5, Hdf5Handle, path=datapath_hdf5_copy)
     DS.write("pq_copy")
     DS.write("hdf5_copy")
 
-    with pytest.raises(KeyError) as errinfo:
+    with pytest.raises(KeyError) as _errinfo:
         DS.read("nope")
-    with pytest.raises(KeyError) as errinfo:
+    with pytest.raises(KeyError) as _errinfo:
         DS.open("nope")
-    with pytest.raises(KeyError) as errinfo:
+    with pytest.raises(KeyError) as _errinfo:
         DS.write("nope")
 
-    with pytest.raises(TypeError) as errinfo:
+    with pytest.raises(TypeError) as _errinfo:
         DS["nope"] = None
-    with pytest.raises(ValueError) as errinfo:
+    with pytest.raises(ValueError) as _errinfo:
         DS["pq"] = DS["pq"]
-    with pytest.raises(ValueError) as errinfo:
+    with pytest.raises(ValueError) as _errinfo:
         DS.pq = DS["pq"]
 
+    a_handle = DS.add_handle("pq_copy_2", PqHandle, path=datapath_pq_copy)
+    assert a_handle
+    
     assert repr(DS)
 
     DS2 = DataStore(pq=DS.pq)
     assert isinstance(DS2.pq, DataHandle)
 
     # pop the 'pq' data item to avoid overwriting file under git control
     DS.pop("pq")
-
+    # pop the 'pq_copy_2' because it is empty
+    DS.pop("pq_copy_2")
+    
     DS.write_all()
     DS.write_all(force=True)
 
     os.remove(datapath_hdf5_copy)
     os.remove(datapath_pq_copy)
 
 
-
 def test_common_params():
     par = copy_param("zmin")
     assert par.default == 0.0
     assert par.value == 0.0
     assert par.dtype == float
 
     set_param_default("zmin", 0.1)
@@ -296,21 +411,29 @@
     """
 
     col_map = ColumnMapper.make_stage(name="col_map", columns={})
     with pytest.raises(FileNotFoundError) as err:
         col_map.set_data("model", None, path="./bad_directory/no_file.py")
         assert "Unable to find file" in err.context
 
+
 def test_set_data_real_file():
     """Create an instance of a child class of RailStage. Exercise the `set_data`
     method and pass in a path to model. The output of set_data should be `None`.
     """
     DS = RailStage.data_store
     DS.clear()
-    model_path = os.path.join(RAILDIR, "rail", "examples_data", "estimation_data", "data", "CWW_HDFN_prior.pkl")
+    model_path = os.path.join(
+        RAILDIR,
+        "rail",
+        "examples_data",
+        "estimation_data",
+        "data",
+        "CWW_HDFN_prior.pkl",
+    )
     DS.add_data("model", None, ModelHandle, path=model_path)
 
     col_map = ColumnMapper.make_stage(name="col_map", columns={})
 
     ret_val = col_map.set_data("model", None, path=model_path, do_read=False)
 
     assert ret_val is None
```

### Comparing `pz-rail-base-0.2.1/tests/core/test_introspection.py` & `pz-rail-base-0.2.2/tests/core/test_introspection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import tempfile
-import pkgutil
-import setuptools
 
 import rail
 from rail.core import RailEnv
 from rail.core.data import DataHandle, TableHandle
 import rail.stages
 
 
 def test_print_rail_packages():
     RailEnv.print_rail_packages()
 
-    
+
 def test_print_rail_namespaces():
     RailEnv.print_rail_namespaces()
 
 
 def test_print_rail_modules():
     RailEnv.print_rail_modules()
```

### Comparing `pz-rail-base-0.2.1/tests/core/test_pipeline.py` & `pz-rail-base-0.2.2/tests/core/test_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import os
 
 import ceci
 import numpy as np
 
-import rail
-from rail.core.data import TableHandle
 from rail.core.stage import RailPipeline, RailStage
 from rail.core.utils import RAILDIR
 from rail.core.util_stages import ColumnMapper, TableConverter
-from rail.creation.degradation.quantityCut import QuantityCut
+
 
 def test_pipeline():
     DS = RailStage.data_store
     DS.__class__.allow_overwrite = True
     DS.clear()
 
-    input_file = os.path.join(RAILDIR, "rail/examples_data/goldenspike_data/data//test_flow_data.pq")
+    input_file = os.path.join(
+        RAILDIR, "rail/examples_data/goldenspike_data/data//test_flow_data.pq"
+    )
     bands = ["u", "g", "r", "i", "z", "y"]
-    band_dict = {band: f"mag_{band}_lsst" for band in bands}
+    _band_dict = {band: f"mag_{band}_lsst" for band in bands}
     rename_dict = {f"mag_{band}_lsst": f"{band}_lsst" for band in bands}
-    post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]
+    _post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]
 
     col_remapper_test = ColumnMapper.make_stage(
         name="col_remapper_test", hdf5_groupname="", columns=rename_dict
     )
 
-    table_conv_test = TableConverter.make_stage(name="table_conv_test", output_format="numpyDict", seed=12345)
+    table_conv_test = TableConverter.make_stage(
+        name="table_conv_test", output_format="numpyDict", seed=12345
+    )
 
     pipe = ceci.Pipeline.interactive()
     stages = [
         col_remapper_test,
         table_conv_test,
     ]
     for stage in stages:
         pipe.add_stage(stage)
 
     table_conv_test.connect_input(col_remapper_test)
 
-    pipe.initialize(dict(input=input_file), dict(output_dir=".", log_dir=".", resume=False), None)
+    pipe.initialize(
+        dict(input=input_file), dict(output_dir=".", log_dir=".", resume=False), None
+    )
 
     pipe.save("stage.yaml")
 
     pr = ceci.Pipeline.read("stage.yaml")
     pr.run()
 
     os.remove("stage.yaml")
@@ -63,29 +67,33 @@
 
 def test_golden_v2():
     DS = RailStage.data_store
     DS.__class__.allow_overwrite = True
     DS.clear()
     pipe = RailPipeline()
 
-    input_file = os.path.join(RAILDIR, "rail/examples_data/goldenspike_data/data//test_flow_data.pq")
+    input_file = os.path.join(
+        RAILDIR, "rail/examples_data/goldenspike_data/data//test_flow_data.pq"
+    )
     bands = ["u", "g", "r", "i", "z", "y"]
-    band_dict = {band: f"mag_{band}_lsst" for band in bands}
+    _band_dict = {band: f"mag_{band}_lsst" for band in bands}
     rename_dict = {f"mag_{band}_lsst": f"{band}_lsst" for band in bands}
-    post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]
+    _post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]
 
     pipe.col_remapper_test = ColumnMapper.build(
-         hdf5_groupname="",
-         columns=rename_dict,
-     )
+        hdf5_groupname="",
+        columns=rename_dict,
+    )
 
     pipe.table_conv_test = TableConverter.build(
-        connections=dict(input=pipe.col_remapper_test.io.output),
+        connections=dict(input=pipe.col_remapper_test.io.output),  # pylint: disable=no-member
         output_format="numpyDict",
         seed=12345,
     )
 
-    pipe.initialize(dict(input=input_file), dict(output_dir=".", log_dir=".", resume=False), None)
+    pipe.initialize(
+        dict(input=input_file), dict(output_dir=".", log_dir=".", resume=False), None
+    )
     pipe.save("stage.yaml")
 
     pr = ceci.Pipeline.read("stage.yaml")
     pr.run()
```

### Comparing `pz-rail-base-0.2.1/tests/core/test_point_estimation.py` & `pz-rail-base-0.2.2/tests/core/test_point_estimation.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,80 +8,84 @@
 
 def test_custom_point_estimate():
     """This test checks to make sure that the inheritance mechanism is working
     for child classes of `CatEstimator`.
     """
 
     MEANING_OF_LIFE = 42.0
+
     class TestEstimator(CatEstimator):
-        name="TestEstimator"
+        name = "TestEstimator"
 
         def __init__(self, args, comm=None):
             CatEstimator.__init__(self, args, comm=comm)
 
         def _calculate_mode_point_estimate(self, qp_dist=None, grid=None):
             return np.ones(100) * MEANING_OF_LIFE
 
-    config_dict = {'calculated_point_estimates': ['mode']}
+    config_dict = {"calculated_point_estimates": ["mode"]}
 
-    test_estimator = TestEstimator.make_stage(name='test', **config_dict)
+    test_estimator = TestEstimator.make_stage(name="test", **config_dict)
 
-    locs = 2* (np.random.uniform(size=(100,1))-0.5)
-    scales = 1 + 0.2*(np.random.uniform(size=(100,1))-0.5)
-    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
+    locs = 2 * (np.random.uniform(size=(100, 1)) - 0.5)
+    scales = 1 + 0.2 * (np.random.uniform(size=(100, 1)) - 0.5)
+    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))  # pylint: disable=no-member
 
     result = test_estimator.calculate_point_estimates(test_ensemble)
 
-    assert np.all(result.ancil['mode'] == MEANING_OF_LIFE)
+    assert np.all(result.ancil["mode"] == MEANING_OF_LIFE)
+
 
 def test_basic_point_estimate():
     """This test checks to make sure that all the basic point estimates are
     executed when requested in the configuration dictionary.
     """
 
-    config_dict = {'calculated_point_estimates': ['mean', 'median', 'mode'],
-                   'zmin': 0.0,
-                   'zmax': 3.0,
-                   'nzbins': 301}
-
-    test_estimator = CatEstimator.make_stage(name='test', **config_dict)
-
-    locs = 2* (np.random.uniform(size=(100,1))-0.5)
-    scales = 1 + 0.2*(np.random.uniform(size=(100,1))-0.5)
-    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
+    config_dict = {
+        "calculated_point_estimates": ["mean", "median", "mode"],
+        "zmin": 0.0,
+        "zmax": 3.0,
+        "nzbins": 301,
+    }
+
+    test_estimator = CatEstimator.make_stage(name="test", **config_dict)
+
+    locs = 2 * (np.random.uniform(size=(100, 1)) - 0.5)
+    scales = 1 + 0.2 * (np.random.uniform(size=(100, 1)) - 0.5)
+    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))  # pylint: disable=no-member
     result = test_estimator.calculate_point_estimates(test_ensemble, None)
 
     # note: we're not interested in testing the values of point estimates,
     # just that they were added to the ancillary data.
-    assert 'mode' in result.ancil
-    assert 'median' in result.ancil
-    assert 'mean' in result.ancil
+    assert "mode" in result.ancil
+    assert "median" in result.ancil
+    assert "mean" in result.ancil
+
 
 def test_mode_no_grid():
-    """This exercises the KeyError logic in `_calculate_mode_point_estimate`.
-    """
-    config_dict = {'zmin':0.0, 'nzbins':100, 'calculated_point_estimates': ['mode']}
+    """This exercises the KeyError logic in `_calculate_mode_point_estimate`."""
+    config_dict = {"zmin": 0.0, "nzbins": 100, "calculated_point_estimates": ["mode"]}
 
-    test_estimator = CatEstimator.make_stage(name='test', **config_dict)
+    test_estimator = CatEstimator.make_stage(name="test", **config_dict)
 
     with pytest.raises(KeyError) as excinfo:
         _ = test_estimator.calculate_point_estimates(None, None)
 
     assert "to be defined in stage configuration" in str(excinfo.value)
 
+
 def test_mode_no_point_estimates():
-    """This exercises the KeyError logic in `_calculate_mode_point_estimate`.
-    """
-    config_dict = {'zmin':0.0, 'nzbins':100}
+    """This exercises the KeyError logic in `_calculate_mode_point_estimate`."""
+    config_dict = {"zmin": 0.0, "nzbins": 100}
 
-    test_estimator = CatEstimator.make_stage(name='test', **config_dict)
+    test_estimator = CatEstimator.make_stage(name="test", **config_dict)
 
-    locs = 2* (np.random.uniform(size=(100,1))-0.5)
-    scales = 1 + 0.2*(np.random.uniform(size=(100,1))-0.5)
-    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
+    locs = 2 * (np.random.uniform(size=(100, 1)) - 0.5)
+    scales = 1 + 0.2 * (np.random.uniform(size=(100, 1)) - 0.5)
+    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))  # pylint: disable=no-member
 
     output_ensemble = test_estimator.calculate_point_estimates(test_ensemble, None)
 
     assert output_ensemble.ancil is None
 
 def test_keep_existing_ancil_data():
     """Make sure that we don't overwrite the ancil data if it already exists.
```

### Comparing `pz-rail-base-0.2.1/tests/creation/test_degraders.py` & `pz-rail-base-0.2.2/tests/creation/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.1/tests/estimation/test_algos.py` & `pz-rail-base-0.2.2/tests/estimation/test_algos.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,32 @@
         "rand_zmin": 0.0,
         "rand_zmax": 3.0,
         "nzbins": 301,
         "hdf5_groupname": "photometry",
         "model": "None",
         "seed": 42,
     }
-    zb_expected = np.array([2.322, 1.317, 2.576, 2.092, 0.283, 2.927, 2.283, 2.358, 0.384, 1.351])
+    zb_expected = np.array(
+        [2.322, 1.317, 2.576, 2.092, 0.283, 2.927, 2.283, 2.358, 0.384, 1.351]
+    )
     train_algo = random_gauss.RandomGaussInformer
     pz_algo = random_gauss.RandomGaussEstimator
     results, _, _ = one_algo(
         "RandomPZ", train_algo, pz_algo, train_config_dict, estim_config_dict
     )
-    assert np.isclose(results.ancil['zmode'], zb_expected).all()
+    assert np.isclose(results.ancil["zmode"], zb_expected).all()
 
 
 def test_train_pz():
     train_config_dict = dict(
-        zmin=0.0, zmax=3.0, nzbins=301, hdf5_groupname="photometry", model="model_train_z.tmp"
+        zmin=0.0,
+        zmax=3.0,
+        nzbins=301,
+        hdf5_groupname="photometry",
+        model="model_train_z.tmp",
     )
     estim_config_dict = dict(hdf5_groupname="photometry", model="model_train_z.tmp")
 
     zb_expected = np.repeat(0.1445183, 10)
     pdf_expected = np.zeros(shape=(301,))
     pdf_expected[10:16] = [7, 23, 8, 23, 26, 13]
     train_algo = train_z.TrainZInformer
```

### Comparing `pz-rail-base-0.2.1/tests/estimation/test_classifier.py` & `pz-rail-base-0.2.2/tests/estimation/test_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,144 +1,157 @@
 import os
 import numpy as np
 import pytest
 
-from rail.core.utils import RAILDIR, find_rail_file
+from rail.core.utils import RAILDIR
 from rail.core.stage import RailStage
 from rail.core.data import QPHandle
 from rail.estimation.algos.uniform_binning import UniformBinningClassifier
 from rail.estimation.algos.equal_count import EqualCountClassifier
 
 
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
-inputdata = os.path.join(RAILDIR, 'rail/examples_data/testdata/output_BPZ_lite.hdf5')
+inputdata = os.path.join(RAILDIR, "rail/examples_data/testdata/output_BPZ_lite.hdf5")
+
 
 @pytest.mark.parametrize(
-    "input_param", 
-    [{"zbin_edges": [0.0, 0.3]},
-     {"zmin": 0.0, "zmax": 0.3, "nbins": 1},
-     {"zbin_edges": [0.0, 0.3], "id_name": "CATAID"},
-    ]
+    "input_param",
+    [
+        {"zbin_edges": [0.0, 0.3]},
+        {"zmin": 0.0, "zmax": 0.3, "nbins": 1},
+        {"zbin_edges": [0.0, 0.3], "id_name": "CATAID"},
+    ],
 )
-
 def test_UniformBinningClassifier(input_param):
-    DS.clear()    
-    input_data = DS.read_file('input_data', QPHandle, inputdata)
+    DS.clear()
+    input_data = DS.read_file("input_data", QPHandle, inputdata)
 
     tomo = UniformBinningClassifier.make_stage(
-        point_estimate='zmode',
+        point_estimate="zmode",
         no_assign=-99,
         **input_param,
     )
-    
-    out_data = tomo.classify(input_data)
-    
+
+    _out_data = tomo.classify(input_data)
+
 
 def test_UniformBinningClassifier_binsize():
-    DS.clear()    
-    input_data = DS.read_file('input_data', QPHandle, inputdata)
+    DS.clear()
+    input_data = DS.read_file("input_data", QPHandle, inputdata)
 
     tomo = UniformBinningClassifier.make_stage(
-        point_estimate='zmode',
+        point_estimate="zmode",
         no_assign=-99,
-        zmin=0.0, 
-        zmax=2.0, 
+        zmin=0.0,
+        zmax=2.0,
         nbins=2,
     )
     output_data = tomo.classify(input_data)
-    out_data=output_data.data
-    
+    out_data = output_data.data
+
     # check length:
-    assert len(out_data["class_id"])==len(out_data["row_index"])
-    
+    assert len(out_data["class_id"]) == len(out_data["row_index"])
+
     # check that the assignment is as expected:
-    assert (np.in1d(np.unique(out_data["class_id"]),[1,2,-99])).all()
-    
-    zb = input_data.data.ancil['zmode']
+    assert (np.in1d(np.unique(out_data["class_id"]), [1, 2, -99])).all()
+
+    zb = input_data.data.ancil["zmode"]
     if 1 in out_data["class_id"]:
-        assert ((zb[out_data["class_id"]==1]>=0.0)&(zb[out_data["class_id"]==1]<1.0)).all()
+        assert (
+            (zb[out_data["class_id"] == 1] >= 0.0)
+            & (zb[out_data["class_id"] == 1] < 1.0)
+        ).all()
     if 2 in out_data["class_id"]:
-        assert ((zb[out_data["class_id"]==2]>=1.0)&(zb[out_data["class_id"]==2]<2.0)).all()
+        assert (
+            (zb[out_data["class_id"] == 2] >= 1.0)
+            & (zb[out_data["class_id"] == 2] < 2.0)
+        ).all()
     if -99 in out_data["class_id"]:
-        assert ((zb[out_data["class_id"]==-99]<0.0)|(zb[out_data["class_id"]==-99]>=2.0)).all()
-        
+        assert (
+            (zb[out_data["class_id"] == -99] < 0.0)
+            | (zb[out_data["class_id"] == -99] >= 2.0)
+        ).all()
+
 
 def test_UniformBinningClassifier_ancil():
-    DS.clear()    
-    input_data = DS.read_file('input_data', QPHandle, inputdata)
+    DS.clear()
+    input_data = DS.read_file("input_data", QPHandle, inputdata)
 
     tomo = UniformBinningClassifier.make_stage(
-        point_estimate='zmedian',
+        point_estimate="zmedian",
         no_assign=-99,
-        zmin=0.0, 
-        zmax=2.0, 
+        zmin=0.0,
+        zmax=2.0,
         nbins=2,
     )
     with pytest.raises(KeyError):
-        out_data = tomo.classify(input_data)
-    
+        _out_data = tomo.classify(input_data)
+
 
 @pytest.mark.parametrize(
-    "input_param",   
-    [{"zmin": 0.0, "zmax": 0.3, "nbins": 1},
-     {"zmin": 0.0, "zmax": 0.3, "nbins": 1, "id_name": "CATAID"},
-    ]
+    "input_param",
+    [
+        {"zmin": 0.0, "zmax": 0.3, "nbins": 1},
+        {"zmin": 0.0, "zmax": 0.3, "nbins": 1, "id_name": "CATAID"},
+    ],
 )
-
 def test_EqualCountClassifier(input_param):
-    DS.clear()    
-    input_data = DS.read_file('input_data', QPHandle, inputdata)
+    DS.clear()
+    input_data = DS.read_file("input_data", QPHandle, inputdata)
 
     tomo = EqualCountClassifier.make_stage(
-        point_estimate='zmode',
+        point_estimate="zmode",
         no_assign=-99,
         **input_param,
     )
-    
-    out_data = tomo.classify(input_data)
+
+    _out_data = tomo.classify(input_data)
 
 
 def test_EqualCountClassifier_nobj():
-    DS.clear()    
-    input_data = DS.read_file('input_data', QPHandle, inputdata)
+    DS.clear()
+    input_data = DS.read_file("input_data", QPHandle, inputdata)
 
     tomo = EqualCountClassifier.make_stage(
-        point_estimate='zmode',
+        point_estimate="zmode",
         no_assign=-99,
-        zmin=0.0, 
-        zmax=2.0, 
+        zmin=0.0,
+        zmax=2.0,
         nbins=2,
     )
     output_data = tomo.classify(input_data)
-    out_data=output_data.data
-    
+    out_data = output_data.data
+
     # check that there are equal number of object in each bin modulo Ngal%Nbins
-    assert (np.in1d(np.unique(out_data["class_id"]), [1,2,-99])).all()
-    
-    Ngal=sum(out_data["class_id"]!=-99)
-    exp_Ngal_perbin=int(Ngal/2)
+    assert (np.in1d(np.unique(out_data["class_id"]), [1, 2, -99])).all()
+
+    Ngal = sum(out_data["class_id"] != -99)
+    exp_Ngal_perbin = int(Ngal / 2)
     # check that each bin does contain number of objects consistent with expected number
     # exp_Ngal_perbin + 1 to account for the cases where Ngal%Nbins!=0
-    assert sum(out_data["class_id"]==1) in [exp_Ngal_perbin, exp_Ngal_perbin+1]
-    assert sum(out_data["class_id"]==2) in [exp_Ngal_perbin, exp_Ngal_perbin+1]
-    
+    assert sum(out_data["class_id"] == 1) in [exp_Ngal_perbin, exp_Ngal_perbin + 1]
+    assert sum(out_data["class_id"] == 2) in [exp_Ngal_perbin, exp_Ngal_perbin + 1]
+
     # check no assignment is correct
-    if Ngal<len(out_data["class_id"]):
-        zb = input_data.data.ancil['zmode']
-        assert ((zb[out_data["class_id"]==-99]<0.0)|(zb[out_data["class_id"]==-99]>=2.0)).all()
+    if Ngal < len(out_data["class_id"]):
+        zb = input_data.data.ancil["zmode"]
+        assert (
+            (zb[out_data["class_id"] == -99] < 0.0)
+            | (zb[out_data["class_id"] == -99] >= 2.0)
+        ).all()
 
 
 def test_EqualCountClassifier_ancil():
-    DS.clear()    
-    input_data = DS.read_file('input_data', QPHandle, inputdata)
+    DS.clear()
+    input_data = DS.read_file("input_data", QPHandle, inputdata)
 
     tomo = EqualCountClassifier.make_stage(
-        point_estimate='zmedian',
+        point_estimate="zmedian",
         no_assign=-99,
-        zmin=0.0, 
-        zmax=2.0, 
+        zmin=0.0,
+        zmax=2.0,
         nbins=2,
     )
     with pytest.raises(KeyError):
-        out_data = tomo.classify(input_data)
+        _out_data = tomo.classify(input_data)
```

### Comparing `pz-rail-base-0.2.1/tests/estimation/test_summarizers.py` & `pz-rail-base-0.2.2/tests/estimation/test_summarizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,44 +14,46 @@
     A basic test of running an summaizer subclass
     Run summarize
     """
     DS.__class__.allow_overwrite = True
     test_data = DS.read_file("test_data", QPHandle, testdata)
     summarizer = summarizer_class.make_stage(name=key, **summary_kwargs)
     summary_ens = summarizer.summarize(test_data)
-    os.remove(summarizer.get_output(summarizer.get_aliased_tag("output"), final_name=True))
-    os.remove(summarizer.get_output(summarizer.get_aliased_tag("single_NZ"), final_name=True))
+    os.remove(
+        summarizer.get_output(summarizer.get_aliased_tag("output"), final_name=True)
+    )
+    os.remove(
+        summarizer.get_output(summarizer.get_aliased_tag("single_NZ"), final_name=True)
+    )
     return summary_ens
 
 
 def test_naive_stack():
-    """Basic end to end test for the Naive stack informer to estimator stages
-    """
+    """Basic end to end test for the Naive stack informer to estimator stages"""
     naive_stack_informer_stage = naive_stack.NaiveStackInformer.make_stage()
-    naive_stack_informer_stage.inform('')
+    naive_stack_informer_stage.inform("")
 
     summary_config_dict = {}
     summarizer_class = naive_stack.NaiveStackSummarizer
     _ = one_algo("NaiveStack", summarizer_class, summary_config_dict)
 
 
 def test_point_estimate_hist():
     """Basic end to end test for the point estimate histogram informer to estimator
     stages
     """
     point_est_informer_stage = point_est_hist.PointEstHistInformer.make_stage()
-    point_est_informer_stage.inform('')
+    point_est_informer_stage.inform("")
 
     summary_config_dict = {}
     summarizer_class = point_est_hist.PointEstHistSummarizer
     _ = one_algo("PointEstimateHist", summarizer_class, summary_config_dict)
 
 
 def test_var_inference_stack():
-    """Basic end to end test for the var inference informer to estimator stages
-    """
+    """Basic end to end test for the var inference informer to estimator stages"""
     var_inf_informer_stage = var_inf.VarInfStackInformer.make_stage()
-    var_inf_informer_stage.inform('')
+    var_inf_informer_stage.inform("")
 
     summary_config_dict = {}
     summarizer_class = var_inf.VarInfStackSummarizer
     _ = one_algo("VariationalInference", summarizer_class, summary_config_dict)
```

