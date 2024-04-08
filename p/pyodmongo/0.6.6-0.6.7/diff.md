# Comparing `tmp/pyodmongo-0.6.6.tar.gz` & `tmp/pyodmongo-0.6.7.tar.gz`

## Comparing `pyodmongo-0.6.6.tar` & `pyodmongo-0.6.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/coverage.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyproject.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    36227 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/delete.md
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/fastapi.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/find.md
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/getting_started.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/indexes.md
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/version.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_db_index.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_queries.py
--rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/tests/test_version.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/coverage.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyproject.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    36227 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/delete.md
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/find.md
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/getting_started.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/indexes.md
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/version.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_db_index.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_queries.py
+-rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_version.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/PKG-INFO
```

### Comparing `pyodmongo-0.6.6/code_of_conduct.md` & `pyodmongo-0.6.7/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/mkdocs.yml` & `pyodmongo-0.6.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyproject.py` & `pyodmongo-0.6.7/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/requirements.txt` & `pyodmongo-0.6.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.6.7/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/.github/workflows/black_formatter.yml` & `pyodmongo-0.6.7/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.6.7/.github/workflows/publishing_docs_s3.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/.github/workflows/python_publish.yml` & `pyodmongo-0.6.7/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/.github/workflows/tests.yml` & `pyodmongo-0.6.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/assets/images/favicon.png` & `pyodmongo-0.6.7/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/assets/images/insomnia_request.png` & `pyodmongo-0.6.7/docs/assets/images/insomnia_request.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/assets/images/logo.png` & `pyodmongo-0.6.7/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/aggregation.md` & `pyodmongo-0.6.7/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/contributing.md` & `pyodmongo-0.6.7/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/db_model.md` & `pyodmongo-0.6.7/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/delete.md` & `pyodmongo-0.6.7/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/fastapi.md` & `pyodmongo-0.6.7/docs/en/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/find.md` & `pyodmongo-0.6.7/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/getting_started.md` & `pyodmongo-0.6.7/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/index.md` & `pyodmongo-0.6.7/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/indexes.md` & `pyodmongo-0.6.7/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/query.md` & `pyodmongo-0.6.7/docs/en/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/en/save.md` & `pyodmongo-0.6.7/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/aggregation.md` & `pyodmongo-0.6.7/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/contributing.md` & `pyodmongo-0.6.7/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/db_model.md` & `pyodmongo-0.6.7/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/delete.md` & `pyodmongo-0.6.7/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/fastapi.md` & `pyodmongo-0.6.7/docs/pt-BR/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/find.md` & `pyodmongo-0.6.7/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/getting_started.md` & `pyodmongo-0.6.7/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/index.md` & `pyodmongo-0.6.7/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/indexes.md` & `pyodmongo-0.6.7/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/query.md` & `pyodmongo-0.6.7/docs/pt-BR/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/docs/pt-BR/save.md` & `pyodmongo-0.6.7/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/async_engine/engine.py` & `pyodmongo-0.6.7/pyodmongo/async_engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/engine/engine.py` & `pyodmongo-0.6.7/pyodmongo/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/engine/utils.py` & `pyodmongo-0.6.7/pyodmongo/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/models/fields.py` & `pyodmongo-0.6.7/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/models/id_model.py` & `pyodmongo-0.6.7/pyodmongo/models/id_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/queries/comparison_operators.py` & `pyodmongo-0.6.7/pyodmongo/queries/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/queries/logical_operators.py` & `pyodmongo-0.6.7/pyodmongo/queries/logical_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/queries/query_string.py` & `pyodmongo-0.6.7/pyodmongo/queries/query_string.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/services/aggregate_stages.py` & `pyodmongo-0.6.7/pyodmongo/services/aggregate_stages.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/services/model_init.py` & `pyodmongo-0.6.7/pyodmongo/services/model_init.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyodmongo/services/query_operators.py` & `pyodmongo-0.6.7/pyodmongo/services/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_async_aggregate.py` & `pyodmongo-0.6.7/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_async_crud_db.py` & `pyodmongo-0.6.7/tests/test_async_crud_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     DeleteResponse,
     ResponsePaginate,
     Id,
     Field,
 )
 from pyodmongo.queries import eq, gte, gt, mount_query_filter
 from pyodmongo.engine.utils import consolidate_dict
-from pydantic import ConfigDict
+from pydantic import ConfigDict, BaseModel
 from typing import ClassVar
 from bson import ObjectId
 from datetime import datetime
 import pytest
 import pytest_asyncio
 
 mongo_uri = "mongodb://localhost:27017"
@@ -444,38 +444,77 @@
 class ClassB(DbModel):
     attr_3: str = "A String 3"
     a: ClassA | Id
     _collection: ClassVar = "col_b"
 
 
 @pytest_asyncio.fixture()
-async def drop_collections():
+async def drop_collections_a_b():
     await db._db[ClassA._collection].drop()
     await db._db[ClassB._collection].drop()
     yield
     await db._db[ClassA._collection].drop()
     await db._db[ClassB._collection].drop()
 
 
 @pytest.mark.asyncio
-async def test_find_nested_field_query(drop_collections):
+async def test_find_nested_field_query(drop_collections_a_b):
     obj_a = ClassA()
     await db.save(obj=obj_a)
     obj_b = ClassB(a=obj_a)
     await db.save(obj=obj_b)
     query = eq(ClassB.a, obj_a.id)
     result = await db.find_many(Model=ClassB, query=query, populate=True)
     assert result == [obj_b]
 
 
 @pytest.mark.asyncio
-async def test_find_nested_field_mount_query(drop_collections):
+async def test_find_nested_field_mount_query(drop_collections_a_b):
     obj_a = ClassA()
     await db.save(obj=obj_a)
     obj_b = ClassB(a=obj_a)
     await db.save(obj=obj_b)
     input_dict = {"a": obj_a.id}
     query = mount_query_filter(
         Model=ClassB, items=input_dict, initial_comparison_operators=[]
     )
     result = await db.find_many(Model=ClassB, query=query, populate=True)
     assert result == [obj_b]
+
+
+class ClassOne(DbModel):
+    attr_1: str = "attr 1"
+    _collection: ClassVar = "class_one"
+
+
+class ClassTwoA(BaseModel):
+    attr_2_a: str = "attr 2 A"
+    class_one: list[ClassOne | Id] | None = []
+
+
+class ClassTwoB(BaseModel):
+    attr_2_b: str
+    class_two_a: ClassTwoA | None
+
+
+class ClassThree(DbModel):
+    attr_3: str = "attr 3"
+    class_two: ClassTwoB | None = ClassTwoB(attr_2_b="attr 2 b", class_two_a=None)
+    _collection: ClassVar = "class_three"
+
+
+@pytest_asyncio.fixture()
+async def drop_collections_one_three():
+    await db._db[ClassOne._collection].drop()
+    await db._db[ClassThree._collection].drop()
+    yield
+    await db._db[ClassOne._collection].drop()
+    await db._db[ClassThree._collection].drop()
+
+
+@pytest.mark.asyncio
+async def test_nested_none_object(drop_collections_one_three):
+    obj = ClassThree()
+    await db.save(obj=ClassOne())
+    await db.save(obj=obj)
+    obj_found = await db.find_one(Model=ClassThree, populate=True)
+    assert obj_found == obj
```

### Comparing `pyodmongo-0.6.6/tests/test_class.py` & `pyodmongo-0.6.7/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_db_field_info.py` & `pyodmongo-0.6.7/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_db_index.py` & `pyodmongo-0.6.7/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_dict_empty.py` & `pyodmongo-0.6.7/tests/test_dict_empty.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_fastapi.py` & `pyodmongo-0.6.7/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_model_init_functions.py` & `pyodmongo-0.6.7/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_object_id.py` & `pyodmongo-0.6.7/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_project_pipeline.py` & `pyodmongo-0.6.7/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_pydantic_validators.py` & `pyodmongo-0.6.7/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_queries.py` & `pyodmongo-0.6.7/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_reference_pipeline.py` & `pyodmongo-0.6.7/tests/test_reference_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_save_dict.py` & `pyodmongo-0.6.7/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_sync_aggregate.py` & `pyodmongo-0.6.7/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/tests/test_sync_crud_db.py` & `pyodmongo-0.6.7/tests/test_sync_crud_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     obj_1 = MyModel1(attr1="attr_1")
     db.save(obj_1)
     obj_2 = MyModel2(attr2="attr_2", my_model_1=obj_1)
     db.save(obj_2)
 
     obj_found = db.find_one(Model=MyModel2, populate=True)
     assert obj_found == obj_2
-
+    db._db[MyModel1._collection].drop()
     db._db[MyModel2._collection].drop()
 
 
 def test_find_without_populate():
     class MyModel1(DbModel):
         attr1: str
         _collection: ClassVar = "model1"
@@ -306,14 +306,15 @@
     db.save(obj_1)
     obj_2 = MyModel2(attr2="attr_2", my_model_1=obj_1.id)
     db.save(obj_2)
 
     obj_found = db.find_one(Model=MyModel2)
     assert obj_found == obj_2
 
+    db._db[MyModel1._collection].drop()
     db._db[MyModel2._collection].drop()
 
 
 class AsDict1(DbModel):
     attr_1: str
     _collection: ClassVar = "as_dict_1"
```

### Comparing `pyodmongo-0.6.6/.gitignore` & `pyodmongo-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/LICENSE` & `pyodmongo-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/README.md` & `pyodmongo-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.6/pyproject.toml` & `pyodmongo-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.6.6"
+version = "0.6.7"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pyodmongo-0.6.6/PKG-INFO` & `pyodmongo-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.6.6
+Version: 0.6.7
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

