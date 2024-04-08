# Comparing `tmp/proxystore-0.6.3.tar.gz` & `tmp/proxystore-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxystore-0.6.3.tar", last modified: Tue Feb  6 16:33:43 2024, max compression
+gzip compressed data, was "proxystore-0.6.4.tar", last modified: Mon Apr  8 15:58:54 2024, max compression
```

## Comparing `proxystore-0.6.3.tar` & `proxystore-0.6.4.tar`

### file list

```diff
@@ -1,294 +1,301 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.973054 proxystore-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/ISSUE_TEMPLATE/01_bug.yml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/ISSUE_TEMPLATE/02_feature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/ISSUE_TEMPLATE/03_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/workflows/cache.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/workflows/check-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-06 16:33:34.000000 proxystore-0.6.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-06 16:33:34.000000 proxystore-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-06 16:33:34.000000 proxystore-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-06 16:33:34.000000 proxystore-0.6.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-06 16:33:34.000000 proxystore-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-02-06 16:33:43.973054 proxystore-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-02-06 16:33:34.000000 proxystore-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/docs/_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/_overrides/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.925054 proxystore-0.6.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.925054 proxystore-0.6.3/docs/_templates/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/docs/_templates/python/material/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/docs/_templates/python/material/docstring/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/_templates/python/material/docstring/admonition.html
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/_templates/python/material/function.html
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/_templates/python/material/module.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.933054 proxystore-0.6.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/api/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.937054 proxystore-0.6.3/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/concepts/connector.md
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/concepts/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/concepts/proxy.md
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/concepts/store.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.937054 proxystore-0.6.3/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/contributing/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/contributing/issues-pull-requests.md
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/contributing/releases.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/contributing/style-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.937054 proxystore-0.6.3/docs/css/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/get-started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.937054 proxystore-0.6.3/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/endpoints-debugging.md
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/globus-compute.md
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/performance.md
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/proxy-futures.md
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/relay-serving.md
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/guides/streaming.md
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/known-issues.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.937054 proxystore-0.6.3/docs/publications/
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/publications/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.941054 proxystore-0.6.3/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   134472 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/endpoint-overview.svg
--rw-r--r--   0 runner    (1001) docker     (127)   149176 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/endpoint-peering.svg
--rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    45464 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31236 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)   106893 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/proxystore-overview.svg
--rw-r--r--   0 runner    (1001) docker     (127)   106939 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/proxystore-schematic.svg
--rw-r--r--   0 runner    (1001) docker     (127)   176467 2024-02-06 16:33:34.000000 proxystore-0.6.3/docs/static/proxystore-streaming.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.941054 proxystore-0.6.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.941054 proxystore-0.6.3/examples/globus-compute/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/globus-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/globus-compute/mapreduce_globus_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/globus-compute/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.941054 proxystore-0.6.3/examples/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/parsl/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/parsl/mapreduce_parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/parsl/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-06 16:33:34.000000 proxystore-0.6.3/examples/store_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-02-06 16:33:34.000000 proxystore-0.6.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.945054 proxystore-0.6.3/proxystore/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.945054 proxystore-0.6.3/proxystore/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/dim.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    23451 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/connectors/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.949054 proxystore-0.6.3/proxystore/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/endpoint/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.949054 proxystore-0.6.3/proxystore/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/globus/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.949054 proxystore-0.6.3/proxystore/p2p/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/nat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.953054 proxystore-0.6.3/proxystore/p2p/relay/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/p2p/relay/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.953054 proxystore-0.6.3/proxystore/store/
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33044 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.953054 proxystore-0.6.3/proxystore/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21544 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.957054 proxystore-0.6.3/proxystore/stream/shims/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/shims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/shims/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/shims/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/shims/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/stream/shims/zmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.957054 proxystore-0.6.3/proxystore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-06 16:33:34.000000 proxystore-0.6.3/proxystore/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.973054 proxystore-0.6.3/proxystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-02-06 16:33:43.000000 proxystore-0.6.3/proxystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-02-06 16:33:43.000000 proxystore-0.6.3/proxystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 16:33:43.000000 proxystore-0.6.3/proxystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-06 16:33:43.000000 proxystore-0.6.3/proxystore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-06 16:33:43.000000 proxystore-0.6.3/proxystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-06 16:33:43.000000 proxystore-0.6.3/proxystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-02-06 16:33:34.000000 proxystore-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 16:33:43.973054 proxystore-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.957054 proxystore-0.6.3/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.957054 proxystore-0.6.3/testing/mocked/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/mocked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/mocked/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/mocked/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/mocked/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/relay_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.961054 proxystore-0.6.3/testing/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/scripts/kafka_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/scripts/peer_connection_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/scripts/peer_endpoint_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/scripts/peer_manager_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/scripts/redis_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-06 16:33:34.000000 proxystore-0.6.3/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.961054 proxystore-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.961054 proxystore-0.6.3/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/connector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/dim_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/endpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/globus_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/local_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/multi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/connectors/redis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.965054 proxystore-0.6.3/tests/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/commands_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/endpoint_peering_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/endpoint_solo_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/serve_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/endpoint/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/ex_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/factory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.965054 proxystore-0.6.3/tests/globus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/scopes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/globus/transfer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.965054 proxystore-0.6.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/integration/endpoints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.965054 proxystore-0.6.3/tests/p2p/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/chunks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/nat_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.965054 proxystore-0.6.3/tests/p2p/relay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/authenticate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/messages_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/run_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/p2p/relay/server_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/serialization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.969054 proxystore-0.6.3/tests/store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/factory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/init_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/store_basics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/store_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/store_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/store/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.969054 proxystore-0.6.3/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/events_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/interface_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.969054 proxystore-0.6.3/tests/stream/shims/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/shims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/shims/kafka_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/shims/queue_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/shims/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/stream/shims/zmq_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:43.969054 proxystore-0.6.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/counter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/data_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/environment_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/imports_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-06 16:33:34.000000 proxystore-0.6.3/tests/utils/timer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-06 16:33:34.000000 proxystore-0.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.514128 proxystore-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/01_bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/02_feature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/03_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/cache.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/check-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 15:58:48.000000 proxystore-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-08 15:58:48.000000 proxystore-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-08 15:58:48.000000 proxystore-0.6.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-08 15:58:48.000000 proxystore-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-08 15:58:54.514128 proxystore-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-08 15:58:48.000000 proxystore-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/docs/_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_overrides/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.462128 proxystore-0.6.4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.462128 proxystore-0.6.4/docs/_templates/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/_templates/python/material/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/_templates/python/material/docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_templates/python/material/docstring/admonition.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_templates/python/material/function.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_templates/python/material/module.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/api/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/connector.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/proxy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/store.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/issues-pull-requests.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/releases.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/style-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/get-started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/endpoints-debugging.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/globus-compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/object-lifetimes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/performance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/proxy-futures.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/relay-serving.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/streaming.md
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/known-issues.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/publications/
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/publications/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   134472 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/endpoint-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   149176 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/endpoint-peering.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45464 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31236 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   106893 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/proxystore-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   106939 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/proxystore-schematic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   176467 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/proxystore-streaming.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/examples/globus-compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/globus-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/globus-compute/mapreduce_globus_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/globus-compute/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/examples/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/parsl/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/parsl/mapreduce_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/parsl/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/store_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-08 15:58:48.000000 proxystore-0.6.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.482128 proxystore-0.6.4/proxystore/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.482128 proxystore-0.6.4/proxystore/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23452 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.486127 proxystore-0.6.4/proxystore/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.486127 proxystore-0.6.4/proxystore/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.486127 proxystore-0.6.4/proxystore/p2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/nat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.490128 proxystore-0.6.4/proxystore/p2p/relay/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13466 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.490128 proxystore-0.6.4/proxystore/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43757 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/lifetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19018 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.490128 proxystore-0.6.4/proxystore/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24393 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.494128 proxystore-0.6.4/proxystore/stream/shims/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.494128 proxystore-0.6.4/proxystore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.510128 proxystore-0.6.4/proxystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-08 15:58:48.000000 proxystore-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:58:54.514128 proxystore-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.494128 proxystore-0.6.4/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.498128 proxystore-0.6.4/testing/mocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/relay_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.498128 proxystore-0.6.4/testing/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/kafka_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/peer_connection_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/peer_endpoint_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/peer_manager_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/redis_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.498128 proxystore-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/connector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/dim_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/endpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/globus_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/multi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/redis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/commands_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/endpoint_peering_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/endpoint_solo_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/serve_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/ex_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/factory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/scopes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/transfer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/integration/endpoints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/p2p/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/chunks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/nat_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.506127 proxystore-0.6.4/tests/p2p/relay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/authenticate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/messages_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/server_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/serialization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.506127 proxystore-0.6.4/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/lifetimes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/ref_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/scopes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/store_basics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/store_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/store_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.506127 proxystore-0.6.4/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/events_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/interface_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.510128 proxystore-0.6.4/tests/stream/shims/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/kafka_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/queue_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/zmq_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.510128 proxystore-0.6.4/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/counter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/data_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/environment_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/imports_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/timer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 15:58:48.000000 proxystore-0.6.4/tox.ini
```

### Comparing `proxystore-0.6.3/.github/CODE_OF_CONDUCT.md` & `proxystore-0.6.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/ISSUE_TEMPLATE/01_bug.yml` & `proxystore-0.6.4/.github/ISSUE_TEMPLATE/01_bug.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/ISSUE_TEMPLATE/02_feature.yml` & `proxystore-0.6.4/.github/ISSUE_TEMPLATE/02_feature.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/SECURITY.md` & `proxystore-0.6.4/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/pull_request_template.md` & `proxystore-0.6.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/release.yml` & `proxystore-0.6.4/.github/release.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/workflows/cache.yml` & `proxystore-0.6.4/.github/workflows/cache.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/workflows/check-docs.yml` & `proxystore-0.6.4/.github/workflows/check-docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/workflows/docs.yml` & `proxystore-0.6.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.github/workflows/publish.yml` & `proxystore-0.6.4/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       - name: Install pypa/build and build
         run: |
           pip install build
           python -m build --sdist --wheel --outdir dist/ .
 
       - name: Upload files to release
         if: startsWith(github.ref, 'refs/tags/')
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
           files: dist/*
 
       - name: Publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `proxystore-0.6.3/.github/workflows/tests.yml` & `proxystore-0.6.4/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
           toxenv: py310
         - os: ubuntu-latest
           python: '3.11'
           toxenv: py311
         - os: ubuntu-latest
           python: '3.12'
           toxenv: py312
-        - os: macos-latest
+        - os: macos-13
           python: 3.8
           toxenv: py38
-        - os: macos-latest
+        - os: macos-13
           python: 3.9
           toxenv: py39
-        - os: macos-latest
+        - os: macos-13
           python: '3.10'
           toxenv: py310
-        - os: macos-latest
+        - os: macos-14
           python: '3.11'
           toxenv: py311
-        - os: macos-latest
+        - os: macos-14
           python: '3.12'
           toxenv: py312
     runs-on: ${{ matrix.os }}
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
```

### Comparing `proxystore-0.6.3/.gitignore` & `proxystore-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/.pre-commit-config.yaml` & `proxystore-0.6.4/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,23 @@
       - id: check-merge-conflict
       - id: name-tests-test
   - repo: 'https://github.com/codespell-project/codespell'
     rev: v2.2.6
     hooks:
       - id: codespell
   - repo: 'https://github.com/charliermarsh/ruff-pre-commit'
-    rev: v0.2.0
+    rev: v0.3.5
     hooks:
       - id: ruff
         args:
           - '--fix'
           - '--exit-non-zero-on-fix'
       - id: ruff-format
   - repo: 'https://github.com/pre-commit/mirrors-mypy'
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies:
           - click >= 8.1.0, != 8.1.4
           - globus-sdk
           - parsl
           - quart
```

### Comparing `proxystore-0.6.3/CITATION.cff` & `proxystore-0.6.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/LICENSE` & `proxystore-0.6.4/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Greg Pauloski
+Copyright (c) 2021-2024 Greg Pauloski and Globus Labs
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `proxystore-0.6.3/PKG-INFO` & `proxystore-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.6.3
+Version: 0.6.4
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: FILE
 Project-URL: homepage, https://proxystore.dev
 Project-URL: documentation, https://docs.proxystore.dev
@@ -29,15 +29,15 @@
 Provides-Extra: all
 Requires-Dist: proxystore[endpoints,extensions,kafka,redis,zmq]; extra == "all"
 Provides-Extra: endpoints
 Requires-Dist: aiortc>=1.3.2; extra == "endpoints"
 Requires-Dist: aiosqlite; extra == "endpoints"
 Requires-Dist: uvicorn[standard]; extra == "endpoints"
 Requires-Dist: psutil; extra == "endpoints"
-Requires-Dist: pydantic>=2.0.0; extra == "endpoints"
+Requires-Dist: pydantic; extra == "endpoints"
 Requires-Dist: pystun3; extra == "endpoints"
 Requires-Dist: python-daemon; extra == "endpoints"
 Requires-Dist: quart>=0.18.0; extra == "endpoints"
 Requires-Dist: requests>=2.27.1; extra == "endpoints"
 Requires-Dist: tomli; python_version < "3.11" and extra == "endpoints"
 Requires-Dist: tomli-w; extra == "endpoints"
 Requires-Dist: websockets>=10.0; extra == "endpoints"
@@ -54,15 +54,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: ruff>=0.2.0; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: types-redis; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mkdocs-click; extra == "docs"
```

### Comparing `proxystore-0.6.3/README.md` & `proxystore-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/_templates/python/material/function.html` & `proxystore-0.6.4/docs/_templates/python/material/function.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/_templates/python/material/module.html` & `proxystore-0.6.4/docs/_templates/python/material/module.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/api/cli.md` & `proxystore-0.6.4/docs/api/cli.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/concepts/connector.md` & `proxystore-0.6.4/docs/concepts/connector.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/concepts/index.md` & `proxystore-0.6.4/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/concepts/proxy.md` & `proxystore-0.6.4/docs/concepts/proxy.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/concepts/store.md` & `proxystore-0.6.4/docs/concepts/store.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/contributing/index.md` & `proxystore-0.6.4/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/contributing/issues-pull-requests.md` & `proxystore-0.6.4/docs/contributing/issues-pull-requests.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/contributing/releases.md` & `proxystore-0.6.4/docs/contributing/releases.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/contributing/style-guide.md` & `proxystore-0.6.4/docs/contributing/style-guide.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/css/mkdocstrings.css` & `proxystore-0.6.4/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/examples.md` & `proxystore-0.6.4/docs/examples.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/generate_api.py` & `proxystore-0.6.4/docs/generate_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generate the code reference pages and navigation."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 import mkdocs_gen_files
 
 nav = mkdocs_gen_files.Nav()
```

### Comparing `proxystore-0.6.3/docs/get-started.md` & `proxystore-0.6.4/docs/get-started.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/guides/endpoints-debugging.md` & `proxystore-0.6.4/docs/guides/endpoints-debugging.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/guides/endpoints.md` & `proxystore-0.6.4/docs/guides/endpoints.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/guides/globus-compute.md` & `proxystore-0.6.4/docs/guides/globus-compute.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/guides/performance.md` & `proxystore-0.6.4/docs/guides/performance.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/guides/proxy-futures.md` & `proxystore-0.6.4/docs/guides/proxy-futures.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # Proxy Futures
 
 *Last updated 1 November 2023*
 
 This guide walks through the use of the
 [`Store.future()`][proxystore.store.base.Store.future] interface and associated
-[`ProxyFuture`][proxystore.store.future.ProxyFuture].
+[`Future`][proxystore.store.future.Future].
 
 !!! note
 
     Some familiarity with ProxyStore is assumed. Check out the
     [Get Started](../get-started.md){target=_blank} guide and
     [Concepts](../concepts/index.md){target=_blank} page to learn more about
     ProxyStore's core concepts.
 
 !!! warning
 
     The [`Store.future()`][proxystore.store.base.Store.future] and
-    [`ProxyFuture`][proxystore.store.future.ProxyFuture] interfaces are
+    [`Future`][proxystore.store.future.Future] interfaces are
     experimental features and may change in future releases.
 
-The [`ProxyFuture`][proxystore.store.future.ProxyFuture] interface enables
+The [`Future`][proxystore.store.future.Future] interface enables
 a data producer to preemptively send a proxy to a data consumer before the
 target data has been created. The consumer of the target data proxy will
 block when the proxy is first used and resolved until the producer
 has created the target data.
 
 Here is a trivial example using a [`Store`][proxystore.store.base.Store] and
 [`LocalConnector`][proxystore.connectors.local.LocalConnector]. The
-[`future.proxy()`][proxystore.store.future.ProxyFuture.proxy] method is used
+[`future.proxy()`][proxystore.store.future.Future.proxy] method is used
 to create a [`Proxy`][proxystore.proxy.Proxy] which will resolve to the
 result of the future.
 
 ```python linenums="1" title="example.py"
 from proxystore.connectors.local import LocalConnector
 from proxystore.store import Store
-from proxystore.store.future import ProxyFuture
+from proxystore.store.future import Future
 
 with Store('proxy-future-example', LocalConnector()) as store:
-    future: ProxyFuture[str] = store.future()
+    future: Future[str] = store.future()
     proxy = future.proxy()
 
     future.set_result('value')
     assert future.result() == 'value'
     assert proxy == 'value'
 ```
 
@@ -61,49 +61,49 @@
     Many of the out-of-the-box implementations implement the
     [`DeferrableConnector`][proxystore.connectors.protocols.DeferrableConnector]
     protocol such as the
     [`EndpointConnector`][proxystore.connectors.endpoint.EndpointConnector],
     [`FileConnector`][proxystore.connectors.file.FileConnector], and
     [`RedisConnector`][proxystore.connectors.redis.RedisConnector].
 
-The power of [`ProxyFuture`][proxystore.store.future.ProxyFuture] comes when
+The power of [`Future`][proxystore.store.future.Future] comes when
 the data producer and consumer are executing independently in time and space
 (i.e., execution occurs in different processes, potentially on different
 systems, and in an undefined order). The
-[`ProxyFuture`][proxystore.store.future.ProxyFuture] enables the producer
+[`Future`][proxystore.store.future.Future] enables the producer
 and consumer to share a data dependency, while allowing the consumer to
 eagerly start execution before the data dependencies are fully satisfied.
 
 Consider the following example where we have a client which invokes two
 functions, `foo()` and `bar()` on remote processes. `foo()` will produce an
 object needed by `bar()`, but we want to start executing `foo()` and `bar()`
 at the same time. (We could even start `bar()` before `foo()`!)
 
 ```python linenums="1" title="client.py"
 from proxystore.connectors.redis import RedisConnector
 from proxystore.store import Store
-from proxystore.store.future import ProxyFuture
+from proxystore.store.future import Future
 
 class MyData:
     ...
 
-def foo(future: ProxyFuture[MyData]) -> None:
+def foo(future: Future[MyData]) -> None:
     data: MyData = compute(...)
     future.set_result(data)
 
 def bar(data: MyData) -> None:
     # Computation not involving data can execute freely.
     compute(...)
     # Computation using data will block until foo
     # sets the result of the future.
     compute(data)
 
 
 with Store('proxy-future-example', RedisConnector(...)) as store:
-    future: ProxyFuture[MyData] = store.future()
+    future: Future[MyData] = store.future()
 
     # The invoke_remote function will execute the function with
     # the provided on arguments on an arbitrary remote process.
     foo_result_future = invoke_remote(foo, future)
     bar_result_future = invoke_remote(bar, future.proxy())
 
     # Wait on the functions to finish executing.
```

### Comparing `proxystore-0.6.3/docs/guides/relay-serving.md` & `proxystore-0.6.4/docs/guides/relay-serving.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/guides/streaming.md` & `proxystore-0.6.4/docs/guides/streaming.md`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,24 @@
    inside the proxy's factory is determined in
    [`StreamProducer.send()`][proxystore.stream.interface.StreamProducer.send].
 4. Closing the [`StreamConsumer`][proxystore.stream.StreamConsumer] will close
    the [`Subscriber`][proxystore.stream.protocols.Subscriber],
    all [`Store`][proxystore.store.base.Store] instances, and
    [`Connector`][proxystore.connectors.protocols.Connector] by default.
 
+!!! tip
+
+    By default, iterating on a
+    [`StreamConsumer`][proxystore.stream.interface.StreamConsumer] yields only
+    a proxy of the next object in the stream. The
+    [`iter_with_metadata()`][proxystore.stream.interface.StreamConsumer.iter_with_metadata],
+    [`iter_objects()`][proxystore.stream.interface.StreamConsumer.iter_objects], and
+    [`iter_objects_with_metadata()`][proxystore.stream.interface.StreamConsumer.iter_objects_with_metadata]
+    methods provide additional mechanisms for iterating over stream data.
+
 ## Multi-Producer/Multi-Consumer
 
 The [`StreamProducer`][proxystore.stream.interface.StreamProducer]
 and [`StreamConsumer`][proxystore.stream.interface.StreamConsumer] can support
 multi-producer and multi-consumer deployments, respectively.
 However, it is *not* a requirement that the
 [`Publisher`][proxystore.stream.protocols.Publisher] or
```

### Comparing `proxystore-0.6.3/docs/installation.md` & `proxystore-0.6.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/known-issues.md` & `proxystore-0.6.4/docs/known-issues.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/publications/index.md` & `proxystore-0.6.4/docs/publications/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/endpoint-overview.svg` & `proxystore-0.6.4/docs/static/endpoint-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/endpoint-peering.svg` & `proxystore-0.6.4/docs/static/endpoint-peering.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/favicon.png` & `proxystore-0.6.4/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/icon.png` & `proxystore-0.6.4/docs/static/icon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/logo-dark.png` & `proxystore-0.6.4/docs/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/logo-light.png` & `proxystore-0.6.4/docs/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/proxystore-overview.svg` & `proxystore-0.6.4/docs/static/proxystore-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/proxystore-schematic.svg` & `proxystore-0.6.4/docs/static/proxystore-schematic.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/docs/static/proxystore-streaming.svg` & `proxystore-0.6.4/docs/static/proxystore-streaming.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/examples/README.md` & `proxystore-0.6.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/examples/globus-compute/README.md` & `proxystore-0.6.4/examples/globus-compute/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/examples/globus-compute/mapreduce_globus_compute.py` & `proxystore-0.6.4/examples/globus-compute/mapreduce_globus_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Globus Compute and ProxyStore example."""
+
 from __future__ import annotations
 
 import argparse
 import sys
 import time
 from typing import Any
```

### Comparing `proxystore-0.6.3/examples/globus-compute/run.sh` & `proxystore-0.6.4/examples/globus-compute/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/examples/parsl/mapreduce_parsl.py` & `proxystore-0.6.4/examples/parsl/mapreduce_parsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MapReduce with Parsl and ProxyStore example."""
+
 from __future__ import annotations
 
 import argparse
 from typing import Any
 
 import numpy as np
 import parsl
```

### Comparing `proxystore-0.6.3/examples/parsl/run.sh` & `proxystore-0.6.4/examples/parsl/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/examples/store_metrics.py` & `proxystore-0.6.4/examples/store_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Store metrics example.
 
 Source code for:
     https://proxystore.readthedocs.io/en/latest/guides/performance.html
 """
+
 from __future__ import annotations
 
 import dataclasses
 import tempfile
 from pprint import pprint
 
 from proxystore.connectors.file import FileConnector
```

### Comparing `proxystore-0.6.3/mkdocs.yml` & `proxystore-0.6.4/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
       - Connector: concepts/connector.md
       - Store: concepts/store.md
   - Guides:
       - guides/index.md
       - Globus Compute: guides/globus-compute.md
       - Endpoints Overview: guides/endpoints.md
       - Endpoints Debugging: guides/endpoints-debugging.md
+      - Object Lifetimes: guides/object-lifetimes.md
       - Performance Tracking: guides/performance.md
       - Proxy Futures: guides/proxy-futures.md
       - Relay Serving: guides/relay-serving.md
       - Streaming: guides/streaming.md
   - API Reference:
       - ProxyStore: api/
       - CLI Reference: api/cli.md
```

### Comparing `proxystore-0.6.3/proxystore/connectors/__init__.py` & `proxystore-0.6.4/proxystore/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/proxystore/connectors/dim.py` & `proxystore-0.6.4/proxystore/connectors/dim.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ```
     and change the imports accordingly. E.g.,
     ```python
     from proxystore.connectors.dim.zmq import ZeroMQConnector  # OLD
     from proxystore.ex.connectors.dim.zmq import ZeroMQConnector  # NEW
     ```
 """
+
 from __future__ import annotations
 
 import warnings
 
 warnings.warn(
     """\
 The proxystore.connectors.dim module has moved to ProxyStore Extensions.
```

### Comparing `proxystore-0.6.3/proxystore/connectors/endpoint.py` & `proxystore-0.6.4/proxystore/connectors/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Endpoint connector implementation."""
+
 from __future__ import annotations
 
 import logging
 import sys
 import uuid
 from types import TracebackType
 from typing import Any
@@ -87,35 +88,43 @@
         # home endpoint
         available_endpoints = get_configs(
             home_dir() if self.proxystore_dir is None else self.proxystore_dir,
         )
         found_endpoint: EndpointConfig | None = None
         for endpoint in available_endpoints:
             endpoint_uuid = UUID(endpoint.uuid)
-            if endpoint_uuid in self.endpoints:
-                logger.debug(f'Attempting connection to {endpoint_uuid}')
-                response = self._session.get(
-                    f'http://{endpoint.host}:{endpoint.port}/endpoint',
+            if endpoint_uuid not in self.endpoints:
+                continue
+            if endpoint.host is None:
+                logger.warning(
+                    'Found valid configuration for endpoint '
+                    f'"{endpoint.name}" ({endpoint_uuid}), but the endpoint '
+                    'has not been started',
                 )
-                if response.status_code == 200:
-                    uuid_ = response.json()['uuid']
-                    if endpoint_uuid == UUID(uuid_):
-                        logger.debug(
-                            f'Connection to {endpoint_uuid} successful, using '
-                            'as local endpoint',
-                        )
-                        found_endpoint = endpoint
-                        break
-                    else:
-                        logger.debug(
-                            f'Connection to {endpoint_uuid} returned '
-                            'different UUID',
-                        )
+                continue
+            logger.debug(f'Attempting connection to {endpoint_uuid}')
+            response = self._session.get(
+                f'http://{endpoint.host}:{endpoint.port}/endpoint',
+            )
+            if response.status_code == 200:
+                uuid_ = response.json()['uuid']
+                if endpoint_uuid == UUID(uuid_):
+                    logger.debug(
+                        f'Connection to {endpoint_uuid} successful, using '
+                        'as local endpoint',
+                    )
+                    found_endpoint = endpoint
+                    break
                 else:
-                    logger.debug(f'Connection to {endpoint_uuid} failed')
+                    logger.debug(
+                        f'Connection to {endpoint_uuid} returned '
+                        'different UUID',
+                    )
+            else:
+                logger.debug(f'Connection to {endpoint_uuid} failed')
 
         if found_endpoint is None:
             self._session.close()
             raise EndpointConnectorError(
                 'Failed to find an endpoint configuration matching one of the '
                 'provided endpoint UUIDs, or an endpoint configuration was '
                 'found but the endpoint could not be connected to. '
```

### Comparing `proxystore-0.6.3/proxystore/connectors/file.py` & `proxystore-0.6.4/proxystore/connectors/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """File system connector implementation."""
+
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 import sys
 import uuid
@@ -80,15 +81,15 @@
             clear: Remove the store directory. Overrides the default
                 value of `clear` provided when the
                 [`FileConnector`][proxystore.connectors.file.FileConnector]
                 was instantiated.
         """
         clear = self.clear if clear is None else clear
         if clear and os.path.isdir(self.store_dir):
-            shutil.rmtree(self.store_dir)
+            shutil.rmtree(self.store_dir, ignore_errors=True)
 
     def config(self) -> dict[str, Any]:
         """Get the connector configuration.
 
         The configuration contains all the information needed to reconstruct
         the connector object.
         """
```

### Comparing `proxystore-0.6.3/proxystore/connectors/globus.py` & `proxystore-0.6.4/proxystore/connectors/globus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Globus transfer connector implementation."""
+
 from __future__ import annotations
 
 import json
 import logging
 import os
 import re
 import sys
```

### Comparing `proxystore-0.6.3/proxystore/connectors/local.py` & `proxystore-0.6.4/proxystore/connectors/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """In-process local storage connector implementation."""
+
 from __future__ import annotations
 
 import logging
 import sys
 import uuid
 from types import TracebackType
 from typing import Any
```

### Comparing `proxystore-0.6.3/proxystore/connectors/multi.py` & `proxystore-0.6.4/proxystore/connectors/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Multi-connector implementation."""
+
 from __future__ import annotations
 
 import dataclasses
 import logging
 import re
 import sys
 import warnings
@@ -19,16 +20,16 @@
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     from typing import Self
 else:  # pragma: <3.11 cover
     from typing_extensions import Self
 
 from proxystore import utils
 from proxystore.connectors.protocols import Connector
-from proxystore.utils.imports import get_class_path
-from proxystore.utils.imports import import_class
+from proxystore.utils.imports import get_object_path
+from proxystore.utils.imports import import_from_path
 from proxystore.warnings import ExperimentalWarning
 
 warnings.warn(
     'MultiConnector is an experimental feature and may change in the future.',
     category=ExperimentalWarning,
     stacklevel=2,
 )
@@ -300,15 +301,15 @@
             self.dormant_connectors
             if self.dormant_connectors is not None
             else {}
         )
         configs.update(
             {
                 name: (
-                    get_class_path(type(connector)),
+                    get_object_path(type(connector)),
                     connector.config(),
                     policy.as_dict(),
                 )
                 for name, (connector, policy) in self.connectors.items()
             },
         )
         return configs
@@ -324,15 +325,15 @@
             config: Configuration returned by `#!python .config()`.
         """
         connectors: dict[str, tuple[Connector[Any], Policy]] = {}
         dormant_connectors: dict[str, ConnectorPolicyConfig] = {}
         for name, (conn_path, conn_config, policy_dict) in config.items():
             policy = Policy(**policy_dict)
             if policy.is_valid_on_host():
-                connector_type = import_class(conn_path)
+                connector_type = import_from_path(conn_path)
                 connector = connector_type.from_config(conn_config)
                 connectors[name] = (connector, policy)
             else:
                 dormant_connectors[name] = config[name]
         return cls(
             connectors=connectors,
             dormant_connectors=dormant_connectors,
```

### Comparing `proxystore-0.6.3/proxystore/connectors/protocols.py` & `proxystore-0.6.4/proxystore/connectors/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Connector protocol."""
+
 from __future__ import annotations
 
 from typing import Any
 from typing import NamedTuple
 from typing import Protocol
 from typing import runtime_checkable
 from typing import Sequence
@@ -16,15 +17,19 @@
     """Connector protocol for interfacing with external object storage.
 
     The Connector protocol defines the interface for interacting with
     a byte-level object store.
     """
 
     def close(self) -> None:
-        """Close the connector and clean up."""
+        """Close the connector and clean up.
+
+        Note:
+            Implementations should make this idempotent.
+        """
         ...
 
     def config(self) -> dict[str, Any]:
         """Get the connector configuration.
 
         The configuration contains all the information needed to reconstruct
         the connector object.
```

### Comparing `proxystore-0.6.3/proxystore/connectors/redis.py` & `proxystore-0.6.4/proxystore/connectors/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Redis connector implementation."""
+
 from __future__ import annotations
 
 import sys
 import uuid
 from types import TracebackType
 from typing import Any
 from typing import NamedTuple
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/__init__.py` & `proxystore-0.6.4/proxystore/endpoint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 
 [`Endpoints`][proxystore.endpoint.endpoint.Endpoint] are in-memory object
 stores with peering capabilities. Endpoints enable peer-to-peer data transfer
 between clients behind different NATs. See the
 [`proxystore-endpoint`](../cli.md#proxystore-endpoint) CLI reference
 to start your own endpoints.
 """
+
 from __future__ import annotations
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/cli.py` & `proxystore-0.6.4/proxystore/endpoint/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """`proxystore-endpoint` command-line interface.
 
 See the CLI Reference for the
 [`proxystore-endpoint`](../cli.md#proxystore-endpoint) usage instructions.
 """
+
 from __future__ import annotations
 
 import logging
 import os
 import sys
 import uuid
 from typing import ClassVar
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/client.py` & `proxystore-0.6.4/proxystore/endpoint/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for client interactions with endpoints."""
+
 from __future__ import annotations
 
 import uuid
 
 import requests
 from requests.exceptions import RequestException  # noqa: F401
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/commands.py` & `proxystore-0.6.4/proxystore/endpoint/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Endpoint management commands.
 
 These are the implementations of the commands available via the
 [`proxystore-endpoint`](../cli.md#proxystore-endpoint) command.
 Subsequently, all commands log errors and results and return status codes
 (rather than raising errors and returning results).
 """
+
 from __future__ import annotations
 
 import contextlib
 import enum
 import logging
 import os
 import shutil
@@ -332,16 +333,17 @@
             pidfile=daemon.pidfile.PIDLockFile(pid_file),
             detach_process=True,
             # Note: stdin, stdout, stderr left as None which binds to /dev/null
         )
     else:
         context = _attached_pid_manager(pid_file)
 
-    # TODO: handle sigterm/sigkill exit codes/graceful shutdown.
     with context:
+        # Note: serve will handle most interrupts which can be reasonably
+        # handled and return gracefully.
         serve(cfg, log_level=log_level, log_file=log_file)
 
     return 0
 
 
 def stop_endpoint(name: str, *, proxystore_dir: str | None = None) -> int:
     """Stop endpoint.
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/config.py` & `proxystore-0.6.4/proxystore/endpoint/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """Endpoint configuration."""
+
 from __future__ import annotations
 
 import os
 import re
 import uuid
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
-from pydantic import field_validator
+
+try:
+    from pydantic import field_validator
+except ImportError:  # pragma: no cover
+    # Pydantic v1 compatibility
+    from pydantic import validator as field_validator
 
 from proxystore.endpoint.constants import MAX_OBJECT_SIZE_DEFAULT
 from proxystore.utils.config import dump
 from proxystore.utils.config import load
 
 ENDPOINT_CONFIG_FILE = 'config.toml'
 ENDPOINT_DATABASE_FILE = 'blobs.db'
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/endpoint.py` & `proxystore-0.6.4/proxystore/endpoint/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Endpoint implementation."""
+
 from __future__ import annotations
 
 import asyncio
 import enum
 import logging
 from types import TracebackType
 from typing import Any
@@ -324,17 +325,17 @@
 
         Any exceptions will be set on the returned future.
         """
         # TODO(gpauloski):
         #   - should some ops be sent to all endpoints that may have
         #     a copy of the data (mostly for evict)?
         assert self.peer_manager is not None
-        self._pending_requests[
-            request.uuid
-        ] = asyncio.get_running_loop().create_future()
+        self._pending_requests[request.uuid] = (
+            asyncio.get_running_loop().create_future()
+        )
         logger.debug(
             f'{self._log_prefix}: sending {request.op} request with '
             f'id={request.uuid} and key={request.key}) to {endpoint}',
         )
         try:
             await self.peer_manager.send(endpoint, serialize(request))
         except Exception as e:
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/exceptions.py` & `proxystore-0.6.4/proxystore/endpoint/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Endpoint exceptions."""
+
 from __future__ import annotations
 
 
 class FileDumpNotAvailableError(Exception):
     """Error raised when dumping objects to file is not available."""
 
     pass
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/messages.py` & `proxystore-0.6.4/proxystore/endpoint/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Endpoint to endpoint messages."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Literal
 
 
 @dataclass
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/serve.py` & `proxystore-0.6.4/proxystore/endpoint/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Endpoint serving."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import os
+import signal
 import uuid
 from typing import Any
 from typing import Literal
 
 try:
     import quart
     import uvicorn
@@ -211,24 +213,40 @@
         logger.info('Installing uvloop as default event loop')
         uvloop.install()
     else:
         logger.warning(
             'Not installing uvloop. Uvicorn may override and install anyways',
         )
 
+    # Convert SIGTERM to SIGINT which will be handled by Uvicorn first,
+    # then passed on by this function.
+    signal.signal(
+        signal.SIGTERM,
+        lambda *_args: signal.raise_signal(signal.SIGINT),
+    )
+
     # The remaining set up and serving code is deferred to within the
     # _serve_async helper function which will be executed within an event loop.
     try:
         asyncio.run(_serve_async(config))
     except Exception as e:
         # Intercept exception so we can log it in the case that the endpoint
         # is running as a daemon process. Otherwise the user will never see
         # the exception.
         logger.exception(f'Caught unhandled exception: {e!r}')
         raise
+    except KeyboardInterrupt:  # pragma: no cover
+        # Uvicorn<0.29.0 captures SIGINT and does not propagate is.
+        # Uvicorn>=0.29.1 changes this behavior to propagate the SIGINT after
+        # Uvicorn has done it's cleanup, so we need to catch the exception
+        # here and pass on it since we let Uvicorn handle our clean up in
+        # the "after_app_serving" shutdown callback. This is excluded from
+        # coverage because it depends on the Uvicorn version.
+        # Relevant PR: https://github.com/encode/uvicorn/pull/1600
+        pass
     finally:
         logger.info(f'Finished serving endpoint: {config.name}')
 
 
 @routes_blueprint.before_app_serving
 async def _startup() -> None:
     endpoint = quart.current_app.config['endpoint']
```

### Comparing `proxystore-0.6.3/proxystore/endpoint/storage.py` & `proxystore-0.6.4/proxystore/endpoint/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Blob storage interface for endpoints."""
+
 from __future__ import annotations
 
 import pathlib
 from typing import Protocol
 from typing import runtime_checkable
 
 import aiosqlite
```

### Comparing `proxystore-0.6.3/proxystore/ex.py` & `proxystore-0.6.4/proxystore/ex.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 [extensions.proxystore.dev/latest/api](https://extensions.proxystore.dev/latest/api/){target=_blank}.
 
 Warning:
     A import error will be raised if `proxystore-ex` is not installed.
     See the [Installation](../installation.md) page for installation
     instructions.
 """
+
 from __future__ import annotations
 
 from typing import Any
 
 _import_error_message = """\
 The proxystore_ex package is not installed.
```

### Comparing `proxystore-0.6.3/proxystore/factory.py` & `proxystore-0.6.4/proxystore/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Factory implementations.
 
 Factories are callable classes that wrap up the functionality needed
 to resolve a proxy, where resolving is the process of retrieving the
 object from wherever it is stored such that the proxy can act as the
 object.
 """
+
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
 from typing import Generic
 from typing import TypeVar
```

### Comparing `proxystore-0.6.3/proxystore/globus/cli.py` & `proxystore-0.6.4/proxystore/globus/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 proxystore-globus-auth logout
 # give consent for specific collections
 proxystore-globus-auth login --collection COLLECTION_UUID --collection COLLECTION_UUID ...
 # specify additional scopes
 proxystore-globus-auth login --scope SCOPE --scope SCOPE ...
 ```
 """  # noqa: E501
+
 from __future__ import annotations
 
 import click
 
 from proxystore.globus.manager import NativeAppAuthManager
 from proxystore.globus.scopes import get_all_scopes_by_resource_server
```

### Comparing `proxystore-0.6.3/proxystore/globus/client.py` & `proxystore-0.6.4/proxystore/globus/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create Globus Auth clients."""
+
 from __future__ import annotations
 
 import os
 import uuid
 
 import globus_sdk
```

### Comparing `proxystore-0.6.3/proxystore/globus/manager.py` & `proxystore-0.6.4/proxystore/globus/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Globus Auth credential managers."""
+
 from __future__ import annotations
 
 import platform
 from typing import Iterable
 from typing import Protocol
 from typing import runtime_checkable
```

### Comparing `proxystore-0.6.3/proxystore/globus/scopes.py` & `proxystore-0.6.4/proxystore/globus/scopes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Build Globus Auth scopes."""
+
 from __future__ import annotations
 
 from typing import Iterable
 
 from globus_sdk.scopes import AuthScopes
 from globus_sdk.scopes import GCSCollectionScopeBuilder
 from globus_sdk.scopes import ScopeBuilder
```

### Comparing `proxystore-0.6.3/proxystore/globus/storage.py` & `proxystore-0.6.4/proxystore/globus/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Globus Auth token storage."""
+
 from __future__ import annotations
 
 import os
 import pathlib
 
 from globus_sdk.tokenstorage import SQLiteAdapter
```

### Comparing `proxystore-0.6.3/proxystore/globus/transfer.py` & `proxystore-0.6.4/proxystore/globus/transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create and authenticate a Globus Transfer client."""
+
 from __future__ import annotations
 
 from typing import Iterable
 
 import click
 import globus_sdk
```

### Comparing `proxystore-0.6.3/proxystore/p2p/__init__.py` & `proxystore-0.6.4/proxystore/p2p/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,9 @@
   NATs. Peer connections are established using
   [aiortc](https://aiortc.readthedocs.io/){target=_blank}, an asyncio WebRTC
   implementation.
 * The [`proxystore.p2p.relay`][proxystore.p2p.relay] module provides
   implementations of the relay server and associated clients that are used by
   peers to facilitate WebRTC peer connections.
 """
+
 from __future__ import annotations
```

### Comparing `proxystore-0.6.3/proxystore/p2p/chunks.py` & `proxystore-0.6.4/proxystore/p2p/chunks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Message chunking utilities."""
+
 from __future__ import annotations
 
 import enum
 import math
 from struct import pack
 from struct import unpack_from
 from typing import Generator
```

### Comparing `proxystore-0.6.3/proxystore/p2p/connection.py` & `proxystore-0.6.4/proxystore/p2p/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Representation of peer-to-peer connection."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import re
 import warnings
 from collections import defaultdict
@@ -103,17 +104,17 @@
         relay_client: RelayClient,
         *,
         channels: int = 1,
     ) -> None:
         self._relay_client = relay_client
         self._max_channels = channels
 
-        self._handshake_success: asyncio.Future[
-            bool
-        ] = asyncio.get_running_loop().create_future()
+        self._handshake_success: asyncio.Future[bool] = (
+            asyncio.get_running_loop().create_future()
+        )
         self._pc = RTCPeerConnection()
 
         self._incoming_queue: asyncio.Queue[bytes | str] = asyncio.Queue()
         self._incoming_chunks: dict[int, list[Chunk]] = defaultdict(list)
         # Max size of unsigned long (4 bytes) is 2^32 - 1
         self._message_counter = AtomicCounter(size=2**32 - 1)
```

### Comparing `proxystore-0.6.3/proxystore/p2p/manager.py` & `proxystore-0.6.4/proxystore/p2p/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manager of many peer-to-peer connections."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from types import TracebackType
 from typing import Any
 from typing import Generator
@@ -92,17 +93,17 @@
         self._relay_client = relay_client
         self._timeout = timeout
         self._peer_channels = peer_channels
 
         self._peers_lock = asyncio.Lock()
         self._peers: dict[frozenset[UUID], PeerConnection] = {}
 
-        self._message_queue: asyncio.Queue[
-            tuple[UUID, bytes | str]
-        ] = asyncio.Queue()
+        self._message_queue: asyncio.Queue[tuple[UUID, bytes | str]] = (
+            asyncio.Queue()
+        )
         self._server_task: asyncio.Task[None] | None = None
         self._tasks: dict[frozenset[UUID], asyncio.Task[None]] = {}
 
     @property
     def _log_prefix(self) -> str:
         return f'{self.__class__.__name__}[{log_name(self.uuid, self.name)}]'
```

### Comparing `proxystore-0.6.3/proxystore/p2p/nat.py` & `proxystore-0.6.4/proxystore/p2p/nat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tools for getting the NAT type using STUN.
 
 This module is a wrapper around the tools provided by
 [pystun3](https://github.com/talkiq/pystun3){target=_blank}.
 """
+
 from __future__ import annotations
 
 import enum
 import logging
 import socket
 from typing import NamedTuple
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/authenticate.py` & `proxystore-0.6.4/proxystore/p2p/relay/authenticate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Authenticate users from request headers."""
+
 from __future__ import annotations
 
 import dataclasses
 import uuid
 from typing import Any
 from typing import Mapping
 from typing import Protocol
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/client.py` & `proxystore-0.6.4/proxystore/p2p/relay/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Client interface to a relay server."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import ssl
 import sys
 import uuid
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/config.py` & `proxystore-0.6.4/proxystore/p2p/relay/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Relay server configuration file parsing."""
+
 from __future__ import annotations
 
 import logging
 import pathlib
 import sys
 from typing import Any
 from typing import Dict
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/exceptions.py` & `proxystore-0.6.4/proxystore/p2p/relay/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Exception types raised by relay clients and servers."""
+
 from __future__ import annotations
 
 
 class RelayClientError(Exception):
     """Base exception type for exceptions raised by relay clients."""
 
     pass
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/manager.py` & `proxystore-0.6.4/proxystore/p2p/relay/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper classes for managing clients connected to a relay server."""
+
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import uuid
 from typing import Generic
 from typing import TypeVar
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/messages.py` & `proxystore-0.6.4/proxystore/p2p/relay/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Message types for relay client and relay server communication."""
+
 from __future__ import annotations
 
 import dataclasses
 import enum
 import json
 import sys
 import uuid
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/run.py` & `proxystore-0.6.4/proxystore/p2p/relay/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI and serving functions for running a Globus Auth relay server."""
+
 from __future__ import annotations
 
 import asyncio
 import datetime
 import logging
 import logging.handlers
 import os
```

### Comparing `proxystore-0.6.3/proxystore/p2p/relay/server.py` & `proxystore-0.6.4/proxystore/p2p/relay/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Relay server implementation for facilitating WebRTC peer connections.
 
 The relay server (or signaling server) is a lightweight server accessible by
 all peers (e.g., has a public IP address) that facilitates the establishment
 of peer WebRTC connections.
 """
+
 from __future__ import annotations
 
 import logging
 import sys
 from typing import Generic
 from typing import TypeVar
```

### Comparing `proxystore-0.6.3/proxystore/proxy.py` & `proxystore-0.6.4/proxystore/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Proxy implementation and helpers."""
+
 from __future__ import annotations
 
 import sys
 from typing import Any
 from typing import Callable
 from typing import Generic
 from typing import SupportsIndex
```

### Comparing `proxystore-0.6.3/proxystore/serialize.py` & `proxystore-0.6.4/proxystore/serialize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Serialization functions."""
+
 from __future__ import annotations
 
 import pickle
 from typing import Any
 
 import cloudpickle
 
@@ -25,29 +26,39 @@
 
     Args:
         obj: Object to serialize.
 
     Returns:
         Bytes that can be passed to \
         [`deserialize()`][proxystore.serialize.deserialize].
+
+    Raises:
+        SerializationError: If serializing the object fails with all available
+            serializers. Cloudpickle is the last resort, so this error will
+            typically be raised from a cloudpickle error.
     """
     if isinstance(obj, bytes):
         identifier = b'01\n'
     elif isinstance(obj, str):
         identifier = b'02\n'
         obj = obj.encode()
     else:
         # Use cloudpickle if pickle fails
         try:
             identifier = b'03\n'
             # Pickle protocol 5 is available in Python 3.8 and later
             obj = pickle.dumps(obj, protocol=5)
         except Exception:
             identifier = b'04\n'
-            obj = cloudpickle.dumps(obj)
+            try:
+                obj = cloudpickle.dumps(obj)
+            except Exception as e:
+                raise SerializationError(
+                    f'Object of type {type(obj)} is not serializable.',
+                ) from e
 
     assert isinstance(identifier, bytes)
     assert isinstance(obj, bytes)
 
     return identifier + obj
 
 
@@ -64,14 +75,16 @@
     Raises:
         ValueError: If `data` is not of type `bytes`.
         SerializationError: If the identifier of `data` is missing or
             invalid. The identifier is prepended to the string in
             [`serialize()`][proxystore.serialize.serialize] to indicate which
             serialization method was used (e.g., no serialization, pickle,
             etc.).
+        SerializationError: If pickle or cloudpickle raise an exception
+            when deserializing the object.
     """
     if not isinstance(data, bytes):
         raise ValueError(
             f'Expected data to be of type bytes, not {type(data)}.',
         )
     identifier, separator, data = data.partition(b'\n')
     if separator == b'' or len(identifier) != len(b'00'):
@@ -79,14 +92,24 @@
             'Data does not have required identifier for deserialization.',
         )
     if identifier == b'01':
         return data
     elif identifier == b'02':
         return data.decode()
     elif identifier == b'03':
-        return pickle.loads(data)
+        try:
+            return pickle.loads(data)
+        except Exception as e:
+            raise SerializationError(
+                'Failed to deserialize object with pickle.',
+            ) from e
     elif identifier == b'04':
-        return cloudpickle.loads(data)
+        try:
+            return cloudpickle.loads(data)
+        except Exception as e:
+            raise SerializationError(
+                'Failed to deserialize object with cloudpickle.',
+            ) from e
     else:
         raise SerializationError(
             f'Unknown identifier {identifier!r} for deserialization,',
         )
```

### Comparing `proxystore-0.6.3/proxystore/store/__init__.py` & `proxystore-0.6.4/proxystore/store/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The ProxyStore [`Store`][proxystore.store.base.Store] interface."""
+
 from __future__ import annotations
 
 import contextlib
 import logging
 from typing import Any
 from typing import Generator
 from typing import Sequence
@@ -146,8 +147,8 @@
         name_or_store: Name of the store to unregister or a store itself.
     """
     name = (
         name_or_store if isinstance(name_or_store, str) else name_or_store.name
     )
     if name in _stores:
         del _stores[name]
-        logger.debug(f'Unregistered a store named {name}')
+        logger.info(f'Unregistered a store named {name}')
```

### Comparing `proxystore-0.6.3/proxystore/store/cache.py` & `proxystore-0.6.4/proxystore/store/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Simple Cache Implementation."""
+
 from __future__ import annotations
 
 from typing import Generic
 from typing import TypeVar
 
 KeyT = TypeVar('KeyT')
 ValueT = TypeVar('ValueT')
```

### Comparing `proxystore-0.6.3/proxystore/store/exceptions.py` & `proxystore-0.6.4/proxystore/store/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Exceptions for Stores."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from proxystore.store import base
```

### Comparing `proxystore-0.6.3/proxystore/store/factory.py` & `proxystore-0.6.4/proxystore/store/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Factory implementations."""
+
 from __future__ import annotations
 
 import logging
 import threading
 import time
 from concurrent.futures import Future
 from concurrent.futures import ThreadPoolExecutor
@@ -158,47 +159,58 @@
             needed.
         deserializer: Optional callable used to deserialize the byte string.
             If `None`, the default deserializer
             ([`deserialize()`][proxystore.serialize.deserialize]) will be used.
         evict: If True, evict the object from the store once
             [`resolve()`][proxystore.store.base.StoreFactory.resolve]
             is called.
-        polling_interval: Seconds to sleep between polling the store for the
-            object.
-        polling_timeout: Optional maximum number of seconds to poll for.
+        polling_interval: Initial seconds to sleep between polling the store
+            for the object.
+        polling_backoff_factor: Multiplicative factor applied to the
+            polling_interval applied after each unsuccessful poll.
+        polling_interval_limit: Maximum polling interval allowed. Prevents
+            the backoff factor from increasing the current polling interval
+            to unreasonable values.
+        polling_timeout: Optional maximum number of seconds to poll for. If
+            the timeout is reached an error is raised.
     """
 
     def __init__(
         self,
         key: ConnectorKeyT,
         store_config: dict[str, Any],
         *,
         deserializer: DeserializerT | None = None,
         evict: bool = False,
         polling_interval: float = 1,
+        polling_backoff_factor: float = 1,
+        polling_interval_limit: float | None = None,
         polling_timeout: float | None = None,
     ) -> None:
         super().__init__(
             key,
             store_config,
             evict=evict,
             deserializer=deserializer,
         )
         self._polling_interval = polling_interval
+        self._polling_backoff_factor = polling_backoff_factor
+        self._polling_interval_limit = polling_interval_limit
         self._polling_timeout = polling_timeout
 
     def resolve(self) -> T:
         """Get object associated with key from store.
 
         Raises:
             ProxyResolveMissingKeyError: If the object associated with the
                 key is not available after `polling_timeout` seconds.
         """
         with Timer() as timer:
             store = self.get_store()
+            sleep_interval = self._polling_interval
             time_waited = 0.0
 
             while True:
                 obj = store.get(
                     self.key,
                     deserializer=self.deserializer,
                     default=_MISSING_OBJECT,
@@ -207,16 +219,22 @@
                 # Break because we found the object or we hit the timeout
                 if obj is not _MISSING_OBJECT or (
                     self._polling_timeout is not None
                     and time_waited >= self._polling_timeout
                 ):
                     break
 
-                time.sleep(self._polling_interval)
-                time_waited += self._polling_interval
+                time.sleep(sleep_interval)
+                time_waited += sleep_interval
+                new_interval = sleep_interval * self._polling_backoff_factor
+                sleep_interval = (
+                    new_interval
+                    if self._polling_interval_limit is None
+                    else min(new_interval, self._polling_interval_limit)
+                )
 
             if obj is _MISSING_OBJECT:
                 raise ProxyResolveMissingKeyError(
                     self.key,
                     type(store),
                     store.name,
                 )
```

### Comparing `proxystore-0.6.3/proxystore/store/future.py` & `proxystore-0.6.4/proxystore/store/future.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Proxy-future interface implementation."""
+
 from __future__ import annotations
 
 from typing import Generic
 from typing import TypeVar
 
 from proxystore.proxy import Proxy
 from proxystore.store.factory import PollingStoreFactory
 from proxystore.store.types import ConnectorT
 from proxystore.store.types import SerializerT
 
 T = TypeVar('T')
 
 
-class ProxyFuture(Generic[T]):
-    """Proxy-Future interface to a [`Store`][proxystore.store.base.Store].
+class Future(Generic[T]):
+    """Future interface to a [`Store`][proxystore.store.base.Store].
 
     Args:
         factory: Factory that can resolve the object once it is resolved.
             This factory should block when resolving until the object is
             available.
         serializer: Use a custom serializer when setting the result object
             of this future.
@@ -28,14 +29,18 @@
         factory: PollingStoreFactory[ConnectorT, T],
         *,
         serializer: SerializerT | None = None,
     ) -> None:
         self._factory = factory
         self._serializer = serializer
 
+    def done(self) -> bool:
+        """Check if the result has been set yet."""
+        return self._factory.get_store().exists(self._factory.key)
+
     def proxy(self) -> Proxy[T]:
         """Create a proxy which will resolve to the result of this future."""
         return Proxy(self._factory)
 
     def result(self) -> T:
         """Get the result object of this future."""
         return self._factory.resolve()
```

### Comparing `proxystore-0.6.3/proxystore/store/metrics.py` & `proxystore-0.6.4/proxystore/store/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utilities for recording Store operation metrics.
 
 See the [Performance Guide](../../guides/performance.md) to learn more about
 interacting with metrics recorded for
 [`Store`][proxystore.store.base.Store] operations.
 """
+
 from __future__ import annotations
 
 import copy
 import dataclasses
 import math
 import sys
 import time
```

### Comparing `proxystore-0.6.3/proxystore/store/types.py` & `proxystore-0.6.4/proxystore/store/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common type definitions."""
+
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
 from typing import Tuple
 from typing import TypeVar
```

### Comparing `proxystore-0.6.3/proxystore/store/utils.py` & `proxystore-0.6.4/proxystore/store/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Store utilities."""
+
 from __future__ import annotations
 
 from typing import Any
 from typing import Tuple
 from typing import TypeVar
 
 from proxystore.proxy import is_resolved
```

### Comparing `proxystore-0.6.3/proxystore/stream/__init__.py` & `proxystore-0.6.4/proxystore/stream/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Note:
     The [StreamProducer][proxystore.stream.interface.StreamProducer]
     and [StreamConsumer][proxystore.stream.interface.StreamConsumer]
     are defined in [`proxystore.stream.interface`][proxystore.stream.interface]
     are re-exported here for convenience.
 """
+
 from __future__ import annotations
 
 import warnings
 
 from proxystore.stream.interface import StreamConsumer
 from proxystore.stream.interface import StreamProducer
 from proxystore.warnings import ExperimentalWarning
```

### Comparing `proxystore-0.6.3/proxystore/stream/events.py` & `proxystore-0.6.4/proxystore/stream/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
     Event types are not considered as part of the public API and may change
     at any time without warning. [`Events`][proxystore.stream.events.Event]
     are created and consumed internally by the
     [StreamProducer][proxystore.stream.interface.StreamProducer] and
     [StreamConsumer][proxystore.stream.interface.StreamConsumer] and
     never exposed to client code.
 """
+
 from __future__ import annotations
 
 import dataclasses
 import enum
 import json
 from typing import Any
 from typing import Union
 
-from proxystore.utils.imports import get_class_path
-from proxystore.utils.imports import import_class
+from proxystore.utils.imports import get_object_path
+from proxystore.utils.imports import import_from_path
 
 
 @dataclasses.dataclass
 class EndOfStreamEvent:
     """End of stream event."""
 
     @classmethod
@@ -49,23 +50,23 @@
         cls,
         key: tuple[Any, ...],
         evict: bool,
         metadata: dict[str, Any],
     ) -> NewObjectEvent:
         """Create a new event from a key and metadata."""
         return cls(
-            key_type=get_class_path(type(key)),
+            key_type=get_object_path(type(key)),
             raw_key=list(key),
             evict=evict,
             metadata=metadata,
         )
 
     def get_key(self) -> Any:
         """Get the object key associated with the event."""
-        key_type = import_class(self.key_type)
+        key_type = import_from_path(self.key_type)
         return key_type(*self.raw_key)
 
 
 Event = Union[EndOfStreamEvent, NewObjectEvent]
 """Event union type."""
```

### Comparing `proxystore-0.6.3/proxystore/stream/filters.py` & `proxystore-0.6.4/proxystore/stream/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Set of common stream filters."""
+
 from __future__ import annotations
 
 import random
 from typing import Any
 
 
 class NullFilter:
```

### Comparing `proxystore-0.6.3/proxystore/stream/interface.py` & `proxystore-0.6.4/proxystore/stream/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Note:
     The [StreamProducer][proxystore.stream.interface.StreamProducer]
     and [StreamConsumer][proxystore.stream.interface.StreamConsumer]
     are re-exported in [`proxystore.stream`][proxystore.stream] for
     convenience.
 """
+
 from __future__ import annotations
 
 import dataclasses
 import logging
 import sys
 import threading
 from collections import defaultdict
@@ -90,14 +91,17 @@
         ```python
         producer = StreamProducer[str](...)
         # mypy will raise an error that StreamProducer.send() expects a str
         # but got a list[int].
         producer.send('default', [1, 2, 3])
         ```
 
+    Attributes:
+        publisher: Publisher interface.
+
     Args:
         publisher: Object which implements the
             [`Publisher`][proxystore.stream.protocols.Publisher] protocol.
             Used to publish event messages when new objects are added to
             the stream.
         stores: Mapping from topic names to the
             [`Store`][proxystore.store.base.Store] instance used to store
@@ -123,15 +127,15 @@
         publisher: Publisher,
         stores: Mapping[str | None, Store[Any]],
         *,
         aggregator: Callable[[list[T]], T] | None = None,
         batch_size: int = 1,
         filter_: Filter | None = None,
     ) -> None:
-        self._publisher = publisher
+        self.publisher = publisher
         self._stores = stores
         self._aggregator = aggregator
         self._batch_size = batch_size
         self._filter: Filter = filter_ if filter_ is not None else NullFilter()
 
         # Mapping between topic and buffers
         self._buffer: dict[str, _TopicBuffer[T]] = defaultdict(
@@ -150,27 +154,28 @@
         self.close()
 
     def close(
         self,
         *,
         topics: Iterable[str] = (),
         publisher: bool = True,
-        stores: bool = True,
+        stores: bool = False,
     ) -> None:
         """Close the producer.
 
         Warning:
             Objects buffered in an incomplete batch will be lost. Call
             [`flush()`][proxystore.stream.interface.StreamProducer] to ensure
             that all objects are sent before closing.
 
         Warning:
-            By default, this will also call `close()` on the
-            [`Store`][proxystore.store.base.Store] and
-            [`Publisher`][proxystore.stream.protocols.Publisher] interfaces.
+            By default, this will close the
+            [`Publisher`][proxystore.stream.protocols.Publisher] interface,
+            but will **not** close the [`Store`][proxystore.store.base.Store]
+            interfaces.
 
         Args:
             topics: Topics to send end of stream events to. Equivalent to
                 calling [`close_topics()`][proxystore.stream.interface.StreamProducer.close_topics]
                 first.
             publisher: Close the
                 [`Publisher`][proxystore.stream.protocols.Publisher] interface.
@@ -179,15 +184,15 @@
         """  # noqa: E501
         self.close_topics(*topics)
         if stores:
             for store in self._stores.values():
                 store.close()
                 unregister_store(store)
         if publisher:
-            self._publisher.close()
+            self.publisher.close()
 
     def close_topics(self, *topics: str) -> None:
         """Send publish an end of stream event to each topic.
 
         A [`StreamConsumer`][proxystore.stream.interface.StreamConsumer]
         will raise a [`StopIteration`][StopIteration] exception when an
         end of stream event is received. The end of stream event is still
@@ -254,31 +259,37 @@
             store = self._stores[None]
         else:
             raise ValueError(
                 f'No store associated with topic "{topic}" found or '
                 'default store.',
             )
 
-        keys = store.put_batch([item.obj for item in objects])
+        events: list[Event] = []
 
-        events: list[Event] = [
-            NewObjectEvent.from_key(
-                key,
-                evict=item.evict,
-                metadata=item.metadata,
-            )
-            for key, item in zip(keys, objects)
-        ]
+        if len(objects) > 0:
+            keys = store.put_batch([item.obj for item in objects])
+
+            for key, item in zip(keys, objects):
+                event = NewObjectEvent.from_key(
+                    key,
+                    evict=item.evict,
+                    metadata=item.metadata,
+                )
+                events.append(event)
 
         if closed:
             events.append(EndOfStreamEvent())
 
+        # If there are no new events and the stream wasn't closed we should
+        # have early exited
+        assert len(events) > 0
+
         batch_event = EventBatch(events, topic, store.config())
         message = event_to_bytes(batch_event)
-        self._publisher.send(topic, message)
+        self.publisher.send(topic, message)
 
     def send(
         self,
         topic: str,
         obj: T,
         *,
         evict: bool = True,
@@ -388,14 +399,17 @@
         [`StreamProducer.send()`][proxystore.stream.interface.StreamProducer.send]
         is set correctly and the there is not code incidentally resolving
         proxies before you expect.
 
     Note:
         The consumer is not thread-safe.
 
+    Attributes:
+        subscriber: Subscriber interface.
+
     Args:
         subscriber: Object which implements the
             [`Subscriber`][proxystore.stream.protocols.Subscriber] protocol.
             Used to listen for new event messages indicating new objects
             in the stream.
         filter_: Optional filter to apply to event metadata received from the
             stream. If the filter returns `True`, the event will be
@@ -406,15 +420,15 @@
 
     def __init__(
         self,
         subscriber: Subscriber,
         *,
         filter_: Filter | None = None,
     ) -> None:
-        self._subscriber = subscriber
+        self.subscriber = subscriber
         self._stores: dict[str, Store[Any]] = {}
         self._filter: Filter = filter_ if filter_ is not None else NullFilter()
 
         self._current_batch: EventBatch | None = None
 
     def __enter__(self) -> Self:
         return self
@@ -431,51 +445,52 @@
         """Return an iterator that will yield proxies of stream objects."""
         return self
 
     def __next__(self) -> Proxy[T]:
         """Alias for [`next()`][proxystore.stream.interface.StreamConsumer.next]."""  # noqa: E501
         return self.next()
 
-    def close(self, *, stores: bool = True, subscriber: bool = True) -> None:
+    def close(self, *, stores: bool = False, subscriber: bool = True) -> None:
         """Close the consumer.
 
         Warning:
-            By default, this will also call `close()` on the
-            [`Store`][proxystore.store.base.Store] and
-            [`Publisher`][proxystore.stream.protocols.Publisher] interfaces.
+            By default, this will close the
+            [`Subscriber`][proxystore.stream.protocols.Subscriber] interface,
+            but will **not** close the [`Store`][proxystore.store.base.Store]
+            interfaces.
 
         Args:
             stores: Close and [unregister][proxystore.store.unregister_store]
                 the [`Store`][proxystore.store.base.Store] instances
                 used to resolve objects consumed from the stream.
             subscriber: Close the
                 [`Subscriber`][proxystore.stream.protocols.Subscriber]
                 interface.
         """
         if stores:
             for store in self._stores.values():
                 store.close()
                 unregister_store(store)
         if subscriber:
-            self._subscriber.close()
+            self.subscriber.close()
 
     def _get_store(self, event_info: _EventInfo) -> Store[Any]:
         if event_info.topic in self._stores:
             return self._stores[event_info.topic]
 
         with _consumer_get_store_lock:
             store = get_store(event_info.store_config['name'])
             if store is None:
                 store = Store.from_config(event_info.store_config)
                 register_store(store)
             self._stores[event_info.topic] = store
             return store
 
     def _next_batch(self) -> EventBatch:
-        message = next(self._subscriber)
+        message = next(self.subscriber)
         event = bytes_to_event(message)
         if isinstance(event, EventBatch):
             return event
         else:
             raise AssertionError('Unreachable.')
 
     def _next_event(self) -> _EventInfo:
@@ -518,27 +533,57 @@
                     store = self._get_store(event_info)
                     key = event.get_key()
                     store.evict(key)
                 continue
 
             return event_info
 
+    def iter_with_metadata(
+        self,
+    ) -> Generator[tuple[dict[str, Any], Proxy[T]], None, None]:
+        """Return an iterator that yields tuples of metadata and proxies.
+
+        Note:
+            This is different from `iter(consumer)` which will yield
+            *only* proxies of objects in the stream.
+        """
+        while True:
+            try:
+                yield self.next_with_metadata()
+            except StopIteration:
+                return
+
     def iter_objects(self) -> Generator[T, None, None]:
-        """Return an iterator that will yield objects from the stream.
+        """Return an iterator that yields objects from the stream.
 
         Note:
             This is different from `iter(consumer)` which will yield
             proxies of objects in the stream.
         """
         while True:
             try:
                 yield self.next_object()
             except StopIteration:
                 return
 
+    def iter_objects_with_metadata(
+        self,
+    ) -> Generator[tuple[dict[str, Any], T], None, None]:
+        """Return an iterator that yields tuples of metadata and objects.
+
+        Note:
+            This is different from `iter(consumer)` which will yield
+            proxies of objects in the stream.
+        """
+        while True:
+            try:
+                yield self.next_object_with_metadata()
+            except StopIteration:
+                return
+
     def next(self) -> Proxy[T]:
         """Return a proxy of the next object in the stream.
 
         Note:
             This method has the potential side effect of initializing and
             globally registering a new [`Store`][proxystore.store.base.Store]
             instance. This will happen at most once per topic because the
@@ -549,21 +594,40 @@
             class is closed.
 
         Raises:
             StopIteration: when an end of stream event is received from a
                 producer. Note that this does not call
                 [`close()`][proxystore.stream.interface.StreamConsumer.close].
         """
+        _, proxy = self.next_with_metadata()
+        return proxy
+
+    def next_with_metadata(self) -> tuple[dict[str, Any], Proxy[T]]:
+        """Return a tuple of metadata and proxy for the next object.
+
+        Note:
+            This method has the same potential side effects as
+            [`next()`][proxystore.stream.interface.StreamConsumer.next].
+
+        Returns:
+            Dictionary of user-provided metadata associated with the object.
+            Proxy of the next object in the stream.
+
+        Raises:
+            StopIteration: when an end of stream event is received from a
+                producer. Note that this does not call
+                [`close()`][proxystore.stream.interface.StreamConsumer.close].
+        """
         event_info = self._next_event_with_filter()
         store = self._get_store(event_info)
         event = event_info.event
         key = event.get_key()
 
         proxy: Proxy[T] = store.proxy_from_key(key, evict=event.evict)
-        return proxy
+        return event.metadata, proxy
 
     def next_object(self) -> T:
         """Return the next object in the stream.
 
         Note:
             This method has the same potential side effects as
             [`next()`][proxystore.stream.interface.StreamConsumer.next].
@@ -571,22 +635,41 @@
         Raises:
             StopIteration: when an end of stream event is received from a
                 producer. Note that this does not call
                 [`close()`][proxystore.stream.interface.StreamConsumer.close].
             ValueError: if the store does not return an object using the key
                 included in the object's event metadata.
         """
+        _, obj = self.next_object_with_metadata()
+        return obj
+
+    def next_object_with_metadata(self) -> tuple[dict[str, Any], T]:
+        """Return a tuple of metadata and the next object in the stream.
+
+        Note:
+            This method has the same potential side effects as
+            [`next()`][proxystore.stream.interface.StreamConsumer.next].
+
+        Returns:
+            Dictionary of user-provided metadata associated with the object.
+            Next object in the stream.
+
+        Raises:
+            StopIteration: when an end of stream event is received from a
+                producer. Note that this does not call
+                [`close()`][proxystore.stream.interface.StreamConsumer.close].
+        """
         event_info = self._next_event_with_filter()
         store = self._get_store(event_info)
         event = event_info.event
         key = event.get_key()
 
         obj = store.get(key)
         if obj is None:
             raise ValueError(
                 f'Store(name="{store.name}") returned None for key={key}.',
             )
 
         if event.evict:
             store.evict(key)
 
-        return cast(T, obj)
+        return event.metadata, cast(T, obj)
```

### Comparing `proxystore-0.6.3/proxystore/stream/protocols.py` & `proxystore-0.6.4/proxystore/stream/protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 Additional protocols, such as the
 [`Filter`][proxystore.stream.protocols.Filter], are plugins used by the
 [`StreamProducer`][proxystore.stream.interface.StreamProducer] and/or
 [`StreamConsumer`][proxystore.stream.interface.StreamConsumer] that alter
 their behavior.
 """
+
 from __future__ import annotations
 
 import sys
 from typing import Any
 from typing import Protocol
 from typing import runtime_checkable
 from typing import TypeVar
@@ -59,19 +60,17 @@
 class Subscriber(Protocol):
     """Subscriber interface to message stream.
 
     The subscriber protocol is an iterable object which yields objects
     from the stream until the stream is closed.
     """
 
-    def __iter__(self) -> Self:
-        ...
+    def __iter__(self) -> Self: ...
 
-    def __next__(self) -> bytes:
-        ...
+    def __next__(self) -> bytes: ...
 
     def close(self) -> None:
         """Close this subscriber."""
         ...
 
 
 class Filter(Protocol):
```

### Comparing `proxystore-0.6.3/proxystore/stream/shims/__init__.py` & `proxystore-0.6.4/proxystore/stream/shims/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/proxystore/stream/shims/kafka.py` & `proxystore-0.6.4/proxystore/stream/shims/kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Kafka publisher and subscriber shims.
 
 Shims to the
 [`kafka-python`](https://github.com/dpkp/kafka-python){target=_blank} package.
 """
+
 from __future__ import annotations
 
 import sys
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     from typing import Self
 else:  # pragma: <3.11 cover
```

### Comparing `proxystore-0.6.3/proxystore/stream/shims/queue.py` & `proxystore-0.6.4/proxystore/stream/shims/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Python queue-based pub/sub implementation.
 
 Warning:
     This implementation is meant for streaming between Python threads
     within the same process, or between Python processes on the same machine.
     Each queue topic may only have one subscriber.
 """
+
 from __future__ import annotations
 
 import multiprocessing
 import multiprocessing.queues
 import queue
 import sys
 from typing import Mapping
```

### Comparing `proxystore-0.6.3/proxystore/stream/shims/zmq.py` & `proxystore-0.6.4/proxystore/stream/shims/zmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Note:
     Unlike some of the other shims that simply interface with a third-party
     message broker system, here the subscriber connects directly to
     the publisher. This means that if the publisher is not alive when creating
     the subscriber, the subscriber will fail.
 """
+
 from __future__ import annotations
 
 import sys
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     from typing import Self
 else:  # pragma: <3.11 cover
```

### Comparing `proxystore-0.6.3/proxystore/utils/config.py` & `proxystore-0.6.4/proxystore/utils/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 """Read and write TOML config files using Pydantic BaseClasses."""
+
 from __future__ import annotations
 
 import sys
 from typing import BinaryIO
 from typing import TypeVar
 
 import tomli_w
 from pydantic import BaseModel
+from pydantic import VERSION
+
+if VERSION.startswith('2'):
+    pydantic_v2 = True
+else:  # pragma: no cover
+    pydantic_v2 = False
+
+    import warnings
+
+    warnings.warn(
+        'Pydantic V1 compatibility is deprecated and will be removed in '
+        'the future.',
+        DeprecationWarning,
+        stacklevel=2,
+    )
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     import tomllib
 else:  # pragma: <3.11 cover
     import tomli as tomllib
 
 
@@ -26,29 +42,35 @@
     """Serialize data class as a TOML formatted stream to file-like object.
 
     Args:
         model: Config model instance to write.
         fp: File-like bytes stream to write to.
         exclude_none: Skip writing none attributes.
     """
-    data_dict = model.model_dump(exclude_none=exclude_none)
+    if pydantic_v2:
+        data_dict = model.model_dump(exclude_none=exclude_none)
+    else:  # pragma: no cover
+        data_dict = model.dict(exclude_none=exclude_none)
     tomli_w.dump(data_dict, fp)
 
 
 def dumps(model: BaseModel, *, exclude_none: bool = True) -> str:
     """Serialize data class to a TOML formatted string.
 
     Args:
         model: Config model instance to write.
         exclude_none: Skip writing none attributes.
 
     Returns:
         TOML string of data class.
     """
-    data_dict = model.model_dump(exclude_none=exclude_none)
+    if pydantic_v2:
+        data_dict = model.model_dump(exclude_none=exclude_none)
+    else:  # pragma: no cover
+        data_dict = model.dict(exclude_none=exclude_none)
     return tomli_w.dumps(data_dict)
 
 
 def load(model: type[BaseModelT], fp: BinaryIO) -> BaseModelT:
     """Parse TOML from a binary file to a data class.
 
     Args:
@@ -68,8 +90,11 @@
         model: Config model type to parse TOML using.
         data: TOML string to parse.
 
     Returns:
         Model initialized from TOML file.
     """
     data = tomllib.loads(data)
-    return model.model_validate(data, strict=True)
+    if pydantic_v2:
+        return model.model_validate(data, strict=True)
+    else:  # pragma: no cover
+        return model.parse_obj(data)
```

### Comparing `proxystore-0.6.3/proxystore/utils/counter.py` & `proxystore-0.6.4/proxystore/utils/counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Atomic counting utilities."""
+
 from __future__ import annotations
 
 import threading
 
 
 class AtomicCounter:
     """Thread-safe counter.
```

### Comparing `proxystore-0.6.3/proxystore/utils/data.py` & `proxystore-0.6.4/proxystore/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for interacting with data."""
+
 from __future__ import annotations
 
 import decimal
 import re
 from typing import Generator
```

### Comparing `proxystore-0.6.3/proxystore/utils/environment.py` & `proxystore-0.6.4/proxystore/utils/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities related to the current execution environment."""
+
 from __future__ import annotations
 
 import os
 import socket
 
 
 def home_dir() -> str:
```

### Comparing `proxystore-0.6.3/proxystore/utils/imports.py` & `proxystore-0.6.4/proxystore/utils/imports.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 """Resolve imports by string paths."""
+
 from __future__ import annotations
 
 import importlib
 from typing import Any
 
 
-def get_class_path(cls: type[Any]) -> str:
-    """Get the fully qualified path of a type.
+def get_object_path(obj: Any) -> str:
+    """Get the fully qualified path of an object.
 
     Example:
         ```python
         >>> from proxystore.connectors.protocols import Connector
-        >>> get_class_path(Connector)
+        >>> get_object_path(Connector)
         'proxystore.connectors.protocols.Connector'
         ```
 
     Args:
-        cls: Class type to get fully qualified path of.
+        obj: Object to get fully qualified path of.
 
     Returns:
-        Fully qualified path of `cls`.
+        Fully qualified path of `obj`.
     """
-    return f'{cls.__module__}.{cls.__qualname__}'
+    return f'{obj.__module__}.{obj.__qualname__}'
 
 
-def import_class(path: str) -> type[Any]:
-    """Import class via its fully qualified path.
+def import_from_path(path: str) -> type[Any]:
+    """Import object via its fully qualified path.
 
     Example:
         ```python
-        >>> import_class('proxystore.connectors.protocols.Connector')
+        >>> import_from_path('proxystore.connectors.protocols.Connector')
         <class 'proxystore.connectors.protocols.Connector'>
         ```
 
     Args:
-        path: Fully qualified path of class to import.
+        path: Fully qualified path of object to import.
 
     Returns:
-        Imported class.
+        Imported object.
 
     Raises:
-        ImportError: If a class at the `path` is not found.
+        ImportError: If an object at the `path` is not found.
     """
     module_path, _, name = path.rpartition('.')
     if len(module_path) == 0:
         raise ImportError(
-            f'Class path must contain at least one module. Got {path}',
+            f'Object path must contain at least one module. Got {path}',
         )
     module = importlib.import_module(module_path)
     return getattr(module, name)
```

### Comparing `proxystore-0.6.3/proxystore/utils/tasks.py` & `proxystore-0.6.4/proxystore/utils/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Safely spawn asyncio background tasks with error handling."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import traceback
 from typing import Any
 from typing import Callable
```

### Comparing `proxystore-0.6.3/proxystore/utils/timer.py` & `proxystore-0.6.4/proxystore/utils/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Timing utilities."""
+
 from __future__ import annotations
 
 import sys
 import time
 from types import TracebackType
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
```

### Comparing `proxystore-0.6.3/proxystore.egg-info/PKG-INFO` & `proxystore-0.6.4/proxystore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.6.3
+Version: 0.6.4
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: FILE
 Project-URL: homepage, https://proxystore.dev
 Project-URL: documentation, https://docs.proxystore.dev
@@ -29,15 +29,15 @@
 Provides-Extra: all
 Requires-Dist: proxystore[endpoints,extensions,kafka,redis,zmq]; extra == "all"
 Provides-Extra: endpoints
 Requires-Dist: aiortc>=1.3.2; extra == "endpoints"
 Requires-Dist: aiosqlite; extra == "endpoints"
 Requires-Dist: uvicorn[standard]; extra == "endpoints"
 Requires-Dist: psutil; extra == "endpoints"
-Requires-Dist: pydantic>=2.0.0; extra == "endpoints"
+Requires-Dist: pydantic; extra == "endpoints"
 Requires-Dist: pystun3; extra == "endpoints"
 Requires-Dist: python-daemon; extra == "endpoints"
 Requires-Dist: quart>=0.18.0; extra == "endpoints"
 Requires-Dist: requests>=2.27.1; extra == "endpoints"
 Requires-Dist: tomli; python_version < "3.11" and extra == "endpoints"
 Requires-Dist: tomli-w; extra == "endpoints"
 Requires-Dist: websockets>=10.0; extra == "endpoints"
@@ -54,15 +54,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: ruff>=0.2.0; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: types-redis; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mkdocs-click; extra == "docs"
```

### Comparing `proxystore-0.6.3/proxystore.egg-info/SOURCES.txt` & `proxystore-0.6.4/proxystore.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 docs/contributing/style-guide.md
 docs/css/extra.css
 docs/css/mkdocstrings.css
 docs/guides/endpoints-debugging.md
 docs/guides/endpoints.md
 docs/guides/globus-compute.md
 docs/guides/index.md
+docs/guides/object-lifetimes.md
 docs/guides/performance.md
 docs/guides/proxy-futures.md
 docs/guides/relay-serving.md
 docs/guides/streaming.md
 docs/publications/index.md
 docs/static/endpoint-overview.svg
 docs/static/endpoint-peering.svg
@@ -127,15 +128,18 @@
 proxystore/p2p/relay/server.py
 proxystore/store/__init__.py
 proxystore/store/base.py
 proxystore/store/cache.py
 proxystore/store/exceptions.py
 proxystore/store/factory.py
 proxystore/store/future.py
+proxystore/store/lifetimes.py
 proxystore/store/metrics.py
+proxystore/store/ref.py
+proxystore/store/scopes.py
 proxystore/store/types.py
 proxystore/store/utils.py
 proxystore/stream/__init__.py
 proxystore/stream/events.py
 proxystore/stream/exceptions.py
 proxystore/stream/filters.py
 proxystore/stream/interface.py
@@ -219,15 +223,18 @@
 tests/p2p/relay/messages_test.py
 tests/p2p/relay/run_test.py
 tests/p2p/relay/server_test.py
 tests/store/__init__.py
 tests/store/cache_test.py
 tests/store/factory_test.py
 tests/store/init_test.py
+tests/store/lifetimes_test.py
 tests/store/metrics_test.py
+tests/store/ref_test.py
+tests/store/scopes_test.py
 tests/store/store_basics_test.py
 tests/store/store_metrics_test.py
 tests/store/store_proxy_test.py
 tests/store/utils_test.py
 tests/stream/__init__.py
 tests/stream/events_test.py
 tests/stream/filters_test.py
```

### Comparing `proxystore-0.6.3/proxystore.egg-info/requires.txt` & `proxystore-0.6.4/proxystore.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 coverage
 mypy
 pre-commit
 pytest
 pytest-asyncio>=0.23.2
 pytest-cov
 pytest-timeout
-ruff
+ruff>=0.2.0
 tox
 types-redis
 types-requests
 virtualenv
 
 [docs]
 black
@@ -36,15 +36,15 @@
 proxystore[all]
 
 [endpoints]
 aiortc>=1.3.2
 aiosqlite
 uvicorn[standard]
 psutil
-pydantic>=2.0.0
+pydantic
 pystun3
 python-daemon
 quart>=0.18.0
 requests>=2.27.1
 tomli-w
 websockets>=10.0
```

### Comparing `proxystore-0.6.3/pyproject.toml` & `proxystore-0.6.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxystore"
-version = "0.6.3"
+version = "0.6.4"
 authors = [
     {name = "Globus Labs"},
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
 ]
 maintainers = [
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
     {name = "Valerie Hayot-Sasson", email = "vhayot@uchicago.edu"},
@@ -45,15 +45,15 @@
 [project.optional-dependencies]
 all = ["proxystore[endpoints,extensions,kafka,redis,zmq]"]
 endpoints = [
     "aiortc>=1.3.2",
     "aiosqlite",
     "uvicorn[standard]",
     "psutil",
-    "pydantic>=2.0.0",
+    "pydantic",
     "pystun3",
     "python-daemon",
     "quart>=0.18.0",
     "requests>=2.27.1",
     "tomli ; python_version<'3.11'",
     "tomli-w",
     "websockets>=10.0",
@@ -69,15 +69,15 @@
     "coverage",
     "mypy",
     "pre-commit",
     "pytest",
     "pytest-asyncio>=0.23.2",
     "pytest-cov",
     "pytest-timeout",
-    "ruff",
+    "ruff>=0.2.0",
     "tox",
     "types-redis",
     "types-requests",
     "virtualenv",
 ]
 docs = [
     "black",
@@ -148,14 +148,22 @@
     "ignore::DeprecationWarning:tests.*",
 ]
 markers = [
     "integration: mark a test as an integration test.",
 ]
 
 [tool.ruff]
+line-length = 79
+target-version = "py38"
+
+[tool.ruff.format]
+indent-style = "space"
+quote-style = "single"
+
+[tool.ruff.lint]
 # See all rules here: https://beta.ruff.rs/docs/rules
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E",
     # mccabe
@@ -211,40 +219,34 @@
     # "COM812",
     # "ISC001",
     # Allow pytest.raises() without match
     "PT011",
     #
     "SIM105", "SIM117",
 ]
-line-length = 79
-target-version = "py38"
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
-[tool.ruff.format]
-indent-style = "space"
-quote-style = "single"
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 known-first-party = ["proxystore", "test", "testing"]
 order-by-type = false
 required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*/__init__.py" = ["F401"]
 "tests/**.py" = ["D10"]
 "proxystore/**.py" = ["PT"]
 "proxystore/store/*.py" = ["D102"]
 "tests/conftest.py" = ["F401"]
 "testing/**.py" = ["D10"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.setuptools.packages.find]
 exclude = ["tests*", "testing*"]
 namespaces = false
```

### Comparing `proxystore-0.6.3/testing/compat.py` & `proxystore-0.6.4/testing/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for supporting across python version."""
+
 from __future__ import annotations
 
 import os
 import random
 import sys
```

### Comparing `proxystore-0.6.3/testing/connectors.py` & `proxystore-0.6.4/testing/connectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Testing fixtures for connector implementations."""
+
 from __future__ import annotations
 
 import os
 import random
 from typing import Any
 from typing import Generator
 from unittest import mock
```

### Comparing `proxystore-0.6.3/testing/endpoint.py` & `proxystore-0.6.4/testing/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for launching endpoints in tests."""
+
 from __future__ import annotations
 
 import contextlib
 import logging
 import time
 import uuid
 from multiprocessing import Process
```

### Comparing `proxystore-0.6.3/testing/mocked/globus.py` & `proxystore-0.6.4/testing/mocked/globus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mock classes for the Globus SDK."""
+
 from __future__ import annotations
 
 import uuid
 from typing import Any
 
 import globus_sdk
```

### Comparing `proxystore-0.6.3/testing/mocked/kafka.py` & `proxystore-0.6.4/testing/mocked/kafka.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/testing/mocked/redis.py` & `proxystore-0.6.4/testing/mocked/redis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mocked classes for Redis."""
+
 from __future__ import annotations
 
 import queue
 from typing import Any
 from typing import TypedDict
 
 
@@ -26,14 +27,26 @@
         **kwargs,
     ):
         self.data = data
         self.pubsub_queue = (
             queue.Queue() if pubsub_queue is None else pubsub_queue
         )
 
+    def blpop(
+        self,
+        *keys: str,
+        timeout: int = 0,
+    ) -> tuple[str | bytes, ...] | None:
+        result: list[str | bytes] = []
+        for key in keys:
+            if key not in self.data or len(self.data[key]) == 0:
+                return None
+            result.extend([key, self.data[key].pop(0)])
+        return tuple(result)
+
     def close(self) -> None:
         """Close the client."""
         pass
 
     def delete(self, key: str) -> None:
         """Delete key."""
         if key in self.data:
@@ -72,14 +85,20 @@
         )
         self.pubsub_queue.put(message)
 
     def pubsub(self) -> MockPubSub:
         """Create a pubsub client."""
         return MockPubSub(self)
 
+    def rpush(self, key: str, *values: bytes) -> None:
+        """Push values onto list."""
+        if key not in self.data:
+            self.data[key] = []
+        self.data[key].extend(values)
+
     def set(self, key: str, value: bytes) -> None:
         """Set value in MockStrictRedis."""
         self.data[key] = value
 
 
 class MockPubSub:
     """Mock PubSub client."""
```

### Comparing `proxystore-0.6.3/testing/mocking.py` & `proxystore-0.6.4/testing/mocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mocking utilities."""
+
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
 from unittest.mock import AsyncMock
```

### Comparing `proxystore-0.6.3/testing/relay_server.py` & `proxystore-0.6.4/testing/relay_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools for running a local relay server for unit tests."""
+
 from __future__ import annotations
 
 from typing import AsyncGenerator
 from typing import NamedTuple
 
 import pytest
 import pytest_asyncio
```

### Comparing `proxystore-0.6.3/testing/scripts/kafka_pubsub.py` & `proxystore-0.6.4/testing/scripts/kafka_pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
    $ python testing/scripts/kafka_pubsub.py subscriber --broker localhost:9092
 
 3. Start the publisher.
 C
    $ python testing/scripts/kafka_pubsub.py publisher --broker localhost:9092
 """
+
 from __future__ import annotations
 
 import argparse
 import sys
 import time
 from typing import Sequence
```

### Comparing `proxystore-0.6.3/testing/scripts/peer_connection_bandwidth.py` & `proxystore-0.6.4/testing/scripts/peer_connection_bandwidth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Peer connection transfer speed test."""
+
 from __future__ import annotations
 
 import argparse
 import asyncio
 import logging
 import sys
 import time
```

### Comparing `proxystore-0.6.3/testing/scripts/peer_endpoint_bandwidth.py` & `proxystore-0.6.4/testing/scripts/peer_endpoint_bandwidth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Peer connection transfer speed test."""
+
 from __future__ import annotations
 
 import argparse
 import asyncio
 import logging
 import sys
 import time
```

### Comparing `proxystore-0.6.3/testing/scripts/peer_manager_bandwidth.py` & `proxystore-0.6.4/testing/scripts/peer_manager_bandwidth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Peer connection transfer speed test."""
+
 from __future__ import annotations
 
 import argparse
 import asyncio
 import logging
 import sys
 import time
```

### Comparing `proxystore-0.6.3/testing/scripts/redis_pubsub.py` & `proxystore-0.6.4/testing/scripts/redis_pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
    $ python testing/scripts/redis_pubsub.py subscriber
 
 3. Start the publisher.
 C
    $ python testing/scripts/redis_pubsub.py publisher
 """
+
 from __future__ import annotations
 
 import argparse
 import sys
 import time
 from typing import Sequence
```

### Comparing `proxystore-0.6.3/testing/ssl.py` & `proxystore-0.6.4/testing/ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     None of the functions in this module are safe and should only be used
     for creating temporary self-signed certificates for testing.
 
 Note:
     Based on the examples in the
     [Cryptography docs](https://cryptography.io/en/latest/x509/tutorial/#creating-a-self-signed-certificate).
 """
+
 from __future__ import annotations
 
 import datetime
 import pathlib
 import ssl
 from typing import NamedTuple
```

### Comparing `proxystore-0.6.3/testing/stores.py` & `proxystore-0.6.4/testing/stores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mocking utilities for Store tests."""
+
 from __future__ import annotations
 
 import uuid
 from typing import Generator
 
 import pytest
```

### Comparing `proxystore-0.6.3/testing/utils.py` & `proxystore-0.6.4/testing/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fixtures and utilities for testing."""
+
 from __future__ import annotations
 
 import socket
 
 _used_ports: set[int] = set()
```

### Comparing `proxystore-0.6.3/tests/conftest.py` & `proxystore-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/connectors/connector_test.py` & `proxystore-0.6.4/tests/connectors/connector_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/connectors/endpoint_test.py` & `proxystore-0.6.4/tests/connectors/endpoint_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
+import logging
+import pathlib
 import uuid
 from unittest import mock
 
 import pytest
 import requests
 
 from proxystore.connectors.endpoint import EndpointConnector
 from proxystore.connectors.endpoint import EndpointConnectorError
+from proxystore.endpoint.config import EndpointConfig
+from proxystore.endpoint.config import write_config
 from proxystore.endpoint.serve import MAX_CHUNK_LENGTH
 from testing.compat import randbytes
 
 
 def test_no_endpoints_provided() -> None:
     with pytest.raises(ValueError):
         EndpointConnector(endpoints=[])
@@ -30,14 +34,39 @@
     response.status_code = 400
 
     with mock.patch('requests.Session.get', return_value=response):
         with pytest.raises(EndpointConnectorError, match='Failed to find'):
             EndpointConnector.from_config(endpoint_connector.config())
 
 
+def test_endpoint_not_started(tmp_path: pathlib.Path, caplog) -> None:
+    endpoint_uuid = uuid.uuid4()
+    config = EndpointConfig(
+        name='test',
+        uuid=str(endpoint_uuid),
+        port=1,
+        host=None,
+    )
+    config_path = tmp_path / 'test'
+    write_config(config, str(config_path))
+
+    caplog.set_level(logging.INFO)
+    with pytest.raises(EndpointConnectorError, match='Failed to find'):
+        EndpointConnector(
+            endpoints=[endpoint_uuid],
+            proxystore_dir=str(tmp_path),
+        )
+
+    message = (
+        f'Found valid configuration for endpoint "test" ({endpoint_uuid}), '
+        'but the endpoint has not been started'
+    )
+    assert any([message == record.message for record in caplog.records])
+
+
 def test_endpoint_uuid_mismatch(endpoint_connector) -> None:
     response = requests.Response()
     response.status_code = 200
     response.json = lambda: {'uuid': str(uuid.uuid4())}  # type: ignore
 
     with mock.patch('requests.Session.get', return_value=response):
         with pytest.raises(EndpointConnectorError, match='Failed to find'):
```

### Comparing `proxystore-0.6.3/tests/connectors/file_test.py` & `proxystore-0.6.4/tests/connectors/file_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/connectors/globus_test.py` & `proxystore-0.6.4/tests/connectors/globus_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/connectors/multi_test.py` & `proxystore-0.6.4/tests/connectors/multi_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/connectors/redis_test.py` & `proxystore-0.6.4/tests/connectors/redis_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/cli_test.py` & `proxystore-0.6.4/tests/endpoint/cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/client_test.py` & `proxystore-0.6.4/tests/endpoint/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/commands_test.py` & `proxystore-0.6.4/tests/endpoint/commands_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/config_test.py` & `proxystore-0.6.4/tests/endpoint/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/endpoint_peering_test.py` & `proxystore-0.6.4/tests/endpoint/endpoint_peering_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/endpoint_solo_test.py` & `proxystore-0.6.4/tests/endpoint/endpoint_solo_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/serve_test.py` & `proxystore-0.6.4/tests/endpoint/serve_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/endpoint/storage_test.py` & `proxystore-0.6.4/tests/endpoint/storage_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/factory_test.py` & `proxystore-0.6.4/tests/factory_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/globus/cli_test.py` & `proxystore-0.6.4/tests/globus/cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/globus/client_test.py` & `proxystore-0.6.4/tests/globus/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/globus/manager_test.py` & `proxystore-0.6.4/tests/globus/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/globus/scopes_test.py` & `proxystore-0.6.4/tests/globus/scopes_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/globus/storage_test.py` & `proxystore-0.6.4/tests/globus/storage_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/globus/transfer_test.py` & `proxystore-0.6.4/tests/globus/transfer_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/integration/endpoints_test.py` & `proxystore-0.6.4/tests/integration/endpoints_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/chunks_test.py` & `proxystore-0.6.4/tests/p2p/chunks_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/connection_test.py` & `proxystore-0.6.4/tests/p2p/connection_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/manager_test.py` & `proxystore-0.6.4/tests/p2p/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/nat_test.py` & `proxystore-0.6.4/tests/p2p/nat_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/authenticate_test.py` & `proxystore-0.6.4/tests/p2p/relay/authenticate_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/client_test.py` & `proxystore-0.6.4/tests/p2p/relay/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/config_test.py` & `proxystore-0.6.4/tests/p2p/relay/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/manager_test.py` & `proxystore-0.6.4/tests/p2p/relay/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/messages_test.py` & `proxystore-0.6.4/tests/p2p/relay/messages_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/run_test.py` & `proxystore-0.6.4/tests/p2p/relay/run_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/p2p/relay/server_test.py` & `proxystore-0.6.4/tests/p2p/relay/server_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/proxy_test.py` & `proxystore-0.6.4/tests/proxy_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/serialization_test.py` & `proxystore-0.6.4/tests/serialization_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from unittest import mock
+
 import pytest
 
 from proxystore.serialize import deserialize
 from proxystore.serialize import SerializationError
 from proxystore.serialize import serialize
 
 
@@ -31,7 +33,36 @@
     with pytest.raises(SerializationError):
         # No identifier
         deserialize(b'xxx')
 
     with pytest.raises(SerializationError):
         # Fake identifier 'xxx'
         deserialize(b'99\nxxx')
+
+
+def test_cloudpickle_dumps_error() -> None:
+    with mock.patch('cloudpickle.dumps', side_effect=Exception()):
+        with pytest.raises(
+            SerializationError,
+            match="Object of type <class 'function'> is not serializable.",
+        ):
+            serialize(lambda x: x + x)  # pragma: no cover
+
+
+def test_pickle_loads_error() -> None:
+    v = serialize([1, 2, 3])
+    with mock.patch('pickle.loads', side_effect=Exception()):
+        with pytest.raises(
+            SerializationError,
+            match='Failed to deserialize object with pickle.',
+        ):
+            deserialize(v)
+
+
+def test_cloudpickle_loads_error() -> None:
+    v = serialize(lambda x: x + x)  # pragma: no cover
+    with mock.patch('cloudpickle.loads', side_effect=Exception()):
+        with pytest.raises(
+            SerializationError,
+            match='Failed to deserialize object with cloudpickle.',
+        ):
+            deserialize(v)
```

### Comparing `proxystore-0.6.3/tests/store/cache_test.py` & `proxystore-0.6.4/tests/store/cache_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/store/factory_test.py` & `proxystore-0.6.4/tests/store/factory_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import time
+
 import pytest
 
 from proxystore.connectors.local import LocalConnector
 from proxystore.serialize import deserialize
 from proxystore.serialize import serialize
 from proxystore.store import Store
 from proxystore.store import store_registration
@@ -72,14 +74,38 @@
                 polling_interval=0.001,
                 polling_timeout=0.002,
             )
             with pytest.raises(ProxyResolveMissingKeyError):
                 factory.resolve()
 
 
+def test_polling_store_factory_backoff() -> None:
+    with Store('polling-store-factory-backoff', LocalConnector()) as store:
+        with store_registration(store):
+            key = store.connector.new_key()
+            factory: FactoryT = PollingStoreFactory(
+                key=key,
+                store_config=store.config(),
+                evict=True,
+                polling_interval=0.001,
+                polling_backoff_factor=2,
+                polling_interval_limit=0.004,
+                polling_timeout=0.011,
+            )
+            start = time.perf_counter()
+            with pytest.raises(ProxyResolveMissingKeyError):
+                factory.resolve()
+            end = time.perf_counter()
+
+            # polling_timeout is 0.011 so we should sleep for 0.001, 0.002,
+            # 0.004, and 0.004 seconds then timeout
+            min_sleep = 0.011
+            assert (end - start) > min_sleep
+
+
 def test_polling_store_factory_serialize() -> None:
     with Store('polling-store-factory-serialize', LocalConnector()) as store:
         with store_registration(store):
             value = 'test-value'
             key = store.put(value)
             factory: FactoryT = PollingStoreFactory(
                 key=key,
```

### Comparing `proxystore-0.6.3/tests/store/init_test.py` & `proxystore-0.6.4/tests/store/init_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/store/metrics_test.py` & `proxystore-0.6.4/tests/store/metrics_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/store/store_basics_test.py` & `proxystore-0.6.4/tests/store/store_basics_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from typing import Any
 from unittest import mock
 
 import pytest
 
 from proxystore.connectors.local import LocalConnector
 from proxystore.proxy import Proxy
+from proxystore.serialize import SerializationError
 from proxystore.store import Store
-from proxystore.store.future import ProxyFuture
+from proxystore.store.future import Future
+from proxystore.store.lifetimes import ContextLifetime
 
 
 def test_negative_cache_size() -> None:
     with pytest.raises(ValueError):
         Store('test', LocalConnector(), cache_size=-1)
 
 
@@ -96,14 +98,27 @@
         store.put([1, 2, 3], serializer=lambda s: s)
 
     with pytest.raises(TypeError, match='bytes'):
         # Should fail because the array is not already serialized
         store.put_batch([[1, 2, 3]], serializer=lambda s: s)
 
 
+def test_custom_deserializer_error(store: Store[LocalConnector]) -> None:
+    key = store.put('value')
+
+    def _deserialize(x: bytes) -> Any:
+        raise Exception()
+
+    with pytest.raises(
+        SerializationError,
+        match='Failed to deserialize object',
+    ):
+        store.get(key, deserializer=_deserialize)
+
+
 def test_put_batch(store: Store[LocalConnector]) -> None:
     values = ['test_value1', 'test_value2', 'test_value3']
 
     # Test without keys
     keys = store.put_batch(values)
     for key in keys:
         assert store.exists(key)
@@ -113,19 +128,23 @@
     values = ['test_value1', 'test_value2', 'test_value3']
 
     new_keys = store.put_batch(values, serializer=lambda s: str.encode(s))
     for key in new_keys:
         assert store.exists(key)
 
 
-def test_set(store: Store[LocalConnector]) -> None:
-    key = store.connector.new_key()
-    assert not store.exists(key)
-    store._set(key, 'test_value')
-    assert store.get(key) == 'test_value'
+def test_set() -> None:
+    with Store('test-set', LocalConnector(), cache_size=1) as store:
+        key = store.connector.new_key()
+        assert not store.exists(key)
+        store._set(key, 'test_value')
+        assert store.get(key) == 'test_value'
+        assert store.is_cached(key)
+        store._set(key, 'new_value')
+        assert not store.is_cached(key)
 
 
 def test_set_bad_connector_type(store: Store[LocalConnector]) -> None:
     key = store.connector.new_key()
     with mock.patch.object(store, 'connector', object()):
         with pytest.raises(NotImplementedError, match='DeferrableConnector'):
             store._set(key, 'new-value')
@@ -137,26 +156,28 @@
     assert store.get(key, deserializer=lambda s: s) == b'test_value'
 
     with pytest.raises(TypeError, match='bytes'):
         store._set(key, 'test_value', serializer=lambda s: s)
 
 
 def test_future(store: Store[LocalConnector]) -> None:
-    future: ProxyFuture[str] = store.future()
+    future: Future[str] = store.future()
     proxy = future.proxy()
+    assert not future.done()
     future.set_result('test_value')
+    assert future.done()
     assert future.result() == 'test_value'
     assert proxy == 'test_value'
 
 
 def test_future_in_threads(store: Store[LocalConnector]) -> None:
-    future: ProxyFuture[str] = store.future()
+    future: Future[str] = store.future()
 
     def _foo(
-        future: ProxyFuture[str],
+        future: Future[str],
         barrier: threading.Barrier,
     ) -> None:
         future.set_result('test_value')
         barrier.wait()
 
     def _bar(value: Proxy[str], barrier: threading.Barrier) -> None:
         barrier.wait()
@@ -173,7 +194,24 @@
     t_bar.join()
 
 
 def test_future_bad_connector_type(store: Store[LocalConnector]) -> None:
     with mock.patch.object(store, 'connector', object()):
         with pytest.raises(NotImplementedError, match='DeferrableConnector'):
             store.future()
+
+
+def test_put_lifetime(store: Store[LocalConnector]) -> None:
+    with ContextLifetime(store) as lifetime:
+        key = store.put('test_value', lifetime=lifetime)
+
+    assert not store.exists(key)
+
+
+def test_put_batch_lifetime(store: Store[LocalConnector]) -> None:
+    values = ['test_value1', 'test_value2', 'test_value3']
+
+    with ContextLifetime(store) as lifetime:
+        keys = store.put_batch(values, lifetime=lifetime)
+
+    for key in keys:
+        assert not store.exists(key)
```

### Comparing `proxystore-0.6.3/tests/store/store_metrics_test.py` & `proxystore-0.6.4/tests/store/store_metrics_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import pathlib
+from typing import Any
 from typing import Generator
 
 import pytest
 
 from proxystore.connectors.file import FileConnector
 from proxystore.serialize import serialize
 from proxystore.store import store_registration
 from proxystore.store.base import Store
+from proxystore.store.future import Future
 
 
 @pytest.fixture()
 def store(
     tmp_path: pathlib.Path,
 ) -> Generator[Store[FileConnector], None, None]:
     # We use FileConnector here instead of LocalConnector (as in the rest of
@@ -69,14 +71,20 @@
     proxy_metrics = store.metrics.get_metrics(proxy)
     assert proxy_metrics is not None
 
     assert proxy_metrics.times['store.proxy'].count == 1
     assert proxy_metrics.times['factory.call'].count == 1
     assert proxy_metrics.times['factory.resolve'].count == 1
 
+    future: Future[Any] = store.future()
+    future_metrics = store.metrics.get_metrics(future._factory.key)
+    assert future_metrics is not None
+    assert future_metrics.times['store.future'].count == 1
+    assert future_metrics.times['store.future.connector'].count == 1
+
 
 def test_store_multi_key_operations(store: Store[FileConnector]) -> None:
     values = ['value1', 'value2', 'value3']
     keys = store.put_batch(values)
     assert all(store.exists(key) for key in keys)
 
     assert store.metrics is not None
```

### Comparing `proxystore-0.6.3/tests/store/utils_test.py` & `proxystore-0.6.4/tests/store/utils_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/stream/events_test.py` & `proxystore-0.6.4/tests/stream/events_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/stream/filters_test.py` & `proxystore-0.6.4/tests/stream/filters_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/stream/interface_test.py` & `proxystore-0.6.4/tests/stream/interface_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,21 +147,25 @@
     publisher, subscriber = create_pubsub_pair(topic)
 
     store = Store(
         'test-use-and-register-default-store',
         FileConnector(str(tmp_path)),
     )
 
-    with StreamProducer[str](publisher, {None: store}) as producer:
-        with StreamConsumer[str](subscriber) as consumer:
-            producer.send(topic, 'value')
-
-            assert get_store(store.name) is None
-            consumer.next()
-            assert get_store(store.name) is not None
+    producer = StreamProducer[str](publisher, {None: store})
+    consumer = StreamConsumer[str](subscriber)
+
+    producer.send(topic, 'value')
+
+    assert get_store(store.name) is None
+    consumer.next()
+    assert get_store(store.name) is not None
+
+    producer.close(stores=True)
+    consumer.close(stores=True)
 
     # Should get unregistered when closed
     assert get_store(store.name) is None
 
 
 def test_missing_store_mapping_error(store: Store[FileConnector]) -> None:
     topic = 'default'
@@ -241,14 +245,52 @@
     assert len(values) == math.ceil(count / batch_size)
     assert sum(values) == count
 
     producer.close()
     consumer.close()
 
 
+def test_iter_with_metadata(store: Store[FileConnector]) -> None:
+    topic = 'default'
+    publisher, subscriber = create_pubsub_pair(topic)
+
+    producer = StreamProducer[int](publisher, {topic: store})
+    consumer = StreamConsumer[int](subscriber)
+
+    count = 10
+    for i in range(count):
+        producer.send(topic, i, metadata={'value': i})
+    producer.close_topics(topic)
+
+    for metadata, proxy in consumer.iter_with_metadata():
+        assert metadata['value'] == proxy
+
+    producer.close()
+    consumer.close()
+
+
+def test_iter_objects_with_metadata(store: Store[FileConnector]) -> None:
+    topic = 'default'
+    publisher, subscriber = create_pubsub_pair(topic)
+
+    producer = StreamProducer[int](publisher, {topic: store})
+    consumer = StreamConsumer[int](subscriber)
+
+    count = 10
+    for i in range(count):
+        producer.send(topic, i, metadata={'value': i})
+    producer.close_topics(topic)
+
+    for metadata, obj in consumer.iter_objects_with_metadata():
+        assert metadata['value'] == obj
+
+    producer.close()
+    consumer.close()
+
+
 @pytest.mark.parametrize('evict', (True, False))
 def test_consumer_next_object_evicts(
     evict: bool,
     store: Store[FileConnector],
 ) -> None:
     topic = 'default'
     publisher, subscriber = create_pubsub_pair(topic)
```

### Comparing `proxystore-0.6.3/tests/stream/shims/kafka_test.py` & `proxystore-0.6.4/tests/stream/shims/kafka_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/stream/shims/queue_test.py` & `proxystore-0.6.4/tests/stream/shims/queue_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/stream/shims/redis_test.py` & `proxystore-0.6.4/tests/stream/shims/zmq_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 from __future__ import annotations
 
-import queue
-from typing import Any
-from typing import Generator
 from unittest import mock
 
-import pytest
-
-from proxystore.stream.shims.redis import RedisPublisher
-from proxystore.stream.shims.redis import RedisSubscriber
-from testing.mocked.redis import Message
-from testing.mocked.redis import MockStrictRedis
-
-
-@pytest.fixture(autouse=True)
-def _mock_redis() -> Generator[None, None, None]:
-    redis_store: dict[str, bytes] = {}
-    redis_queue: queue.Queue[Message] = queue.Queue()
-
-    def create_mocked_redis(*args: Any, **kwargs: Any) -> MockStrictRedis:
-        return MockStrictRedis(redis_store, redis_queue, *args, **kwargs)
-
-    with mock.patch('redis.StrictRedis', side_effect=create_mocked_redis):
-        yield
+from proxystore.stream.shims.zmq import ZeroMQPublisher
+from proxystore.stream.shims.zmq import ZeroMQSubscriber
+from testing.utils import open_port
 
 
 def test_basic_publish_subscribe() -> None:
-    publisher = RedisPublisher('localhost', 0)
-    subscriber = RedisSubscriber('localhost', 0, 'default')
+    address, port = '127.0.0.1', open_port()
+
+    publisher = ZeroMQPublisher(address, port)
+    subscriber = ZeroMQSubscriber(address, port)
 
     messages = [f'message_{i}'.encode() for i in range(3)]
 
-    for message in messages:
-        publisher.send('default', message)
+    with mock.patch.object(publisher._socket, 'send_multipart'):
+        for message in messages:
+            publisher.send('default', message)
 
-    publisher.close()
+        publisher.close()
 
     received = []
-    for _, message in zip(messages, subscriber):
-        received.append(message)
+
+    with mock.patch.object(
+        subscriber._socket,
+        'recv_multipart',
+        side_effect=[(b'default', message) for message in messages],
+    ):
+        for _, message in zip(messages, subscriber):
+            received.append(message)
 
     subscriber.close()
 
     assert messages == received
```

### Comparing `proxystore-0.6.3/tests/utils/config_test.py` & `proxystore-0.6.4/tests/utils/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/utils/counter_test.py` & `proxystore-0.6.4/tests/utils/counter_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/utils/data_test.py` & `proxystore-0.6.4/tests/utils/data_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/utils/environment_test.py` & `proxystore-0.6.4/tests/utils/environment_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/utils/tasks_test.py` & `proxystore-0.6.4/tests/utils/tasks_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tests/utils/timer_test.py` & `proxystore-0.6.4/tests/utils/timer_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.3/tox.ini` & `proxystore-0.6.4/tox.ini`

 * *Files identical despite different names*

