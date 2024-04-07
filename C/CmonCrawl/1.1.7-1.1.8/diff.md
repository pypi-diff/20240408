# Comparing `tmp/CmonCrawl-1.1.7.tar.gz` & `tmp/CmonCrawl-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CmonCrawl-1.1.7.tar", last modified: Wed Feb 14 00:16:34 2024, max compression
+gzip compressed data, was "CmonCrawl-1.1.8.tar", last modified: Sun Apr  7 23:57:56 2024, max compression
```

## Comparing `CmonCrawl-1.1.7.tar` & `CmonCrawl-1.1.8.tar`

### file list

```diff
@@ -1,175 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.622062 CmonCrawl-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.590062 CmonCrawl-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.598062 CmonCrawl-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.github/workflows/sphinx_build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.github/workflows/test_and_types.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.598062 CmonCrawl-1.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/.vscode/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.622062 CmonCrawl-1.1.7/CmonCrawl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-02-14 00:16:34.000000 CmonCrawl-1.1.7/CmonCrawl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-02-14 00:16:34.000000 CmonCrawl-1.1.7/CmonCrawl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 00:16:34.000000 CmonCrawl-1.1.7/CmonCrawl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-14 00:16:34.000000 CmonCrawl-1.1.7/CmonCrawl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-14 00:16:34.000000 CmonCrawl-1.1.7/CmonCrawl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 00:16:34.000000 CmonCrawl-1.1.7/CmonCrawl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-02-14 00:16:34.622062 CmonCrawl-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   164308 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/banner.webp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.598062 CmonCrawl-1.1.7/cmoncrawl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/aggregator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/aggregator/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20970 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/athena_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/gateway_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/athena_query_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/ndjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/common/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/common/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/integrations/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/integrations/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/integrations/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/integrations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/middleware/stompware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/middleware/synchronized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.602062 CmonCrawl-1.1.7/cmoncrawl/processor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/cmoncrawl/processor/dao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/dao/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/dao/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/dao/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/cmoncrawl/processor/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/extraction/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/docs/source/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/cli/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/cli/download.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/cli/extract.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.606062 CmonCrawl-1.1.7/docs/source/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/extraction/config_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/extraction/creating_extractor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/extraction/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/extraction/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.614062 CmonCrawl-1.1.7/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.athena_query.rst
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.gateway_query.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.utils.athena_query_maker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.utils.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.utils.ndjson.rst
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.aggregator.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.common.loggers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.common.throttling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.common.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.integrations.commands.rst
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.integrations.download.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.integrations.extract.rst
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.integrations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.integrations.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.middleware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.middleware.stompware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.middleware.synchronized.rst
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.dao.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.dao.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.dao.rst
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.dao.s3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.extraction.filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.extraction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.extraction.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.downloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.extractor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.router.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.streamer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.614062 CmonCrawl-1.1.7/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/images/domain_record.drawio.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    49717 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/images/when_to_use.drawio.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.614062 CmonCrawl-1.1.7/docs/source/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/misc/athena.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/misc/domain_record.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/misc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.614062 CmonCrawl-1.1.7/docs/source/prog_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/prog_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/prog_guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/prog_guide/practice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.594062 CmonCrawl-1.1.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.614062 CmonCrawl-1.1.7/examples/code-usage/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/examples/code-usage/offline-warc-iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.614062 CmonCrawl-1.1.7/examples/extractor_tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/examples/extractor_tutorial/Extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/examples/extractor_tutorial/Extractors/bbc_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/examples/extractor_tutorial/Extractors/idnes_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/examples/extractor_tutorial/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/extractors/my_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 00:16:34.622062 CmonCrawl-1.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/end_to_end_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/tests/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/files/mini.warc.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/gateway_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/processor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/tests/test_extract/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/test_extract/cfg.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/tests/test_extract/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/test_extract/extractors/test_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.618062 CmonCrawl-1.1.7/tests/test_extract/files/
--rw-r--r--   0 runner    (1001) docker     (127)   828135 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/test_extract/files/file.html
--rw-r--r--   0 runner    (1001) docker     (127)  1743032 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/test_extract/files/file.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:16:34.622062 CmonCrawl-1.1.7/tests/test_routes/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/test_routes/a.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/test_routes/b.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-02-14 00:16:16.000000 CmonCrawl-1.1.7/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.432906 CmonCrawl-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.396906 CmonCrawl-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.404906 CmonCrawl-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.github/workflows/sphinx_build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.github/workflows/test_and_types.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.404906 CmonCrawl-1.1.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/.vscode/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.432906 CmonCrawl-1.1.8/CmonCrawl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-04-07 23:57:56.000000 CmonCrawl-1.1.8/CmonCrawl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-07 23:57:56.000000 CmonCrawl-1.1.8/CmonCrawl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:57:56.000000 CmonCrawl-1.1.8/CmonCrawl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-07 23:57:56.000000 CmonCrawl-1.1.8/CmonCrawl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-07 23:57:56.000000 CmonCrawl-1.1.8/CmonCrawl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 23:57:56.000000 CmonCrawl-1.1.8/CmonCrawl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-04-07 23:57:56.432906 CmonCrawl-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   164308 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/banner.webp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.408906 CmonCrawl-1.1.8/cmoncrawl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.408906 CmonCrawl-1.1.8/cmoncrawl/aggregator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.408906 CmonCrawl-1.1.8/cmoncrawl/aggregator/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20970 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/gateway_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.408906 CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/athena_query_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/ndjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.408906 CmonCrawl-1.1.8/cmoncrawl/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/common/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/common/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/common/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.412906 CmonCrawl-1.1.8/cmoncrawl/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/integrations/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/integrations/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/integrations/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/integrations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.412906 CmonCrawl-1.1.8/cmoncrawl/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/middleware/stompware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/middleware/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.412906 CmonCrawl-1.1.8/cmoncrawl/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.412906 CmonCrawl-1.1.8/cmoncrawl/processor/dao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/dao/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/dao/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/dao/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.412906 CmonCrawl-1.1.8/cmoncrawl/processor/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/extraction/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.412906 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.416906 CmonCrawl-1.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.416906 CmonCrawl-1.1.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.416906 CmonCrawl-1.1.8/docs/source/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/cli/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/cli/download.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/cli/extract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.416906 CmonCrawl-1.1.8/docs/source/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/extraction/config_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/extraction/creating_extractor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/extraction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/extraction/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.athena_query.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.gateway_query.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.utils.athena_query_maker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.utils.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.utils.ndjson.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.aggregator.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.common.loggers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.common.throttling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.common.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.integrations.commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.integrations.download.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.integrations.extract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.integrations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.integrations.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.middleware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.middleware.stompware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.middleware.synchronized.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.dao.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.dao.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.dao.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.dao.s3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.extraction.filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.extraction.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.downloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.extractor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.router.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.streamer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/images/domain_record.drawio.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    49717 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/images/when_to_use.drawio.png
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/docs/source/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/misc/athena.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/misc/domain_record.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/misc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/docs/source/prog_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/prog_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/prog_guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/prog_guide/practice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.400905 CmonCrawl-1.1.8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/examples/code-usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/examples/code-usage/offline-warc-iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/examples/extractor_tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/examples/extractor_tutorial/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/examples/extractor_tutorial/Extractors/bbc_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/examples/extractor_tutorial/Extractors/idnes_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/examples/extractor_tutorial/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.424906 CmonCrawl-1.1.8/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/extractors/my_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:57:56.432906 CmonCrawl-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.428906 CmonCrawl-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/end_to_end_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.428906 CmonCrawl-1.1.8/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/files/mini.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/gateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/processor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.428906 CmonCrawl-1.1.8/tests/test_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_extract/cfg.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_extract/cfg_invalid.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.428906 CmonCrawl-1.1.8/tests/test_extract/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_extract/extractors/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.428906 CmonCrawl-1.1.8/tests/test_extract/files/
+-rw-r--r--   0 runner    (1001) docker     (127)   828135 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_extract/files/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1743032 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_extract/files/file.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:57:56.432906 CmonCrawl-1.1.8/tests/test_routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_routes/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/test_routes/b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-07 23:57:45.000000 CmonCrawl-1.1.8/tests/utils.py
```

### Comparing `CmonCrawl-1.1.7/.github/workflows/release.yml` & `CmonCrawl-1.1.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/.github/workflows/sphinx_build.yml` & `CmonCrawl-1.1.8/.github/workflows/sphinx_build.yml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/.github/workflows/test_and_types.yml` & `CmonCrawl-1.1.8/.github/workflows/test_and_types.yml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/.gitignore` & `CmonCrawl-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/.pre-commit-config.yaml` & `CmonCrawl-1.1.8/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: mixed-line-ending
 
 - repo: https://github.com/myint/autoflake
-  rev: v1.4
+  rev: v2.3.1
   hooks:
     - id: autoflake
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
   rev: v0.1.5
   hooks:
```

### Comparing `CmonCrawl-1.1.7/.vscode/launch.json` & `CmonCrawl-1.1.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/.vscode/settings.json` & `CmonCrawl-1.1.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/CmonCrawl.egg-info/PKG-INFO` & `CmonCrawl-1.1.8/CmonCrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 1.1.7
+Version: 1.1.8
 License: MIT License
         
         Copyright (c) [2023] [Hynek Kydlíček]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,22 +28,22 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles~=23.2.1
-Requires-Dist: aiohttp~=3.8.5
-Requires-Dist: beautifulsoup4~=4.11.1
-Requires-Dist: pydantic~=2.3.0
-Requires-Dist: stomp.py~=8.0.1
+Requires-Dist: aiohttp~=3.9.3
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: pydantic~=2.6.4
+Requires-Dist: stomp.py~=8.1.0
 Requires-Dist: tqdm~=4.66.1
 Requires-Dist: warcio~=1.7.4
-Requires-Dist: aiocsv~=1.2.4
-Requires-Dist: aioboto3~=11.3.0
+Requires-Dist: aiocsv~=1.3.1
+Requires-Dist: aioboto3~=12.3.0
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: python-dotenv==1.0.0
 
 ![CmonCrawl Banner](./banner.webp)
 
 
 ## CommonCrawl Extractor with great versatility
@@ -145,14 +145,16 @@
                 "to": "2025-01-01"
             }]
         },
         # More routes here
     ]
 }
 ```
+Please note that the configuration file `config.json` must be a valid JSON. Therefore, comments as shown in the example above cannot be included directly in the JSON file.
+
 
 ### Step: 4 Run the extractor
 Test your extractor with the following command:
 
 ```bash
 $ cmon extract config.json extracted_output html_output/*.html html
 ```
```

### Comparing `CmonCrawl-1.1.7/CmonCrawl.egg-info/SOURCES.txt` & `CmonCrawl-1.1.8/CmonCrawl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 cmoncrawl/aggregator/.vscode/settings.json
 cmoncrawl/aggregator/utils/__init__.py
 cmoncrawl/aggregator/utils/athena_query_maker.py
 cmoncrawl/aggregator/utils/constants.py
 cmoncrawl/aggregator/utils/helpers.py
 cmoncrawl/aggregator/utils/ndjson.py
 cmoncrawl/common/__init__.py
+cmoncrawl/common/caching.py
 cmoncrawl/common/loggers.py
 cmoncrawl/common/throttling.py
 cmoncrawl/common/types.py
 cmoncrawl/integrations/__init__.py
 cmoncrawl/integrations/commands.py
 cmoncrawl/integrations/download.py
 cmoncrawl/integrations/extract.py
@@ -127,12 +128,13 @@
 tests/end_to_end_test.py
 tests/gateway_test.py
 tests/helpers_test.py
 tests/processor_test.py
 tests/utils.py
 tests/files/mini.warc.gz
 tests/test_extract/cfg.json
+tests/test_extract/cfg_invalid.json
 tests/test_extract/extractors/test_extract.py
 tests/test_extract/files/file.html
 tests/test_extract/files/file.jsonl
 tests/test_routes/a.py
 tests/test_routes/b.py
```

### Comparing `CmonCrawl-1.1.7/LICENSE` & `CmonCrawl-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/PKG-INFO` & `CmonCrawl-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 1.1.7
+Version: 1.1.8
 License: MIT License
         
         Copyright (c) [2023] [Hynek Kydlíček]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,22 +28,22 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles~=23.2.1
-Requires-Dist: aiohttp~=3.8.5
-Requires-Dist: beautifulsoup4~=4.11.1
-Requires-Dist: pydantic~=2.3.0
-Requires-Dist: stomp.py~=8.0.1
+Requires-Dist: aiohttp~=3.9.3
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: pydantic~=2.6.4
+Requires-Dist: stomp.py~=8.1.0
 Requires-Dist: tqdm~=4.66.1
 Requires-Dist: warcio~=1.7.4
-Requires-Dist: aiocsv~=1.2.4
-Requires-Dist: aioboto3~=11.3.0
+Requires-Dist: aiocsv~=1.3.1
+Requires-Dist: aioboto3~=12.3.0
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: python-dotenv==1.0.0
 
 ![CmonCrawl Banner](./banner.webp)
 
 
 ## CommonCrawl Extractor with great versatility
@@ -145,14 +145,16 @@
                 "to": "2025-01-01"
             }]
         },
         # More routes here
     ]
 }
 ```
+Please note that the configuration file `config.json` must be a valid JSON. Therefore, comments as shown in the example above cannot be included directly in the JSON file.
+
 
 ### Step: 4 Run the extractor
 Test your extractor with the following command:
 
 ```bash
 $ cmon extract config.json extracted_output html_output/*.html html
 ```
```

### Comparing `CmonCrawl-1.1.7/README.md` & `CmonCrawl-1.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,16 @@
                 "to": "2025-01-01"
             }]
         },
         # More routes here
     ]
 }
 ```
+Please note that the configuration file `config.json` must be a valid JSON. Therefore, comments as shown in the example above cannot be included directly in the JSON file.
+
 
 ### Step: 4 Run the extractor
 Test your extractor with the following command:
 
 ```bash
 $ cmon extract config.json extracted_output html_output/*.html html
 ```
```

### Comparing `CmonCrawl-1.1.7/banner.webp` & `CmonCrawl-1.1.8/banner.webp`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/aggregator/athena_query.py` & `CmonCrawl-1.1.8/cmoncrawl/aggregator/athena_query.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/aggregator/gateway_query.py` & `CmonCrawl-1.1.8/cmoncrawl/aggregator/gateway_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,14 +112,15 @@
             match_type=self.match_type,
             since=self.since,
             to=self.to,
             limit=self.limit,
             max_retry=self.max_retry,
             prefetch_size=self.prefetch_size,
             sleep_base=self.sleep_base,
+            throttler=self.throttler,
         )
         self.iterators.append(iterator)
         return iterator
 
     async def aclose(
         self,
         exc_type: Type[BaseException] | None,
@@ -142,14 +143,15 @@
     async def get_number_of_pages(
         client: ClientSession,
         cdx_server: str,
         domain: str,
         match_type: MatchType | None,
         max_retry: int,
         sleep_base: float,
+        throttler: Throttler,
         page_size: int | None = None,
     ) -> int:
         params: Dict[str, str | int] = {
             "showNumPages": "true",
             "output": "json",
             "url": domain,
         }
@@ -162,14 +164,15 @@
         response = await retrieve(
             client,
             cdx_server,
             params,
             "text/x-ndjson",
             max_retry=max_retry,
             sleep_base=sleep_base,
+            throttler=throttler,
             log_additional_info={
                 "type": "num_pages",
                 "domain": domain,
                 "cdx_server": cdx_server,
             },
         )
         pages = response[0].get("pages", 0)
@@ -181,14 +184,15 @@
         client: ClientSession,
         cdx_server: str,
         domain: str,
         match_type: MatchType | None,
         max_retry: int,
         sleep_base: float,
         page: int,
+        throttler: Throttler,
         since: datetime = datetime.min,
         to: datetime = datetime.max,
     ) -> List[DomainRecord]:
         params: Dict[str, str | int] = {
             "output": "json",
             "page": page,
             "url": domain,
@@ -201,14 +205,15 @@
             reponse = await retrieve(
                 client,
                 cdx_server,
                 params,
                 "text/x-ndjson",
                 max_retry=max_retry,
                 sleep_base=sleep_base,
+                throttler=throttler,
                 log_additional_info={
                     "type": "page",
                     "domain": domain,
                     "page": page,
                     "cdx_server": cdx_server,
                 },
             )
@@ -244,26 +249,28 @@
             match_type: MatchType | None,
             since: datetime,
             to: datetime,
             limit: int | None,
             max_retry: int,
             prefetch_size: int,
             sleep_base: float,
+            throttler: Throttler,
         ):
             self.__client = client
             self.__opt_prefetch_size = prefetch_size
             self.__domain_records: Deque[DomainRecord] = deque()
             self.prefetch_queue: Set[asyncio.Task[List[DomainRecord]]] = set()
             self.__since = since
             self.__to = to
             self.__limit = limit
             self.__max_retry = max_retry
             self.__total = 0
             self.__sleep_base = sleep_base
             self.__match_type = match_type
+            self.__throttler = throttler
 
             self.__crawls_remaining = self.init_crawls_queue(urls, CC_files)
 
         def init_crawls_queue(
             self, urls: List[str], CC_files: List[str]
         ) -> Deque[DomainCrawl]:
             # TODO Be smarter about this, The last -XX determines the week in the year
@@ -290,14 +297,15 @@
                     num_pages = await GatewayAggregator.get_number_of_pages(
                         self.__client,
                         next_crawl.cdx_server,
                         next_crawl.url,
                         match_type=self.__match_type,
                         max_retry=self.__max_retry,
                         sleep_base=self.__sleep_base,
+                        throttler=self.__throttler,
                     )
                 except Exception as e:
                     all_purpose_logger.error(
                         f"Failed to retrieve number of pages for {next_crawl.url} from {next_crawl.cdx_server} with reason {e}"
                     )
                     continue
                 all_purpose_logger.info(
@@ -314,14 +322,15 @@
                                 dc.url,
                                 match_type=self.__match_type,
                                 page=dc.page,
                                 since=self.__since,
                                 to=self.__to,
                                 max_retry=self.__max_retry,
                                 sleep_base=self.__sleep_base,
+                                throttler=self.__throttler,
                             ),
                         )
                     )
                 return num_pages
             return 0
 
         async def __await_next_prefetch(self):
```

### Comparing `CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/athena_query_maker.py` & `CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/athena_query_maker.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/aggregator/utils/helpers.py` & `CmonCrawl-1.1.8/cmoncrawl/aggregator/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 from cmoncrawl.aggregator.utils import ndjson
 from cmoncrawl.common.loggers import all_purpose_logger
+from cmoncrawl.common.throttling import Throttler
 
 ALLOWED_ERR_FOR_RETRIES = [500, 502, 503, 504]
 
 
 class DownloadError(Exception):
     def __init__(self, reason: str, status: int):
         self.reason = reason
@@ -110,66 +111,74 @@
     cdx_server: str,
     params: dict[str, Any],
     content_type: str,
     max_retry: int,
     sleep_base: float,
     allowed_status_errors: list[int] = ALLOWED_ERR_FOR_RETRIES,
     log_additional_info: dict[str, Any] = {},  # type: ignore
+    throttler: Throttler | None = None,
 ):
     @retry(
         stop=stop_after_attempt(max_retry + 1),
         wait=wait_random_exponential(multiplier=5, exp_base=sleep_base, max=120),
         retry=retry_if_exception_type(DownloadError),
         reraise=True,
         before_sleep=log_after_retry,
     )
-    async def _retrieve(
+    async def _retrieve_with_throttling(
         client: ClientSession,
         cdx_server: str,
         params: dict[str, Any],
         content_type: str,
         allowed_status_errors: list[int],
         log_additional_info: dict[str, Any],
     ):
         all_purpose_logger.debug(
             f"Sending request to {cdx_server} with params: {params}"
         )
-        try:
-            async with client.get(cdx_server, params=params) as response:
-                status = response.status
-                if not response.ok:
-                    reason = str(response.reason) if response.reason else "Unknown"  # type: ignore
-                    if status in allowed_status_errors:
-                        raise DownloadError(reason, status)
-                    raise ValueError(
-                        f"Failed to download {cdx_server} with status {status} and reason {reason}"
-                    )
-                else:
-                    if content_type == "text/x-ndjson":
-                        content = await response.json(
-                            content_type=content_type,
-                            loads=ndjson.Decoder().decode,
+
+        async def _request():
+            try:
+                async with client.get(cdx_server, params=params) as response:
+                    status = response.status
+                    if not response.ok:
+                        reason = str(response.reason) if response.reason else "Unknown"  # type: ignore
+                        if status in allowed_status_errors:
+                            raise DownloadError(reason, status)
+                        raise ValueError(
+                            f"Failed to download {cdx_server} with status {status} and reason {reason}"
                         )
-                    elif content_type == "application/json":
-                        content = await response.json(content_type=content_type)
                     else:
-                        raise ValueError(f"Unknown content type: {content_type}")
-        except (
-            ClientError,
-            TimeoutError,
-            ServerConnectionError,
-            ContentTypeError,
-        ) as e:
-            reason = f"{type(e)} {str(e)}"
-            status = 500
-            raise DownloadError(reason, status)
-
-        return content
+                        if content_type == "text/x-ndjson":
+                            content = await response.json(
+                                content_type=content_type,
+                                loads=ndjson.Decoder().decode,
+                            )
+                        elif content_type == "application/json":
+                            content = await response.json(content_type=content_type)
+                        else:
+                            raise ValueError(f"Unknown content type: {content_type}")
+            except (
+                ClientError,
+                TimeoutError,
+                ServerConnectionError,
+                ContentTypeError,
+            ) as e:
+                reason = f"{type(e)} {str(e)}"
+                status = 500
+                raise DownloadError(reason, status)
+
+            return content
+
+        if throttler is not None:
+            return await throttler.throttle(_request)
+        else:
+            return await _request()
 
-    return await _retrieve(
+    return await _retrieve_with_throttling(
         client=client,
         cdx_server=cdx_server,
         params=params,
         content_type=content_type,
         allowed_status_errors=allowed_status_errors,
         log_additional_info=log_additional_info,
     )
```

### Comparing `CmonCrawl-1.1.7/cmoncrawl/common/loggers.py` & `CmonCrawl-1.1.8/cmoncrawl/common/loggers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/common/throttling.py` & `CmonCrawl-1.1.8/cmoncrawl/common/throttling.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/common/types.py` & `CmonCrawl-1.1.8/cmoncrawl/common/types.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/integrations/commands.py` & `CmonCrawl-1.1.8/cmoncrawl/integrations/commands.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/integrations/download.py` & `CmonCrawl-1.1.8/cmoncrawl/integrations/download.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/integrations/extract.py` & `CmonCrawl-1.1.8/cmoncrawl/integrations/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,16 +170,21 @@
             DomainRecord(filename="", url=url, offset=0, length=0, timestamp=date),
             {},
         )
     ]
 
 
 def load_config(config_path: Path) -> ExtractConfig:
-    with open(config_path, "r") as f:
-        config = json.load(f)
+    try:
+        with open(config_path, "r") as f:
+            config = json.load(f)
+    except Exception as e:
+        raise ValueError(
+            f"Failed to load extractor config. Ensure it's valid JSON."
+        ) from e
     return ExtractConfig.model_validate(config)
 
 
 def create_router(config: ExtractConfig) -> Router:
     router = Router()
     router.load_modules(config.extractors_path)
     router.register_routes(config.routes)
@@ -269,17 +274,19 @@
 def run_extract(args: argparse.Namespace):
     config = load_config(args.config_path)
     pool = multiprocessing.Pool(args.n_proc)
     pool.starmap(
         _extract_task,
         [
             (
-                args.output_path / f"{file.stem}"
-                if args.n_proc != 1
-                else args.output_path,
+                (
+                    args.output_path / f"{file.stem}"
+                    if args.n_proc != 1
+                    else args.output_path
+                ),
                 config,
                 [file],
                 args,
             )
             for _, file in enumerate(args.files)
         ],
     )
```

### Comparing `CmonCrawl-1.1.7/cmoncrawl/integrations/utils.py` & `CmonCrawl-1.1.8/cmoncrawl/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/middleware/stompware.py` & `CmonCrawl-1.1.8/cmoncrawl/middleware/stompware.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/middleware/synchronized.py` & `CmonCrawl-1.1.8/cmoncrawl/middleware/synchronized.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/dao/api.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/dao/api.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/dao/base.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/dao/base.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/dao/s3.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/dao/s3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Any
 
 import aioboto3
 from botocore.config import Config
 from botocore.exceptions import ClientError
 
+from cmoncrawl.common.caching import AbstractDomainRecordCache
 from cmoncrawl.common.types import DomainRecord
 from cmoncrawl.processor.dao.base import DownloadError, ICC_Dao
 
 
 class S3Dao(ICC_Dao):
     """
     S3Dao is a class that provides methods to interact with AWS S3 for downloading warc files from the commoncrawl bucket.
 
     Args:
         aws_profile (str, optional): The AWS profile to use for the download. Defaults to None.
         bucket_name (str, optional): The name of the S3 bucket. Defaults to "commoncrawl".
+        cache (AbstractDomainRecordCache, optional): Cache to use for downloading from s3.
 
     Attributes:
         bucket_name (str): The name of the S3 bucket.
         aws_profile (str): The AWS profile to use for the download.
         client (aioboto3.client): The S3 client.
 
     Methods:
@@ -28,19 +30,23 @@
 
     Raises:
         ValueError: If the S3Dao client is not initialized.
 
     """
 
     def __init__(
-        self, aws_profile: str | None = None, bucket_name: str = "commoncrawl"
+        self,
+        aws_profile: str | None = None,
+        bucket_name: str = "commoncrawl",
+        cache: AbstractDomainRecordCache | None = None,
     ) -> None:
         self.bucket_name = bucket_name
         self.aws_profile = aws_profile
         self.client = None
+        self.cache = cache
 
     async def __aenter__(self) -> "S3Dao":
         # We handle the retries ourselves, so we disable the botocore retries
         config = Config(
             retries={
                 "max_attempts": 1,
             }
@@ -69,19 +75,27 @@
         """
 
         if self.client is None:
             raise ValueError(
                 "S3Dao client is not initialized, did you forget to use async with?"
             )
 
+        if self.cache:
+            cached_bytes = self.cache.get(domain_record)
+            if cached_bytes is not None:
+                return cached_bytes
+
         file_name = domain_record.filename
         byte_range = f"bytes={domain_record.offset}-{domain_record.offset+domain_record.length-1}"
 
         try:
             response = await self.client.get_object(
                 Bucket=self.bucket_name, Key=file_name, Range=byte_range
             )
             file_bytes = await response["Body"].read()
         except ClientError as e:
             raise DownloadError(f"AWS: {e.response['Error']['Message']}", 500)
 
+        if self.cache:
+            self.cache.set(domain_record, file_bytes)
+
         return file_bytes
```

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/extraction/filters.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/extraction/filters.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/extraction/utils.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/extraction/utils.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/downloader.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/downloader.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/extractor.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/pipeline.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/router.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/router.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/cmoncrawl/processor/pipeline/streamer.py` & `CmonCrawl-1.1.8/cmoncrawl/processor/pipeline/streamer.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/Makefile` & `CmonCrawl-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/make.bat` & `CmonCrawl-1.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/cli/cli.rst` & `CmonCrawl-1.1.8/docs/source/cli/cli.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/cli/download.rst` & `CmonCrawl-1.1.8/docs/source/cli/download.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/cli/extract.rst` & `CmonCrawl-1.1.8/docs/source/cli/extract.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/conf.py` & `CmonCrawl-1.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/extraction/config_file.rst` & `CmonCrawl-1.1.8/docs/source/extraction/config_file.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/extraction/creating_extractor.rst` & `CmonCrawl-1.1.8/docs/source/extraction/creating_extractor.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/extraction/utils.rst` & `CmonCrawl-1.1.8/docs/source/extraction/utils.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.common.types.rst` & `CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.common.types.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.integrations.download.rst` & `CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.integrations.download.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/generated/cmoncrawl.processor.pipeline.downloader.rst` & `CmonCrawl-1.1.8/docs/source/generated/cmoncrawl.processor.pipeline.downloader.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/images/domain_record.drawio.pdf` & `CmonCrawl-1.1.8/docs/source/images/domain_record.drawio.pdf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/images/when_to_use.drawio.png` & `CmonCrawl-1.1.8/docs/source/images/when_to_use.drawio.png`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/index.rst` & `CmonCrawl-1.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/misc/athena.rst` & `CmonCrawl-1.1.8/docs/source/misc/athena.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/misc/domain_record.rst` & `CmonCrawl-1.1.8/docs/source/misc/domain_record.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/prog_guide/index.rst` & `CmonCrawl-1.1.8/docs/source/prog_guide/index.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/prog_guide/overview.rst` & `CmonCrawl-1.1.8/docs/source/prog_guide/overview.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/prog_guide/practice.rst` & `CmonCrawl-1.1.8/docs/source/prog_guide/practice.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/docs/source/usage.rst` & `CmonCrawl-1.1.8/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/examples/code-usage/offline-warc-iteration.py` & `CmonCrawl-1.1.8/examples/code-usage/offline-warc-iteration.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/examples/extractor_tutorial/Extractors/bbc_extractor.py` & `CmonCrawl-1.1.8/examples/extractor_tutorial/Extractors/bbc_extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/examples/extractor_tutorial/Extractors/idnes_extractor.py` & `CmonCrawl-1.1.8/examples/extractor_tutorial/Extractors/idnes_extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/extractors/my_extractor.py` & `CmonCrawl-1.1.8/extractors/my_extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/pyproject.toml` & `CmonCrawl-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/athena_test.py` & `CmonCrawl-1.1.8/tests/athena_test.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/end_to_end_test.py` & `CmonCrawl-1.1.8/tests/end_to_end_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from parameterized import parameterized
 
 from cmoncrawl.common.types import ExtractConfig
 from cmoncrawl.integrations.extract import (
     ExtractMode,
     extract_from_files,
+    load_config,
 )
 from cmoncrawl.integrations.utils import DAOname
 
 
 class ExtractFiles(unittest.IsolatedAsyncioTestCase):
     """
     CLI Testing
@@ -26,20 +27,23 @@
     async def asyncTearDown(self) -> None:
         # remoev output folder
         if self.output_folder.exists():
             shutil.rmtree(self.output_folder)
 
     async def test_load_config(self):
         cfg_path = self.base_folder / "cfg.json"
-        with open(cfg_path, "r") as f:
-            js = json.load(f)
-            cfg: ExtractConfig = ExtractConfig.model_validate(js)
+        cfg: ExtractConfig = load_config(cfg_path)
 
         self.assertEqual(cfg.routes[0].extractors[0].name, "test_extractor")
 
+    async def test_load_config_invalid_json(self):
+        cfg_path = self.base_folder / "cfg_invalid.json"
+        with self.assertRaises(ValueError):
+            load_config(cfg_path)
+
     @parameterized.expand([(DAOname.API,), (DAOname.S3,)])
     async def test_extract_from_records(self, dao: DAOname):
         cfg_path = self.base_folder / "cfg.json"
         with open(cfg_path, "r") as f:
             js = json.load(f)
             cfg: ExtractConfig = ExtractConfig.model_validate(js)
         await extract_from_files(
```

### Comparing `CmonCrawl-1.1.7/tests/files/mini.warc.gz` & `CmonCrawl-1.1.8/tests/files/mini.warc.gz`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/gateway_test.py` & `CmonCrawl-1.1.8/tests/gateway_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,43 @@
 from cmoncrawl.aggregator.athena_query import (
     DomainRecord,
     MatchType,
 )
 from cmoncrawl.aggregator.gateway_query import GatewayAggregator
 from cmoncrawl.aggregator.utils.constants import CC_INDEXES_SERVER
 from cmoncrawl.aggregator.utils.helpers import get_all_CC_indexes, unify_url_id
+from cmoncrawl.common.throttling import Throttler
 
 
 class TestIndexerAsync(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self) -> None:
         self.CC_SERVERS = ["https://index.commoncrawl.org/CC-MAIN-2022-05-index"]
         self.di = await GatewayAggregator(
             ["idnes.cz"],
             cc_servers=self.CC_SERVERS,
             max_retry=100,
             sleep_base=1.4,
             prefetch_size=1,
             match_type=MatchType.DOMAIN,
         ).aopen()
         self.client = self.di.client
+        self.throttler = Throttler(1)
 
     async def asyncTearDown(self) -> None:
         await self.di.aclose(None, None, None)
 
     async def test_indexer_num_pages(self):
         num_pages = await self.di.get_number_of_pages(
             self.client,
             self.CC_SERVERS[0],
             "idnes.cz",
             max_retry=20,
             sleep_base=1.4,
             match_type=MatchType.DOMAIN,
+            throttler=self.throttler,
         )
         self.assertEqual(num_pages, 14)
 
     async def test_indexer_all_CC(self):
         indexes = await get_all_CC_indexes(self.client, CC_INDEXES_SERVER)
         indexes = sorted(indexes)
         indexes = indexes[
@@ -78,14 +81,15 @@
             since=datetime(2022, 5, 1),
             to=datetime(2022, 1, 10),
             limit=None,
             max_retry=10,
             sleep_base=4,
             prefetch_size=2,
             match_type=MatchType.DOMAIN,
+            throttler=self.throttler,
         )
         self.assertIsNotNone(self.di.cc_servers)
         # Generates only for 2020
         q = iterator.init_crawls_queue(
             self.di.urls,
             self.di.cc_servers
             + [
```

### Comparing `CmonCrawl-1.1.7/tests/helpers_test.py` & `CmonCrawl-1.1.8/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/processor_test.py` & `CmonCrawl-1.1.8/tests/processor_test.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/test_extract/files/file.html` & `CmonCrawl-1.1.8/tests/test_extract/files/file.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/test_extract/files/file.jsonl` & `CmonCrawl-1.1.8/tests/test_extract/files/file.jsonl`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.1.7/tests/utils.py` & `CmonCrawl-1.1.8/tests/utils.py`

 * *Files identical despite different names*

