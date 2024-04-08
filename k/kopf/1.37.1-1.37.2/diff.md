# Comparing `tmp/kopf-1.37.1.tar.gz` & `tmp/kopf-1.37.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopf-1.37.1.tar", last modified: Sat Jan 20 17:31:36 2024, max compression
+gzip compressed data, was "kopf-1.37.2.tar", last modified: Mon Apr  8 12:59:33 2024, max compression
```

## Comparing `kopf-1.37.1.tar` & `kopf-1.37.2.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.897913 kopf-1.37.1/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-20 17:31:24.000000 kopf-1.37.1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.841913 kopf-1.37.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.841913 kopf-1.37.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/ISSUE_TEMPLATE/feature-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/ISSUE_TEMPLATE/question.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.841913 kopf-1.37.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-01-20 17:31:24.000000 kopf-1.37.1/.github/workflows/thorough.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-20 17:31:24.000000 kopf-1.37.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-01-20 17:31:24.000000 kopf-1.37.1/.importlinter
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-20 17:31:24.000000 kopf-1.37.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-01-20 17:31:24.000000 kopf-1.37.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-20 17:31:24.000000 kopf-1.37.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-01-20 17:31:24.000000 kopf-1.37.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-01-20 17:31:24.000000 kopf-1.37.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-20 17:31:24.000000 kopf-1.37.1/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-01-20 17:31:24.000000 kopf-1.37.1/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-20 17:31:24.000000 kopf-1.37.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-20 17:31:24.000000 kopf-1.37.1/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-01-20 17:31:36.897913 kopf-1.37.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-01-20 17:31:24.000000 kopf-1.37.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-20 17:31:24.000000 kopf-1.37.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-01-20 17:31:24.000000 kopf-1.37.1/_importlinter_conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.849913 kopf-1.37.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)    30976 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/admission.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (127)   815980 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/architecture-layers.png
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/architecture-layers.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/async.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21376 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/continuity.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/daemons.rst
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/deployment-depl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/deployment-rbac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/hierarchies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/idempotence.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12008 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/memos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/minikube.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/naming.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/peering.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/probing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/reconciliation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/scopes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/shutdown.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/startup.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/timers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/tips-and-tricks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/vision.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/docs/walkthrough/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/cleanup.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/creation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/deletion.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/diffs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/prerequisites.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/problem.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/starting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-01-20 17:31:24.000000 kopf-1.37.1/docs/walkthrough/updates.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/01-minimal/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/01-minimal/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/01-minimal/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/02-children/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/02-children/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/02-children/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/03-exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/03-exceptions/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/03-exceptions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/04-events/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/04-events/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/04-events/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/05-handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/05-handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/05-handlers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/06-peering/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/06-peering/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/06-peering/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/07-subhandlers/
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/07-subhandlers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/07-subhandlers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.853913 kopf-1.37.1/examples/08-events/
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/08-events/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/08-events/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/09-testing/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/09-testing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/09-testing/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/09-testing/test_example_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/10-builtins/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/10-builtins/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/10-builtins/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/10-builtins/test_example_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/11-filtering-handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/11-filtering-handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/11-filtering-handlers/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/11-filtering-handlers/test_example_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/12-embedded/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/12-embedded/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/12-embedded/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/12-embedded/test_nothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/13-hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/13-hooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/13-hooks/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/14-daemons/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/14-daemons/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/15-timers/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/15-timers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/16-indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/16-indexing/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/17-admission/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/17-admission/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/examples/99-all-at-once/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/99-all-at-once/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/99-all-at-once/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/crd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/obj.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-20 17:31:24.000000 kopf-1.37.1/examples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.857913 kopf-1.37.1/kopf/
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.861913 kopf-1.37.1/kopf/_cogs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.861913 kopf-1.37.1/kopf/_cogs/aiokits/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aioadapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aiobindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aioenums.py
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aiotasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aiotime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aiotoggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/aiokits/aiovalues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.861913 kopf-1.37.1/kopf/_cogs/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/creating.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/fetching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/scanning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/clients/watching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.861913 kopf-1.37.1/kopf/_cogs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/configs/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/configs/conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/configs/diffbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/configs/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.865913 kopf-1.37.1/kopf/_cogs/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/helpers/hostnames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/helpers/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/helpers/thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/helpers/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/helpers/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.865913 kopf-1.37.1/kopf/_cogs/structs/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/bodies.py
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/ephemera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/finalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    22215 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/references.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_cogs/structs/reviews.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.865913 kopf-1.37.1/kopf/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.869913 kopf-1.37.1/kopf/_core/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/lifecycles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/progression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/actions/throttlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.869913 kopf-1.37.1/kopf/_core/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)    19663 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/admission.py
--rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/daemons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/peering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/posting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/engines/probing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.869913 kopf-1.37.1/kopf/_core/intents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/causes.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/piggybacking.py
--rw-r--r--   0 runner    (1001) docker     (127)    21832 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/intents/stoppers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.869913 kopf-1.37.1/kopf/_core/reactor/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/queueing.py
--rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/running.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_core/reactor/subhandling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.873913 kopf-1.37.1/kopf/_kits/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_kits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_kits/hierarchies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_kits/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_kits/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_kits/webhacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30321 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/_kits/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43299 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/on.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-20 17:31:24.000000 kopf-1.37.1/kopf/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/kopf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 17:31:36.000000 kopf-1.37.1/kopf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-20 17:31:24.000000 kopf-1.37.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-20 17:31:24.000000 kopf-1.37.1/peering.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-20 17:31:24.000000 kopf-1.37.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-20 17:31:24.000000 kopf-1.37.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 17:31:36.897913 kopf-1.37.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-20 17:31:24.000000 kopf-1.37.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.873913 kopf-1.37.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/admission/
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_admission_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_admission_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_jsonpatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_managed_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_serving_ephemeral_memos.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_serving_handler_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_serving_kwargs_passthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_serving_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_webhook_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_webhook_ngrok.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/admission/test_webhook_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/apis/
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/apis/test_api_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/apis/test_default_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/apis/test_error_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/apis/test_iterjsonlines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_connectioninfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_login_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_login_serviceaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_reauthentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_tempfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/authentication/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/basic-structs/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/basic-structs/test_causes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/basic-structs/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/basic-structs/test_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/basic-structs/test_memos.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/basic-structs/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/causation/
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/causation/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/causation/test_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/cli/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/cli/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/cli/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/cli/test_preloading.py
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/dicts/
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_cherrypicking.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_dictviews.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_ensuring.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_removing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_resolving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/dicts/test_walking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/diffs/
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/diffs/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/diffs/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/diffs/test_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.877913 kopf-1.37.1/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/e2e/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.881913 kopf-1.37.1/tests/handling/
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.881913 kopf-1.37.1/tests/handling/daemons/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_daemon_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_daemon_filtration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_daemon_rematching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_daemon_spawning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_daemon_termination.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_timer_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_timer_filtration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_timer_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/daemons/test_timer_triggering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.881913 kopf-1.37.1/tests/handling/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/indexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/indexing/test_blocking_until_indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/indexing/test_index_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/indexing/test_index_population.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.881913 kopf-1.37.1/tests/handling/subhandling/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/subhandling/test_subhandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_activity_triggering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_cause_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_cause_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_delays.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_multistep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_no_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_parametrization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_retrying_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/handling/test_timing_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/hierarchies/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/test_contextual_owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/test_labelling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/test_name_harmonizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/test_namespace_adjusting.py
--rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/test_owner_referencing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/hierarchies/test_type_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/invocations/
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/invocations/test_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_creating.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_list_objs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_scanning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_watching_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_watching_continuously.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_watching_infinitely.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/k8s/test_watching_with_freezes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/lifecycles/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/lifecycles/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/lifecycles/test_global_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/lifecycles/test_handler_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/lifecycles/test_real_invocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/logging/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/logging/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/logging/test_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/observation/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/observation/test_processing_of_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/observation/test_processing_of_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/observation/test_revision_of_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/observation/test_revision_of_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.885913 kopf-1.37.1/tests/orchestration/
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/orchestration/test_task_adjustments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.889913 kopf-1.37.1/tests/peering/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/test_freeze_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/test_id_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/test_keepalive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/test_peer_patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/test_peers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/peering/test_resource_guessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.889913 kopf-1.37.1/tests/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/persistence/test_annotations_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/persistence/test_essences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/persistence/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (127)    33051 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/persistence/test_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/persistence/test_storing_of_diffbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/persistence/test_storing_of_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.889913 kopf-1.37.1/tests/posting/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/posting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/posting/test_log2k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/posting/test_poster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/posting/test_threadsafety.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.889913 kopf-1.37.1/tests/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/primitives/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/primitives/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/primitives/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/primitives/test_toggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/primitives/test_togglesets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.889913 kopf-1.37.1/tests/reactor/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/reactor/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/reactor/test_patching_inconsistencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/reactor/test_queueing.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/reactor/test_uids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.889913 kopf-1.37.1/tests/references/
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/references/test_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/references/test_namespace_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/references/test_namespace_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/references/test_selector_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/references/test_selector_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/references/test_selector_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/tests/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23936 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_default_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_handler_getting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_id_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    29077 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_matching_for_changing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17265 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_matching_for_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17733 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_matching_for_spawning.py
--rw-r--r--   0 runner    (1001) docker     (127)    17321 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_matching_for_watching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_matching_of_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_matching_of_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_requires_finalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_resumes_mixed_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/registries/test_subhandlers_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/tests/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/settings/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/settings/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_absent_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_filtering_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_finalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_it.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_liveness.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/testing/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/tests/timing/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/timing/test_sleeping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/timing/test_throttling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.837913 kopf-1.37.1/tests/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/tests/utilities/aiotasks/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/utilities/aiotasks/test_coro_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/utilities/aiotasks/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/utilities/aiotasks/test_task_guarding.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/utilities/aiotasks/test_task_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/utilities/aiotasks/test_task_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-20 17:31:24.000000 kopf-1.37.1/tests/utilities/aiotasks/test_task_waiting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 17:31:36.893913 kopf-1.37.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-01-20 17:31:24.000000 kopf-1.37.1/tools/install-kind.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-01-20 17:31:24.000000 kopf-1.37.1/tools/install-kubectl.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-01-20 17:31:24.000000 kopf-1.37.1/tools/install-minikube.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.742808 kopf-1.37.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 12:59:19.000000 kopf-1.37.2/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.682809 kopf-1.37.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.682809 kopf-1.37.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/ISSUE_TEMPLATE/feature-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/ISSUE_TEMPLATE/question.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.686809 kopf-1.37.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-08 12:59:19.000000 kopf-1.37.2/.github/workflows/thorough.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 12:59:19.000000 kopf-1.37.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-08 12:59:19.000000 kopf-1.37.2/.importlinter
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 12:59:19.000000 kopf-1.37.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-08 12:59:19.000000 kopf-1.37.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-08 12:59:19.000000 kopf-1.37.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-08 12:59:19.000000 kopf-1.37.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-08 12:59:19.000000 kopf-1.37.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-08 12:59:19.000000 kopf-1.37.2/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-08 12:59:19.000000 kopf-1.37.2/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-08 12:59:19.000000 kopf-1.37.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 12:59:19.000000 kopf-1.37.2/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-04-08 12:59:33.738808 kopf-1.37.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-08 12:59:19.000000 kopf-1.37.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 12:59:19.000000 kopf-1.37.2/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-08 12:59:19.000000 kopf-1.37.2/_importlinter_conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.690809 kopf-1.37.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)    30976 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/admission.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   815980 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/architecture-layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/architecture-layers.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21376 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/continuity.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/daemons.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/deployment-depl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/deployment-rbac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/hierarchies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/idempotence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12008 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/memos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/minikube.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/naming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/peering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/probing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/reconciliation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/scopes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/shutdown.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/startup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/timers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/tips-and-tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/vision.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/docs/walkthrough/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/cleanup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/creation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/deletion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/diffs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/prerequisites.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/problem.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/starting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-08 12:59:19.000000 kopf-1.37.2/docs/walkthrough/updates.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/01-minimal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/01-minimal/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/01-minimal/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/02-children/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/02-children/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/02-children/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/03-exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/03-exceptions/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/03-exceptions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/04-events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/04-events/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/04-events/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/05-handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/05-handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/05-handlers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/06-peering/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/06-peering/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/06-peering/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/07-subhandlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/07-subhandlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/07-subhandlers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.694809 kopf-1.37.2/examples/08-events/
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/08-events/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/08-events/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/09-testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/09-testing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/09-testing/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/09-testing/test_example_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/10-builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/10-builtins/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/10-builtins/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/10-builtins/test_example_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/11-filtering-handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/11-filtering-handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/11-filtering-handlers/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/11-filtering-handlers/test_example_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/12-embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/12-embedded/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/12-embedded/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/12-embedded/test_nothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/13-hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/13-hooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/13-hooks/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/14-daemons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/14-daemons/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/15-timers/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/15-timers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/16-indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/16-indexing/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/17-admission/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/17-admission/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/examples/99-all-at-once/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/99-all-at-once/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/99-all-at-once/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/crd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/obj.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 12:59:19.000000 kopf-1.37.2/examples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.698809 kopf-1.37.2/kopf/
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.702808 kopf-1.37.2/kopf/_cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.702808 kopf-1.37.2/kopf/_cogs/aiokits/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aioadapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aiobindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aioenums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aiotasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aiotime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aiotoggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/aiokits/aiovalues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.702808 kopf-1.37.2/kopf/_cogs/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/creating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/scanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/clients/watching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.702808 kopf-1.37.2/kopf/_cogs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/configs/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/configs/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/configs/diffbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/configs/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.706809 kopf-1.37.2/kopf/_cogs/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/helpers/hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/helpers/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/helpers/thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/helpers/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/helpers/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.706809 kopf-1.37.2/kopf/_cogs/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/bodies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/ephemera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22215 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_cogs/structs/reviews.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.706809 kopf-1.37.2/kopf/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.706809 kopf-1.37.2/kopf/_core/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/lifecycles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/progression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/actions/throttlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.710809 kopf-1.37.2/kopf/_core/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19663 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/admission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/peering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/posting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/engines/probing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.710809 kopf-1.37.2/kopf/_core/intents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/causes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/piggybacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21832 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/intents/stoppers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.710809 kopf-1.37.2/kopf/_core/reactor/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/queueing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_core/reactor/subhandling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.710809 kopf-1.37.2/kopf/_kits/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_kits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_kits/hierarchies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_kits/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_kits/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_kits/webhacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30321 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/_kits/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43299 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/on.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 12:59:19.000000 kopf-1.37.2/kopf/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/kopf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:59:33.000000 kopf-1.37.2/kopf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 12:59:19.000000 kopf-1.37.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 12:59:19.000000 kopf-1.37.2/peering.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 12:59:19.000000 kopf-1.37.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 12:59:19.000000 kopf-1.37.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:59:33.742808 kopf-1.37.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-08 12:59:19.000000 kopf-1.37.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.714809 kopf-1.37.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.714809 kopf-1.37.2/tests/admission/
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_admission_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_admission_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_jsonpatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_managed_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_serving_ephemeral_memos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_serving_handler_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_serving_kwargs_passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_serving_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_webhook_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_webhook_ngrok.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/admission/test_webhook_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.714809 kopf-1.37.2/tests/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/apis/test_api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/apis/test_default_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/apis/test_error_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/apis/test_iterjsonlines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.718809 kopf-1.37.2/tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_connectioninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_login_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_login_serviceaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_reauthentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_tempfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/authentication/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.718809 kopf-1.37.2/tests/basic-structs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/basic-structs/test_causes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/basic-structs/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/basic-structs/test_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/basic-structs/test_memos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/basic-structs/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.718809 kopf-1.37.2/tests/causation/
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/causation/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/causation/test_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.718809 kopf-1.37.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/cli/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/cli/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/cli/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/cli/test_preloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.718809 kopf-1.37.2/tests/dicts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_cherrypicking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_dictviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_ensuring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_removing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_resolving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/dicts/test_walking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.722808 kopf-1.37.2/tests/diffs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/diffs/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/diffs/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/diffs/test_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.722808 kopf-1.37.2/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/e2e/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.722808 kopf-1.37.2/tests/handling/
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.726808 kopf-1.37.2/tests/handling/daemons/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_daemon_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_daemon_filtration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_daemon_rematching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_daemon_spawning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_daemon_termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_timer_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_timer_filtration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_timer_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/daemons/test_timer_triggering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.726808 kopf-1.37.2/tests/handling/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/indexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/indexing/test_blocking_until_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/indexing/test_index_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/indexing/test_index_population.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.726808 kopf-1.37.2/tests/handling/subhandling/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/subhandling/test_subhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_activity_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_cause_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_cause_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_delays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_multistep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_no_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_parametrization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_retrying_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/handling/test_timing_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.726808 kopf-1.37.2/tests/hierarchies/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/test_contextual_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/test_labelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/test_name_harmonizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/test_namespace_adjusting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/test_owner_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/hierarchies/test_type_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.726808 kopf-1.37.2/tests/invocations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/invocations/test_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.726808 kopf-1.37.2/tests/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_creating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_list_objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_scanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_watching_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_watching_continuously.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_watching_infinitely.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/k8s/test_watching_with_freezes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.730808 kopf-1.37.2/tests/lifecycles/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/lifecycles/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/lifecycles/test_global_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/lifecycles/test_handler_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/lifecycles/test_real_invocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.730808 kopf-1.37.2/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/logging/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/logging/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/logging/test_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.730808 kopf-1.37.2/tests/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/observation/test_processing_of_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/observation/test_processing_of_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/observation/test_revision_of_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/observation/test_revision_of_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.730808 kopf-1.37.2/tests/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/orchestration/test_task_adjustments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.730808 kopf-1.37.2/tests/peering/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/test_freeze_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/test_id_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/test_keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/test_peer_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/test_peers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/peering/test_resource_guessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.730808 kopf-1.37.2/tests/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/persistence/test_annotations_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/persistence/test_essences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/persistence/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33051 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/persistence/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/persistence/test_storing_of_diffbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/persistence/test_storing_of_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.734809 kopf-1.37.2/tests/posting/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/posting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/posting/test_log2k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/posting/test_poster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/posting/test_threadsafety.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.734809 kopf-1.37.2/tests/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/primitives/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/primitives/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/primitives/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/primitives/test_toggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/primitives/test_togglesets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.734809 kopf-1.37.2/tests/reactor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/reactor/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/reactor/test_patching_inconsistencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/reactor/test_queueing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/reactor/test_uids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.734809 kopf-1.37.2/tests/references/
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/references/test_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/references/test_namespace_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/references/test_namespace_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/references/test_selector_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/references/test_selector_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/references/test_selector_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/tests/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23936 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_default_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_handler_getting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_id_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29077 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_matching_for_changing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17265 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_matching_for_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17733 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_matching_for_spawning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17321 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_matching_for_watching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_matching_of_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_matching_of_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_requires_finalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_resumes_mixed_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/registries/test_subhandlers_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/tests/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/settings/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/settings/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_absent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_filtering_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_it.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_liveness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/testing/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/tests/timing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/timing/test_sleeping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/timing/test_throttling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.678809 kopf-1.37.2/tests/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/tests/utilities/aiotasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/utilities/aiotasks/test_coro_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/utilities/aiotasks/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/utilities/aiotasks/test_task_guarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/utilities/aiotasks/test_task_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/utilities/aiotasks/test_task_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 12:59:19.000000 kopf-1.37.2/tests/utilities/aiotasks/test_task_waiting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:59:33.738808 kopf-1.37.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-04-08 12:59:19.000000 kopf-1.37.2/tools/install-kind.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-04-08 12:59:19.000000 kopf-1.37.2/tools/install-kubectl.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-04-08 12:59:19.000000 kopf-1.37.2/tools/install-minikube.sh
```

### Comparing `kopf-1.37.1/.github/ISSUE_TEMPLATE/bug-report.yaml` & `kopf-1.37.2/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.github/ISSUE_TEMPLATE/feature-request.yaml` & `kopf-1.37.2/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.github/ISSUE_TEMPLATE/question.yaml` & `kopf-1.37.2/.github/ISSUE_TEMPLATE/question.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.github/workflows/ci.yaml` & `kopf-1.37.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.github/workflows/codeql.yml` & `kopf-1.37.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.github/workflows/publish.yaml` & `kopf-1.37.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.github/workflows/thorough.yaml` & `kopf-1.37.2/.github/workflows/thorough.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.importlinter` & `kopf-1.37.2/.importlinter`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/.pre-commit-config.yaml` & `kopf-1.37.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/CODE_OF_CONDUCT.md` & `kopf-1.37.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/CONTRIBUTING.md` & `kopf-1.37.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/CONTRIBUTORS.md` & `kopf-1.37.2/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/DEVELOPMENT.md` & `kopf-1.37.2/DEVELOPMENT.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 To develop the framework and the operators in an isolated Kubernetes cluster,
 use [minikube](https://github.com/kubernetes/minikube):
 
 MacOS:
 
 ```bash
-brew install docker-machine-driver-hyperkit
-sudo chown root:wheel /usr/local/opt/docker-machine-driver-hyperkit/bin/docker-machine-driver-hyperkit
-sudo chmod u+s /usr/local/opt/docker-machine-driver-hyperkit/bin/docker-machine-driver-hyperkit
+brew install minikube
+brew install hyperkit
 
-brew cask install minikube
-minikube config set vm-driver hyperkit
+minikube config set driver hyperkit
 ```
 
 Start the minikube cluster:
 
 ```bash
 minikube start
 minikube dashboard
```

### Comparing `kopf-1.37.1/LICENSE` & `kopf-1.37.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/PKG-INFO` & `kopf-1.37.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopf
-Version: 1.37.1
+Version: 1.37.2
 Summary: Kubernetes Operator Pythonic Framework (Kopf)
 Home-page: https://github.com/nolar/kopf
 Author: Sergey Vasilyev
 Author-email: nolar@nolar.info
 Maintainer: Sergey Vasilyev
 Maintainer-email: nolar@nolar.info
 License: MIT
```

### Comparing `kopf-1.37.1/README.md` & `kopf-1.37.2/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/_importlinter_conditional.py` & `kopf-1.37.2/_importlinter_conditional.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/admission.rst` & `kopf-1.37.2/docs/admission.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/alternatives.rst` & `kopf-1.37.2/docs/alternatives.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/architecture-layers.png` & `kopf-1.37.2/docs/architecture-layers.png`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/architecture-layers.xml` & `kopf-1.37.2/docs/architecture-layers.xml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/architecture.rst` & `kopf-1.37.2/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/async.rst` & `kopf-1.37.2/docs/async.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/authentication.rst` & `kopf-1.37.2/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/cli.rst` & `kopf-1.37.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/concepts.rst` & `kopf-1.37.2/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/conf.py` & `kopf-1.37.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/configuration.rst` & `kopf-1.37.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/continuity.rst` & `kopf-1.37.2/docs/continuity.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/contributing.rst` & `kopf-1.37.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/daemons.rst` & `kopf-1.37.2/docs/daemons.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/deployment-rbac.yaml` & `kopf-1.37.2/docs/deployment-rbac.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/deployment.rst` & `kopf-1.37.2/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/embedding.rst` & `kopf-1.37.2/docs/embedding.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/errors.rst` & `kopf-1.37.2/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/events.rst` & `kopf-1.37.2/docs/events.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/filters.rst` & `kopf-1.37.2/docs/filters.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/handlers.rst` & `kopf-1.37.2/docs/handlers.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/hierarchies.rst` & `kopf-1.37.2/docs/hierarchies.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/idempotence.rst` & `kopf-1.37.2/docs/idempotence.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/index.rst` & `kopf-1.37.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/indexing.rst` & `kopf-1.37.2/docs/indexing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/install.rst` & `kopf-1.37.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/kwargs.rst` & `kopf-1.37.2/docs/kwargs.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/loading.rst` & `kopf-1.37.2/docs/loading.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/memos.rst` & `kopf-1.37.2/docs/memos.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/peering.rst` & `kopf-1.37.2/docs/peering.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/probing.rst` & `kopf-1.37.2/docs/probing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/reconciliation.rst` & `kopf-1.37.2/docs/reconciliation.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/resources.rst` & `kopf-1.37.2/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/results.rst` & `kopf-1.37.2/docs/results.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/scopes.rst` & `kopf-1.37.2/docs/scopes.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/shutdown.rst` & `kopf-1.37.2/docs/shutdown.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/startup.rst` & `kopf-1.37.2/docs/startup.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/testing.rst` & `kopf-1.37.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/timers.rst` & `kopf-1.37.2/docs/timers.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/tips-and-tricks.rst` & `kopf-1.37.2/docs/tips-and-tricks.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/troubleshooting.rst` & `kopf-1.37.2/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/vision.rst` & `kopf-1.37.2/docs/vision.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/creation.rst` & `kopf-1.37.2/docs/walkthrough/creation.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/deletion.rst` & `kopf-1.37.2/docs/walkthrough/deletion.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/diffs.rst` & `kopf-1.37.2/docs/walkthrough/diffs.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/prerequisites.rst` & `kopf-1.37.2/docs/walkthrough/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/problem.rst` & `kopf-1.37.2/docs/walkthrough/problem.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/resources.rst` & `kopf-1.37.2/docs/walkthrough/resources.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/starting.rst` & `kopf-1.37.2/docs/walkthrough/starting.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/docs/walkthrough/updates.rst` & `kopf-1.37.2/docs/walkthrough/updates.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/01-minimal/README.md` & `kopf-1.37.2/examples/01-minimal/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/02-children/README.md` & `kopf-1.37.2/examples/02-children/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/02-children/example.py` & `kopf-1.37.2/examples/02-children/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/03-exceptions/README.md` & `kopf-1.37.2/examples/03-exceptions/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/03-exceptions/example.py` & `kopf-1.37.2/examples/03-exceptions/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/04-events/README.md` & `kopf-1.37.2/examples/04-events/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/04-events/example.py` & `kopf-1.37.2/examples/04-events/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/05-handlers/README.md` & `kopf-1.37.2/examples/05-handlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/05-handlers/example.py` & `kopf-1.37.2/examples/05-handlers/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/06-peering/README.md` & `kopf-1.37.2/examples/06-peering/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/07-subhandlers/README.md` & `kopf-1.37.2/examples/07-subhandlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/08-events/README.md` & `kopf-1.37.2/examples/08-events/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/09-testing/test_example_09.py` & `kopf-1.37.2/examples/09-testing/test_example_09.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/10-builtins/README.md` & `kopf-1.37.2/examples/10-builtins/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/10-builtins/example.py` & `kopf-1.37.2/examples/10-builtins/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/10-builtins/test_example_10.py` & `kopf-1.37.2/examples/10-builtins/test_example_10.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/11-filtering-handlers/README.md` & `kopf-1.37.2/examples/11-filtering-handlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/11-filtering-handlers/example.py` & `kopf-1.37.2/examples/11-filtering-handlers/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/11-filtering-handlers/test_example_11.py` & `kopf-1.37.2/examples/11-filtering-handlers/test_example_11.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/12-embedded/README.md` & `kopf-1.37.2/examples/12-embedded/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/12-embedded/example.py` & `kopf-1.37.2/examples/12-embedded/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/13-hooks/README.md` & `kopf-1.37.2/examples/13-hooks/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/13-hooks/example.py` & `kopf-1.37.2/examples/13-hooks/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/14-daemons/example.py` & `kopf-1.37.2/examples/14-daemons/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/16-indexing/example.py` & `kopf-1.37.2/examples/16-indexing/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/17-admission/example.py` & `kopf-1.37.2/examples/17-admission/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/99-all-at-once/example.py` & `kopf-1.37.2/examples/99-all-at-once/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/examples/crd.yaml` & `kopf-1.37.2/examples/crd.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/__init__.py` & `kopf-1.37.2/kopf/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aioadapters.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aioadapters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aiobindings.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aiobindings.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aioenums.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aioenums.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aiotasks.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aiotasks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aiotime.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aiotime.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aiotoggles.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aiotoggles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/aiokits/aiovalues.py` & `kopf-1.37.2/kopf/_cogs/aiokits/aiovalues.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/__init__.py` & `kopf-1.37.2/kopf/_cogs/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/api.py` & `kopf-1.37.2/kopf/_cogs/clients/api.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/auth.py` & `kopf-1.37.2/kopf/_cogs/clients/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import functools
 import os
 import ssl
 import tempfile
 from contextvars import ContextVar
-from typing import Any, Callable, Dict, Iterator, Mapping, Optional, TypeVar, cast
+from typing import Any, Callable, Dict, Iterator, List, Mapping, Optional, TypeVar, cast
 
 import aiohttp
 
 from kopf._cogs.clients import errors
 from kopf._cogs.helpers import versions
 from kopf._cogs.structs import credentials
 
@@ -32,21 +32,30 @@
     """
     @functools.wraps(fn)
     async def wrapper(*args: Any, **kwargs: Any) -> Any:
 
         # If a context is explicitly passed, make it a simple call without re-auth.
         # Exceptions are escalated to a caller, which is probably wrapped itself.
         if 'context' in kwargs:
-            return await fn(*args, **kwargs)
+            context = kwargs['context']
+            response = await fn(*args, **kwargs)
+            if isinstance(response, aiohttp.ClientResponse):
+                # Keep track of responses which are using this context.
+                context.add_response(response)
+            return response
 
         # Otherwise, attempt the execution with the vault credentials and re-authenticate on 401s.
         vault: credentials.Vault = vault_var.get()
         async for key, info, context in vault.extended(APIContext, 'contexts'):
             try:
-                return await fn(*args, **kwargs, context=context)
+                response = await fn(*args, **kwargs, context=context)
+                if isinstance(response, aiohttp.ClientResponse):
+                    # Keep track of responses which are using this context.
+                    context.add_response(response)
+                return response
             except errors.APIUnauthorizedError as e:
                 await vault.invalidate(key, exc=e)
 
         # Normally, either `vault.extended()` or `vault.invalidate()` raise the login errors.
         # The for-cycle can only end if the yielded credentials are not invalidated before trying
         # the next ones -- but this case exits by `return` or by other (non-401) errors.
         raise RuntimeError("Reached an impossible state: the end of the authentication cycle.")
@@ -70,14 +79,17 @@
     # The main contained object used by the API methods.
     session: aiohttp.ClientSession
 
     # Contextual information for URL building.
     server: str
     default_namespace: Optional[str]
 
+    # List of open responses.
+    responses: List[aiohttp.ClientResponse]
+
     # Temporary caches of the information retrieved for and from the environment.
     _tempfiles: "_TempFiles"
 
     def __init__(
             self,
             info: credentials.ConnectionInfo,
     ) -> None:
@@ -162,18 +174,40 @@
             auth=auth,
         )
 
         # Add the extra payload information. We avoid overriding the constructor.
         self.server = info.server
         self.default_namespace = info.default_namespace
 
+        self.responses = []
+
         # For purging on garbage collection.
         self._tempfiles = tempfiles
 
+    def flush_closed_responses(self) -> None:
+        # There's no point keeping references to already closed responses.
+        self.responses[:] = [_response for _response in self.responses if not _response.closed]
+
+    def add_response(self, response: aiohttp.ClientResponse) -> None:
+        # Keep track of responses so they can be closed later when the session
+        # is closed.
+        self.flush_closed_responses()
+        if not response.closed:
+            self.responses.append(response)
+
+    def close_open_responses(self) -> None:
+        # Close all responses that are still open and are using this session.
+        for response in self.responses:
+            if not response.closed:
+                response.close()
+        self.responses.clear()
+
     async def close(self) -> None:
+        # Close all open responses that use this session before closing the session itself.
+        self.close_open_responses()
 
         # Closing is triggered by `Vault._flush_caches()` -- forward it to the actual session.
         await self.session.close()
 
         # Additionally, explicitly remove any temporary files we have created.
         # They will be purged on garbage collection anyway, but it is better to make it sooner.
         self._tempfiles.purge()
```

### Comparing `kopf-1.37.1/kopf/_cogs/clients/creating.py` & `kopf-1.37.2/kopf/_cogs/clients/creating.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/errors.py` & `kopf-1.37.2/kopf/_cogs/clients/errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/events.py` & `kopf-1.37.2/kopf/_cogs/clients/events.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/fetching.py` & `kopf-1.37.2/kopf/_cogs/clients/fetching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/patching.py` & `kopf-1.37.2/kopf/_cogs/clients/patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/scanning.py` & `kopf-1.37.2/kopf/_cogs/clients/scanning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/clients/watching.py` & `kopf-1.37.2/kopf/_cogs/clients/watching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/configs/configuration.py` & `kopf-1.37.2/kopf/_cogs/configs/configuration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/configs/conventions.py` & `kopf-1.37.2/kopf/_cogs/configs/conventions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/configs/diffbase.py` & `kopf-1.37.2/kopf/_cogs/configs/diffbase.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/configs/progress.py` & `kopf-1.37.2/kopf/_cogs/configs/progress.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/helpers/__init__.py` & `kopf-1.37.2/kopf/_cogs/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/helpers/hostnames.py` & `kopf-1.37.2/kopf/_cogs/helpers/hostnames.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/helpers/loaders.py` & `kopf-1.37.2/kopf/_cogs/helpers/loaders.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/helpers/thirdparty.py` & `kopf-1.37.2/kopf/_cogs/helpers/thirdparty.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/helpers/typedefs.py` & `kopf-1.37.2/kopf/_cogs/helpers/typedefs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/helpers/versions.py` & `kopf-1.37.2/kopf/_cogs/helpers/versions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/bodies.py` & `kopf-1.37.2/kopf/_cogs/structs/bodies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/credentials.py` & `kopf-1.37.2/kopf/_cogs/structs/credentials.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/dicts.py` & `kopf-1.37.2/kopf/_cogs/structs/dicts.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/diffs.py` & `kopf-1.37.2/kopf/_cogs/structs/diffs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/ephemera.py` & `kopf-1.37.2/kopf/_cogs/structs/ephemera.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/finalizers.py` & `kopf-1.37.2/kopf/_cogs/structs/finalizers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/patches.py` & `kopf-1.37.2/kopf/_cogs/structs/patches.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/references.py` & `kopf-1.37.2/kopf/_cogs/structs/references.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_cogs/structs/reviews.py` & `kopf-1.37.2/kopf/_cogs/structs/reviews.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/application.py` & `kopf-1.37.2/kopf/_core/actions/application.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/execution.py` & `kopf-1.37.2/kopf/_core/actions/execution.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/invocation.py` & `kopf-1.37.2/kopf/_core/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/lifecycles.py` & `kopf-1.37.2/kopf/_core/actions/lifecycles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/loggers.py` & `kopf-1.37.2/kopf/_core/actions/loggers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/progression.py` & `kopf-1.37.2/kopf/_core/actions/progression.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/actions/throttlers.py` & `kopf-1.37.2/kopf/_core/actions/throttlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/activities.py` & `kopf-1.37.2/kopf/_core/engines/activities.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/admission.py` & `kopf-1.37.2/kopf/_core/engines/admission.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/daemons.py` & `kopf-1.37.2/kopf/_core/engines/daemons.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/indexing.py` & `kopf-1.37.2/kopf/_core/engines/indexing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/peering.py` & `kopf-1.37.2/kopf/_core/engines/peering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/posting.py` & `kopf-1.37.2/kopf/_core/engines/posting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/engines/probing.py` & `kopf-1.37.2/kopf/_core/engines/probing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/callbacks.py` & `kopf-1.37.2/kopf/_core/intents/callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/causes.py` & `kopf-1.37.2/kopf/_core/intents/causes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/filters.py` & `kopf-1.37.2/kopf/_core/intents/filters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/handlers.py` & `kopf-1.37.2/kopf/_core/intents/handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/piggybacking.py` & `kopf-1.37.2/kopf/_core/intents/piggybacking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/registries.py` & `kopf-1.37.2/kopf/_core/intents/registries.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/intents/stoppers.py` & `kopf-1.37.2/kopf/_core/intents/stoppers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/inventory.py` & `kopf-1.37.2/kopf/_core/reactor/inventory.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/observation.py` & `kopf-1.37.2/kopf/_core/reactor/observation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/orchestration.py` & `kopf-1.37.2/kopf/_core/reactor/orchestration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/processing.py` & `kopf-1.37.2/kopf/_core/reactor/processing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/queueing.py` & `kopf-1.37.2/kopf/_core/reactor/queueing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/running.py` & `kopf-1.37.2/kopf/_core/reactor/running.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_core/reactor/subhandling.py` & `kopf-1.37.2/kopf/_core/reactor/subhandling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_kits/__init__.py` & `kopf-1.37.2/kopf/_kits/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_kits/hierarchies.py` & `kopf-1.37.2/kopf/_kits/hierarchies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_kits/loops.py` & `kopf-1.37.2/kopf/_kits/loops.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_kits/runner.py` & `kopf-1.37.2/kopf/_kits/runner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_kits/webhacks.py` & `kopf-1.37.2/kopf/_kits/webhacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/_kits/webhooks.py` & `kopf-1.37.2/kopf/_kits/webhooks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/cli.py` & `kopf-1.37.2/kopf/cli.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf/on.py` & `kopf-1.37.2/kopf/on.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/kopf.egg-info/PKG-INFO` & `kopf-1.37.2/kopf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopf
-Version: 1.37.1
+Version: 1.37.2
 Summary: Kubernetes Operator Pythonic Framework (Kopf)
 Home-page: https://github.com/nolar/kopf
 Author: Sergey Vasilyev
 Author-email: nolar@nolar.info
 Maintainer: Sergey Vasilyev
 Maintainer-email: nolar@nolar.info
 License: MIT
```

### Comparing `kopf-1.37.1/kopf.egg-info/SOURCES.txt` & `kopf-1.37.2/kopf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/peering.yaml` & `kopf-1.37.2/peering.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/setup.py` & `kopf-1.37.2/setup.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/conftest.py` & `kopf-1.37.2/tests/admission/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_admission_manager.py` & `kopf-1.37.2/tests/admission/test_admission_manager.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_admission_server.py` & `kopf-1.37.2/tests/admission/test_admission_server.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_certificates.py` & `kopf-1.37.2/tests/admission/test_certificates.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_jsonpatch.py` & `kopf-1.37.2/tests/admission/test_jsonpatch.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_managed_webhooks.py` & `kopf-1.37.2/tests/admission/test_managed_webhooks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_serving_ephemeral_memos.py` & `kopf-1.37.2/tests/admission/test_serving_ephemeral_memos.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_serving_handler_selection.py` & `kopf-1.37.2/tests/admission/test_serving_handler_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_serving_kwargs_passthrough.py` & `kopf-1.37.2/tests/admission/test_serving_kwargs_passthrough.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_serving_responses.py` & `kopf-1.37.2/tests/admission/test_serving_responses.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_webhook_detection.py` & `kopf-1.37.2/tests/admission/test_webhook_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_webhook_ngrok.py` & `kopf-1.37.2/tests/admission/test_webhook_ngrok.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/admission/test_webhook_server.py` & `kopf-1.37.2/tests/admission/test_webhook_server.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/apis/test_api_requests.py` & `kopf-1.37.2/tests/apis/test_api_requests.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/apis/test_error_retries.py` & `kopf-1.37.2/tests/apis/test_error_retries.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/apis/test_iterjsonlines.py` & `kopf-1.37.2/tests/apis/test_iterjsonlines.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_authentication.py` & `kopf-1.37.2/tests/authentication/test_authentication.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_connectioninfo.py` & `kopf-1.37.2/tests/authentication/test_connectioninfo.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_credentials.py` & `kopf-1.37.2/tests/authentication/test_credentials.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_login_kubeconfig.py` & `kopf-1.37.2/tests/authentication/test_login_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_login_serviceaccount.py` & `kopf-1.37.2/tests/authentication/test_login_serviceaccount.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_reauthentication.py` & `kopf-1.37.2/tests/authentication/test_reauthentication.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_tempfiles.py` & `kopf-1.37.2/tests/authentication/test_tempfiles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/authentication/test_vault.py` & `kopf-1.37.2/tests/authentication/test_vault.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/basic-structs/test_causes.py` & `kopf-1.37.2/tests/basic-structs/test_causes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/basic-structs/test_handlers.py` & `kopf-1.37.2/tests/basic-structs/test_handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/basic-structs/test_memories.py` & `kopf-1.37.2/tests/basic-structs/test_memories.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/basic-structs/test_memos.py` & `kopf-1.37.2/tests/basic-structs/test_memos.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/basic-structs/test_resource.py` & `kopf-1.37.2/tests/basic-structs/test_resource.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/causation/test_detection.py` & `kopf-1.37.2/tests/causation/test_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/causation/test_kwargs.py` & `kopf-1.37.2/tests/causation/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/cli/conftest.py` & `kopf-1.37.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/cli/test_help.py` & `kopf-1.37.2/tests/cli/test_help.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/cli/test_logging.py` & `kopf-1.37.2/tests/cli/test_logging.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/cli/test_options.py` & `kopf-1.37.2/tests/cli/test_options.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/cli/test_preloading.py` & `kopf-1.37.2/tests/cli/test_preloading.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/conftest.py` & `kopf-1.37.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_cherrypicking.py` & `kopf-1.37.2/tests/dicts/test_cherrypicking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_dictviews.py` & `kopf-1.37.2/tests/dicts/test_dictviews.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_ensuring.py` & `kopf-1.37.2/tests/dicts/test_ensuring.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_parsing.py` & `kopf-1.37.2/tests/dicts/test_parsing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_removing.py` & `kopf-1.37.2/tests/dicts/test_removing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_resolving.py` & `kopf-1.37.2/tests/dicts/test_resolving.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/dicts/test_walking.py` & `kopf-1.37.2/tests/dicts/test_walking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/diffs/test_calculation.py` & `kopf-1.37.2/tests/diffs/test_calculation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/diffs/test_protocols.py` & `kopf-1.37.2/tests/diffs/test_protocols.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/diffs/test_reduction.py` & `kopf-1.37.2/tests/diffs/test_reduction.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/e2e/conftest.py` & `kopf-1.37.2/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/e2e/test_examples.py` & `kopf-1.37.2/tests/e2e/test_examples.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/conftest.py` & `kopf-1.37.2/tests/handling/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/conftest.py` & `kopf-1.37.2/tests/handling/daemons/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_daemon_errors.py` & `kopf-1.37.2/tests/handling/daemons/test_daemon_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_daemon_filtration.py` & `kopf-1.37.2/tests/handling/daemons/test_daemon_filtration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_daemon_rematching.py` & `kopf-1.37.2/tests/handling/daemons/test_daemon_rematching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_daemon_spawning.py` & `kopf-1.37.2/tests/handling/daemons/test_daemon_spawning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_daemon_termination.py` & `kopf-1.37.2/tests/handling/daemons/test_daemon_termination.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_timer_errors.py` & `kopf-1.37.2/tests/handling/daemons/test_timer_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_timer_filtration.py` & `kopf-1.37.2/tests/handling/daemons/test_timer_filtration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_timer_intervals.py` & `kopf-1.37.2/tests/handling/daemons/test_timer_intervals.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/daemons/test_timer_triggering.py` & `kopf-1.37.2/tests/handling/daemons/test_timer_triggering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/indexing/conftest.py` & `kopf-1.37.2/tests/handling/indexing/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/indexing/test_blocking_until_indexed.py` & `kopf-1.37.2/tests/handling/indexing/test_blocking_until_indexed.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/indexing/test_index_exclusion.py` & `kopf-1.37.2/tests/handling/indexing/test_index_exclusion.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/indexing/test_index_population.py` & `kopf-1.37.2/tests/handling/indexing/test_index_population.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/subhandling/test_subhandling.py` & `kopf-1.37.2/tests/handling/subhandling/test_subhandling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_activity_triggering.py` & `kopf-1.37.2/tests/handling/test_activity_triggering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_cause_handling.py` & `kopf-1.37.2/tests/handling/test_cause_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_cause_logging.py` & `kopf-1.37.2/tests/handling/test_cause_logging.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_delays.py` & `kopf-1.37.2/tests/handling/test_delays.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_error_handling.py` & `kopf-1.37.2/tests/handling/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_event_handling.py` & `kopf-1.37.2/tests/handling/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_multistep.py` & `kopf-1.37.2/tests/handling/test_multistep.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_no_handlers.py` & `kopf-1.37.2/tests/handling/test_no_handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_parametrization.py` & `kopf-1.37.2/tests/handling/test_parametrization.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_retrying_limits.py` & `kopf-1.37.2/tests/handling/test_retrying_limits.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/handling/test_timing_consistency.py` & `kopf-1.37.2/tests/handling/test_timing_consistency.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/conftest.py` & `kopf-1.37.2/tests/hierarchies/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/test_contextual_owner.py` & `kopf-1.37.2/tests/hierarchies/test_contextual_owner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/test_labelling.py` & `kopf-1.37.2/tests/hierarchies/test_labelling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/test_name_harmonizing.py` & `kopf-1.37.2/tests/hierarchies/test_name_harmonizing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/test_namespace_adjusting.py` & `kopf-1.37.2/tests/hierarchies/test_namespace_adjusting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/test_owner_referencing.py` & `kopf-1.37.2/tests/hierarchies/test_owner_referencing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/hierarchies/test_type_validation.py` & `kopf-1.37.2/tests/hierarchies/test_type_validation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/invocations/test_callbacks.py` & `kopf-1.37.2/tests/invocations/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_creating.py` & `kopf-1.37.2/tests/k8s/test_creating.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_errors.py` & `kopf-1.37.2/tests/k8s/test_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_events.py` & `kopf-1.37.2/tests/k8s/test_events.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_list_objs.py` & `kopf-1.37.2/tests/k8s/test_list_objs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_patching.py` & `kopf-1.37.2/tests/k8s/test_patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_scanning.py` & `kopf-1.37.2/tests/k8s/test_scanning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_watching_bookmarks.py` & `kopf-1.37.2/tests/k8s/test_watching_bookmarks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_watching_continuously.py` & `kopf-1.37.2/tests/k8s/test_watching_continuously.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_watching_infinitely.py` & `kopf-1.37.2/tests/k8s/test_watching_infinitely.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/k8s/test_watching_with_freezes.py` & `kopf-1.37.2/tests/k8s/test_watching_with_freezes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/lifecycles/test_global_defaults.py` & `kopf-1.37.2/tests/lifecycles/test_global_defaults.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/lifecycles/test_handler_selection.py` & `kopf-1.37.2/tests/lifecycles/test_handler_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/lifecycles/test_real_invocation.py` & `kopf-1.37.2/tests/lifecycles/test_real_invocation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/logging/conftest.py` & `kopf-1.37.2/tests/logging/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/logging/test_configuration.py` & `kopf-1.37.2/tests/logging/test_configuration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/logging/test_formatters.py` & `kopf-1.37.2/tests/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/logging/test_loggers.py` & `kopf-1.37.2/tests/logging/test_loggers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/observation/test_processing_of_namespaces.py` & `kopf-1.37.2/tests/observation/test_processing_of_namespaces.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/observation/test_processing_of_resources.py` & `kopf-1.37.2/tests/observation/test_processing_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/observation/test_revision_of_namespaces.py` & `kopf-1.37.2/tests/observation/test_revision_of_namespaces.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/observation/test_revision_of_resources.py` & `kopf-1.37.2/tests/observation/test_revision_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/orchestration/test_task_adjustments.py` & `kopf-1.37.2/tests/orchestration/test_task_adjustments.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/peering/test_freeze_mode.py` & `kopf-1.37.2/tests/peering/test_freeze_mode.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/peering/test_id_generation.py` & `kopf-1.37.2/tests/peering/test_id_generation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/peering/test_keepalive.py` & `kopf-1.37.2/tests/peering/test_keepalive.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/peering/test_peer_patching.py` & `kopf-1.37.2/tests/peering/test_peer_patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/peering/test_peers.py` & `kopf-1.37.2/tests/peering/test_peers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/peering/test_resource_guessing.py` & `kopf-1.37.2/tests/peering/test_resource_guessing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/persistence/test_annotations_hashing.py` & `kopf-1.37.2/tests/persistence/test_annotations_hashing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/persistence/test_essences.py` & `kopf-1.37.2/tests/persistence/test_essences.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/persistence/test_outcomes.py` & `kopf-1.37.2/tests/persistence/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/persistence/test_states.py` & `kopf-1.37.2/tests/persistence/test_states.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/persistence/test_storing_of_diffbase.py` & `kopf-1.37.2/tests/persistence/test_storing_of_diffbase.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/persistence/test_storing_of_progress.py` & `kopf-1.37.2/tests/persistence/test_storing_of_progress.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/posting/test_log2k8s.py` & `kopf-1.37.2/tests/posting/test_log2k8s.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/posting/test_poster.py` & `kopf-1.37.2/tests/posting/test_poster.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/posting/test_threadsafety.py` & `kopf-1.37.2/tests/posting/test_threadsafety.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/primitives/test_conditions.py` & `kopf-1.37.2/tests/primitives/test_conditions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/primitives/test_containers.py` & `kopf-1.37.2/tests/primitives/test_containers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/primitives/test_flags.py` & `kopf-1.37.2/tests/primitives/test_flags.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/primitives/test_toggles.py` & `kopf-1.37.2/tests/primitives/test_toggles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/primitives/test_togglesets.py` & `kopf-1.37.2/tests/primitives/test_togglesets.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/reactor/conftest.py` & `kopf-1.37.2/tests/reactor/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/reactor/test_patching_inconsistencies.py` & `kopf-1.37.2/tests/reactor/test_patching_inconsistencies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/reactor/test_queueing.py` & `kopf-1.37.2/tests/reactor/test_queueing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/reactor/test_uids.py` & `kopf-1.37.2/tests/reactor/test_uids.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/references/test_backbone.py` & `kopf-1.37.2/tests/references/test_backbone.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/references/test_namespace_matching.py` & `kopf-1.37.2/tests/references/test_namespace_matching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/references/test_namespace_selection.py` & `kopf-1.37.2/tests/references/test_namespace_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/references/test_selector_matching.py` & `kopf-1.37.2/tests/references/test_selector_matching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/references/test_selector_parsing.py` & `kopf-1.37.2/tests/references/test_selector_parsing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/references/test_selector_properties.py` & `kopf-1.37.2/tests/references/test_selector_properties.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/conftest.py` & `kopf-1.37.2/tests/registries/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_creation.py` & `kopf-1.37.2/tests/registries/test_creation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_decorators.py` & `kopf-1.37.2/tests/registries/test_decorators.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_handler_getting.py` & `kopf-1.37.2/tests/registries/test_handler_getting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_id_detection.py` & `kopf-1.37.2/tests/registries/test_id_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_matching_for_changing.py` & `kopf-1.37.2/tests/registries/test_matching_for_changing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_matching_for_indexing.py` & `kopf-1.37.2/tests/registries/test_matching_for_indexing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_matching_for_spawning.py` & `kopf-1.37.2/tests/registries/test_matching_for_spawning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_matching_for_watching.py` & `kopf-1.37.2/tests/registries/test_matching_for_watching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_matching_of_callbacks.py` & `kopf-1.37.2/tests/registries/test_matching_of_callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_matching_of_resources.py` & `kopf-1.37.2/tests/registries/test_matching_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_requires_finalizer.py` & `kopf-1.37.2/tests/registries/test_requires_finalizer.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_resumes_mixed_in.py` & `kopf-1.37.2/tests/registries/test_resumes_mixed_in.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/registries/test_subhandlers_ids.py` & `kopf-1.37.2/tests/registries/test_subhandlers_ids.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/settings/test_defaults.py` & `kopf-1.37.2/tests/settings/test_defaults.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/settings/test_executor.py` & `kopf-1.37.2/tests/settings/test_executor.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/test_async.py` & `kopf-1.37.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/test_filtering_helpers.py` & `kopf-1.37.2/tests/test_filtering_helpers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/test_finalizers.py` & `kopf-1.37.2/tests/test_finalizers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/test_liveness.py` & `kopf-1.37.2/tests/test_liveness.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/test_thirdparty.py` & `kopf-1.37.2/tests/test_thirdparty.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/test_versions.py` & `kopf-1.37.2/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/testing/test_runner.py` & `kopf-1.37.2/tests/testing/test_runner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/timing/test_sleeping.py` & `kopf-1.37.2/tests/timing/test_sleeping.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/timing/test_throttling.py` & `kopf-1.37.2/tests/timing/test_throttling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/utilities/aiotasks/test_coro_cancellation.py` & `kopf-1.37.2/tests/utilities/aiotasks/test_coro_cancellation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/utilities/aiotasks/test_scheduler.py` & `kopf-1.37.2/tests/utilities/aiotasks/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/utilities/aiotasks/test_task_guarding.py` & `kopf-1.37.2/tests/utilities/aiotasks/test_task_guarding.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tests/utilities/aiotasks/test_task_stopping.py` & `kopf-1.37.2/tests/utilities/aiotasks/test_task_stopping.py`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tools/install-kind.sh` & `kopf-1.37.2/tools/install-kind.sh`

 * *Files identical despite different names*

### Comparing `kopf-1.37.1/tools/install-minikube.sh` & `kopf-1.37.2/tools/install-minikube.sh`

 * *Files identical despite different names*

