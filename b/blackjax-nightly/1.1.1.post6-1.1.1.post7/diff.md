# Comparing `tmp/blackjax-nightly-1.1.1.post6.tar.gz` & `tmp/blackjax-nightly-1.1.1.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackjax-nightly-1.1.1.post6.tar", last modified: Mon Apr  1 06:47:32 2024, max compression
+gzip compressed data, was "blackjax-nightly-1.1.1.post7.tar", last modified: Mon Apr  8 11:35:23 2024, max compression
```

## Comparing `blackjax-nightly-1.1.1.post6.tar` & `blackjax-nightly-1.1.1.post7.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.394999 blackjax-nightly-1.1.1.post6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.394999 blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/meeting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/sampler_proposal.md
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.394999 blackjax-nightly-1.1.1.post6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/schedule-meeting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.398999 blackjax-nightly-1.1.1.post6/blackjax/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-01 06:47:32.000000 blackjax-nightly-1.1.1.post6/blackjax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.398999 blackjax-nightly-1.1.1.post6/blackjax/adaptation/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/chees_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/mclmc_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/meads_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/pathfinder_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/step_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/adaptation/window_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.402999 blackjax-nightly-1.1.1.post6/blackjax/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/barker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/dynamic_hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/elliptical_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/ghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/mala.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/marginal_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/mclmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/periodic_orbital.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/rmhmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/termination.py
--rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/mcmc/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.402999 blackjax-nightly-1.1.1.post6/blackjax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/optimizers/dual_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/optimizers/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.402999 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/csgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/sghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/sgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/sgnht.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.406999 blackjax-nightly-1.1.1.post6/blackjax/smc/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/adaptive_tempered.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/inner_kernel_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/tempered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.406999 blackjax-nightly-1.1.1.post6/blackjax/smc/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/tuning/from_kernel_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/smc/tuning/from_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.406999 blackjax-nightly-1.1.1.post6/blackjax/vi/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/vi/meanfield_vi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/vi/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/vi/schrodinger_follmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/blackjax/vi/svgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-01 06:47:32.000000 blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-01 06:47:32.000000 blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 06:47:32.000000 blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 06:47:32.000000 blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 06:47:32.000000 blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.410999 blackjax-nightly-1.1.1.post6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.410999 blackjax-nightly-1.1.1.post6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   161829 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/_static/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/bib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.410999 blackjax-nightly-1.1.1.post6/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.418999 blackjax-nightly-1.1.1.post6/docs/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/data/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (127)    63251 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/data/google.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_custom_gradients.md
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_metropolis_within_gibbs.md
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_other_frameworks.md
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_reproduce_the_blackjax_image.md
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_sample_multiple_chains.md
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_use_aesara.md
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_use_numpyro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_use_oryx.md
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_use_pymc.md
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/howto_use_tfp.md
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)  4461357 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/examples/scatter.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/jupytex.toml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-01 06:47:24.000000 blackjax-nightly-1.1.1.post6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.418999 blackjax-nightly-1.1.1.post6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.418999 blackjax-nightly-1.1.1.post6/tests/adaptation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/adaptation/test_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/adaptation/test_mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/adaptation/test_step_size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/tests/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_barker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_random_walk_without_chex.py
--rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/mcmc/test_uturn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/tests/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/optimizers/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/optimizers/test_pathfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/tests/smc/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_inner_kernel_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_kernel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_smc_ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/smc/test_tempered_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/test_compilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:32.422999 blackjax-nightly-1.1.1.post6/tests/vi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/vi/test_meanfield_vi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/vi/test_schrodinger_follmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-01 06:47:23.000000 blackjax-nightly-1.1.1.post6/tests/vi/test_svgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.867102 blackjax-nightly-1.1.1.post7/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.835102 blackjax-nightly-1.1.1.post7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.839102 blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/meeting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/sampler_proposal.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.839102 blackjax-nightly-1.1.1.post7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/schedule-meeting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-08 11:35:23.867102 blackjax-nightly-1.1.1.post7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.839102 blackjax-nightly-1.1.1.post7/blackjax/
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 11:35:23.000000 blackjax-nightly-1.1.1.post7/blackjax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.843102 blackjax-nightly-1.1.1.post7/blackjax/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17121 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/chees_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/mclmc_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/meads_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/pathfinder_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/step_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/adaptation/window_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.843102 blackjax-nightly-1.1.1.post7/blackjax/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/dynamic_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/elliptical_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/ghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/mala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/marginal_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/mclmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/periodic_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/rmhmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/mcmc/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.847102 blackjax-nightly-1.1.1.post7/blackjax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/optimizers/dual_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/optimizers/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.847102 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/csgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/sghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/sgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/sgnht.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.847102 blackjax-nightly-1.1.1.post7/blackjax/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/adaptive_tempered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/inner_kernel_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/tempered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.847102 blackjax-nightly-1.1.1.post7/blackjax/smc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/tuning/from_kernel_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/smc/tuning/from_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.851102 blackjax-nightly-1.1.1.post7/blackjax/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/vi/meanfield_vi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/vi/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/vi/schrodinger_follmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/blackjax/vi/svgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.867102 blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-08 11:35:23.000000 blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-08 11:35:23.000000 blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:35:23.000000 blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:35:23.000000 blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 11:35:23.000000 blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.851102 blackjax-nightly-1.1.1.post7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.851102 blackjax-nightly-1.1.1.post7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   161829 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/_static/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/bib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.855102 blackjax-nightly-1.1.1.post7/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.859102 blackjax-nightly-1.1.1.post7/docs/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/data/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63251 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/data/google.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_custom_gradients.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_metropolis_within_gibbs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_other_frameworks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_reproduce_the_blackjax_image.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_sample_multiple_chains.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_use_aesara.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_use_numpyro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_use_oryx.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_use_pymc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/howto_use_tfp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)  4461357 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/examples/scatter.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/jupytex.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 11:35:23.867102 blackjax-nightly-1.1.1.post7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.859102 blackjax-nightly-1.1.1.post7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.863102 blackjax-nightly-1.1.1.post7/tests/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/adaptation/test_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/adaptation/test_mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/adaptation/test_step_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.863102 blackjax-nightly-1.1.1.post7/tests/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_random_walk_without_chex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28432 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/mcmc/test_uturn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.863102 blackjax-nightly-1.1.1.post7/tests/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/optimizers/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/optimizers/test_pathfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.863102 blackjax-nightly-1.1.1.post7/tests/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_inner_kernel_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_kernel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_smc_ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/smc/test_tempered_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/test_compilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:23.867102 blackjax-nightly-1.1.1.post7/tests/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/vi/test_meanfield_vi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/vi/test_schrodinger_follmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-08 11:35:19.000000 blackjax-nightly-1.1.1.post7/tests/vi/test_svgd.py
```

### Comparing `blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/bug_report.yml` & `blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/enhancement.md` & `blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/meeting.md` & `blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/meeting.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/ISSUE_TEMPLATE/sampler_proposal.md` & `blackjax-nightly-1.1.1.post7/.github/ISSUE_TEMPLATE/sampler_proposal.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/PULL_REQUEST_TEMPLATE.md` & `blackjax-nightly-1.1.1.post7/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/workflows/benchmark.yml` & `blackjax-nightly-1.1.1.post7/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/workflows/build_documentation.yml` & `blackjax-nightly-1.1.1.post7/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/workflows/nightly.yml` & `blackjax-nightly-1.1.1.post7/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/workflows/publish_documentation.yml` & `blackjax-nightly-1.1.1.post7/.github/workflows/publish_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/workflows/release.yml` & `blackjax-nightly-1.1.1.post7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.github/workflows/test.yml` & `blackjax-nightly-1.1.1.post7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.gitignore` & `blackjax-nightly-1.1.1.post7/.gitignore`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.gitlint` & `blackjax-nightly-1.1.1.post7/.gitlint`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/.pre-commit-config.yaml` & `blackjax-nightly-1.1.1.post7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/CODE_OF_CONDUCT.md` & `blackjax-nightly-1.1.1.post7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/CONTRIBUTING.md` & `blackjax-nightly-1.1.1.post7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/GOVERNANCE.md` & `blackjax-nightly-1.1.1.post7/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/LICENSE` & `blackjax-nightly-1.1.1.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/Makefile` & `blackjax-nightly-1.1.1.post7/Makefile`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/PKG-INFO` & `blackjax-nightly-1.1.1.post7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax-nightly
-Version: 1.1.1.post6
+Version: 1.1.1.post7
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
@@ -114,16 +114,16 @@
 
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
-for _ in range(100):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for step in range(100):
+    nuts_key = jax.random.fold_in(rng_key, step)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 See [the documentation](https://blackjax-devs.github.io/blackjax/index.html) for more examples of how to use the library: how to write inference loops for one or several chains, how to use the Stan warmup, etc.
 
 ## Philosophy
```

### Comparing `blackjax-nightly-1.1.1.post6/README.md` & `blackjax-nightly-1.1.1.post7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
-for _ in range(100):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for step in range(100):
+    nuts_key = jax.random.fold_in(rng_key, step)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 See [the documentation](https://blackjax-devs.github.io/blackjax/index.html) for more examples of how to use the library: how to write inference loops for one or several chains, how to use the Stan warmup, etc.
 
 ## Philosophy
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/__init__.py` & `blackjax-nightly-1.1.1.post7/blackjax/__init__.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/base.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/chees_adaptation.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/chees_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,28 +357,26 @@
         assert all(
             jax.tree_util.tree_flatten(
                 jax.tree_util.tree_map(lambda p: p.shape[0] == num_chains, positions)
             )[0]
         ), "initial `positions` leading dimension must be equal to the `num_chains`"
         num_dim = pytree_size(positions) // num_chains
 
-        key_init, key_step = jax.random.split(rng_key)
+        next_random_arg_fn = lambda i: i + 1
+        init_random_arg = 0
 
         if jitter_generator is not None:
-            jitter_gn = lambda key: jitter_generator(key) * jitter_amount + (
-                1.0 - jitter_amount
-            )
-            next_random_arg_fn = lambda key: jax.random.split(key)[1]
-            init_random_arg = key_init
+            rng_key, carry_key = jax.random.split(rng_key)
+            jitter_gn = lambda i: jitter_generator(
+                jax.random.fold_in(carry_key, i)
+            ) * jitter_amount + (1.0 - jitter_amount)
         else:
             jitter_gn = lambda i: dynamic_hmc.halton_sequence(
                 i, np.ceil(np.log2(num_steps + max_sampling_steps))
             ) * jitter_amount + (1.0 - jitter_amount)
-            next_random_arg_fn = lambda i: i + 1
-            init_random_arg = 0
 
         def integration_steps_fn(random_generator_arg, trajectory_length_adjusted):
             return jnp.asarray(
                 jnp.ceil(jitter_gn(random_generator_arg) * trajectory_length_adjusted),
                 dtype=int,
             )
 
@@ -421,15 +419,15 @@
 
         batch_init = jax.vmap(
             lambda p: dynamic_hmc.init(p, logdensity_fn, init_random_arg)
         )
         init_states = batch_init(positions)
         init_adaptation_state = init(init_random_arg, step_size)
 
-        keys_step = jax.random.split(key_step, num_steps)
+        keys_step = jax.random.split(rng_key, num_steps)
         (last_states, last_adaptation_state), info = jax.lax.scan(
             one_step, (init_states, init_adaptation_state), keys_step
         )
 
         trajectory_length_adjusted = jnp.exp(
             last_adaptation_state.log_trajectory_length_moving_average
             - last_adaptation_state.log_step_size_moving_average
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/mass_matrix.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/mclmc_adaptation.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/mclmc_adaptation.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,20 +227,20 @@
         # we use the last num_steps2 to compute the diagonal preconditioner
         outer_weights = jnp.concatenate((jnp.zeros(num_steps1), jnp.ones(num_steps2)))
 
         # initial state of the kalman filter
         kalman_state = (0.0, jnp.zeros(dim), jnp.zeros(dim))
 
         # run the steps
-        kalman_state = jax.lax.scan(
+        kalman_state, *_ = jax.lax.scan(
             step,
             init=(state, params, adap0, kalman_state),
             xs=(outer_weights, L_step_size_adaptation_keys),
             length=num_steps1 + num_steps2,
-        )[0]
+        )
         state, params, _, kalman_state_output = kalman_state
 
         L = params.L
         # determine L
         if num_steps2 != 0.0:
             _, F1, F2 = kalman_state_output
             variances = F2 - jnp.square(F1)
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/meads_adaptation.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/meads_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,24 +89,24 @@
 
         Returns
         -------
         New values of the step size, and the alpha and delta parameters
         of the generalized HMC algorithm.
 
         """
-        mean_position = jax.tree_map(lambda p: p.mean(axis=0), positions)
-        sd_position = jax.tree_map(lambda p: p.std(axis=0), positions)
-        normalized_positions = jax.tree_map(
+        mean_position = jax.tree.map(lambda p: p.mean(axis=0), positions)
+        sd_position = jax.tree.map(lambda p: p.std(axis=0), positions)
+        normalized_positions = jax.tree.map(
             lambda p, mu, sd: (p - mu) / sd,
             positions,
             mean_position,
             sd_position,
         )
 
-        batch_grad_scaled = jax.tree_map(
+        batch_grad_scaled = jax.tree.map(
             lambda grad, sd: grad * sd, logdensity_grad, sd_position
         )
 
         epsilon = jnp.minimum(
             0.5 / jnp.sqrt(maximum_eigenvalue(batch_grad_scaled)), 1.0
         )
         gamma = jnp.maximum(
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/pathfinder_adaptation.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/pathfinder_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/step_size.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/step_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,28 +154,28 @@
 #                 REASONABLE FIRST STEP SIZE
 # -------------------------------------------------------------------
 
 
 class ReasonableStepSizeState(NamedTuple):
     """State carried through the search for a reasonable first step size.
 
-    rng_key
-        Key used by JAX's random number generator.
+    step
+        The current iteration step.
     direction: {-1, 1}
         Determines whether the step size should be increased or decreased during the
         previous step search. If direction = 1 it will be increased, otherwise decreased.
     previous_direction
         The previous direction. It is necessary to carry it because the choice of step
         size is made at the end of the search update.
     step_size
         The current step size in the search.
 
     """
 
-    rng_key: PRNGKey
+    step: int
     direction: int
     previous_direction: int
     step_size: float
 
 
 def find_reasonable_step_size(
     rng_key: PRNGKey,
@@ -239,21 +239,21 @@
         has_acceptance_rate_not_crossed_threshold = (previous_direction == 0) | (
             direction == previous_direction
         )
         return is_step_size_not_extreme & has_acceptance_rate_not_crossed_threshold
 
     def update(rss_state: ReasonableStepSizeState) -> ReasonableStepSizeState:
         """Perform one step of the step size search."""
-        rng_key, direction, _, step_size = rss_state
-        rng_key, subkey = jax.random.split(rng_key)
+        i, direction, _, step_size = rss_state
+        subkey = jax.random.fold_in(rng_key, i)
 
         step_size = (2.0**direction) * step_size
         kernel = kernel_generator(step_size)
         _, info = kernel(subkey, reference_state)
 
         new_direction = jnp.where(target_accept < info.acceptance_rate, 1, -1)
-        return ReasonableStepSizeState(rng_key, new_direction, direction, step_size)
+        return ReasonableStepSizeState(i + 1, new_direction, direction, step_size)
 
-    rss_state = ReasonableStepSizeState(rng_key, 0, 0, initial_step_size)
+    rss_state = ReasonableStepSizeState(0, 0, 0, initial_step_size)
     rss_state = jax.lax.while_loop(do_continue, update, rss_state)
 
     return rss_state.step_size
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/adaptation/window_adaptation.py` & `blackjax-nightly-1.1.1.post7/blackjax/adaptation/window_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/base.py` & `blackjax-nightly-1.1.1.post7/blackjax/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/diagnostics.py` & `blackjax-nightly-1.1.1.post7/blackjax/diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/barker.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/barker.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/diffusions.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/dynamic_hmc.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/dynamic_hmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/elliptical_slice.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/elliptical_slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
     """
 
     def generate(
         rng_key: PRNGKey, state: EllipSliceState
     ) -> tuple[EllipSliceState, EllipSliceInfo]:
         position, logdensity = state
-        key_momentum, key_uniform, key_theta = jax.random.split(rng_key, 3)
+        key_slice, key_momentum, key_uniform, key_theta = jax.random.split(rng_key, 4)
         # step 1: sample momentum
         momentum = momentum_generator(key_momentum, position)
         # step 2: get slice (y)
         logy = logdensity + jnp.log(jax.random.uniform(key_uniform))
         # step 3: get theta (ellipsis move), set inital interval
         theta = 2 * jnp.pi * jax.random.uniform(key_theta)
         theta_min = theta - 2 * jnp.pi
@@ -231,28 +231,28 @@
 
             As the bracket `[theta_min, theta_max]` shrinks, the proposal gets closer
             to the original position, which has likelihood larger than the slice variable.
             It is guaranteed to stop in a finite number of iterations as long as the
             likelihood is continuous with respect to the parameter being sampled.
 
             """
-            rng, _, subiter, theta, theta_min, theta_max, *_ = vals
-            rng, thetak = jax.random.split(rng)
+            _, subiter, theta, theta_min, theta_max, *_ = vals
+            thetak = jax.random.fold_in(key_slice, subiter)
             theta = jax.random.uniform(thetak, minval=theta_min, maxval=theta_max)
             p, m = ellipsis(position, momentum, theta, mean)
             logdensity = logdensity_fn(p)
             theta_min = jnp.where(theta < 0, theta, theta_min)
             theta_max = jnp.where(theta > 0, theta, theta_max)
             subiter += 1
-            return rng, logdensity, subiter, theta, theta_min, theta_max, p, m
+            return logdensity, subiter, theta, theta_min, theta_max, p, m
 
-        _, logdensity, subiter, theta, *_, position, momentum = jax.lax.while_loop(
-            lambda vals: vals[1] <= logy,
+        logdensity, subiter, theta, *_, position, momentum = jax.lax.while_loop(
+            lambda vals: vals[0] <= logy,
             slice_fn,
-            (rng_key, logdensity, 1, theta, theta_min, theta_max, p, m),
+            (logdensity, 1, theta, theta_min, theta_max, p, m),
         )
         return (
             EllipSliceState(position, logdensity),
             EllipSliceInfo(momentum, theta, subiter),
         )
 
     return generate
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/ghmc.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/ghmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     an updated momentum that is a mixture of the previous momentum a new sample
     from a Gaussian density (dependent on alpha). The weights of the mixture of
     these two components are a function of alpha.
 
     """
     position, momentum, *_ = state
 
-    momentum = jax.tree_map(
+    momentum = jax.tree.map(
         lambda prev_momentum, shifted_momentum: prev_momentum * jnp.sqrt(1.0 - alpha)
         + jnp.sqrt(alpha) * shifted_momentum,
         momentum,
         momentum_generator(rng_key, position),
     )
 
     return momentum
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/hmc.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/hmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/integrators.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/mala.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/mala.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/marginal_latent_gaussian.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/marginal_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/mclmc.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/mclmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/metrics.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/nuts.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/periodic_orbital.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/periodic_orbital.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/proposal.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/random_walk.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/random_walk.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/rmhmc.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/rmhmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/termination.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/termination.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/mcmc/trajectory.py` & `blackjax-nightly-1.1.1.post7/blackjax/mcmc/trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,25 +197,25 @@
             Initial energy H0 of the HMC step (not to confused with the initial
             energy of the subtree)
 
         """
 
         def do_keep_integrating(loop_state):
             """Decide whether we should continue integrating the trajectory"""
-            _, integration_state, (is_diverging, has_terminated) = loop_state
+            integration_state, (is_diverging, has_terminated) = loop_state
             return (
                 (integration_state.step < max_num_steps)
                 & ~has_terminated
                 & ~is_diverging
             )
 
         def add_one_state(loop_state):
-            rng_key, integration_state, _ = loop_state
+            integration_state, _ = loop_state
             step, proposal, trajectory, termination_state = integration_state
-            rng_key, proposal_key = jax.random.split(rng_key)
+            proposal_key = jax.random.fold_in(rng_key, step)
 
             new_state = integrator(trajectory.rightmost_state, direction * step_size)
             new_proposal = generate_proposal(initial_energy, new_state)
             is_diverging = -new_proposal.weight > divergence_threshold
 
             # At step 0, we always accept the proposal, since we
             # take one step to get the leftmost state of the tree.
@@ -242,33 +242,33 @@
             new_integration_state = DynamicIntegrationState(
                 step + 1,
                 sampled_proposal,
                 new_trajectory,
                 new_termination_state,
             )
 
-            return (rng_key, new_integration_state, (is_diverging, has_terminated))
+            return (new_integration_state, (is_diverging, has_terminated))
 
         proposal_placeholder = generate_proposal(initial_energy, initial_state)
         trajectory_placeholder = Trajectory(
             initial_state, initial_state, initial_state.momentum, 0
         )
         integration_state_placeholder = DynamicIntegrationState(
             0,
             proposal_placeholder,
             trajectory_placeholder,
             termination_state,
         )
 
-        _, integration_state, (is_diverging, has_terminated) = jax.lax.while_loop(
+        new_integration_state, (is_diverging, has_terminated) = jax.lax.while_loop(
             do_keep_integrating,
             add_one_state,
-            (rng_key, integration_state_placeholder, (False, False)),
+            (integration_state_placeholder, (False, False)),
         )
-        step, proposal, trajectory, termination_state = integration_state
+        _, proposal, trajectory, termination_state = new_integration_state
 
         # In the while_loop we always extend on the right most direction.
         new_trajectory = jax.lax.cond(
             direction > 0,
             lambda _: trajectory,
             lambda _: Trajectory(
                 trajectory.rightmost_state,
@@ -492,16 +492,15 @@
         A function that runs the symplectic integrators and returns a new proposal
         and the integrated trajectory.
     uturn_check_fn
         Function used to check the U-Turn criterion.
     step_size
         The step size used by the symplectic integrator.
     max_num_expansions
-        The maximum number of trajectory expansions until the proposal is
-        returned.
+        The maximum number of trajectory expansions until the proposal is returned.
     rate
         The rate of the geometrical expansion. Typically 2 in NUTS, this is why
         the literature often refers to "tree doubling".
 
     """
     proposal_sampler = progressive_biased_sampling
 
@@ -509,15 +508,15 @@
         rng_key: PRNGKey,
         initial_expansion_state: DynamicExpansionState,
         initial_energy: float,
         step_size: float,
     ):
         def do_keep_expanding(loop_state) -> bool:
             """Determine whether we need to keep expanding the trajectory."""
-            _, expansion_state, (is_diverging, is_turning) = loop_state
+            expansion_state, (is_diverging, is_turning) = loop_state
             return (
                 (expansion_state.step < max_num_expansions)
                 & ~is_diverging
                 & ~is_turning
             )
 
         def expand_once(loop_state):
@@ -527,20 +526,19 @@
             starting from the leftmost or rightmost point of the current
             trajectory that is twice as long as the current trajectory.
 
             Once that is done, possibly update the current proposal with that of
             the subtrajectory.
 
             """
-            rng_key, expansion_state, _ = loop_state
+            expansion_state, _ = loop_state
             step, proposal, trajectory, termination_state = expansion_state
 
-            rng_key, direction_key, trajectory_key, proposal_key = jax.random.split(
-                rng_key, 4
-            )
+            subkey = jax.random.fold_in(rng_key, step)
+            direction_key, trajectory_key, proposal_key = jax.random.split(subkey, 3)
 
             # create new subtrajectory that is twice as long as the current
             # trajectory.
             direction = jnp.where(jax.random.bernoulli(direction_key), 1, -1)
             start_state = jax.lax.cond(
                 direction > 0,
                 lambda _: trajectory.rightmost_state,
@@ -604,20 +602,20 @@
             )
 
             new_state = DynamicExpansionState(
                 step + 1, updated_proposal, merged_trajectory, termination_state
             )
             info = (is_diverging, is_turning_subtree | is_turning)
 
-            return (rng_key, new_state, info)
+            return (new_state, info)
 
-        _, expansion_state, (is_diverging, is_turning) = jax.lax.while_loop(
+        expansion_state, (is_diverging, is_turning) = jax.lax.while_loop(
             do_keep_expanding,
             expand_once,
-            (rng_key, initial_expansion_state, (False, False)),
+            (initial_expansion_state, (False, False)),
         )
 
         return expansion_state, (is_diverging, is_turning)
 
     return expand
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/optimizers/dual_averaging.py` & `blackjax-nightly-1.1.1.post7/blackjax/optimizers/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/optimizers/lbfgs.py` & `blackjax-nightly-1.1.1.post7/blackjax/optimizers/lbfgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     # Unravel optimization path history.
     history = LBFGSHistory(
         x=unravel_fn_mapped(history_raveled.x),
         f=history_raveled.f,
         g=unravel_fn_mapped(history_raveled.g),
         alpha=unravel_fn_mapped(history_raveled.alpha),
-        update_mask=jax.tree_map(
+        update_mask=jax.tree.map(
             lambda x: x.astype(history_raveled.update_mask.dtype),
             unravel_fn_mapped(history_raveled.update_mask.astype(x0_raveled.dtype)),
         ),
     )
 
     return last_step, history
 
@@ -226,15 +226,15 @@
         update_mask=jnp.zeros_like(x0, dtype=bool),
     )
 
     ((last_step, _), _), history = lax.scan(
         scan_body, ((init_step, initial_history), True), jnp.arange(maxiter)
     )
     # Append initial state to history.
-    history = jax.tree_map(
+    history = jax.tree.map(
         lambda x, y: jnp.concatenate([x[None, ...], y], axis=0),
         initial_history,
         history,
     )
     return last_step, history
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/progress_bar.py` & `blackjax-nightly-1.1.1.post7/blackjax/progress_bar.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/csgld.py` & `blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/csgld.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/diffusions.py` & `blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/gradients.py` & `blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         An approximation of the value of the log-posterior density function for
         the current value of the random variables.
 
         """
         grad_estimate = logdensity_grad_estimator(position, minibatch)
         center_grad_estimate = logdensity_grad_estimator(centering_position, minibatch)
 
-        return jax.tree_map(
+        return jax.tree.map(
             lambda grad_est, cv_grad_est, cv_grad: cv_grad + grad_est - cv_grad_est,
             grad_estimate,
             center_grad_estimate,
             cv_grad_value,
         )
 
     return cv_grad_estimator_fn
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/sghmc.py` & `blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/sghmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/sgld.py` & `blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/sgld.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/sgmcmc/sgnht.py` & `blackjax-nightly-1.1.1.post7/blackjax/sgmcmc/sgnht.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/adaptive_tempered.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/adaptive_tempered.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/base.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     num_particles = state.weights.shape[0]
 
     if num_resampled is None:
         num_resampled = num_particles
 
     resampling_idx = resample_fn(resampling_key, state.weights, num_resampled)
-    particles = jax.tree_map(lambda x: x[resampling_idx], state.particles)
+    particles = jax.tree.map(lambda x: x[resampling_idx], state.particles)
 
     keys = jax.random.split(updating_key, num_resampled)
     particles, update_info = update_fn(keys, particles, state.update_parameters)
 
     log_weights = weight_fn(particles)
     logsum_weights = jax.scipy.special.logsumexp(log_weights)
     normalizing_constant = logsum_weights - jnp.log(num_particles)
@@ -154,8 +154,8 @@
     """Given a dictionary of params, repeats them for every single particle. The expected
     usage is in cases where the aim is to repeat the same parameters for all chains within SMC.
     """
 
     def extend(param):
         return jnp.repeat(jnp.asarray(param)[None, ...], n_particles, axis=0)
 
-    return jax.tree_map(extend, params)
+    return jax.tree.map(extend, params)
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/ess.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/inner_kernel_tuning.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/inner_kernel_tuning.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/resampling.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/solver.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/tempered.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/tempered.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/tuning/from_kernel_info.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/tuning/from_kernel_info.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/smc/tuning/from_particles.py` & `blackjax-nightly-1.1.1.post7/blackjax/smc/tuning/from_particles.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/types.py` & `blackjax-nightly-1.1.1.post7/blackjax/types.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/util.py` & `blackjax-nightly-1.1.1.post7/blackjax/util.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/vi/meanfield_vi.py` & `blackjax-nightly-1.1.1.post7/blackjax/vi/meanfield_vi.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def init(
     position: ArrayLikeTree,
     optimizer: GradientTransformation,
     *optimizer_args,
     **optimizer_kwargs,
 ) -> MFVIState:
     """Initialize the mean-field VI state."""
-    mu = jax.tree_map(jnp.zeros_like, position)
-    rho = jax.tree_map(lambda x: -2.0 * jnp.ones_like(x), position)
+    mu = jax.tree.map(jnp.zeros_like, position)
+    rho = jax.tree.map(lambda x: -2.0 * jnp.ones_like(x), position)
     opt_state = optimizer.init((mu, rho))
     return MFVIState(mu, rho, opt_state)
 
 
 def step(
     rng_key: PRNGKey,
     state: MFVIState,
@@ -95,15 +95,15 @@
             rho = jax.lax.stop_gradient(rho)
         logq = jax.vmap(generate_meanfield_logdensity(mu, rho))(z)
         logp = jax.vmap(logdensity_fn)(z)
         return (logq - logp).mean()
 
     elbo, elbo_grad = jax.value_and_grad(kl_divergence_fn)(parameters)
     updates, new_opt_state = optimizer.update(elbo_grad, state.opt_state, parameters)
-    new_parameters = jax.tree_map(lambda p, u: p + u, parameters, updates)
+    new_parameters = jax.tree.map(lambda p, u: p + u, parameters, updates)
     new_state = MFVIState(new_parameters[0], new_parameters[1], new_opt_state)
     return new_state, MFVIInfo(elbo)
 
 
 def sample(rng_key: PRNGKey, state: MFVIState, num_samples: int = 1):
     """Sample from the mean-field approximation."""
     return _sample(rng_key, state.mu, state.rho, num_samples)
@@ -147,26 +147,26 @@
         def sample_fn(rng_key: PRNGKey, state: MFVIState, num_samples: int):
             return cls.sample(rng_key, state, num_samples)
 
         return VIAlgorithm(init_fn, step_fn, sample_fn)
 
 
 def _sample(rng_key, mu, rho, num_samples):
-    sigma = jax.tree_map(jnp.exp, rho)
+    sigma = jax.tree.map(jnp.exp, rho)
     mu_flatten, unravel_fn = jax.flatten_util.ravel_pytree(mu)
     sigma_flat, _ = jax.flatten_util.ravel_pytree(sigma)
     flatten_sample = (
         jax.random.normal(rng_key, (num_samples,) + mu_flatten.shape) * sigma_flat
         + mu_flatten
     )
     return jax.vmap(unravel_fn)(flatten_sample)
 
 
 def generate_meanfield_logdensity(mu, rho):
-    sigma_param = jax.tree_map(jnp.exp, rho)
+    sigma_param = jax.tree.map(jnp.exp, rho)
 
     def meanfield_logdensity(position):
-        logq_pytree = jax.tree_map(jsp.stats.norm.logpdf, position, mu, sigma_param)
-        logq = jax.tree_map(jnp.sum, logq_pytree)
+        logq_pytree = jax.tree.map(jsp.stats.norm.logpdf, position, mu, sigma_param)
+        logq = jax.tree.map(jnp.sum, logq_pytree)
         return jax.tree_util.tree_reduce(jnp.add, logq)
 
     return meanfield_logdensity
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/vi/pathfinder.py` & `blackjax-nightly-1.1.1.post7/blackjax/vi/pathfinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         unravel_fn_mapped(grad_position),
         alpha,
         beta,
         gamma,
     )
 
     max_elbo_idx = jnp.argmax(elbo)
-    return jax.tree_map(lambda x: x[max_elbo_idx], pathfinder_result), PathfinderInfo(
+    return jax.tree.map(lambda x: x[max_elbo_idx], pathfinder_result), PathfinderInfo(
         pathfinder_result
     )
 
 
 def sample(
     rng_key: PRNGKey,
     state: PathfinderState,
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/vi/schrodinger_follmer.py` & `blackjax-nightly-1.1.1.post7/blackjax/vi/schrodinger_follmer.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Approximation of the drift term of the SDE
     """
 
     drift: ArrayLikeTree
 
 
 def init(example_position: ArrayLikeTree) -> SchrodingerFollmerState:
-    zero = jax.tree_map(jnp.zeros_like, example_position)
+    zero = jax.tree.map(jnp.zeros_like, example_position)
     return SchrodingerFollmerState(zero, 0.0)
 
 
 def step(
     rng_key: PRNGKey,
     state: SchrodingerFollmerState,
     logdensity_fn: Callable,
@@ -91,32 +91,32 @@
 
     ravelled_position, unravel_fn = ravel_pytree(state.position)
     scale = jnp.sqrt(1 - state.time)
 
     eps_drift = jax.random.normal(drift_key, (n_samples,) + ravelled_position.shape)
     eps_drift = jax.vmap(unravel_fn)(eps_drift)
 
-    perturbed_position = jax.tree_map(
+    perturbed_position = jax.tree.map(
         lambda a, b: a[None, ...] + scale * b, state.position, eps_drift
     )
 
     log_pdf = jax.vmap(_log_fn_corrected, in_axes=[0, None])(
         perturbed_position, logdensity_fn
     )
     log_pdf -= jnp.max(log_pdf, axis=0, keepdims=True)
     pdf = jnp.exp(log_pdf)
 
-    num = jax.tree_map(lambda a: pdf @ a, eps_drift)
+    num = jax.tree.map(lambda a: pdf @ a, eps_drift)
     den = scale * jnp.sum(pdf, axis=0)
 
-    drift = jax.tree_map(lambda a: a / den, num)
+    drift = jax.tree.map(lambda a: a / den, num)
 
     eps_sde = jax.random.normal(sde_key, ravelled_position.shape)
     eps_sde = unravel_fn(eps_sde)
-    next_position = jax.tree_map(
+    next_position = jax.tree.map(
         lambda a, b, c: a + step_size * b + step_size**0.5 * c,
         state.position,
         drift,
         eps_sde,
     )
     next_state = SchrodingerFollmerState(next_position, state.time + step_size)
     return next_state, SchrodingerFollmerInfo(drift)
@@ -147,40 +147,40 @@
         Number of samples to use to approximate the drift term
     n_samples
         Number of samples to draw
     """
     dt = 1.0 / n_steps
 
     initial_position = initial_state.position
-    initial_positions = jax.tree_map(
+    initial_positions = jax.tree.map(
         lambda a: jnp.zeros([n_samples, *a.shape], dtype=a.dtype), initial_position
     )
     initial_states = SchrodingerFollmerState(initial_positions, jnp.zeros((n_samples,)))
 
-    def body(_, carry):
-        key, states = carry
-        keys = jax.random.split(key, 1 + n_samples)
-        states, _ = jax.vmap(step, [0, 0, None, None, None])(
-            keys[1:], states, log_density_fn, dt, n_inner_samples
+    def body(i, states):
+        subkey = jax.random.fold_in(rng_key, i)
+        keys = jax.random.split(subkey, n_samples)
+        next_states, _ = jax.vmap(step, [0, 0, None, None, None])(
+            keys, states, log_density_fn, dt, n_inner_samples
         )
-        return keys[0], states
+        return next_states
 
-    _, final_states = jax.lax.fori_loop(0, n_steps, body, (rng_key, initial_states))
+    final_states = jax.lax.fori_loop(0, n_steps, body, initial_states)
 
     return final_states
 
 
 def _log_fn_corrected(position, logdensity_fn):
     """
     The Schrödinger-Föllmer algorithm requires the log-density to be given with respect to a standard Gaussian base measure
     but the log-density function passed to the algorithm in BlackJAX is typically given with respect to the Borel measure.
     This corrects the gradient of the log-density function to account for this.
     """
     log_pdf_val = logdensity_fn(position)
-    norm = jax.tree_map(lambda a: 0.5 * jnp.sum(a**2), position)
+    norm = jax.tree.map(lambda a: 0.5 * jnp.sum(a**2), position)
     norm = sum(tree_leaves(norm))
     return log_pdf_val + norm
 
 
 class schrodinger_follmer:
     """Implements the (basic) user interface for the Schrödinger-Föllmer algortithm :cite:p:`huang2021schrodingerfollmer`.
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax/vi/svgd.py` & `blackjax-nightly-1.1.1.post7/blackjax/vi/svgd.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/PKG-INFO` & `blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax-nightly
-Version: 1.1.1.post6
+Version: 1.1.1.post7
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
@@ -114,16 +114,16 @@
 
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
-for _ in range(100):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for step in range(100):
+    nuts_key = jax.random.fold_in(rng_key, step)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 See [the documentation](https://blackjax-devs.github.io/blackjax/index.html) for more examples of how to use the library: how to write inference loops for one or several chains, how to use the Stan warmup, etc.
 
 ## Philosophy
```

### Comparing `blackjax-nightly-1.1.1.post6/blackjax_nightly.egg-info/SOURCES.txt` & `blackjax-nightly-1.1.1.post7/blackjax_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/_static/blackjax.png` & `blackjax-nightly-1.1.1.post7/docs/_static/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/conf.py` & `blackjax-nightly-1.1.1.post7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/data/blackjax.png` & `blackjax-nightly-1.1.1.post7/docs/examples/data/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/data/google.csv` & `blackjax-nightly-1.1.1.post7/docs/examples/data/google.csv`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_custom_gradients.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_custom_gradients.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_metropolis_within_gibbs.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_metropolis_within_gibbs.md`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     num_samples=10_000
 )
 ```
 
 ### Check Result
 
 ```{code-cell} ipython3
-jax.tree_map(lambda x, y: jnp.max(jnp.abs(x-y)), positions, positions_general)
+jax.tree.map(lambda x, y: jnp.max(jnp.abs(x-y)), positions, positions_general)
 ```
 
 ## Developer Notes
 
 - The update method above (using `blackjax.algorithm.init()`) should work out-of-the-box for most (if not all) MCMC algorithms in BlackJAX.  However, it is not optimally efficient.  For example for the RMH update, after obtaining $\yy_{t-1}$ but before drawing $\xx_t$, the method above would calculate `RWState.log_density` to be $\log p(\xx_{t-1}, \yy_{t-1})$.  But we've already calculated this value from the previous HMC update of $\yy_{t-1} \sim p(\yy \mid \xx_{t-1})$.  So, we could save ourselves the cost of calculating the log-density twice, at the expense of a deeper understanding of the low-level components of the algorithms at hand and less generalizable code.
 
 - The general MWG kernel prototyped above should be adequate for problems with a small number of components.  However, the for-loop over the components of `state` gets unrolled by the JAX JIT compiler (as discussed [here](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#structured-control-flow-primitives)), which can cause long compilation times when the number of components is large.  To mitigate this problem, the for-loop could be replaced by a `lax.scan()` primitive.  For the sake of simplicity this approach is not fully developed here.
```

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_other_frameworks.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_other_frameworks.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_reproduce_the_blackjax_image.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_reproduce_the_blackjax_image.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,20 +135,20 @@
 ```python
 # Define the loop
 def smc_inference_loop(loop_key, smc_kernel, init_state, schedule):
     """Run the tempered SMC algorithm.
     """
 
     def body_fn(carry, lmbda):
-        carry_key, state = carry
-        carry_key, subkey = jax.random.split(carry_key)
+        i, state = carry
+        subkey = jax.random.fold_in(loop_key, i)
         new_state, info = smc_kernel(subkey, state, lmbda)
-        return (rng_key, new_state), (new_state, info)
+        return (i + 1, new_state), (new_state, info)
 
-    _, (all_samples, _) = jax.lax.scan(body_fn, (loop_key, init_state), schedule)
+    _, (all_samples, _) = jax.lax.scan(body_fn, (0, init_state), schedule)
 
     return all_samples
 
 
 # Run the SMC sampler
 blackjax_samples = smc_inference_loop(rng_key, tempered.step, initial_smc_state, lambda_schedule)
 ```
```

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_sample_multiple_chains.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_sample_multiple_chains.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_use_aesara.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_use_aesara.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_use_numpyro.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_use_numpyro.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_use_oryx.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_use_oryx.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_use_pymc.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_use_pymc.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/howto_use_tfp.md` & `blackjax-nightly-1.1.1.post7/docs/examples/howto_use_tfp.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/quickstart.md` & `blackjax-nightly-1.1.1.post7/docs/examples/quickstart.md`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/examples/scatter.gif` & `blackjax-nightly-1.1.1.post7/docs/examples/scatter.gif`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/docs/index.md` & `blackjax-nightly-1.1.1.post7/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
 step = jax.jit(nuts.step)
-for _ in range(1_000):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for i in range(1_000):
+    nuts_key = jax.random.fold_in(rng_key, i)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 :::{note}
 If you want to use Blackjax with a model implemented with a PPL, go to the related tutorials in the left menu.
 :::
```

### Comparing `blackjax-nightly-1.1.1.post6/docs/refs.bib` & `blackjax-nightly-1.1.1.post7/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/pyproject.toml` & `blackjax-nightly-1.1.1.post7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/adaptation/test_adaptation.py` & `blackjax-nightly-1.1.1.post7/tests/adaptation/test_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ).sum()
 
     num_burnin_steps = 1000
     num_results = 500
     num_chains = 16
     step_size = 0.1
 
-    init_key, warmup_key, inference_key = jax.random.split(jax.random.key(0), 3)
+    init_key, warmup_key, inference_key = jax.random.split(jax.random.key(346), 3)
 
     warmup = blackjax.chees_adaptation(
         logprob_fn, num_chains=num_chains, target_acceptance_rate=0.75
     )
 
     initial_positions = jax.random.normal(init_key, (num_chains, 2))
     (last_states, parameters), warmup_info = warmup.run(
@@ -64,8 +64,8 @@
     _, _, infos = jax.vmap(
         lambda key, state: run_inference_algorithm(key, state, algorithm, num_results)
     )(chain_keys, last_states)
 
     harmonic_mean = 1.0 / jnp.mean(1.0 / infos.acceptance_rate)
     np.testing.assert_allclose(harmonic_mean, 0.75, rtol=1e-1)
     np.testing.assert_allclose(parameters["step_size"], 1.5, rtol=2e-1)
-    np.testing.assert_allclose(infos.num_integration_steps.mean(), 15.0, rtol=3e-1)
+    np.testing.assert_array_less(infos.num_integration_steps.mean(), 15.0)
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/adaptation/test_mass_matrix.py` & `blackjax-nightly-1.1.1.post7/tests/adaptation/test_mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/adaptation/test_step_size.py` & `blackjax-nightly-1.1.1.post7/tests/adaptation/test_step_size.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_barker.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_barker.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_integrators.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_latent_gaussian.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_metrics.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_proposal.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_random_walk_without_chex.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_random_walk_without_chex.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_sampling.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,52 +453,50 @@
 
         init_position = 1.0
         init_position = sghmc.init(init_position)
         data_batch = X_data[:100, :]
         _ = sghmc.step(rng_key, init_position, data_batch, 1e-3)
 
     def test_linear_regression_sgnht(self):
-        rng_key, data_key = jax.random.split(self.key, 2)
+        step_key, data_key = jax.random.split(self.key, 2)
 
         data_size = 1000
         X_data = jax.random.normal(data_key, shape=(data_size, 5))
 
         grad_fn = blackjax.sgmcmc.grad_estimator(
             self.logprior_fn, self.loglikelihood_fn, data_size
         )
         sgnht = blackjax.sgnht(grad_fn)
 
-        _, rng_key = jax.random.split(rng_key)
         data_batch = X_data[100:200, :]
         init_position = 1.0
         data_batch = X_data[:100, :]
         init_state = sgnht.init(init_position, self.key)
-        _ = sgnht.step(rng_key, init_state, data_batch, 1e-3)
+        _ = sgnht.step(step_key, init_state, data_batch, 1e-3)
 
     def test_linear_regression_sgnhtc_cv(self):
-        rng_key, data_key = jax.random.split(self.key, 2)
+        step_key, data_key = jax.random.split(self.key, 2)
 
         data_size = 1000
         X_data = jax.random.normal(data_key, shape=(data_size, 5))
 
         centering_position = 1.0
         grad_fn = blackjax.sgmcmc.grad_estimator(
             self.logprior_fn, self.loglikelihood_fn, data_size
         )
         cv_grad_fn = blackjax.sgmcmc.gradients.control_variates(
             grad_fn, centering_position, X_data
         )
 
         sgnht = blackjax.sgnht(cv_grad_fn)
 
-        _, rng_key = jax.random.split(rng_key)
         init_position = 1.0
         data_batch = X_data[:100, :]
         init_state = sgnht.init(init_position, self.key)
-        _ = sgnht.step(rng_key, init_state, data_batch, 1e-3)
+        _ = sgnht.step(step_key, init_state, data_batch, 1e-3)
 
 
 class LatentGaussianTest(chex.TestCase):
     """Test sampling of a linear regression model."""
 
     def setUp(self):
         super().setUp()
@@ -734,15 +732,15 @@
 
 
 class MonteCarloStandardErrorTest(chex.TestCase):
     """Test sampler correctness using Monte Carlo Central Limit Theorem."""
 
     def setUp(self):
         super().setUp()
-        self.key = jax.random.key(20220203)
+        self.key = jax.random.key(8456)
 
     def generate_multivariate_target(self, rng=None):
         """Genrate a Multivariate Normal distribution as target."""
         if rng is None:
             loc = jnp.array([0.0, 3])
             scale = jnp.array([1.0, 2.0])
             rho = jnp.array(0.75)
@@ -817,15 +815,15 @@
         posterior_samples = states.position[:, -1000:]
         posterior_delta = posterior_samples - true_loc
         posterior_variance = posterior_delta**2.0
         posterior_correlation = jnp.prod(posterior_delta, axis=-1, keepdims=True) / (
             true_scale[0] * true_scale[1]
         )
 
-        _ = jax.tree_map(
+        _ = jax.tree.map(
             self.mcse_test,
             [posterior_samples, posterior_variance, posterior_correlation],
             [true_loc, true_scale**2, true_rho],
         )
 
 
 if __name__ == "__main__":
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_trajectory.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Test the trajectory integration"""
-import functools
-
 import chex
 import jax
 import jax.numpy as jnp
 import numpy as np
 from absl.testing import absltest, parameterized
 
 import blackjax.mcmc.dynamic_hmc as dynamic_hmc
@@ -71,15 +69,15 @@
             step_size,
             initial_energy,
         )
 
         assert is_diverging.item() is should_diverge
 
     def test_dynamic_progressive_equal_recursive(self):
-        rng_key = jax.random.key(23132)
+        rng_key = jax.random.key(23133)
 
         def logdensity_fn(x):
             return -((1.0 - x[0]) ** 2) - 1.5 * (x[1] - x[0] ** 2) ** 2
 
         inverse_mass_matrix = jnp.asarray([[1.0, 0.5], [0.5, 1.25]])
         (
             momentum_generator,
@@ -120,23 +118,24 @@
         buildtree_integrator = trajectory.dynamic_recursive_integration(
             integrator,
             kinetic_energy_fn,
             uturn_check_fn,
             divergence_threshold,
         )
 
-        for _ in range(50):
+        for i in range(50):
+            subkey = jax.random.fold_in(rng_key, i)
             (
-                rng_key,
+                rng_buildtree,
                 rng_direction,
                 rng_tree_depth,
                 rng_step_size,
                 rng_position,
                 rng_momentum,
-            ) = jax.random.split(rng_key, 6)
+            ) = jax.random.split(subkey, 6)
             direction = jax.random.choice(rng_direction, jnp.array([-1, 1]))
             tree_depth = jax.random.choice(rng_tree_depth, np.arange(2, 5))
             initial_state = integrators.new_integrator_state(
                 logdensity_fn,
                 jax.random.normal(rng_position, [2]),
                 jax.random.normal(rng_momentum, [2]),
             )
@@ -149,15 +148,15 @@
             (
                 proposal0,
                 trajectory0,
                 _,
                 is_diverging0,
                 has_terminated0,
             ) = trajectory_integrator(
-                rng_key,
+                rng_buildtree,
                 initial_state,
                 direction,
                 termination_state,
                 2**tree_depth,
                 step_size,
                 initial_energy,
             )
@@ -165,27 +164,24 @@
             (
                 _,
                 proposal1,
                 trajectory1,
                 is_diverging1,
                 has_terminated1,
             ) = buildtree_integrator(
-                rng_key,
+                rng_buildtree,
                 initial_state,
                 direction,
                 tree_depth,
                 step_size,
                 initial_energy,
             )
             # Assert that the trajectory being built is the same
-            jax.tree_map(
-                functools.partial(np.testing.assert_allclose, rtol=1e-5),
-                trajectory0,
-                trajectory1,
-            )
+            chex.assert_trees_all_close(trajectory0, trajectory1, rtol=1e-5)
+
             assert is_diverging0 == is_diverging1
             assert has_terminated0 == has_terminated1
             # We dont expect the proposal to be the same (even with the same PRNGKey
             # as the order of selection is different). but the property associate
             # with the full trajectory should be the same.
             np.testing.assert_allclose(proposal0.weight, proposal1.weight, rtol=1e-5)
             np.testing.assert_allclose(
@@ -283,19 +279,15 @@
         # performed using a scan
         scan_state = static_integration(initial_state, 0.1, 10)
 
         # When jitted, the number of steps is no longer static - make sure that
         # we still get the same result
         fori_state = jax.jit(static_integration)(initial_state, 0.1, 10)
 
-        jax.tree_util.tree_map(
-            functools.partial(np.testing.assert_allclose, rtol=1e-5),
-            fori_state,
-            scan_state,
-        )
+        chex.assert_trees_all_close(fori_state, scan_state, rtol=1e-5)
 
     def test_dynamic_hmc_integration_steps(self):
         rng_key = jax.random.key(0)
         num_step_key, sample_key = jax.random.split(rng_key)
         initial_position = jnp.array(3.0)
         parameters = {"step_size": 3.9, "inverse_mass_matrix": jnp.array([1.0])}
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/mcmc/test_uturn.py` & `blackjax-nightly-1.1.1.post7/tests/mcmc/test_uturn.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/optimizers/test_optimizers.py` & `blackjax-nightly-1.1.1.post7/tests/optimizers/test_optimizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         b0_flatten, unravel_fn = ravel_pytree(b0)
         objective_fn = lambda x: -fn(unravel_fn(x))
         (_, status), history = self.variant(
             functools.partial(
                 minimize_lbfgs, objective_fn, maxiter=maxiter, maxcor=maxcor
             )
         )(b0_flatten)
-        history = jax.tree_map(lambda x: x[: status.iter_num + 1], history)
+        history = jax.tree.map(lambda x: x[: status.iter_num + 1], history)
 
         # Test recover alpha
         S = jnp.diff(history.x, axis=0)
         Z = jnp.diff(history.g, axis=0)
         alpha0 = history.alpha[0]
 
         def scan_fn(alpha, val):
@@ -134,15 +134,15 @@
 
         def loss_fn(x):
             return -stats.multivariate_normal.logpdf(x, mean, cov)
 
         (result, status), history = self.variant(
             functools.partial(minimize_lbfgs, loss_fn, maxiter=50)
         )(np.zeros(nd))
-        history = jax.tree_map(lambda x: x[: status.iter_num + 1], history)
+        history = jax.tree.map(lambda x: x[: status.iter_num + 1], history)
 
         np.testing.assert_allclose(result, mean, rtol=0.01)
 
         S_partial = jnp.diff(history.x, axis=0)[-10:].T
         Z_partial = jnp.diff(history.g, axis=0)[-10:].T
         alpha = history.alpha[-1]
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/optimizers/test_pathfinder.py` & `blackjax-nightly-1.1.1.post7/tests/optimizers/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/__init__.py` & `blackjax-nightly-1.1.1.post7/tests/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_inner_kernel_tuning.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_inner_kernel_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,26 +309,26 @@
             target_ess=0.5,
         )
         init_state = init(init_particles)
         smc_kernel = self.variant(step)
 
         def inference_loop(kernel, rng_key, initial_state):
             def cond(carry):
-                state, key = carry
+                _, state = carry
                 return state.sampler_state.lmbda < 1
 
             def body(carry):
-                state, op_key = carry
-                op_key, subkey = jax.random.split(op_key, 2)
+                i, state = carry
+                subkey = jax.random.fold_in(rng_key, i)
                 state, _ = kernel(subkey, state)
-                return state, op_key
+                return i + 1, state
 
-            return jax.lax.while_loop(cond, body, (initial_state, rng_key))
+            return jax.lax.while_loop(cond, body, (0, initial_state))
 
-        state, _ = inference_loop(smc_kernel, self.key, init_state)
+        _, state = inference_loop(smc_kernel, self.key, init_state)
 
         assert state.parameter_override["inverse_mass_matrix"].shape == (100, 2, 2)
         self.assert_linear_regression_test_case(state.sampler_state)
 
     @chex.all_variants(with_pmap=False)
     def test_with_tempered_smc(self):
         num_tempering_steps = 10
@@ -369,20 +369,20 @@
 
         init_state = init(init_particles)
         smc_kernel = self.variant(step)
 
         lambda_schedule = np.logspace(-5, 0, num_tempering_steps)
 
         def body_fn(carry, lmbda):
-            rng_key, state = carry
-            rng_key, subkey = jax.random.split(rng_key)
+            i, state = carry
+            subkey = jax.random.fold_in(self.key, i)
             new_state, info = smc_kernel(subkey, state, lmbda=lmbda)
-            return (rng_key, new_state), (new_state, info)
+            return (i + 1, new_state), (new_state, info)
 
-        (_, result), _ = jax.lax.scan(body_fn, (self.key, init_state), lambda_schedule)
+        (_, result), _ = jax.lax.scan(body_fn, (0, init_state), lambda_schedule)
         self.assert_linear_regression_test_case(result.sampler_state)
 
 
 class ParticlesAsRowsTest(unittest.TestCase):
     def test_particles_as_rows(self):
         n_particles = 1000
         test_particles = {
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_kernel_compatibility.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_kernel_compatibility.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_resampling.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_smc.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_smc.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_smc_ess.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_smc_ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_solver.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/smc/test_tempered_smc.py` & `blackjax-nightly-1.1.1.post7/tests/smc/test_tempered_smc.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 def inference_loop(kernel, rng_key, initial_state):
     def cond(carry):
         _, state, *_ = carry
         return state.lmbda < 1
 
     def body(carry):
-        i, state, op_key, curr_loglikelihood = carry
-        op_key, subkey = jax.random.split(op_key, 2)
+        i, state, curr_loglikelihood = carry
+        subkey = jax.random.fold_in(rng_key, i)
         state, info = kernel(subkey, state)
-        return i + 1, state, op_key, curr_loglikelihood + info.log_likelihood_increment
+        return i + 1, state, curr_loglikelihood + info.log_likelihood_increment
 
-    total_iter, final_state, _, log_likelihood = jax.lax.while_loop(
-        cond, body, (0, initial_state, rng_key, 0.0)
+    total_iter, final_state, log_likelihood = jax.lax.while_loop(
+        cond, body, (0, initial_state, 0.0)
     )
 
     return total_iter, final_state, log_likelihood
 
 
 class TemperedSMCTest(SMCLinearRegressionTestCase):
     """Test posterior mean estimate."""
@@ -132,20 +132,20 @@
             resampling.systematic,
             10,
         )
         init_state = tempering.init(init_particles)
         smc_kernel = self.variant(tempering.step)
 
         def body_fn(carry, lmbda):
-            rng_key, state = carry
-            rng_key, subkey = jax.random.split(rng_key)
+            i, state = carry
+            subkey = jax.random.fold_in(self.key, i)
             new_state, info = smc_kernel(subkey, state, lmbda)
-            return (rng_key, new_state), (new_state, info)
+            return (i + 1, new_state), (new_state, info)
 
-        (_, result), _ = jax.lax.scan(body_fn, (self.key, init_state), lambda_schedule)
+        (_, result), _ = jax.lax.scan(body_fn, (0, init_state), lambda_schedule)
         self.assert_linear_regression_test_case(result)
 
 
 def normal_logdensity_fn(x, chol_cov):
     """minus log-density of a centered multivariate normal distribution"""
     dim = chol_cov.shape[0]
     y = jax.scipy.linalg.solve_triangular(chol_cov, x, lower=True)
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/test_benchmarks.py` & `blackjax-nightly-1.1.1.post7/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/test_compilation.py` & `blackjax-nightly-1.1.1.post7/tests/test_compilation.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             logdensity_fn,
             step_size=1e-2,
             inverse_mass_matrix=jnp.array([1.0]),
             num_integration_steps=10,
         )
         step = jax.jit(kernel.step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = step(sample_key, state)
 
     def test_nuts(self):
         """Count the number of times the logdensity is compiled when using NUTS.
 
         The logdensity is compiled twice: when initializing the state and when
         compiling the kernel.
@@ -62,16 +62,16 @@
         state = blackjax.nuts.init(1.0, logdensity_fn)
 
         kernel = blackjax.nuts(
             logdensity_fn, step_size=1e-2, inverse_mass_matrix=jnp.array([1.0])
         )
         step = jax.jit(kernel.step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = step(sample_key, state)
 
     def test_hmc_warmup(self):
         """Count the number of times the logdensity is compiled when using window
         adaptation to adapt the value of the step size and the inverse mass
         matrix for the HMC algorithm.
 
@@ -90,16 +90,16 @@
             logdensity_fn=logdensity_fn,
             target_acceptance_rate=0.8,
             num_integration_steps=10,
         )
         (state, parameters), _ = warmup.run(rng_key, 1.0, num_steps=100)
         kernel = jax.jit(blackjax.hmc(logdensity_fn, **parameters).step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = kernel(sample_key, state)
 
     def test_nuts_warmup(self):
         """Count the number of times the logdensity is compiled when using window
         adaptation to adapt the value of the step size and the inverse mass
         matrix for the NUTS algorithm.
 
@@ -117,14 +117,14 @@
             algorithm=blackjax.nuts,
             logdensity_fn=logdensity_fn,
             target_acceptance_rate=0.8,
         )
         (state, parameters), _ = warmup.run(rng_key, 1.0, num_steps=100)
         step = jax.jit(blackjax.nuts(logdensity_fn, **parameters).step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = step(sample_key, state)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/test_diagnostics.py` & `blackjax-nightly-1.1.1.post7/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/test_util.py` & `blackjax-nightly-1.1.1.post7/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/vi/test_meanfield_vi.py` & `blackjax-nightly-1.1.1.post7/tests/vi/test_meanfield_vi.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,20 @@
         num_samples = 500
 
         optimizer = optax.sgd(1e-2)
         mfvi = blackjax.meanfield_vi(logdensity_fn, optimizer, num_samples)
         state = mfvi.init(initial_position)
 
         rng_key = self.key
-        for _ in range(num_steps):
-            rng_key, subkey = jax.random.split(rng_key)
+        for i in range(num_steps):
+            subkey = jax.random.fold_in(rng_key, i)
             state, _ = jax.jit(mfvi.step)(subkey, state)
 
         loc_1, loc_2 = state.mu["x_1"], state.mu["x_2"]
-        scale = jax.tree_map(jnp.exp, state.rho)
+        scale = jax.tree.map(jnp.exp, state.rho)
         scale_1, scale_2 = scale["x_1"], scale["x_2"]
         self.assertAlmostEqual(loc_1, ground_truth[0][0], delta=0.01)
         self.assertAlmostEqual(scale_1, ground_truth[0][1], delta=0.01)
         self.assertAlmostEqual(loc_2, ground_truth[1][0], delta=0.01)
         self.assertAlmostEqual(scale_2, ground_truth[1][1], delta=0.01)
```

### Comparing `blackjax-nightly-1.1.1.post6/tests/vi/test_schrodinger_follmer.py` & `blackjax-nightly-1.1.1.post7/tests/vi/test_schrodinger_follmer.py`

 * *Files identical despite different names*

### Comparing `blackjax-nightly-1.1.1.post6/tests/vi/test_svgd.py` & `blackjax-nightly-1.1.1.post7/tests/vi/test_svgd.py`

 * *Files identical despite different names*

