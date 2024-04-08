# Comparing `tmp/ralph-malph-4.1.0.tar.gz` & `tmp/ralph-malph-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-4.1.0.tar", last modified: Mon Feb 12 11:07:29 2024, max compression
+gzip compressed data, was "ralph-malph-4.2.0.tar", last modified: Mon Apr  8 15:41:25 2024, max compression
```

## Comparing `ralph-malph-4.1.0.tar` & `ralph-malph-4.2.0.tar`

### file list

```diff
@@ -1,204 +1,264 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.812498 ralph-malph-4.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12827 2024-02-12 11:07:29.812498 ralph-malph-4.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6868 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5964 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-12 11:07:29.812498 ralph-malph-4.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.780497 ralph-malph-4.1.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.784497 ralph-malph-4.1.0/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.784497 ralph-malph-4.1.0/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.784497 ralph-malph-4.1.0/src/ralph/api/auth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/auth/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5774 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/auth/basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5162 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/auth/oidc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2035 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/auth/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.784497 ralph-malph-4.1.0/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22459 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.784497 ralph-malph-4.1.0/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.788498 ralph-malph-4.1.0/src/ralph/backends/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11851 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/async_es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10305 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/async_lrs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14091 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/async_mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8971 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/async_ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26653 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15896 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16196 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14832 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11544 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11101 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/lrs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2301 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17850 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16547 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/data/swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3326 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/loader.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.788498 ralph-malph-4.1.0/src/ralph/backends/lrs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/async_es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2120 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/async_mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4592 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7150 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5168 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15698 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5618 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/backends/lrs/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26509 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7741 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.788498 ralph-malph-4.1.0/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9412 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.788498 ralph-malph-4.1.0/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2066 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.788498 ralph-malph-4.1.0/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.788498 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1795 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1620 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/enrollment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7553 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      950 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4860 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      977 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3719 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9797 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8201 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12749 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10544 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1927 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10102 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12455 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.792497 ralph-malph-4.1.0/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3013 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7778 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5250 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3135 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.796497 ralph-malph-4.1.0/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.796497 ralph-malph-4.1.0/src/ralph/models/xapi/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/agents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/ifi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1479 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2367 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4105 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/base/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.796497 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.796497 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1369 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/audio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2925 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      896 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.800498 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/lms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.800498 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1095 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1228 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1673 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1648 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4597 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.800498 ralph-malph-4.1.0/src/ralph/models/xapi/lms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/lms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5807 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/lms/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/lms/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8206 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/lms/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.800498 ralph-malph-4.1.0/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/navigation/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.800498 ralph-malph-4.1.0/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9291 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/video/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/video/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6898 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/video/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.800498 ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8050 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2896 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10245 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.804498 ralph-malph-4.1.0/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12827 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6566 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-12 11:07:29.000000 ralph-malph-4.1.0/src/ralph_malph.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-12 11:07:29.804498 ralph-malph-4.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35542 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25068 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_cli_usage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4118 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_dependencies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5995 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2374 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4823 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2024-02-12 11:07:28.000000 ralph-malph-4.1.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.094102 ralph-malph-4.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12817 2024-04-08 15:41:25.094102 ralph-malph-4.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6868 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7122 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 15:41:25.094102 ralph-malph-4.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.050101 ralph-malph-4.2.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1514 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/api/auth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1948 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5810 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5162 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/oidc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2035 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22459 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.058101 ralph-malph-4.2.0/src/ralph/backends/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11851 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10305 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14074 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8971 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26653 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15896 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16196 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14832 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11544 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11101 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2301 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17787 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16547 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2826 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/loader.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.058101 ralph-malph-4.2.0/src/ralph/backends/lrs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/async_es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2120 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/async_mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4592 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7030 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15698 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5557 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26509 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7543 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9412 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3670 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2833 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/certificate/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2858 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4288 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/cohort/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2351 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3184 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2543 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1795 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1621 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/enrollment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7554 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1984 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2433 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      950 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4860 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      977 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3719 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/notes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6788 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9797 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8201 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/poll/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/poll/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12749 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10544 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1927 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/survey/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1728 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3914 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5549 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10102 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12455 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3013 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7778 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5250 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3134 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/xapi/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/ifi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1479 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2367 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4105 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.078101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.078101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1497 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/audio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2933 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.078101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/lms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1095 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2182 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4613 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/lms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5807 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8206 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/navigation/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9291 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6898 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8052 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2896 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10245 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.086101 ralph-malph-4.2.0/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12817 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8538 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.086101 ralph-malph-4.2.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35542 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25068 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5995 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2374 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4823 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_utils.py
```

### Comparing `ralph-malph-4.1.0/LICENSE.md` & `ralph-malph-4.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/PKG-INFO` & `ralph-malph-4.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 4.1.0
+Version: 4.2.0
 Summary: Ralph, the ultimate Learning Record Store (and more!) for your learning analytics.
 Author-email: "Open FUN (France Université Numérique)" <fun.dev@fun-mooc.fr>
 License: MIT License
         
         Copyright (c) 2020-present France Université Numérique
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: importlib-metadata<8.0,>=7.0.1
 Requires-Dist: langcodes>=3.2.0
 Requires-Dist: pydantic[dotenv,email]<2.0,>=1.10.0
 Requires-Dist: rfc3987>=1.3.0
 Provides-Extra: backend-clickhouse
 Requires-Dist: clickhouse-connect[numpy,pandas]<0.6; extra == "backend-clickhouse"
 Requires-Dist: python-dateutil>=2.8.2; extra == "backend-clickhouse"
 Provides-Extra: backend-es
@@ -68,56 +69,55 @@
 Requires-Dist: python-keystoneclient>=5.0.0; extra == "backend-swift"
 Requires-Dist: python-swiftclient>=4.0.0; extra == "backend-swift"
 Provides-Extra: backend-ws
 Requires-Dist: websockets>=10.3; extra == "backend-ws"
 Provides-Extra: backends
 Requires-Dist: ralph-malph[backend-clickhouse,backend-es,backend-ldp,backend-lrs,backend-mongo,backend-s3,backend-swift]; extra == "backends"
 Provides-Extra: ci
-Requires-Dist: twine==4.0.2; extra == "ci"
+Requires-Dist: twine==5.0.0; extra == "ci"
 Provides-Extra: cli
 Requires-Dist: bcrypt>=4.0.0; extra == "cli"
 Requires-Dist: click>=8.1.0; extra == "cli"
 Requires-Dist: click-option-group>=0.5.0; extra == "cli"
 Requires-Dist: sentry-sdk[fastapi]>=1.9.0; extra == "cli"
 Provides-Extra: dev
-Requires-Dist: anyio<4.2.1; extra == "dev"
-Requires-Dist: black==23.12.1; extra == "dev"
-Requires-Dist: cryptography==41.0.7; extra == "dev"
+Requires-Dist: anyio<4.3.1; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: factory-boy==3.3.0; extra == "dev"
 Requires-Dist: hypothesis<6.92.0; extra == "dev"
-Requires-Dist: logging-gelf==0.0.31; extra == "dev"
+Requires-Dist: logging-gelf==0.0.32; extra == "dev"
 Requires-Dist: mike==2.0.0; extra == "dev"
 Requires-Dist: mkdocs==1.5.3; extra == "dev"
 Requires-Dist: mkdocs-click==0.8.1; extra == "dev"
-Requires-Dist: mkdocs-material==9.5.3; extra == "dev"
-Requires-Dist: mkdocstrings[python-legacy]==0.24.0; extra == "dev"
-Requires-Dist: moto==4.2.13; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
-Requires-Dist: neoteroi-mkdocs==1.0.4; extra == "dev"
-Requires-Dist: pyfakefs==5.3.2; extra == "dev"
-Requires-Dist: pymdown-extensions==10.7; extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.3; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: mkdocs-material==9.5.17; extra == "dev"
+Requires-Dist: mkdocstrings[python-legacy]==0.24.3; extra == "dev"
+Requires-Dist: moto==5.0.5; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: neoteroi-mkdocs==1.0.5; extra == "dev"
+Requires-Dist: pyfakefs==5.4.0; extra == "dev"
+Requires-Dist: pymdown-extensions==10.7.1; extra == "dev"
+Requires-Dist: pytest<8.0.0; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-httpx<0.23.0; extra == "dev"
-Requires-Dist: requests-mock==1.11.0; extra == "dev"
+Requires-Dist: requests-mock==1.12.1; extra == "dev"
 Requires-Dist: responses==0.24.1; extra == "dev"
-Requires-Dist: ruff==0.1.11; extra == "dev"
-Requires-Dist: types-python-dateutil==2.8.19.20240106; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
+Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == "dev"
 Requires-Dist: types-python-jose==3.3.4.20240106; extra == "dev"
-Requires-Dist: types-requests<2.31.0.20240107; extra == "dev"
+Requires-Dist: types-requests<2.31.0.20240407; extra == "dev"
 Requires-Dist: types-cachetools==5.3.0.7; extra == "dev"
 Provides-Extra: lrs
 Requires-Dist: bcrypt==4.1.2; extra == "lrs"
-Requires-Dist: fastapi==0.108.0; extra == "lrs"
-Requires-Dist: cachetools==5.3.2; extra == "lrs"
+Requires-Dist: fastapi==0.110.1; extra == "lrs"
+Requires-Dist: cachetools==5.3.3; extra == "lrs"
 Requires-Dist: httpx<0.25.0; extra == "lrs"
-Requires-Dist: sentry_sdk==1.39.1; extra == "lrs"
+Requires-Dist: sentry_sdk==1.44.1; extra == "lrs"
 Requires-Dist: python-jose==3.3.0; extra == "lrs"
-Requires-Dist: uvicorn[standard]==0.25.0; extra == "lrs"
+Requires-Dist: uvicorn[standard]==0.29.0; extra == "lrs"
 Provides-Extra: full
 Requires-Dist: ralph-malph[backends,cli,lrs]; extra == "full"
 
 
 <p align="center">
   <a href="https://openfun.github.io/ralph"><img src="https://raw.githubusercontent.com/openfun/logos/main/ralph/ralph-color-dark.png" alt="Ralph logo" width="400"></a>
 </p>
```

### Comparing `ralph-malph-4.1.0/README.md` & `ralph-malph-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/pyproject.toml` & `ralph-malph-4.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ]
 requires-python = ">=3.8"
 license = { file = "LICENSE.md" }
 keywords = ["LRS", "Analytics", "xAPI", "Open edX"]
 dependencies = [
     # By default, we only consider core dependencies required to use Ralph as a
     # library (mostly models).
+    "importlib-metadata>=7.0.1, <8.0",
     "langcodes>=3.2.0",
     "pydantic[dotenv,email]>=1.10.0, <2.0",
     "rfc3987>=1.3.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
@@ -74,68 +75,89 @@
 backend-ws = [
     "websockets>=10.3",
 ]
 backends = [
     "ralph-malph[backend-clickhouse,backend-es,backend-ldp,backend-lrs,backend-mongo,backend-s3,backend-swift]",
 ]
 ci = [
-    "twine==4.0.2",
+    "twine==5.0.0",
 ]
 cli = [
     "bcrypt>=4.0.0",
     "click>=8.1.0",
     "click-option-group>=0.5.0",
     "sentry-sdk[fastapi]>=1.9.0",
 ]
 dev = [
-    "anyio<4.2.1", # unpin until fastapi supports new major version of anyio
-    "black==23.12.1",
-    "cryptography==41.0.7",
+    "anyio<4.3.1", # unpin until fastapi supports new major version of anyio
+    "black==24.3.0",
+    "cryptography==42.0.5",
     "factory-boy==3.3.0",
     "hypothesis<6.92.0", # pin as hypothesis 6.92.0 observability feature seems broken
-    "logging-gelf==0.0.31",
+    "logging-gelf==0.0.32",
     "mike==2.0.0",
     "mkdocs==1.5.3",
     "mkdocs-click==0.8.1",
-    "mkdocs-material==9.5.3",
-    "mkdocstrings[python-legacy]==0.24.0",
-    "moto==4.2.13",
-    "mypy==1.8.0",
-    "neoteroi-mkdocs==1.0.4",
-    "pyfakefs==5.3.2",
-    "pymdown-extensions==10.7",
-    "pytest==7.4.4",
-    "pytest-asyncio==0.23.3",
-    "pytest-cov==4.1.0",
+    "mkdocs-material==9.5.17",
+    "mkdocstrings[python-legacy]==0.24.3",
+    "moto==5.0.5",
+    "mypy==1.9.0",
+    "neoteroi-mkdocs==1.0.5",
+    "pyfakefs==5.4.0",
+    "pymdown-extensions==10.7.1",
+    "pytest<8.0.0", # pin as pytest-httpx<0.23.0 is not compatible with pytest 8.0.0 
+    "pytest-cov==5.0.0",
     "pytest-httpx<0.23.0", # pin as Python 3.8 is no longer supported from release 0.23.0
-    "requests-mock==1.11.0",
+    "requests-mock==1.12.1",
     "responses==0.24.1",
-    "ruff==0.1.11",
-    "types-python-dateutil ==2.8.19.20240106",
+    "ruff==0.3.5",
+    "types-python-dateutil ==2.9.0.20240316",
     "types-python-jose ==3.3.4.20240106",
-    "types-requests<2.31.0.20240107",
+    "types-requests<2.31.0.20240407",
     "types-cachetools ==5.3.0.7",
 ]
 lrs = [
     "bcrypt==4.1.2",
-    "fastapi==0.108.0",
-    "cachetools==5.3.2",
+    "fastapi==0.110.1",
+    "cachetools==5.3.3",
     "httpx<0.25.0", # pin as `pytest-httpx<0.23.0` requires `httpx==0.24.*`
-    "sentry_sdk==1.39.1",
+    "sentry_sdk==1.44.1",
     "python-jose==3.3.0",
-    "uvicorn[standard]==0.25.0",
+    "uvicorn[standard]==0.29.0",
 ]
 full = [
     "ralph-malph[backends,cli,lrs]",
 ]
 
 
 [project.scripts]
 ralph = "ralph.__main__:cli.cli"
 
+[project.entry-points."ralph.backends.data"]
+async_es = "ralph.backends.data.async_es:AsyncESDataBackend"
+async_lrs = "ralph.backends.data.async_lrs:AsyncLRSDataBackend"
+async_mongo = "ralph.backends.data.async_mongo:AsyncMongoDataBackend"
+async_ws = "ralph.backends.data.async_ws:AsyncWSDataBackend"
+clickhouse = "ralph.backends.data.clickhouse:ClickHouseDataBackend"
+es = "ralph.backends.data.es:ESDataBackend"
+fs = "ralph.backends.data.fs:FSDataBackend"
+ldp = "ralph.backends.data.ldp:LDPDataBackend"
+lrs = "ralph.backends.data.lrs:LRSDataBackend"
+mongo = "ralph.backends.data.mongo:MongoDataBackend"
+s3 = "ralph.backends.data.s3:S3DataBackend"
+swift = "ralph.backends.data.swift:SwiftDataBackend"
+
+[project.entry-points."ralph.backends.lrs"]
+async_es = "ralph.backends.lrs.async_es:AsyncESLRSBackend"
+async_mongo = "ralph.backends.lrs.async_mongo:AsyncMongoLRSBackend"
+clickhouse = "ralph.backends.lrs.clickhouse:ClickHouseLRSBackend"
+es = "ralph.backends.lrs.es:ESLRSBackend"
+fs = "ralph.backends.lrs.fs:FSLRSBackend"
+mongo = "ralph.backends.lrs.mongo:MongoLRSBackend"
+
 [tool.setuptools]
 packages = { find = { where = ["src"] } }
 zip-safe = true
 
 [tool.setuptools.dynamic]
 version = { attr = "ralph.__version__" }
 
@@ -188,27 +210,27 @@
 ]
 
 [tool.ruff.lint.isort]
 section-order = ["future", "standard-library", "third-party", "ralph", "first-party", "local-folder"]
 [tool.ruff.lint.isort.sections]
 ralph = ["ralph"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "ARG",  # flake8-unused-arguments
     "D",  # pydocstyle
     "S",  # flake8-bandit
     "SLF",  # flake8-self
     "PLR2004",  # Pylint magic-value-comparison
 ]
 "setup.py" = [
     "D" # Pydocstyle rules
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 # Use Google-style docstrings.
 convention = "google"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
 disallow_untyped_defs = true
```

### Comparing `ralph-malph-4.1.0/src/ralph/__main__.py` & `ralph-malph-4.2.0/src/ralph/__main__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/api/__init__.py` & `ralph-malph-4.2.0/src/ralph/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main module for Ralph's LRS API."""
+
 from functools import lru_cache
 from typing import Any, Dict, List, Union
 from urllib.parse import urlparse
 
 import sentry_sdk
 from fastapi import Depends, FastAPI
```

### Comparing `ralph-malph-4.1.0/src/ralph/api/auth/__init__.py` & `ralph-malph-4.2.0/src/ralph/api/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main module for Ralph's LRS API authentication."""
+
 from typing import Optional
 
 from fastapi import Depends, HTTPException, status
 from fastapi.security import SecurityScopes
 
 from ralph.api.auth.basic import AuthenticatedUser, get_basic_auth_user
 from ralph.api.auth.oidc import get_oidc_user
```

### Comparing `ralph-malph-4.1.0/src/ralph/api/auth/basic.py` & `ralph-malph-4.2.0/src/ralph/api/auth/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,19 +99,21 @@
     return ServerUsersCredentials.parse_file(auth_file)
 
 
 @cached(
     TTLCache(maxsize=settings.AUTH_CACHE_MAX_SIZE, ttl=settings.AUTH_CACHE_TTL),
     lock=Lock(),
     key=lambda credentials: (
-        credentials.username,
-        credentials.password,
-    )
-    if credentials is not None
-    else None,
+        (
+            credentials.username,
+            credentials.password,
+        )
+        if credentials is not None
+        else None
+    ),
 )
 def get_basic_auth_user(
     credentials: Optional[HTTPBasicCredentials] = Depends(security),
 ) -> AuthenticatedUser:
     """Check valid auth parameters.
 
     Get the basic auth parameters from the Authorization header, and checks them
```

### Comparing `ralph-malph-4.1.0/src/ralph/api/auth/oidc.py` & `ralph-malph-4.2.0/src/ralph/api/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/api/auth/user.py` & `ralph-malph-4.2.0/src/ralph/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/api/forwarding.py` & `ralph-malph-4.2.0/src/ralph/api/forwarding.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/api/models.py` & `ralph-malph-4.2.0/src/ralph/api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API-specific data models definition.
 
 Allows to be exactly as lax as we want when it comes to exact object shape and
 validation.
 """
+
 from typing import Optional, Union
 from uuid import UUID
 
 from pydantic import AnyUrl, BaseModel, Extra
 
 from ..models.xapi.base.agents import BaseXapiAgent
 from ..models.xapi.base.groups import BaseXapiGroup
```

### Comparing `ralph-malph-4.1.0/src/ralph/api/routers/health.py` & `ralph-malph-4.2.0/src/ralph/api/routers/health.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/api/routers/statements.py` & `ralph-malph-4.2.0/src/ralph/api/routers/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/async_es.py` & `ralph-malph-4.2.0/src/ralph/backends/data/async_es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/async_lrs.py` & `ralph-malph-4.2.0/src/ralph/backends/data/async_lrs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/async_mongo.py` & `ralph-malph-4.2.0/src/ralph/backends/data/async_mongo.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         except (ConnectionFailure, PyMongoError) as error:
             logger.error("Failed to connect to MongoDB: %s", error)
             return DataBackendStatus.AWAY
 
         # Check MongoDB server status.
         try:
             server_status = await self.client.admin.command("serverStatus")
-            if server_status.get("ok") != 1.0:  # noqa: PLR2004
+            if server_status.get("ok") != 1.0:
                 logger.error("MongoDB `serverStatus` command did not return 1.0")
                 return DataBackendStatus.ERROR
         except PyMongoError as error:
             logger.error("Failed to get MongoDB server status: %s", error)
             return DataBackendStatus.ERROR
 
         return DataBackendStatus.OK
```

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/async_ws.py` & `ralph-malph-4.2.0/src/ralph/backends/data/async_ws.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/base.py` & `ralph-malph-4.2.0/src/ralph/backends/data/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/clickhouse.py` & `ralph-malph-4.2.0/src/ralph/backends/data/clickhouse.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/es.py` & `ralph-malph-4.2.0/src/ralph/backends/data/es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/fs.py` & `ralph-malph-4.2.0/src/ralph/backends/data/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/ldp.py` & `ralph-malph-4.2.0/src/ralph/backends/data/ldp.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/lrs.py` & `ralph-malph-4.2.0/src/ralph/backends/data/lrs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/mixins.py` & `ralph-malph-4.2.0/src/ralph/backends/data/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/mongo.py` & `ralph-malph-4.2.0/src/ralph/backends/data/mongo.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     class Config(BaseSettingsConfig):
         """Pydantic Configuration."""
 
         env_prefix = "RALPH_BACKENDS__DATA__MONGO__"
 
     CONNECTION_URI: MongoDsn = MongoDsn("mongodb://localhost:27017/", scheme="mongodb")
     DEFAULT_DATABASE: constr(regex=r"^[^\s.$/\\\"\x00]+$") = "statements"
-    DEFAULT_COLLECTION: constr(
-        regex=r"^(?!.*\.\.)[^.$\x00]+(?:\.[^.$\x00]+)*$"
-    ) = "marsha"
+    DEFAULT_COLLECTION: constr(regex=r"^(?!.*\.\.)[^.$\x00]+(?:\.[^.$\x00]+)*$") = (
+        "marsha"
+    )
     CLIENT_OPTIONS: MongoClientOptions = MongoClientOptions()
 
 
 class MongoQuery(BaseQuery):
     """MongoDB query model.
 
     Attributes:
@@ -122,18 +122,15 @@
             self.client.admin.command("ping")
         except (ConnectionFailure, InvalidOperation) as error:
             logger.error("Failed to connect to MongoDB: %s", error)
             return DataBackendStatus.AWAY
 
         # Check MongoDB server status.
         try:
-            if (
-                self.client.admin.command("serverStatus").get("ok")
-                != 1.0  # noqa: PLR2004
-            ):
+            if self.client.admin.command("serverStatus").get("ok") != 1.0:
                 logger.error("MongoDB `serverStatus` command did not return 1.0")
                 return DataBackendStatus.ERROR
         except PyMongoError as error:
             logger.error("Failed to get MongoDB server status: %s", error)
             return DataBackendStatus.ERROR
 
         return DataBackendStatus.OK
```

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/s3.py` & `ralph-malph-4.2.0/src/ralph/backends/data/s3.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/data/swift.py` & `ralph-malph-4.2.0/src/ralph/backends/data/swift.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/loader.py` & `ralph-malph-4.2.0/src/ralph/backends/loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,92 @@
 """Ralph backend loader."""
 
 import logging
-import pkgutil
+import sys
 from functools import lru_cache
-from importlib import import_module
-from importlib.util import find_spec
-from inspect import getmembers, isabstract, isclass
-from typing import Dict, Tuple, Type
+from typing import Dict, Tuple
+
+if sys.version_info < (3, 10):
+    from importlib_metadata import EntryPoints, entry_points
+else:
+    from importlib.metadata import EntryPoints, entry_points
 
 from ralph.backends.data.base import (
     AsyncListable,
     AsyncWritable,
     BaseAsyncDataBackend,
     BaseDataBackend,
     Listable,
     Writable,
 )
 from ralph.backends.lrs.base import BaseAsyncLRSBackend, BaseLRSBackend
 
 logger = logging.getLogger(__name__)
 
 
-@lru_cache()
-def get_backends(packages: Tuple[str], base_backends: Tuple[Type]) -> Dict[str, Type]:
-    """Return sub-classes of `base_backends` found in sub-modules of `packages`.
+def get_backends(
+    backends: EntryPoints, base_backends: Tuple[type, ...]
+) -> Dict[str, type]:
+    """Return sub-classes of `base_backends` from `backends`.
 
     Args:
-        packages (tuple of str): A tuple of dotted package names.
-            Ex.: ("ralph.backends.data", "ralph.backends.lrs").
-        base_backends (tuple of type): A tuple of base backend classes to search for.
+        backends (EntryPoints): EntryPoints pointing to backend classes.
+            Ex.: [EntryPoint(name="backend_name", value="foo.bar:BackendA"].
+        base_backends (tuple of type): A tuple of base backend classes to filter for.
             Ex.: ("BaseDataBackend",)
 
     Return:
-        dict: A dictionary of found non-abstract backend classes by their name property.
+        dict: A dictionary of backend classes by their `EntryPoint.name` property.
             Ex.: {"fs": FSDataBackend}
     """
-    module_specs = []
-    for package in packages:
-        try:
-            module_spec = find_spec(package)
-        except ModuleNotFoundError:
-            module_spec = None
-
-        if not module_spec:
-            logger.warning("Could not find '%s' package; skipping it", package)
-            continue
-
-        module_specs.append(module_spec)
-
-    modules = []
-    for module_spec in module_specs:
-        paths = module_spec.submodule_search_locations
-        for module_info in pkgutil.iter_modules(paths, prefix=f"{module_spec.name}."):
-            modules.append(module_info.name)
-
-    backend_classes = set()
-    for module in modules:
+    backend_classes = {}
+    for backend in sorted(backends, key=lambda x: x.name, reverse=True):
         try:
-            backend_module = import_module(module)
+            backend_class = backend.load()
         except Exception as error:  # noqa: BLE001
-            logger.debug("Failed to import %s module: %s", module, error)
+            logger.debug(
+                "Failed to import '%s' backend from '%s': %s",
+                backend.name,
+                backend.value,
+                error,
+            )
             continue
-        for _, class_ in getmembers(backend_module, isclass):
-            if issubclass(class_, base_backends) and not isabstract(class_):
-                backend_classes.add(class_)
 
-    return {
-        backend.name: backend
-        for backend in sorted(backend_classes, key=lambda x: x.name, reverse=True)
-    }
+        if issubclass(backend_class, base_backends):
+            backend_classes[backend.name] = backend_class
+
+    return backend_classes
 
 
 @lru_cache(maxsize=1)
-def get_cli_backends() -> Dict[str, Type]:
+def get_cli_backends() -> Dict[str, type]:
     """Return Ralph's backend classes for cli usage."""
     base_backends = (BaseAsyncDataBackend, BaseDataBackend)
-    return get_backends(("ralph.backends.data",), base_backends)
+    data_backends = entry_points(group="ralph.backends.data")
+    return get_backends(data_backends, base_backends)
 
 
 @lru_cache(maxsize=1)
-def get_cli_write_backends() -> Dict[str, Type]:
+def get_cli_write_backends() -> Dict[str, type]:
     """Return Ralph's backends classes for cli write usage."""
     return {
         name: backend
         for name, backend in get_cli_backends().items()
         if issubclass(backend, (Writable, AsyncWritable))
     }
 
 
 @lru_cache(maxsize=1)
-def get_cli_list_backends() -> Dict[str, Type]:
+def get_cli_list_backends() -> Dict[str, type]:
     """Return Ralph's backends classes for cli list usage."""
     return {
         name: backend
         for name, backend in get_cli_backends().items()
         if issubclass(backend, (Listable, AsyncListable))
     }
 
 
 @lru_cache(maxsize=1)
-def get_lrs_backends() -> Dict[str, Type]:
+def get_lrs_backends() -> Dict[str, type]:
     """Return Ralph's backend classes for LRS usage."""
-    return get_backends(("ralph.backends.lrs",), (BaseAsyncLRSBackend, BaseLRSBackend))
+    lrs_backends = entry_points(group="ralph.backends.lrs")
+    return get_backends(lrs_backends, (BaseAsyncLRSBackend, BaseLRSBackend))
```

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/async_es.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/async_es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/async_mongo.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/async_mongo.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/base.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/clickhouse.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,14 @@
         self._add_agent_filters(ch_params, where, params.authority, "authority")
         ch_params.pop("authority", None)
 
         if params.verb:
             where.append("JSONExtractString(event, 'verb', 'id') = {verb:String}")
 
         if params.activity:
-            where.append(
-                "JSONExtractString(event, 'object', 'objectType') = 'Activity'"
-            )
             where.append("JSONExtractString(event, 'object', 'id') = {activity:String}")
 
         if params.since:
             where.append("emission_time > {since:DateTime64(6)}")
 
         if params.until:
             where.append("emission_time <= {until:DateTime64(6)}")
```

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/es.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/es.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         ESLRSBackend._add_agent_filters(es_query_filters, params.authority, "authority")
 
         if params.verb:
             es_query_filters += [{"term": {"verb.id.keyword": params.verb}}]
 
         if params.activity:
             es_query_filters += [
-                {"term": {"object.objectType.keyword": "Activity"}},
                 {"term": {"object.id.keyword": params.activity}},
             ]
 
         if params.since:
             es_query_filters += [{"range": {"timestamp": {"gt": params.since}}}]
 
         if params.until:
```

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/fs.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/backends/lrs/mongo.py` & `ralph-malph-4.2.0/src/ralph/backends/lrs/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 
         if params.verb:
             mongo_query_filters.update({"_source.verb.id": params.verb})
 
         if params.activity:
             mongo_query_filters.update(
                 {
-                    "_source.object.objectType": "Activity",
                     "_source.object.id": params.activity,
                 },
             )
 
         if params.since:
             mongo_query_filters.update({"_source.timestamp": {"$gt": params.since}})
```

### Comparing `ralph-malph-4.1.0/src/ralph/cli.py` & `ralph-malph-4.2.0/src/ralph/cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/conf.py` & `ralph-malph-4.2.0/src/ralph/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 """Configurations for Ralph."""
 
 import io
-import sys
 from enum import Enum
 from pathlib import Path
 from typing import List, Sequence, Tuple, Union
 
 from pydantic import AnyHttpUrl, AnyUrl, BaseModel, BaseSettings, Extra, root_validator
 
 from ralph.exceptions import ConfigurationException
-
-from .utils import import_string
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+from ralph.utils import import_string
 
 try:
     from click import get_app_dir
 except ImportError:
     # If we use Ralph as a library and Click is not installed, we consider the
     # application directory to be the current directory. For non-CLI usage, it
     # has no consequences.
@@ -218,17 +211,15 @@
             },
         },
     }
     PARSERS: ParserSettings = ParserSettings()
     RUNSERVER_AUTH_BACKENDS: AuthBackends = AuthBackends([AuthBackend.BASIC])
     RUNSERVER_AUTH_OIDC_AUDIENCE: str = None
     RUNSERVER_AUTH_OIDC_ISSUER_URI: AnyHttpUrl = None
-    RUNSERVER_BACKEND: Literal[
-        "async_es", "async_mongo", "clickhouse", "es", "fs", "mongo"
-    ] = "es"
+    RUNSERVER_BACKEND: str = "es"
     RUNSERVER_HOST: str = "0.0.0.0"  # noqa: S104
     RUNSERVER_MAX_SEARCH_HITS_COUNT: int = 100
     RUNSERVER_POINT_IN_TIME_KEEP_ALIVE: str = "1m"
     RUNSERVER_PORT: int = 8100
     LRS_RESTRICT_BY_AUTHORITY: bool = False
     LRS_RESTRICT_BY_SCOPES: bool = False
     SENTRY_CLI_TRACES_SAMPLE_RATE: float = 1.0
```

### Comparing `ralph-malph-4.1.0/src/ralph/exceptions.py` & `ralph-malph-4.2.0/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/filters.py` & `ralph-malph-4.2.0/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/converter.py` & `ralph-malph-4.2.0/src/ralph/models/converter.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/base.py` & `ralph-malph-4.2.0/src/ralph/models/edx/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/browser.py` & `ralph-malph-4.2.0/src/ralph/models/edx/browser.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/enrollment.py` & `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/enrollment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Enrollment event xAPI Converter."""
+
 from typing import Set
 
 from ralph.models.converter import ConversionItem
 from ralph.models.edx.enrollment.statements import (
     EdxCourseEnrollmentActivated,
     EdxCourseEnrollmentDeactivated,
 )
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Navigational event xAPI Converter."""
+
 from typing import Set
 
 from ralph.models.converter import ConversionItem
 from ralph.models.edx.navigational.statements import UIPageClose
 from ralph.models.xapi.navigation.statements import PageTerminated
 
 from .base import BaseXapiConverter
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Video event xAPI Converter."""
+
 from typing import Set
 
 from ralph.models.converter import ConversionItem
 from ralph.models.edx.video.statements import (
     UILoadVideo,
     UIPauseVideo,
     UIPlayVideo,
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/enrollment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/navigational/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/open_response_assessment/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/peer_instruction/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/server.py` & `ralph-malph-4.2.0/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-4.2.0/src/ralph/models/edx/video/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/edx/video/statements.py` & `ralph-malph-4.2.0/src/ralph/models/edx/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/selector.py` & `ralph-malph-4.2.0/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/validator.py` & `ralph-malph-4.2.0/src/ralph/models/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Event validator definition."""
 
-
 import json
 import logging
 from typing import Any, Generator, Optional, TextIO
 
 from pydantic import ValidationError
 
 from ralph.exceptions import BadFormatException, UnknownEventException
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/__init__.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/agents.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/agents.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/attachments.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/attachments.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/common.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/common.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/contexts.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/groups.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/groups.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/ifi.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/ifi.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/objects.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/results.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/statements.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/base/unnested_objects.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/base/unnested_objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     """Pydantic model for message `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `https://w3id.org/xapi/acrossx/activities/message`.
     """
 
-    type: Literal[
+    type: Literal["https://w3id.org/xapi/acrossx/activities/message"] = (
         "https://w3id.org/xapi/acrossx/activities/message"
-    ] = "https://w3id.org/xapi/acrossx/activities/message"
+    )
 
 
 class MessageActivity(BaseXapiActivity):
     """Pydantic model for message `Activity` type.
 
     Attributes:
         definition (dict): see MessageActivityDefinition.
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 class PageActivityDefinition(BaseXapiActivityDefinition):
     """Pydantic model for page `Activity` type `definition` property.
 
     Attributes:
        type (str): Consists of the value `http://activitystrea.ms/schema/1.0/page`.
     """
 
-    type: Literal[
+    type: Literal["http://activitystrea.ms/schema/1.0/page"] = (
         "http://activitystrea.ms/schema/1.0/page"
-    ] = "http://activitystrea.ms/schema/1.0/page"
+    )
 
 
 class PageActivity(BaseXapiActivity):
     """Pydantic model for page `Activity` type.
 
     Attributes:
         definition (dict): See PageActivityDefinition.
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/audio.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/audio.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     """Pydantic model for CMI Interaction `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `http://adlnet.gov/expapi/activities/cmi.interaction`.
     """
 
-    type: Literal[
+    type: Literal["http://adlnet.gov/expapi/activities/cmi.interaction"] = (
         "http://adlnet.gov/expapi/activities/cmi.interaction"
-    ] = "http://adlnet.gov/expapi/activities/cmi.interaction"
+    )
 
 
 class CMIInteractionActivity(BaseXapiActivity):
     """Pydantic model for CMI Interaction `Activity` type.
 
     Attributes:
         definition (dict): see CMIInteractionActivityDefinition.
@@ -43,17 +43,17 @@
     """Pydantic model for profile `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `http://adlnet.gov/expapi/activities/profile`.
     """
 
-    type: Literal[
+    type: Literal["http://adlnet.gov/expapi/activities/profile"] = (
         "http://adlnet.gov/expapi/activities/profile"
-    ] = "http://adlnet.gov/expapi/activities/profile"
+    )
 
 
 class ProfileActivity(BaseXapiActivity):
     """Pydantic model for profile `Activity` type.
 
     Attributes:
         definition (dict): see ProfileActivityDefinition.
@@ -69,17 +69,17 @@
     """Pydantic model for course `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `http://adlnet.gov/expapi/activities/course`.
     """
 
-    type: Literal[
+    type: Literal["http://adlnet.gov/expapi/activities/course"] = (
         "http://adlnet.gov/expapi/activities/course"
-    ] = "http://adlnet.gov/expapi/activities/course"
+    )
 
 
 class CourseActivity(BaseXapiActivity):
     """Pydantic model for course `Activity` type.
 
     Attributes:
         definition (dict): see CourseActivityDefinition.
@@ -95,17 +95,17 @@
     """Pydantic model for module `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `http://adlnet.gov/expapi/activities/module`.
     """
 
-    type: Literal[
+    type: Literal["http://adlnet.gov/expapi/activities/module"] = (
         "http://adlnet.gov/expapi/activities/module"
-    ] = "http://adlnet.gov/expapi/activities/module"
+    )
 
 
 class ModuleActivity(BaseXapiActivity):
     """Pydantic model for module `Activity` type.
 
     Attributes:
         definition (dict): see ModuleActivityDefinition.
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/video.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/video.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     """Pydantic model for video `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `https://w3id.org/xapi/video/activity-type/video`.
     """
 
-    type: Literal[
+    type: Literal["https://w3id.org/xapi/video/activity-type/video"] = (
         "https://w3id.org/xapi/video/activity-type/video"
-    ] = "https://w3id.org/xapi/video/activity-type/video"
+    )
 
 
 class VideoActivity(BaseXapiActivity):
     """Pydantic model for video `Activity` type.
 
     Attributes:
         definition (dict): See VideoActivityDefinition.
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/constants/video.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     """Pydantic model for posted `verb`.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/acrossx/verbs/posted`.
         display (dict): Consists of the dictionary `{"en-US": "posted"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/acrossx/verbs/posted"] = (
         "https://w3id.org/xapi/acrossx/verbs/posted"
-    ] = "https://w3id.org/xapi/acrossx/verbs/posted"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["posted"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,39 +16,39 @@
     """Pydantic model for asked `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/asked`.
         display (dict): Consists of the dictionary `{"en-US": "asked"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/asked"] = (
         "http://adlnet.gov/expapi/verbs/asked"
-    ] = "http://adlnet.gov/expapi/verbs/asked"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["asked"]]]
 
 
 class AnsweredVerb(BaseXapiVerb):
     """Pydantic model for answered `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/answered`.
         display (dict): Consists of the dictionary `{"en-US": "answered"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/answered"] = (
         "http://adlnet.gov/expapi/verbs/answered"
-    ] = "http://adlnet.gov/expapi/verbs/answered"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["answered"]]]
 
 
 class RegisteredVerb(BaseXapiVerb):
     """Pydantic model for registered `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/registered`.
         display (dict): Consists of the dictionary `{"en-US": "registered"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/registered"] = (
         "http://adlnet.gov/expapi/verbs/registered"
-    ] = "http://adlnet.gov/expapi/verbs/registered"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["registered"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     """Pydantic model for accessed `verb`.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/netc/verbs/accessed`.
         display (dict): Consists of the dictionary `{"en-US": "accessed"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/netc/verbs/accessed"] = (
         "https://w3id.org/xapi/netc/verbs/accessed"
-    ] = "https://w3id.org/xapi/netc/verbs/accessed"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["accessed"]]]
 
 
 class UploadedVerb(BaseXapiVerb):
     """Pydantic model for uploaded `verb`.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/netc/verbs/uploaded`.
         display (dict): Consists of the dictionary `{"en-US": "uploaded"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/netc/verbs/uploaded"] = (
         "https://w3id.org/xapi/netc/verbs/uploaded"
-    ] = "https://w3id.org/xapi/netc/verbs/uploaded"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["uploaded"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,53 +16,53 @@
     """Pydantic model for completed `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/completed`.
         display (dict): Consists of the dictionary `{"en-US": "completed"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/completed"] = (
         "http://adlnet.gov/expapi/verbs/completed"
-    ] = "http://adlnet.gov/expapi/verbs/completed"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["completed"]]]
 
 
 class InitializedVerb(BaseXapiVerb):
     """Pydantic model for initialized `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/initialized`.
         display (Dict): Consists of the dictionary `{"en-US": "initialized"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/initialized"] = (
         "http://adlnet.gov/expapi/verbs/initialized"
-    ] = "http://adlnet.gov/expapi/verbs/initialized"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["initialized"]]]
 
 
 class InteractedVerb(BaseXapiVerb):
     """Pydantic model for interacted `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/interacted`.
         display (dict): Consists of the dictionary `{"en-US": "interacted"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/interacted"] = (
         "http://adlnet.gov/expapi/verbs/interacted"
-    ] = "http://adlnet.gov/expapi/verbs/interacted"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["interacted"]]]
 
 
 class TerminatedVerb(BaseXapiVerb):
     """Pydantic model for terminated `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/terminated`.
         display (dict): Consists of the dictionary `{"en-US": "terminated"}`.
     """
 
-    id: Literal[
+    id: Literal["http://adlnet.gov/expapi/verbs/terminated"] = (
         "http://adlnet.gov/expapi/verbs/terminated"
-    ] = "http://adlnet.gov/expapi/verbs/terminated"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["terminated"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,39 +16,39 @@
     """Pydantic model for viewed `verb`.
 
     Attributes:
         id (str): Consists of the value `http://id.tincanapi.com/verb/viewed`.
         display (dict): Consists of the dictionary `{"en-US": "viewed"}`.
     """
 
-    id: Literal[
+    id: Literal["http://id.tincanapi.com/verb/viewed"] = (
         "http://id.tincanapi.com/verb/viewed"
-    ] = "http://id.tincanapi.com/verb/viewed"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["viewed"]]]
 
 
 class DownloadedVerb(BaseXapiVerb):
     """Pydantic model for downloaded `verb`.
 
     Attributes:
         id (str): Consists of the value `http://id.tincanapi.com/verb/downloaded`.
         display (dict): Consists of the dictionary `{"en-US": "downloaded"}`.
     """
 
-    id: Literal[
+    id: Literal["http://id.tincanapi.com/verb/downloaded"] = (
         "http://id.tincanapi.com/verb/downloaded"
-    ] = "http://id.tincanapi.com/verb/downloaded"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["downloaded"]]]
 
 
 class UnregisteredVerb(BaseXapiVerb):
     """Pydantic model for unregistered `verb`.
 
     Attributes:
         id (str): Consists of the value `http://id.tincanapi.com/verb/unregistered`.
         display (dict): Consists of the dictionary `{"en-US": "unregistered"}`.
     """
 
-    id: Literal[
+    id: Literal["http://id.tincanapi.com/verb/unregistered"] = (
         "http://id.tincanapi.com/verb/unregistered"
-    ] = "http://id.tincanapi.com/verb/unregistered"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unregistered"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/video.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,39 +16,39 @@
     """Pydantic model for played `verb`.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/video/verbs/played`.
         display (dict): Consists of the dictionary `{"en-US": "played"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/video/verbs/played"] = (
         "https://w3id.org/xapi/video/verbs/played"
-    ] = "https://w3id.org/xapi/video/verbs/played"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["played"]]]
 
 
 class PausedVerb(BaseXapiVerb):
     """Pydantic model for paused `verb` field.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/video/verbs/paused`.
         display (dict): Consists of the dictionary `{"en-US": "paused"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/video/verbs/paused"] = (
         "https://w3id.org/xapi/video/verbs/paused"
-    ] = "https://w3id.org/xapi/video/verbs/paused"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["paused"]]]
 
 
 class SeekedVerb(BaseXapiVerb):
     """Pydantic model for seeked `verb` field.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/video/verbs/seeked`.
         display (dict): Consists of the dictionary `{"en-US": "seeked"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/video/verbs/seeked"] = (
         "https://w3id.org/xapi/video/verbs/seeked"
-    ] = "https://w3id.org/xapi/video/verbs/seeked"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["seeked"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,116 +17,116 @@
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/muted`.
         display (dict): Consists of the dictionary `{"en-US": "muted"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/muted"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/muted"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/muted"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["muted"]]]
 
 
 class UnmutedVerb(BaseXapiVerb):
     """Pydantic model for unmuted `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/unmuted`.
         display (dict): Consists of the dictionary `{"en-US": "unmuted"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/unmuted"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/unmuted"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/unmuted"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unmuted"]]]
 
 
 class StartedCameraVerb(BaseXapiVerb):
     """Pydantic model for started camera `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/started-camera`.
         display (dict): Consists of the dictionary `{"en-US": "started camera"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/started-camera"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/started-camera"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/started-camera"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["started camera"]]]
 
 
 class StoppedCameraVerb(BaseXapiVerb):
     """Pydantic model for stopped camera `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera`.
         display (dict): Consists of the dictionary `{"en-US": "stopped camera"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["stopped camera"]]]
 
 
 class SharedScreenVerb(BaseXapiVerb):
     """Pydantic model for shared screen `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/shared-screen`.
         display (dict): Consists of the dictionary `{"en-US": "shared screen"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/shared-screen"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/shared-screen"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/shared-screen"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["shared screen"]]]
 
 
 class UnsharedScreenVerb(BaseXapiVerb):
     """Pydantic model for unshared screen `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen`.
         display (dict): Consists of the dictionary `{"en-US": "unshared screen"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unshared screen"]]]
 
 
 class RaisedHandVerb(BaseXapiVerb):
     """Pydantic model for raised hand `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/raised-hand`.
         display (dict): Consists of the dictionary `{"en-US": "raised hand"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/raised-hand"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/raised-hand"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/raised-hand"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["raised hand"]]]
 
 
 class LoweredHandVerb(BaseXapiVerb):
     """Pydantic model for lowered hand `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand`.
         display (dict): Consists of the dictionary `{"en-US": "lowered hand"}`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand"
-    ] = "https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand"
+    )
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["lowered hand"]]]
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/lms/contexts.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/lms/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/lms/objects.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/lms/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/lms/statements.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/lms/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/navigation/statements.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/navigation/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/video/contexts.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/video/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/video/results.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/video/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/video/statements.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/contexts.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 class VirtualClassroomProfileActivity(ProfileActivity):
     """Pydantic model for virtual classroom profile `Activity` type.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/virtual-classroom`.
     """
 
-    id: Literal[
+    id: Literal["https://w3id.org/xapi/virtual-classroom"] = (
         "https://w3id.org/xapi/virtual-classroom"
-    ] = "https://w3id.org/xapi/virtual-classroom"
+    )
 
 
 class VirtualClassroomContextContextActivities(BaseXapiContextContextActivities):
     """Pydantic model for virtual classroom `context`.`contextActivities` property.
 
     Attributes:
         category (dict or list): see VirtualClassroomProfileActivity.
```

### Comparing `ralph-malph-4.1.0/src/ralph/models/xapi/virtual_classroom/statements.py` & `ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/parsers.py` & `ralph-malph-4.2.0/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph/utils.py` & `ralph-malph-4.2.0/src/ralph/utils.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-4.2.0/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 4.1.0
+Version: 4.2.0
 Summary: Ralph, the ultimate Learning Record Store (and more!) for your learning analytics.
 Author-email: "Open FUN (France Université Numérique)" <fun.dev@fun-mooc.fr>
 License: MIT License
         
         Copyright (c) 2020-present France Université Numérique
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: importlib-metadata<8.0,>=7.0.1
 Requires-Dist: langcodes>=3.2.0
 Requires-Dist: pydantic[dotenv,email]<2.0,>=1.10.0
 Requires-Dist: rfc3987>=1.3.0
 Provides-Extra: backend-clickhouse
 Requires-Dist: clickhouse-connect[numpy,pandas]<0.6; extra == "backend-clickhouse"
 Requires-Dist: python-dateutil>=2.8.2; extra == "backend-clickhouse"
 Provides-Extra: backend-es
@@ -68,56 +69,55 @@
 Requires-Dist: python-keystoneclient>=5.0.0; extra == "backend-swift"
 Requires-Dist: python-swiftclient>=4.0.0; extra == "backend-swift"
 Provides-Extra: backend-ws
 Requires-Dist: websockets>=10.3; extra == "backend-ws"
 Provides-Extra: backends
 Requires-Dist: ralph-malph[backend-clickhouse,backend-es,backend-ldp,backend-lrs,backend-mongo,backend-s3,backend-swift]; extra == "backends"
 Provides-Extra: ci
-Requires-Dist: twine==4.0.2; extra == "ci"
+Requires-Dist: twine==5.0.0; extra == "ci"
 Provides-Extra: cli
 Requires-Dist: bcrypt>=4.0.0; extra == "cli"
 Requires-Dist: click>=8.1.0; extra == "cli"
 Requires-Dist: click-option-group>=0.5.0; extra == "cli"
 Requires-Dist: sentry-sdk[fastapi]>=1.9.0; extra == "cli"
 Provides-Extra: dev
-Requires-Dist: anyio<4.2.1; extra == "dev"
-Requires-Dist: black==23.12.1; extra == "dev"
-Requires-Dist: cryptography==41.0.7; extra == "dev"
+Requires-Dist: anyio<4.3.1; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: factory-boy==3.3.0; extra == "dev"
 Requires-Dist: hypothesis<6.92.0; extra == "dev"
-Requires-Dist: logging-gelf==0.0.31; extra == "dev"
+Requires-Dist: logging-gelf==0.0.32; extra == "dev"
 Requires-Dist: mike==2.0.0; extra == "dev"
 Requires-Dist: mkdocs==1.5.3; extra == "dev"
 Requires-Dist: mkdocs-click==0.8.1; extra == "dev"
-Requires-Dist: mkdocs-material==9.5.3; extra == "dev"
-Requires-Dist: mkdocstrings[python-legacy]==0.24.0; extra == "dev"
-Requires-Dist: moto==4.2.13; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
-Requires-Dist: neoteroi-mkdocs==1.0.4; extra == "dev"
-Requires-Dist: pyfakefs==5.3.2; extra == "dev"
-Requires-Dist: pymdown-extensions==10.7; extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.3; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: mkdocs-material==9.5.17; extra == "dev"
+Requires-Dist: mkdocstrings[python-legacy]==0.24.3; extra == "dev"
+Requires-Dist: moto==5.0.5; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: neoteroi-mkdocs==1.0.5; extra == "dev"
+Requires-Dist: pyfakefs==5.4.0; extra == "dev"
+Requires-Dist: pymdown-extensions==10.7.1; extra == "dev"
+Requires-Dist: pytest<8.0.0; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-httpx<0.23.0; extra == "dev"
-Requires-Dist: requests-mock==1.11.0; extra == "dev"
+Requires-Dist: requests-mock==1.12.1; extra == "dev"
 Requires-Dist: responses==0.24.1; extra == "dev"
-Requires-Dist: ruff==0.1.11; extra == "dev"
-Requires-Dist: types-python-dateutil==2.8.19.20240106; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
+Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == "dev"
 Requires-Dist: types-python-jose==3.3.4.20240106; extra == "dev"
-Requires-Dist: types-requests<2.31.0.20240107; extra == "dev"
+Requires-Dist: types-requests<2.31.0.20240407; extra == "dev"
 Requires-Dist: types-cachetools==5.3.0.7; extra == "dev"
 Provides-Extra: lrs
 Requires-Dist: bcrypt==4.1.2; extra == "lrs"
-Requires-Dist: fastapi==0.108.0; extra == "lrs"
-Requires-Dist: cachetools==5.3.2; extra == "lrs"
+Requires-Dist: fastapi==0.110.1; extra == "lrs"
+Requires-Dist: cachetools==5.3.3; extra == "lrs"
 Requires-Dist: httpx<0.25.0; extra == "lrs"
-Requires-Dist: sentry_sdk==1.39.1; extra == "lrs"
+Requires-Dist: sentry_sdk==1.44.1; extra == "lrs"
 Requires-Dist: python-jose==3.3.0; extra == "lrs"
-Requires-Dist: uvicorn[standard]==0.25.0; extra == "lrs"
+Requires-Dist: uvicorn[standard]==0.29.0; extra == "lrs"
 Provides-Extra: full
 Requires-Dist: ralph-malph[backends,cli,lrs]; extra == "full"
 
 
 <p align="center">
   <a href="https://openfun.github.io/ralph"><img src="https://raw.githubusercontent.com/openfun/logos/main/ralph/ralph-color-dark.png" alt="Ralph logo" width="400"></a>
 </p>
```

### Comparing `ralph-malph-4.1.0/src/ralph_malph.egg-info/SOURCES.txt` & `ralph-malph-4.2.0/src/ralph_malph.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -51,42 +51,82 @@
 src/ralph/models/converter.py
 src/ralph/models/selector.py
 src/ralph/models/validator.py
 src/ralph/models/edx/__init__.py
 src/ralph/models/edx/base.py
 src/ralph/models/edx/browser.py
 src/ralph/models/edx/server.py
+src/ralph/models/edx/bookmark/__init__.py
+src/ralph/models/edx/bookmark/statements.py
+src/ralph/models/edx/bookmark/fields/__init__.py
+src/ralph/models/edx/bookmark/fields/events.py
+src/ralph/models/edx/certificate/__init__.py
+src/ralph/models/edx/certificate/statements.py
+src/ralph/models/edx/certificate/fields/__init__.py
+src/ralph/models/edx/certificate/fields/events.py
+src/ralph/models/edx/cohort/__init__.py
+src/ralph/models/edx/cohort/statements.py
+src/ralph/models/edx/cohort/fields/__init__.py
+src/ralph/models/edx/cohort/fields/events.py
+src/ralph/models/edx/content_library_interaction/__init__.py
+src/ralph/models/edx/content_library_interaction/statements.py
+src/ralph/models/edx/content_library_interaction/fields/__init__.py
+src/ralph/models/edx/content_library_interaction/fields/events.py
 src/ralph/models/edx/converters/__init__.py
 src/ralph/models/edx/converters/xapi/__init__.py
 src/ralph/models/edx/converters/xapi/base.py
 src/ralph/models/edx/converters/xapi/enrollment.py
 src/ralph/models/edx/converters/xapi/navigational.py
 src/ralph/models/edx/converters/xapi/server.py
 src/ralph/models/edx/converters/xapi/video.py
+src/ralph/models/edx/course_content_completion/__init__.py
+src/ralph/models/edx/course_content_completion/statements.py
+src/ralph/models/edx/course_content_completion/fields/__init__.py
+src/ralph/models/edx/course_content_completion/fields/events.py
+src/ralph/models/edx/drag_and_drop/__init__.py
+src/ralph/models/edx/drag_and_drop/statements.py
+src/ralph/models/edx/drag_and_drop/fields/__init__.py
+src/ralph/models/edx/drag_and_drop/fields/events.py
 src/ralph/models/edx/enrollment/__init__.py
 src/ralph/models/edx/enrollment/statements.py
 src/ralph/models/edx/enrollment/fields/__init__.py
 src/ralph/models/edx/enrollment/fields/contexts.py
 src/ralph/models/edx/enrollment/fields/events.py
 src/ralph/models/edx/navigational/__init__.py
 src/ralph/models/edx/navigational/statements.py
 src/ralph/models/edx/navigational/fields/__init__.py
 src/ralph/models/edx/navigational/fields/events.py
+src/ralph/models/edx/notes/__init__.py
+src/ralph/models/edx/notes/statements.py
+src/ralph/models/edx/notes/fields/__init__.py
+src/ralph/models/edx/notes/fields/events.py
 src/ralph/models/edx/open_response_assessment/__init__.py
 src/ralph/models/edx/open_response_assessment/statements.py
 src/ralph/models/edx/open_response_assessment/fields/__init__.py
 src/ralph/models/edx/open_response_assessment/fields/events.py
 src/ralph/models/edx/peer_instruction/__init__.py
 src/ralph/models/edx/peer_instruction/statements.py
 src/ralph/models/edx/peer_instruction/fields/__init__.py
 src/ralph/models/edx/peer_instruction/fields/events.py
+src/ralph/models/edx/poll/__init__.py
+src/ralph/models/edx/poll/statements.py
+src/ralph/models/edx/poll/fields/__init__.py
+src/ralph/models/edx/poll/fields/events.py
 src/ralph/models/edx/problem_interaction/__init__.py
 src/ralph/models/edx/problem_interaction/statements.py
 src/ralph/models/edx/problem_interaction/fields/__init__.py
 src/ralph/models/edx/problem_interaction/fields/events.py
+src/ralph/models/edx/survey/__init__.py
+src/ralph/models/edx/survey/statements.py
+src/ralph/models/edx/survey/fields/__init__.py
+src/ralph/models/edx/survey/fields/events.py
+src/ralph/models/edx/teams_related/__init__.py
+src/ralph/models/edx/teams_related/statements.py
+src/ralph/models/edx/teams_related/fields/__init__.py
+src/ralph/models/edx/teams_related/fields/events.py
 src/ralph/models/edx/textbook_interaction/__init__.py
 src/ralph/models/edx/textbook_interaction/statements.py
 src/ralph/models/edx/textbook_interaction/fields/__init__.py
 src/ralph/models/edx/textbook_interaction/fields/events.py
 src/ralph/models/edx/video/__init__.py
 src/ralph/models/edx/video/statements.py
 src/ralph/models/edx/video/fields/__init__.py
```

### Comparing `ralph-malph-4.1.0/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-4.2.0/src/ralph_malph.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+importlib-metadata<8.0,>=7.0.1
 langcodes>=3.2.0
 pydantic[dotenv,email]<2.0,>=1.10.0
 rfc3987>=1.3.0
 
 [backend-clickhouse]
 clickhouse-connect[numpy,pandas]<0.6
 python-dateutil>=2.8.2
@@ -33,55 +34,54 @@
 [backend-ws]
 websockets>=10.3
 
 [backends]
 ralph-malph[backend-clickhouse,backend-es,backend-ldp,backend-lrs,backend-mongo,backend-s3,backend-swift]
 
 [ci]
-twine==4.0.2
+twine==5.0.0
 
 [cli]
 bcrypt>=4.0.0
 click>=8.1.0
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
-anyio<4.2.1
-black==23.12.1
-cryptography==41.0.7
+anyio<4.3.1
+black==24.3.0
+cryptography==42.0.5
 factory-boy==3.3.0
 hypothesis<6.92.0
-logging-gelf==0.0.31
+logging-gelf==0.0.32
 mike==2.0.0
 mkdocs==1.5.3
 mkdocs-click==0.8.1
-mkdocs-material==9.5.3
-mkdocstrings[python-legacy]==0.24.0
-moto==4.2.13
-mypy==1.8.0
-neoteroi-mkdocs==1.0.4
-pyfakefs==5.3.2
-pymdown-extensions==10.7
-pytest==7.4.4
-pytest-asyncio==0.23.3
-pytest-cov==4.1.0
+mkdocs-material==9.5.17
+mkdocstrings[python-legacy]==0.24.3
+moto==5.0.5
+mypy==1.9.0
+neoteroi-mkdocs==1.0.5
+pyfakefs==5.4.0
+pymdown-extensions==10.7.1
+pytest<8.0.0
+pytest-cov==5.0.0
 pytest-httpx<0.23.0
-requests-mock==1.11.0
+requests-mock==1.12.1
 responses==0.24.1
-ruff==0.1.11
-types-python-dateutil==2.8.19.20240106
+ruff==0.3.5
+types-python-dateutil==2.9.0.20240316
 types-python-jose==3.3.4.20240106
-types-requests<2.31.0.20240107
+types-requests<2.31.0.20240407
 types-cachetools==5.3.0.7
 
 [full]
 ralph-malph[backends,cli,lrs]
 
 [lrs]
 bcrypt==4.1.2
-fastapi==0.108.0
-cachetools==5.3.2
+fastapi==0.110.1
+cachetools==5.3.3
 httpx<0.25.0
-sentry_sdk==1.39.1
+sentry_sdk==1.44.1
 python-jose==3.3.0
-uvicorn[standard]==0.25.0
+uvicorn[standard]==0.29.0
```

### Comparing `ralph-malph-4.1.0/tests/test_cli.py` & `ralph-malph-4.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_cli_usage.py` & `ralph-malph-4.2.0/tests/test_cli_usage.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_conf.py` & `ralph-malph-4.2.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_dependencies.py` & `ralph-malph-4.2.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_filters.py` & `ralph-malph-4.2.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_helpers.py` & `ralph-malph-4.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_logger.py` & `ralph-malph-4.2.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_parsers.py` & `ralph-malph-4.2.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.1.0/tests/test_utils.py` & `ralph-malph-4.2.0/tests/test_utils.py`

 * *Files identical despite different names*

