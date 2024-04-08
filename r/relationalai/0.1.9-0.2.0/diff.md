# Comparing `tmp/relationalai-0.1.9.tar.gz` & `tmp/relationalai-0.2.0.tar.gz`

## Comparing `relationalai-0.1.9.tar` & `relationalai-0.2.0.tar`

### file list

```diff
@@ -1,121 +1,360 @@
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 relationalai-0.1.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 relationalai-0.1.9/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.1.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.1.9/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/README.md
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/quickstart.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/README.md
--rw-r--r--   0        0        0     8436 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Aggregates.md
--rw-r--r--   0        0        0     9333 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Context.md
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/ContextSelect.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Instance.md
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/InstanceProperty.md
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Model.md
--rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Producer.md
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Type.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/README.md
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/SF_pagerank.ipynb
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/cdc.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/fraud.py
--rw-r--r--   0        0        0   698999 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/graph.ipynb
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/graph.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/graphlib.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/load_raw.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/or_types.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/requirements.txt
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/simple_recursion.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/snowflake_pagerank.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/solver.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/data/transactions.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/rel/foo.rel
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/rel/solver.rel
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/__init__.py
--rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/emit.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/__init__.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/compiler.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/debugging.py
--rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/dsl.py
--rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/errors.py
--rw-r--r--   0        0        0    26388 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/metagen.py
--rw-r--r--   0        0        0    23175 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    27114 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/rel.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/client.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    26254 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/sqlite.py
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/test.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/graphs/__init__.py
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/graphs/lib.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    21470 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/conftest.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 relationalai-0.1.9/.gitignore
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.1.9/PYPI_README.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 relationalai-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 relationalai-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 relationalai-0.2.0/README.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 relationalai-0.2.0/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.2.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/README.md
+-rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Edges/README.md
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Edges/add.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Edges/extend.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/edges.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/nodes.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Nodes/README.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Nodes/add.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/python/std/graphs/Nodes/extend.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/cdc.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/fraud.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/requirements.txt
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/simple_recursion.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/rel/foo.rel
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.0/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/index.html
+-rw-r--r--   0        0        0   454881 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/package.json
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/app.styl
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/assets/favicon.ico
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Button.styl
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Button.tsx
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Field.stories.tsx
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Field.styl
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Field.tsx
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Modal.stories.tsx
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Modal.styl
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Modal.tsx
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Tooltip.styl
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Tooltip.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.0/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/emit.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/compiler.py
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    44525 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    18690 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    32550 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    50480 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.0/src/relationalai/tools/notes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/README.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/cosine_similarity/query0.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/eigenvector_centrality/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query0.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/infomap/query0.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query0.txt
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query1.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/louvain/query0.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query0.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query1.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/page_rank/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/cosine_similarity.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/eigenvector_centrality.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/indegree.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/infomap.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/jaccard_similarity.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/louvain.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/outdegree.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/page_rank.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.0/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 relationalai-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.0/docs/pypi/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.0/PKG-INFO
```

### Comparing `relationalai-0.1.9/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/.github/workflows/ruff.yml` & `relationalai-0.2.0/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/docs/getting_started.md` & `relationalai-0.2.0/docs/getting_started.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,72 @@
 # Getting Started With RelationalAI
 
 Ready to dive into RelationalAI?
 This document will quickly get you up and running.
 
 ## Install The `relationalai` Python Package
 
-First, install the `relationalai` package with `pip`:
+### Quick Start
+
+To install the `relationalai` package:
+
+```sh
+pip install relationalai
+```
+
+If you use another Python package management solution (such as Conda, Poetry, etc.), use whichever command is appropriate for installing PyPI packages in your environment.
+
+### Full Guide
 
 > [!IMPORTANT]
-> RelationalAI is compatible with Python version 3.11 (recommended) and 3.10.
-> Python 3.12 is currently not supported.
+> RelationalAI is compatible with Python version 3.10, 3.11, and 3.12.
 > Visit [https://www.python.org/downloads/](https://www.python.org/downloads/)
 > to download a compatible version of Python.
 
 ```sh
 # Check your Python version.
-python3 --version
+python --version
+```
 
-# If the above command fails or displays a version other than 3.10 or 3.11,
-# you will need to install a compatible version of Python. You may need to use
-# the `python3.10` or `python3.11` command instead of the `python3` command.
-# If one of those two commands works, use it instead of `python3` in subsequent steps.
+If the above command fails or displays a version other than 3.10, 3.11, or 3.12,
+you will need to install a compatible version of Python. You may need to use
+a command like `python3` or `python3.10` or `python3.11` or `python3.12`
+instead of the `python3` command. If one of those two commands works, use it
+instead of `python3` in subsequent steps.
 
+```sh
 # Create a virtual environment.
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate # On Windows use `.venv\Scripts\activate`
 
 # Install the relationalai package.
 python -m pip install relationalai
 ```
 
+> [!TIP]
+> If you would prefer not to activate your virtual environment every time you work on your project,
+> you can reference the executables in your virtual environment directly.
+> For example, you can use `./.venv/bin/python` instead of `python` and `./.venv/bin/rai` instead of `rai`.
+
 Then, use the included `rai` CLI to initialize your project:
 
 ```sh
-rai init
+rai init  # Or .venv/bin/rai init, see caution callout below.
 ```
 
 Follow the prompts to connect to your cloud platform
 and configure your project's resources. You can inspect the status of your
 configuration at any time by running `rai config:explain`.
 
 > [!CAUTION]
-> If you have the [original RelationalAI CLI](https://github.com/RelationalAI/rai-cli/) installed
-> and encounter an error that `init` is not a valid command, you may need to adjust your PATH
-> so that the folder containing the original CLI binary comes _after_ your project's folder.
-> You can also rename your original RAI binary, typically located at `~/usr/local/bin/rai.`
-> If you do not need the original CLI, the best solution is to delete it.
+> If you encounter an error saying that `init` is not a valid command,
+> you may have the [original RelationalAI CLI](https://github.com/RelationalAI/rai-cli/) installed.
+> If you no longer need the original CLI, you can delete it to resolve the error.
+> To keep both CLIs, you may either rename the original CLI or use the command
+> `/path/to/project/.venv/bin/rai` instead of `rai` to run the new CLI.
 >
 > You may also encounter issues with workflows using the original CLI
 > if you install `relationalai` in your global environment.
 > Always using a project-specific virtual environment is highly recommended.
 > See [Virtual Environments and Packages](https://docs.python.org/3/tutorial/venv.html)
 > for a primer on Python virtual environments.
 
@@ -357,20 +374,22 @@
 # 3    Deb   17
 # 0   Alex   19
 # 1    Bob   47
 ```
 
 In some cases, though, you may need to use the sort order in the query itself.
 Or, you may need to sort a collection that is too big for a DataFrame.
-To sort results inside of a query, use `model.aggregates.rank_asc()` or `.rank_desc()`:
+To sort results inside of a query, use `aggregates.rank_asc()` or `.rank_desc()`:
 
 ```python
+from relationalai.std import aggregates
+
 with model.query() as select:
     person = Person()
-    rank = model.aggregates.rank_asc(person.age, person)
+    rank = aggregates.rank_asc(person.age, person)
     response = select(rank, person.name, person.age)
 
 print(response.results)
 # Output:
 #    v   name  age
 # 0  1  Carol   17
 # 1  2    Deb   17
@@ -379,17 +398,19 @@
 ```
 
 You must pass `person.age` _and_ `person` to `.rank_asc()` because there may be
 (and, in fact, are) multiple people with the same age.
 `.rank_asc(person.age)` sorts the _set_ of all people's ages:
 
 ```python
+from relationalai.std import aggregates
+
 with model.query() as select:
     person = Person()
-    rank = model.aggregates.rank_asc(person.age)
+    rank = aggregates.rank_asc(person.age)
     response = select(rank, person.name, person.age)
 
 print(response.results)
 # Output:
 #    v   name  age
 # 0  1  Carol   17
 # 1  1    Deb   17
@@ -405,21 +426,23 @@
 ### Customize Result Column Names
 
 In the preceding example, `select(rank, person.name, person.age)` returns results
 with columns named `v`, `name`, and `age`.
 Property names are automatically used as column names.
 But `rank` isn't a property, so its column is given the generic name `v`.
 
-You may provide custom column names using `model.alias()`:
+You may provide custom column names using `relationalai.std.alias()`:
 
 ```python
+from relationalai.std import aggregates, alias
+
 with model.query() as select:
     person = Person()
-    rank = model.aggregates.rank_asc(person.age, person)
-    response = select(model.alias(rank, "rank"), person.name, person.age)
+    rank = aggregates.rank_asc(person.age, person)
+    response = select(alias(rank, "rank"), person.name, person.age)
 
 print(response.results)
 # Output:
 #    rank   name  age
 # 0     1  Carol   17
 # 1     2    Deb   17
 # 2     3   Alex   19
@@ -438,21 +461,23 @@
 # Use pandas `.mean()` to find the average age of people in the model.
 print(response.results.age.mean())
 # Output:
 # 25.0
 ```
 
 But sometimes you need to use aggregate values in queries.
-Aggregate methods are available in the `model.aggregates` namespace.
-For instance, to find the average age of all people in the model, use `model.aggregates.avg`:
+Aggregate methods are available in the `relationalai.std.aggregates` namespace.
+For instance, to find the average age of all people in the model, use `avg()`:
 
 ```python
+from relationalai.std import aggregates
+
 with model.query() as select:
     person = Person()
-    avg_age = model.aggregates.avg(person, person.age)
+    avg_age = aggregates.avg(person, person.age)
     response = select(avg_age)
 
 print(response.results)
 # Output:
 #       v
 # 0  25.0
 ```
@@ -462,17 +487,19 @@
 For instance, `.avg(person.age)` aggregates over the _set_ of ages and so won't count `17` twice for both Carol and Deb.
 In contrast, `.avg(person, person.age)` aggregates over the set of _pairs_ of people and ages.
 The aggregation is done over the last positional parameter.
 
 You may group results using an aggregate method's `per` parameter:
 
 ```python
+from relationalai.std import aggregates
+
 with model.query() as select:
     person = Person()
-    avg_friend_age = model.aggregates.avg(person.friend, person.friend.age, per=[person])
+    avg_friend_age = aggregates.avg(person.friend, person.friend.age, per=[person])
     response = select(person.name, avg_friend_age)
 
 print(response.results)
 # Output:
 #     name     v
 # 0   Alex  32.0
 # 1  Carol  17.0
@@ -521,17 +548,19 @@
     person = Person()
     person.friend.set(friend=person)
 ```
 
 Now, every person is friends with somebody else:
 
 ```python
+from relationalai.std import aggregates
+
 with model.query():
     person = Person()
-    friend_count = model.aggregates.count(person.friend, per=[person])
+    friend_count = aggregates.count(person.friend, per=[person])
     response = select(person.name, friend_count)
 
 print(response.results)
 # Output:
 #     name  v
 # 0   Alex  2
 # 1    Bob  1
```

### Comparing `relationalai-0.1.9/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.0/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/docs/_old/metamodel.md` & `relationalai-0.2.0/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/docs/_old/python_dsl.md` & `relationalai-0.2.0/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/docs/_old/quickstart.md` & `relationalai-0.2.0/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/docs/api_reference/python/InstanceProperty.md` & `relationalai-0.2.0/docs/api_reference/python/InstanceProperty/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 <!-- markdownlint-disable MD024 -->
 
-# InstanceProperty
+# `relationalai.InstanceProperty`
 
-Instance properties are [producers](./Producer.md) that produce property values of objects in a [model](./Model.md).
-You create properties using the [`Type.add()`](./Type.md#typeadd) and [`Instance.set()`](./Instance.md#instanceset) methods,
-which return [`Instance`](./Instance.md) objects.
-You access properties as [`Instance` attributes](./Producer.md#producer__getattribute__),
+Instance properties are [producers](./Producer/README.md) that produce property values of objects in a [model](./Model/README.md).
+You create properties using the [`Type.add()`](./Type/add.md) and [`Instance.set()`](./Instance/set.md) methods,
+which return [`Instance`](./Instance/README.md) objects.
+You access properties as [`Instance` attributes](./Producer/getattribute__.md),
 which return instances of the `InstanceProperty` class.
 
 ```python
 class InstanceProperty(model: Model)
 ```
 
-The `InstanceProperty` class is a subclass of [`Producer`](./Producer.md).
-
-## Parameters
+The `InstanceProperty` class is a subclass of [`Producer`](./Producer/README.md).
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `model` | [`Model`](./Model.md) | The model in which the instance property is created. |
+| `model` | [`Model`](./Model/README.md) | The model in which the instance property is created. |
+
+## Methods
+
+- [`InstanceProperty.or_()`](./or_.md)
 
 ## Example
 
 You do not create `InstanceProperty` objects directly.
-Accessing a property as an [`Instance`](./Instance.md) attribute returns an `InstanceProperty` object:
+Accessing a property as an [`Instance`](./Instance/README.md) attribute returns an `InstanceProperty` object:
 
 ```python
 import relationalai as rai
 
 model = rai.Model("books")
 Book = model.Type("Book")
 
@@ -40,12 +42,12 @@
     book = Book()
     # Both `book.author` and `book.name` are `InstanceProperty` objects.
     book.author == "Isaac Asimov"
     response = select(book.name)
 ```
 
 `InstanceProperty` objects are `Producer` objects and support the same attributes and methods.
-See [`Producer`](./Producer.md) for details.
+See [`Producer`](./Producer/README.md) for details.
 
 ## See Also
 
-[`Producer`](./Producer.md) and [`Instance`](./Instance.md).
+[`Producer`](./Producer/README.md) and [`Instance`](./Instance/README.md).
```

### Comparing `relationalai-0.1.9/examples/README.md` & `relationalai-0.2.0/examples/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 ```sh
 # Clone the examples locally
 git clone git@github.com:RelationalAI/relationalai-python.git
 cd relationalai-python/examples
 
 # set up virtual environment
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
 pip install -r requirements.txt
 ```
 
-> :bulb: If you plan to hack on relationalai-python code, you can install it in editable mode to avoid having to reinstall after every modification:
+> :bulb: If you plan to hack on `relationalai-python` code, you can install it in editable mode to avoid having to reinstall after every modification:
 
 ```sh
 cd PATH/TO/examples
 
 # Activate the venv if you haven't already
 source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
 
@@ -38,9 +38,11 @@
 
 ## Debugging 
 
 @TODO: Detail the debugging experience.
 
 ```sh
 # run debugger (in a separate terminal)
-python -m relationalai.tools.debugger
+rai debugger
 ```
+
+This will open a browser window with the debugger UI. The debugger will automatically connect to any Python process that uses the RelationalAI library in the same environment.
```

### Comparing `relationalai-0.1.9/examples/SF_pagerank.ipynb` & `relationalai-0.2.0/examples/social-money-network/SF_pagerank.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968661606799583%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, 'from relationalai.std import aggregates\\n'), (5, 'from "*

 * *            "relationalai.std.graphs import Graph\\n')], delete: [4]}}, 8: {'source': {insert: "*

 * *            "[(1, 'Node, Edge = graph.Node, graph.Edge\\n'), (4, 'Node.extend(Account, "*

 * *            'name=Account.name)\\n\'), (5, \'Node.extend(Person, kind="person")\\n\'), (6, '*

 * *            '\'Node.extend(Merchant, kind="merchant", label=Merchant.name)\\n\'), (11, \'    '*

 * *            "Edge.add(t.from_, t.to,  […]*

```diff
@@ -15,15 +15,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from typing import Tuple\n",
                 "import rich\n",
                 "\n",
                 "import relationalai as rai\n",
-                "from relationalai.graphs import Graph\n",
+                "from relationalai.std import aggregates\n",
+                "from relationalai.std.graphs import Graph\n",
                 "from relationalai.clients.snowflake import Snowflake, PrimaryKey\n",
                 "\n",
                 "model = rai.Model(\"SFPagerank\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -106,25 +107,25 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "50b6e017-49e4-4334-87cc-d3171667da41",
             "metadata": {},
             "outputs": [],
             "source": [
                 "graph = Graph(model)\n",
-                "nodes, edges = graph.nodes, graph.edges\n",
+                "Node, Edge = graph.Node, graph.Edge\n",
                 "\n",
                 "# add some nodes\n",
-                "nodes.extend(Account, name=Account.name)\n",
-                "nodes.extend(Person, kind=\"person\")\n",
-                "nodes.extend(Merchant, kind=\"merchant\", label=Merchant.name)\n",
+                "Node.extend(Account, name=Account.name)\n",
+                "Node.extend(Person, kind=\"person\")\n",
+                "Node.extend(Merchant, kind=\"merchant\", label=Merchant.name)\n",
                 "\n",
                 "# add edges for transactions\n",
                 "with model.rule():\n",
                 "    t = Transaction()\n",
-                "    edges.add(t.from_, t.to, amount=t.amount)"
+                "    Edge.add(t.from_, t.to, amount=t.amount)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a4694972-4208-45f1-b7ab-999632c98509",
             "metadata": {},
             "source": [
@@ -137,15 +138,15 @@
             "id": "6394e745-e1ee-4557-a95d-29112989ff83",
             "metadata": {},
             "outputs": [],
             "source": [
                 "with model.rule():\n",
                 "    m = Merchant()\n",
                 "    rank = graph.compute.pagerank(m)\n",
-                "    nodes.add(m, rank=rank)\n",
+                "    Node(m).set(rank=rank)\n",
                 "    m.set(rank=rank)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "73859cc7-da3d-4593-b7be-fd93bed890e9",
             "metadata": {},
@@ -199,15 +200,15 @@
             "outputs": [],
             "source": [
                 "@model.export(\"sandbox.public\")\n",
                 "def merchant_rank(minimum: float) -> Tuple[str, float, int]:\n",
                 "    m = Merchant()\n",
                 "    m.rank >= minimum\n",
                 "    t = Transaction(to=m)\n",
-                "    total = model.aggregates.sum(t, t.amount, per=[m])\n",
+                "    total = aggregates.sum(t, t.amount, per=[m])\n",
                 "    return m.name, m.rank, total"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "759d066f-7874-42b5-8236-1b542a4a0872",
@@ -239,13 +240,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "version": "3.10.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `relationalai-0.1.9/examples/cdc.py` & `relationalai-0.2.0/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/emit_playground.py` & `relationalai-0.2.0/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/found.py` & `relationalai-0.2.0/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/fraud.ipynb` & `relationalai-0.2.0/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/fraud.py` & `relationalai-0.2.0/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/or_types.py` & `relationalai-0.2.0/examples/or_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #pyright: reportUnusedExpression=false
 import relationalai as rai
 
-graph = rai.Graph("MyCoolDatabase")
+graph = rai.Model("MyCoolDatabase")
 Person = graph.Type("Person")
 Adult = graph.Type("Adult")
 Child = graph.Type("Woop")
 
 with graph.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
```

### Comparing `relationalai-0.1.9/examples/simple_recursion.py` & `relationalai-0.2.0/examples/simple_recursion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import relationalai as rai
 
-graph = rai.Graph("RecursiveExample")
+graph = rai.Model("RecursiveExample")
 Edge = graph.Type("Edge")
 
 ## Find all paths reachable from a given start node and an initial set of 1-hop edges.
 
 with graph.rule():
     # Create some initial edges
     Edge.add(start=1, finish=2)
```

### Comparing `relationalai-0.1.9/examples/simple_streamlit.py` & `relationalai-0.2.0/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/snowflake_pagerank.py` & `relationalai-0.2.0/examples/social-money-network/snowflake_pagerank.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #pyright: reportUnusedExpression=false
 from typing import Tuple
 import rich
 import relationalai as rai
-from relationalai.graphs import Graph
+from relationalai.std import aggregates
+from relationalai.std.graphs import Graph
 from relationalai.clients.snowflake import Snowflake, PrimaryKey
 
 model = rai.Model("SFPagerank", dry_run=False)
 
 #--------------------------------------------------
 # Initialize Snowflake data
 #--------------------------------------------------
@@ -39,28 +40,28 @@
         a.set(Person)
 
 #--------------------------------------------------
 # Create a graph
 #--------------------------------------------------
 
 graph = Graph(model)
-nodes, edges = graph.nodes, graph.edges
+Node, Edge = graph.Node, graph.Edge
 
-nodes.extend(Account, name=Account.name)
-nodes.extend(Person, kind="person")
-nodes.extend(Merchant, kind="merchant", label=Merchant.name)
+Node.extend(Account, name=Account.name)
+Node.extend(Person, kind="person")
+Node.extend(Merchant, kind="merchant", label=Merchant.name)
 
 with model.rule():
     t = Transaction()
-    edges.add(t.from_, t.to, amount=t.amount)
+    Edge.add(t.from_, t.to, amount=t.amount)
 
 with model.rule():
     m = Merchant()
     rank = graph.compute.pagerank(m)
-    nodes.add(m, rank=rank)
+    Node(m).set(rank=rank)
     m.set(rank=rank)
 
 #--------------------------------------------------
 # Visualize the graph
 #--------------------------------------------------
 
 graph.visualize(
@@ -88,15 +89,15 @@
 #--------------------------------------------------
 
 @model.export("sandbox.public")
 def merchant_rank(minimum: float) -> Tuple[str, float, int]:
     m = Merchant()
     m.rank >= minimum
     t = Transaction(to=m)
-    total = model.aggregates.sum(t, t.amount, per=[m])
+    total = aggregates.sum(t, t.amount, per=[m])
     return m.name, m.rank, total #type: ignore
 
 print("\nCalling merchant rank from Snowflake!\n")
 for row in model.resources._exec("call sandbox.public.merchant_rank(0.04);"):
     rich.print(row)
```

### Comparing `relationalai-0.1.9/examples/solver.py` & `relationalai-0.2.0/examples/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #pyright: reportUnusedExpression=false
 import rich
 import relationalai as rai
+from relationalai.std import rel as r, Vars
 
 #--------------------------------------------------
 # Helpers
 #--------------------------------------------------
 
 def pprint(title, res):
     rich.print("[dim]\n--------------------------------------------------")
@@ -21,18 +22,16 @@
 model = rai.Model("MyCoolModel")
 model.load_raw("rel/")
 
 #--------------------------------------------------
 # Do a query with some of our loaded relations
 #--------------------------------------------------
 
-r = model.rel # get a handle to the root namespace
-
 with model.query() as select:
-    a,b = model.Vars(2)
+    a,b = Vars(2)
     r.foo(a, b)
     r.bar(a + 5)
     z = select(a, b)
 
 pprint("Foo/Bar results", z)
 
 #--------------------------------------------------
@@ -62,15 +61,15 @@
 pprint("Solver results", info)
 
 #--------------------------------------------------
 # Read a relation from solver.rel
 #--------------------------------------------------
 
 with model.query() as select:
-    status, x, y, obj = model.Vars(4)
+    status, x, y, obj = Vars(4)
     r.info(status, x, y, obj)
     info = select(status, x, y, obj)
 
 pprint("Solver info", info)
 
 #--------------------------------------------------
 # Load some data
```

### Comparing `relationalai-0.1.9/examples/data/people.csv` & `relationalai-0.2.0/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/data/transactions.csv` & `relationalai-0.2.0/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/examples/rel/solver.rel` & `relationalai-0.2.0/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/README.md` & `relationalai-0.2.0/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/emit.py` & `relationalai-0.2.0/src/gentest/emit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Set, assert_never
+from typing import List, Set
 from contextlib import contextmanager
 import pprint
 import keyword
 import re
 import unicodedata
 from relationalai import metamodel as mm
 from relationalai.clients.test import Document, Install, Query
@@ -74,15 +74,15 @@
                         cur = f"{base}{ix}"
 
                     self.used_entity_names.add(cur)
                     str_repr = sanitize_variable_name(cur)
                 else:
                     str_repr = sanitize_variable_name(f"{of.type.name.lower()}_{str(of)}" )
             case _:
-                assert_never(of)
+                assert of is None
 
         self.mappings[of] = str_repr
         return str_repr
 
     def value(self, of:mm.Var|mm.Value, as_entity = False):
         match of:
             case mm.Var():
```

### Comparing `relationalai-0.1.9/src/gentest/fixtures.py` & `relationalai-0.2.0/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/patch.py` & `relationalai-0.2.0/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/util.py` & `relationalai-0.2.0/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/cli/__main__.py` & `relationalai-0.2.0/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/cli/collect_failures.py` & `relationalai-0.2.0/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/cli/collect_tests.py` & `relationalai-0.2.0/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/cli/repro.py` & `relationalai-0.2.0/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/cli/watch.py` & `relationalai-0.2.0/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/action.py` & `relationalai-0.2.0/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/context.py` & `relationalai-0.2.0/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/document.py` & `relationalai-0.2.0/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/group_limited.py` & `relationalai-0.2.0/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/ir.py` & `relationalai-0.2.0/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/scope.py` & `relationalai-0.2.0/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/task.py` & `relationalai-0.2.0/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/gen/test.py` & `relationalai-0.2.0/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/harness/database.py` & `relationalai-0.2.0/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/validate/diff.py` & `relationalai-0.2.0/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/validate/errors.py` & `relationalai-0.2.0/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/validate/mapping.py` & `relationalai-0.2.0/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/gentest/validate/roundtrip.py` & `relationalai-0.2.0/src/gentest/validate/roundtrip.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,20 @@
     return proxies
 
 def get_proxied_client():
     proxies = drain_proxied_clients()
     assert len(proxies) == 1
     return proxies[0]
 
-def exec_and_run_callback(code: str, callback: Callable[..., Any] = return_document, *args: Any):
+def exec_and_run_callback(code: str, callback: Callable[..., Any]|None, *args: Any, ns:dict|None = None):
+    if callback is None:
+         callback = return_document
+
     try:
-        ns = None
-        exec(code, None, ns)
+        exec(code, ns, None)
         return callback(get_proxied_client(), *args)
     finally:
         drain_proxied_clients()
 
 #===============================================================================
 # From code
 #===============================================================================
```

### Comparing `relationalai-0.1.9/src/relationalai/__init__.py` & `relationalai-0.2.0/src/relationalai/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,59 @@
-from .clients import config
+from typing import cast
+from relationalai.tools.debugger_server import start_debugger_session
+from .clients import config as cfg
 from . import clients
 from . import dsl
 from . import debugging
 from . import metamodel
 from . import rel
 from .loaders import csv
 from . import analysis
 from . import tools
-from . import graphs
+import importlib.metadata
 
-def Model(name:str, dry_run:bool=False):
-    cfg = config.Config()
-    if not cfg.file_path:
-        raise Exception("No configuration file found. Please run `rai init` to create one.")
-    platform = cfg.get("platform", "snowflake")
+__version__ = importlib.metadata.version(__package__ or __name__)
+
+def Model(name:str, *, profile:str|None=None, config:cfg.Config|None=None, dry_run:bool=False, debug=None):
+    config = config or cfg.Config(profile=profile)
+    if debug is None:
+        debug = config.get("debug", False)
+    if debug:
+        start_debugger_session(True)
+    if not config.file_path:
+        if cfg.legacy_config_exists():
+            message = (
+                "Use `rai init` to migrate your configuration file "
+                "to the new format (raiconfig.toml)"
+            )
+        else:
+            message = "No configuration file found. Please run `rai init` to create one."
+        raise Exception(message)
+    if config.get("platform") is None:
+        config.set("platform", "snowflake")
+    platform = config.get("platform")
+    dry_run = cast(bool, dry_run or config.get("compiler.dry_run", False))
     if platform == "azure":
-        return clients.azure.Graph(name, dry_run)
+        return clients.azure.Graph(
+            name, profile=profile, config=config, dry_run=dry_run
+        )
     elif platform == "snowflake":
-        return clients.snowflake.Graph(name, dry_run)
+        return clients.snowflake.Graph(
+            name, profile=profile, config=config, dry_run=dry_run
+        )
     else:
         raise Exception(f"Unknown platform: {platform}")
 
-def Resources(profile:str|None=None, cfg:config.Config|None=None):
-    cfg = cfg or config.Config(profile)
-    platform = cfg.get("platform", "snowflake")
+def Resources(profile:str|None=None, config:cfg.Config|None=None):
+    config = config or cfg.Config(profile)
+    platform = config.get("platform", "snowflake")
     if platform == "azure":
-        return clients.azure.Resources(config=cfg)
+        return clients.azure.Resources(config=config)
     elif platform == "snowflake":
-        return clients.snowflake.Resources(config=cfg)
+        return clients.snowflake.Resources(config=config)
     else:
         raise Exception(f"Unknown platform: {platform}")
 
 def Graph(name:str, dry_run:bool=False):
-    return Model(name, dry_run=dry_run)
+    return Model(name, profile=None, dry_run=dry_run)
 
-__all__ = ['Model', 'Resources', 'Graph', 'dsl', 'rel', 'debugging', 'metamodel', 'csv', 'analysis', 'tools', 'graphs']
+__all__ = ['Model', 'Resources', 'dsl', 'rel', 'debugging', 'metamodel', 'csv', 'analysis', 'tools']
```

### Comparing `relationalai-0.1.9/src/relationalai/compiler.py` & `relationalai-0.2.0/src/relationalai/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 # Compiler Pass
 #--------------------------------------------------
 
 T = TypeVar('T', bound='AllItems')
 
 class Pass:
     backlinks = {}
+    forwardlinks = {}
 
     def __init__(self, copying = True) -> None:
         self.seen = set()
         self.copying = copying
 
     def clone(self, item:T) -> T:
         copied = copy.copy(item)
         copied.id = next_id()
         Pass.backlinks[copied] = item
+        Pass.forwardlinks[item] = copied
         return copied
 
     def walk(self, item: T, parent=None) -> T:
         if not item or item in self.seen:
-            return item
+            return Pass.forwardlinks.get(item, item)
         if self.copying and not Pass.backlinks.get(item) and not isinstance(item, Var) and (isinstance(item, Task) or not isinstance(item, Type)):
             item = self.clone(item)
+        elif self.copying and isinstance(item, Var) and isinstance(item.value, Task) and len(item.value.items):
+            item = self.clone(item)
         self.seen.add(item)
 
         if isinstance(item, Task):
             self.task(cast(Task, item), parent)
         elif isinstance(item, Type):
             self.type(item, parent)
         elif isinstance(item, Property):
@@ -51,15 +55,15 @@
             return [self.walk(item, parent) for item in items]
         else:
             for item in items:
                 self.walk(item, parent)
             return items
 
     def reset(self):
-        self.seen = set()
+        self.seen.clear()
 
     def type(self, type: Type, parent=None):
         type.properties = self.walk_all(type.properties, type)
 
     def property(self, property: Property, parent=None):
         property.type = self.walk(property.type)
 
@@ -94,15 +98,16 @@
         catch.items = self.walk_all(catch.items, catch)
 
     def agent(self, agent: Agent, parent=None):
         pass
 
     def var(self, var: Var, parent=None):
         var.type = self.walk(var.type, parent)
-        if isinstance(var.value, Type) or isinstance(var.value, Property):
+        if (isinstance(var.value, Type) or isinstance(var.value, Property)) \
+            and (not isinstance(var.value, Task) or len(var.value.items)):
             var.value = self.walk(var.value, parent)
 
     def action(self, action: Action, parent=None):
         action.entity = self.walk(action.entity, parent)
         action.types = self.walk_all(action.types, parent)
         action.bindings = {k: self.walk(v, parent) for k, v in action.bindings.items()}
 
@@ -135,15 +140,16 @@
         if not pyrel_info:
             sources = []
             for i in self.task.items:
                 source = debugging.get_source(i)
                 if source:
                     if not pyrel_info:
                         pyrel_info = source
-                    sources.append(source.source)
+                    if source.source not in sources:
+                        sources.append(source.source)
             pyrel_block = "\n".join(sources)
         else:
             pyrel_block = pyrel_info.source
         if not pyrel_info:
             pyrel_info = debugging.SourceInfo()
         return (pyrel_info.file, pyrel_info.line, pyrel_block)
 
@@ -164,12 +170,13 @@
             compilation.pass_result(pass_, task, time.perf_counter() - start)
         return task
 
     def compile(self, task: Task):
         compilation = Compilation(task)
         task = self.rewrite(task, compilation)
         start = time.perf_counter()
+        self.emitter.reset()
         code = self.emitter.emit(task)
         compilation.emitted = code
         compilation.emit_time = time.perf_counter() - start
         debugging.handle_compilation(compilation)
         return code
```

### Comparing `relationalai-0.1.9/src/relationalai/dsl.py` & `relationalai-0.2.0/src/relationalai/dsl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from enum import Enum
 import inspect
 from itertools import zip_longest
+import re
+import threading
 import typing
-from typing import Any, Dict, List, Optional, Tuple, get_type_hints
+from typing import Any, Dict, List, Optional, Set, Tuple, TypeGuard, Union, get_type_hints
 import numbers
 import os
+import sys
 import datetime
 import hashlib
+import traceback
+import rich
 
 from pandas import DataFrame
 
 from .metamodel import Behavior, Builtins, ActionType, Var, Task, Action, Builder, Type as mType, Property as mProperty
 from . import debugging
-from .errors import Errors
+from .errors import Errors, RAIException, RelQueryError
 
 from bytecode import Instr, Bytecode
 
 #--------------------------------------------------
+# Constants
+#--------------------------------------------------
+
+RESERVED_PROPS = ["add", "set", "persist", "unpersist"]
+
+#--------------------------------------------------
 # Helpers
 #--------------------------------------------------
 
 def to_var(x:Any):
     if isinstance(x, Var):
         return x
     if getattr(x, "_to_var", None):
@@ -68,14 +79,17 @@
         return all(is_static(i) for i in x)
     if isinstance(x, tuple):
         return all(is_static(i) for i in x)
     if isinstance(x, dict):
         return all(is_static(i) for i in x.values())
     return False
 
+def is_collection(x:Any) -> TypeGuard[Union[List, Tuple, Set]]:
+    return isinstance(x, list) or isinstance(x, tuple) or isinstance(x, set)
+
 #--------------------------------------------------
 # Base
 #--------------------------------------------------
 
 id = 0
 def next_id():
     global id
@@ -89,36 +103,40 @@
 class Producer():
     def __init__(self, graph:'Graph', builtins:List[str]):
         self._id = next_id()
         self._graph = graph
         self._builtins = builtins
         self._subs = {}
 
-    def __getattribute__(self, __name: str) -> Any:
-        if __name.startswith("_") or __name in self._builtins:
-            return object.__getattribute__(self, __name)
-        self._subs[__name] = self._make_sub(__name, self._subs.get(__name))
-        return self._subs[__name]
+    def __getattribute__(self, name: str) -> Any:
+        if name.startswith("_") or name in self._builtins:
+            return object.__getattribute__(self, name)
+        if name == "getdoc":
+            rich.print("[red bold]GETDOC CALLED")
+            traceback.print_stack()
+            return
+        self._subs[name] = self._make_sub(name, self._subs.get(name))
+        return self._subs[name]
 
     def _make_sub(self, name:str, existing:Optional['Producer']=None) -> Any:
         raise Exception("Implement Producer._make_sub")
 
     def _use_var(self):
         pass
 
     #--------------------------------------------------
-    # Graph helpers
+    # Boolean overloads
     #--------------------------------------------------
 
-    def _add_action(self, action: Action):
-        self._graph._action(action)
-        pass
-
-    def _add_type(self, type: mType):
-        self._graph._types[type.name] = type
+    def __bool__(self):
+        # This doesn't seem to be safe as Python can call bool on Producers in lots of random cases
+        # Errors.invalid_bool(Errors.call_source(3))
+        # class_name = self.__class__.__name__
+        # raise TypeError(f"Can't convert an {class_name} to a boolean.")
+        return True
 
     #--------------------------------------------------
     # Math overloads
     #--------------------------------------------------
 
     def _wrapped_op(self, op, left, right):
         args = [left, right]
@@ -145,14 +163,17 @@
         return self._wrapped_op(Builtins.div, other, self)
 
     def __pow__(self, other):
         return self._wrapped_op(Builtins.pow, self, other)
     def __rpow__(self, other):
         return self._wrapped_op(Builtins.pow, other, self)
 
+    def __neg__(self):
+        return self._wrapped_op(Builtins.mult, self, -1)
+
     #--------------------------------------------------
     # Filter overloads
     #--------------------------------------------------
 
     def __gt__(self, other):
         return self._wrapped_op(Builtins.gt, self, other)
     def __ge__(self, other):
@@ -193,15 +214,15 @@
         self._insts = []
         self._vars = []
         self._props = {}
 
     def _assign_vars(self):
         task = self._context._task
         if not len(self._vars) and self._select_len:
-            self._insts = to_list(self._context.graph.Vars(self._select_len))
+            self._insts = to_list(Vars(self._select_len))
             self._vars = [to_var(v) for v in self._insts]
             task.properties = [Builtins.Relation.properties[i] for i in range(self._select_len)]
             task.bindings.update({Builtins.Relation.properties[i]: v for i, v in enumerate(self._vars)})
 
     def __call__(self, *args: Any) -> Any:
         graph = self._context.graph
         task = self._context._task
@@ -236,43 +257,54 @@
                 self._props[k] = v
 
         graph = self._context.graph
         graph._action(build.return_([item, *[kwargs[k] for k in self._props.keys()]]))
 
 class Context():
     def __init__(self, graph:'Graph', *args, behavior=Behavior.Query, op=None,
-                 exec_type=TaskExecType.Rule, source_steps=1, dynamic=False, name="None",
-                 inputs=None, outputs=None):
+                 exec_type=TaskExecType.Rule, dynamic=False, name="None",
+                 inputs=None, outputs=None, engine=None):
         self._id = next_id()
         self.results = DataFrame()
         self.graph = graph
         self._task = Task(behavior=behavior)
         self._op = op
         self._args = list(args)
         self._exec_type = exec_type
         self._select_len = None
         self._rel = None
-        self._source_steps = source_steps
         self._dynamic = dynamic
         self._name = name
         self._inputs = inputs
         self._outputs = outputs
+        self._engine= engine
 
     def __enter__(self):
-        debugging.set_source(self._task, self._source_steps, dynamic=self._dynamic)
+        debugging.set_source(self._task, dynamic=self._dynamic)
         self.graph._push(self)
         return ContextSelect(self)
 
     def __exit__(self, *args):
-        try:
-            self.graph._pop(self)
-        except Exception as e:
-            if len(e.args) and "Rel " in e.args[0]:
-                raise Exception(e.args[0]) from None
-            raise e
+        # If no exception info has been passed to args,
+        # then proceed with the normal exit process.
+        # Otherwise, return False to propagate the exception.
+        if args[0] is None:
+            try:
+                self.graph._pop(self)
+            except KeyboardInterrupt as e:
+                print("Canceling transactions...")
+                self.graph.resources.cancel_pending_transactions()
+                raise e
+            except RAIException as e:
+                raise RAIException(e.message) from None
+            except RelQueryError:
+                raise RAIException("An error occured translating Python into RelationalAI") from None
+        else:
+            self.graph._pop(self, exec=False)
+        return False
 
     def _ensure_rel(self, vs:List[Var]):
         if self._rel is None:
             self._rel = build.relation_action(ActionType.Get, self._task, vs)
         self.graph._action(self._rel)
 
     def __iter__(self):
@@ -299,47 +331,78 @@
     combined_bytes = combined.encode('utf-8')
     hasher = hashlib.sha256()
     hasher.update(combined_bytes)
     hash_128_bit = hasher.digest()[:16]
     return hash_128_bit
 
 class Type(Producer):
-    def __init__(self, graph:'Graph', name:str, builtins:List[str] = []):
-        super().__init__(graph, ["add", "persist"] + builtins)
-        self._type = mType(name)
-        self._add_type(self._type)
+    def __init__(self, graph:'Graph', name:str, builtins:List[str] = [], scope:str=""):
+        super().__init__(graph, ["add", "persist", "extend", "known_properties"] + builtins)
+        self._type = mType(scope+name)
+        self._scope = scope
+        if graph._config.get("compiler.use_value_types", False):
+            self._type.parents.append(Builtins.ValueType)
+            install = build.install(self._type)
+            self._graph._action(install)
+            debugging.set_source(install)
 
     def __call__(self, *args, **kwargs):
-        return Instance(self._graph, ActionType.Get, [self, *args], kwargs, name=self._type.name.lower())
+        return Instance(self._graph, ActionType.Get, [self, *args], kwargs, name=self._type.name.lower(), scope=self._scope)
 
     def add(self, *args, **kwargs):
-        inst = Instance(self._graph, ActionType.Bind, [self, *args], kwargs, name=self._type.name.lower())
+        inst = Instance(self._graph, ActionType.Bind, [self, *args], kwargs, name=self._type.name.lower(), is_add=True, scope=self._scope)
         if is_static(args) and is_static(kwargs):
-            inst._action.entity.value = hash_values_sha256_truncated(kwargs.values())
-        else:
-            self._graph._action(build.ident(inst._action), True)
+            params = [Var(value=t.name) for t in inst._action.types]
+            params.extend(inst._action.bindings.values())
+            inst._action.entity.value = hash_values_sha256_truncated(params)
+        elif all([isinstance(a, Type) for a in args]):
+            self._graph._action(build.ident(inst._action))
+        inst._add_to_graph()
         return inst
 
     def persist(self, *args, **kwargs):
-        inst = Instance(self._graph, ActionType.Persist, [self, *args], kwargs, name=self._type.name.lower())
+        inst = Instance(self._graph, ActionType.Persist, [self, *args], kwargs, name=self._type.name.lower(), is_add=True, scope=self._scope)
         if is_static(args) and is_static(kwargs):
-            inst._action.entity.value = hash_values_sha256_truncated(kwargs.values())
-        else:
-            self._graph._action(build.ident(inst._action), True)
+            params = [Var(value=t.name) for t in inst._action.types]
+            params.extend(inst._action.bindings.values())
+            inst._action.entity.value = hash_values_sha256_truncated(params)
+        elif all([isinstance(a, Type) for a in args]):
+            self._graph._action(build.ident(inst._action))
+        inst._add_to_graph()
         return inst
 
+    def extend(self, *args, **kwargs):
+        for arg in args:
+            if not isinstance(arg, Type):
+                raise Exception("Can only extend a type with another type")
+            with self._graph.rule(dynamic=True):
+                a = arg()
+                a.set(self)
+            with self._graph.rule(dynamic=True):
+                a = arg()
+                neue = self(a)
+                for k, v in kwargs.items():
+                    if isinstance(v, Property):
+                        v = getattr(a, v._prop.name)
+                    neue.set(**{k:v})
+
     def __or__(self, __value: Any) -> 'TypeUnion':
         if isinstance(__value, Type):
             return TypeUnion(self._graph, [self, __value])
         if isinstance(__value, TypeUnion):
             return TypeUnion(self._graph, [self, *__value._types])
         raise Exception("Can't or a type with a non-type")
 
     def _make_sub(self, name: str, existing=None):
-        return existing or Property(self._graph, name, [self._type], self)
+        if existing is not None:
+            return existing
+        return Property(self._graph, name, [self._type], self, scope=self._scope)
+
+    def known_properties(self):
+        return [p.name for p in self._type.properties]
 
 #--------------------------------------------------
 # TypeUnion
 #--------------------------------------------------
 
 class TypeUnion(Producer):
     def __init__(self, graph:'Graph', types:List[Type]):
@@ -360,176 +423,249 @@
         if isinstance(__value, Type):
             return TypeUnion(self._graph, [*self._types, __value])
         if isinstance(__value, TypeUnion):
             return TypeUnion(self._graph, [*self._types, *__value._types])
         raise Exception("Can't or a type with a non-type")
 
     def _make_sub(self, name: str, existing=None):
-        return existing or Property(self._graph, name, [t._type for t in self._types], self)
+        if existing is not None:
+            return existing
+        return Property(self._graph, name, [t._type for t in self._types], self)
 
 #--------------------------------------------------
 # Property
 #--------------------------------------------------
 
 class Property(Producer):
-    def __init__(self, graph:'Graph', name:str, types:List[mType], provider:Type|TypeUnion):
-        super().__init__(graph, ["to_property"])
+    def __init__(self, graph:'Graph', name:str, types:List[mType], provider:Type|TypeUnion, scope:str=""):
+        super().__init__(graph, ["to_property", "has_many"])
         self._name = name
         self._type = types[0]
+        self._scope = scope
         self._provider = provider
-        self._prop = build.property_named(name, types)
+        self._prop = build.property_named(scope+name, types)
 
-    def __call__(self, *args, **kwargs):
-
-        raise Exception("Expressions can't be called")
+    def __call__(self, key:Any, value:Any):
+        action = build.relation_action(ActionType.Get, self._prop, [key, value])
+        self._graph._action(action)
 
     def _use_var(self):
         raise Exception("Support properties being used as vars")
 
     def _make_sub(self, name: str, existing=None):
         raise Exception("Support properties on properties?")
 
     def to_property(self):
         return self._prop
 
+    def has_many(self):
+        self._graph._check_property(self._prop, multi_valued=True)
+
 #--------------------------------------------------
 # Instance
 #--------------------------------------------------
 
-RESERVED_PROPS = ["add", "set", "persist", "unpersist"]
-def check_prop(prop):
-    if prop in RESERVED_PROPS:
-        Errors.reserved_property(Errors.call_source(4), prop)
-
 class Instance(Producer):
-    def __init__(self, graph, action_type:ActionType, positionals:List[Any], named:Dict[str,Any], var:Var|None=None, name=None, namespace=None):
+    def __init__(self, graph:'Graph', action_type:ActionType, positionals:List[Any], named:Dict[str,Any], var:Var|None=None, name=None, is_add=False, scope:str=""):
         super().__init__(graph, RESERVED_PROPS)
         self._action = Action(action_type, to_var(var) if var else Var(name=name))
+        self._actions = [self._action]
         self._sets = {}
         self._context = graph._stack.active()
+        self._scope = scope
         available_types = []
         last_pos_var = None
+
+        #--------------------------------------------------
+        # Positionals
+        #--------------------------------------------------
         for pos in positionals:
             if isinstance(pos, Type):
                 self._action.append(pos._type)
             elif isinstance(pos, Instance):
                 self._action.append(to_var(pos))
                 available_types.extend(pos._action.types)
                 if last_pos_var:
-                    self._add_action(build.eq(last_pos_var, self._action.entity))
+                    self._graph._action(build.eq(last_pos_var, self._action.entity))
                 last_pos_var = self._action.entity
             elif isinstance(pos, TypeUnion):
                 self._action.append(to_var(pos()))
                 available_types.extend([t._type for t in pos._types])
                 if last_pos_var:
-                    self._add_action(build.eq(last_pos_var, self._action.entity))
+                    self._graph._action(build.eq(last_pos_var, self._action.entity))
                 last_pos_var = self._action.entity
             elif isinstance(pos, Producer):
                 self._action.append(to_var(pos))
                 if last_pos_var:
-                    self._add_action(build.eq(last_pos_var, self._action.entity))
+                    self._graph._action(build.eq(last_pos_var, self._action.entity))
                 last_pos_var = self._action.entity
             else:
                 raise Exception(f"Unknown input type: {pos}")
         available_types.extend(self._action.types)
+
+        #--------------------------------------------------
+        # Handle properties
+        #--------------------------------------------------
         for name, val in named.items():
-            check_prop(name)
-            prop = build.property_named(name, available_types)
+            prop = build.property_named(scope+name, available_types)
+
+            if val is None:
+                raise Exception(f"{prop}'s value is None, please provide a value for the property")
+
             prop_var = to_var(val)
+            if is_collection(prop_var.value):
+                raise Exception("Can't set a property to a collection")
+
             if not prop_var.name:
                 prop_var.name = prop.name
+            if prop_var.value is None:
+                self._graph._check_property(prop, unknown_cardinality=True)
+            else:
+                self._graph._check_property(prop)
             self._action.append(prop, prop_var)
+
+        #--------------------------------------------------
+        # Entities
+        #--------------------------------------------------
         self._var = self._action.entity
         if self._var.type == Builtins.Unknown and len(self._action.types):
             self._var.type = self._action.types[0]
-        self._add_action(self._action)
+        if not is_add:
+            self._add_to_graph()
+
+    def _add_to_graph(self):
+        for action in self._actions:
+            self._graph._action(action)
 
     def __call__(self, *args, **kwargs):
         pass
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name.startswith("_"):
             return super().__setattr__(name, value)
         Errors.set_on_instance(Errors.call_source(3), name, value)
 
     def _make_sub(self, name: str, existing=None):
-        if self._sets.get(name):
+        if self._sets.get(name) is not None:
             return self._sets[name]
-        if existing:
-            return InstanceProperty(self._graph, self, name, var=existing._var)
+        if existing is not None:
+            return InstanceProperty(self._graph, self, name, var=existing._var, scope=self._scope)
         prop = build.property_named(name, self._action.types)
         if self._action.bindings.get(prop):
-            return InstanceProperty(self._graph, self, name, var=self._action.bindings[prop])
-        return InstanceProperty(self._graph, self, name)
+            return InstanceProperty(self._graph, self, name, var=self._action.bindings[prop], scope=self._scope)
+        return InstanceProperty(self._graph, self, name, scope=self._scope)
 
     def set(self, *args, **kwargs):
         if self._graph._stack.active() is self._context:
             self._sets.update(kwargs)
-        Instance(self._graph, ActionType.Bind, [self, *args], kwargs, var=self._var)
+        Instance(self._graph, ActionType.Bind, [self, *args], kwargs, var=self._var, scope=self._scope)
         return self
 
     def persist(self, *args, **kwargs):
-
-        Instance(self._graph, ActionType.Persist, [self, *args], kwargs, var=self._var)
+        Instance(self._graph, ActionType.Persist, [self, *args], kwargs, var=self._var, scope=self._scope)
         return self
 
     def unpersist(self, *args, **kwargs):
-        Instance(self._graph, ActionType.Unpersist, [self, *args], kwargs, var=self._var)
+        Instance(self._graph, ActionType.Unpersist, [self, *args], kwargs, var=self._var, scope=self._scope)
         return self
 
 #--------------------------------------------------
 # InstanceProperty
 #--------------------------------------------------
 
 class InstanceProperty(Producer):
-    def __init__(self, graph:'Graph', instance:Instance, name:str, var=None):
-        super().__init__(graph, ["or_"])
+    def __init__(self, graph:'Graph', instance:Instance, name:str, var=None, scope:str=""):
+        super().__init__(graph, ["or_", "in_", "add", "extend", "choose"])
         self._instance = instance
-        self._prop = build.property_named(name, instance._action.types)
+        self._prop = build.property_named(scope+name, instance._action.types)
         self._var = var or Var(self._prop.type, name=name)
-        new = Instance(self._graph, ActionType.Get, [instance], {name: self._var})
+        self._scope = scope
+        new = Instance(self._graph, ActionType.Get, [instance], {name: self._var}, scope=self._scope)
         self._action = new._action
 
     def __call__(self, *args, **kwargs):
         raise Exception("Properties can't be called")
 
     def _make_sub(self, name: str, existing=None):
+        if existing is not None and existing._instance._context is self._graph._stack.active():
+            return existing
         return getattr(Instance(self._graph, ActionType.Get, [self], {}), name)
 
     def or_(self, other):
         self._graph._remove_action(self._action)
-        self._graph.rel.pyrel_default(self._prop, other, self._instance, self)
+        rel.pyrel_default(self._prop, other, self._instance, self)
         return self
 
+    def in_(self, others):
+        other_rel = InlineRelation(self._graph, [(x,) for x in others])
+        return self == other_rel
+
+    def _remove_if_unused(self):
+        # When calling append/extend we aren't necessarily doing a get on the property,
+        # but we will already have added one. If we're the only thing using this get,
+        # we remove it so that it doesn't unnecessarily constrain the query.
+        remove = True
+        for item in reversed(self._graph._stack.items):
+            if item is self._action:
+                break
+            elif isinstance(item, Action):
+                if self._var in item.vars():
+                    remove = False
+                    break
+        if remove:
+            self._graph._remove_action(self._action)
+
+    def add(self, other):
+        self._remove_if_unused()
+        self._graph._check_property(self._prop, multi_valued=True)
+        rel = Action(ActionType.Bind, to_var(self._instance), [], {self._prop: to_var(other)})
+        self._graph._action(rel)
+
+    def extend(self, others):
+        self._remove_if_unused()
+        self._graph._check_property(self._prop, True)
+        for other in others:
+            rel = Action(ActionType.Bind, to_var(self._instance), [], {self._prop: to_var(other)})
+            self._graph._action(rel)
+
+    def choose(self, num, unique=True):
+        self._remove_if_unused()
+        items = [getattr(Instance(self._graph, ActionType.Get, [self._instance], {}), self._prop.name) for ix in range(num)]
+        if unique:
+            for ix in range(num-1):
+                items[ix] < items[ix+1]
+        return items
+
 #--------------------------------------------------
 # Expression
 #--------------------------------------------------
 
 class Expression(Producer):
     def __init__(self, graph:'Graph', op:mType|Task, args:List[Any]):
+
         super().__init__(graph, [])
         self._var = None
 
         # For calls to tasks with known signatures, normalize their arguments by
         # throwing on missing inputs or constructing vars for missing outputs
         if op.properties and not op.isa(Builtins.Anonymous):
             for prop, arg in zip_longest(op.properties, args):
                 if arg is None:
                     if prop.is_input:
                         raise TypeError(f"{op.name} is missing a required argument: '{prop.name}'")
                     else:
                         args.append(Var(prop.type, name=prop.name))
 
             # Expose the last output as the result, to ensure we don't double-create it in _use_var.
-            # @NOTE: Literal values like 1 show up here from calls like `graph.rel.range(0, len(df), 1)`
+            # @NOTE: Literal values like 1 show up here from calls like `rel.range(0, len(df), 1)`
             if not op.properties[-1].is_input and isinstance(args[-1], Var):
                 self._var = args[-1]
 
         self._expr = build.call(op, args)
-        self._add_action(self._expr)
+        self._graph._action(self._expr)
 
     def __call__(self, *args, **kwargs):
         raise Exception("Expressions can't be called")
 
     def _use_var(self):
         if not self._var:
             self._var = Var(Builtins.Unknown)
@@ -539,42 +675,69 @@
     def _make_sub(self, name: str, existing=None):
         return None
 
 #--------------------------------------------------
 # RelationNS
 #--------------------------------------------------
 
-class RelationNS(Producer):
-    def __init__(self, graph:'Graph', ns:List[str], name:str):
-        super().__init__(graph, ["add"])
+unsafe_symbol_pattern = re.compile(r"[^a-zA-Z0-9_]", re.UNICODE)
+def safe_symbol(name: str):
+    return f':"{name}"' if unsafe_symbol_pattern.search(name) else f":{name}"
+
+class RelationNS():
+    def __init__(self, ns:List[str], name:str, use_rel_namespaces=False):
+        if name == "getdoc":
+            rich.print("[red bold]GETDOC CALLED")
+            traceback.print_stack()
+            return
         self._name = name
         self._ns = ns
+        self._subs = {}
+        self._use_rel_namespaces = use_rel_namespaces
+        self._rel = self._build_rel()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
-        name = ":".join([*self._ns, self._name])
-        op = build.relation(name, len(args))
-        return Expression(self._graph, op, list(args))
+        op = self._rel
+        self._ensure_args(len(args))
+        return Expression(get_graph(), op, list(args))
+
+    def __getattribute__(self, __name: str) -> Any:
+        if __name.startswith("_") or __name in ["add"]:
+            return object.__getattribute__(self, __name)
+        self._subs[__name] = self._make_sub(__name, self._subs.get(__name))
+        return self._subs[__name]
 
     def _make_sub(self, name: str, existing=None):
-        if existing:
+        if existing is not None:
             return existing
         ns = self._ns[:]
         if self._name:
             ns.append(self._name)
-        return RelationNS(self._graph, ns, name)
+        return RelationNS(ns, name, use_rel_namespaces=self._use_rel_namespaces)
+
+    def _build_rel(self, arg_count = 0):
+        fqn_parts = self._ns + [self._name]
+        if self._use_rel_namespaces:
+            return build.relation('::'+'::'.join(fqn_parts), arg_count)
+        if len(fqn_parts) == 1:
+            return build.relation(fqn_parts[0], arg_count)
+        else:
+            return build.relation(f"{fqn_parts[0]}[{', '.join(safe_symbol(part) for part in fqn_parts[1:])}]", arg_count)
+
+    def _ensure_args(self, arg_count):
+        if len(self._rel.properties) <= arg_count:
+            self._rel.properties = [Builtins.Relation.properties[i] for i in range(arg_count)]
 
     def add(self, *args):
-        name = ":".join([*self._ns, self._name])
-        op = build.relation(name, len(args))
-        self._graph._action(build.relation_action(ActionType.Bind, op, list(args)))
+        op = self._rel
+        self._ensure_args(len(args))
+        get_graph()._action(build.relation_action(ActionType.Bind, op, list(args)))
 
     def _to_var(self):
-        name = ":".join([*self._ns, self._name])
-        rel = build.relation(name, 0)
-        return Var(Builtins.Relation, value=rel)
+        return Var(Builtins.Relation, value=self._build_rel())
 
 #--------------------------------------------------
 # RawRelation
 #--------------------------------------------------
 
 class RawRelation(Producer):
     def __init__(self, graph:'Graph', name:str, arity:int):
@@ -687,89 +850,72 @@
         new_bytecode.argnames = func.__code__.co_varnames
         new_bytecode.docstring = func.__doc__
         new_bytecode.name = func.__name__
 
         for instr in original_bytecode:
             if isinstance(instr, Instr) and instr.name == "RETURN_VALUE":
                 # Insert a call to the ret function before the return instruction
-                new_bytecode.extend([
-                    Instr("STORE_FAST", "______x"),
-                    Instr("LOAD_GLOBAL", (True, "ret")),
-                    Instr("LOAD_FAST", "______x"),
-                    Instr("PRECALL", 0),
-                    Instr("CALL", 1),
-                ])
+                if sys.version_info < (3, 11): # 3.10
+                    new_bytecode.extend([
+                        Instr("STORE_FAST", "______x"),
+                        Instr("LOAD_GLOBAL", "ret"),
+                        Instr("LOAD_FAST", "______x"),
+                        Instr("CALL_FUNCTION", 1),
+                    ])
+                elif sys.version_info < (3, 12): # 3.11
+                    new_bytecode.extend([
+                        Instr("STORE_FAST", "______x"),
+                        Instr("LOAD_GLOBAL", (True, "ret")),
+                        Instr("LOAD_FAST", "______x"),
+                        Instr("PRECALL", 0),
+                        Instr("CALL", 1),
+                    ])
+                else: #3.12+
+                    new_bytecode.extend([
+                        Instr("STORE_FAST", "______x"),
+                        Instr("LOAD_GLOBAL", (True, "ret")),
+                        Instr("LOAD_FAST", "______x"),
+                        Instr("CALL", 1),
+                    ])
             else:
                 new_bytecode.append(instr)
 
         # Create a new code object from the modified bytecode
         new_bytecode.append(Instr("RETURN_VALUE"))
         new_code = new_bytecode.to_code()
 
         # Create a new function from the new code object with the correct globals
         new_func = type(func)(new_code, func.__globals__, func.__name__, func.__defaults__, func.__closure__)
 
         # Update the globals dictionary of the new function to include 'ret'
         name = f"{schema}.{func.__name__}" if schema else func.__name__
         ctx = Context(model, exec_type=TaskExecType.Procedure, name=name, outputs=output_types, **kwargs)
         with ctx as ret:
-            inputs = to_list(model.Vars(len(arg_names)))
+            inputs = to_list(Vars(len(arg_names)))
             ctx._inputs = list(zip(arg_names, [to_var(i) for i in inputs], input_types))
             # Get the bytecode of the original function
             new_func.__globals__["ret"] = ret
             # Call the new function with the provided arguments
             new_func(*inputs)
 
         def wrapper():
             raise Exception("Exports can't be called directly. They are exported to the underlying platform")
 
         return wrapper
     return decorator
 
 #--------------------------------------------------
-# Aggregates
-#--------------------------------------------------
-
-class Aggregates():
-    def __init__(self, graph:'Graph'):
-        self._graph = graph
-        self.rank_desc_def = build.aggregate_def("reverse_sort")
-        self.rank_desc_def.parents.append(Builtins.Extender)
-        self.rank_asc_def = build.aggregate_def("sort")
-        self.rank_asc_def.parents.append(Builtins.Extender)
-
-    def count(self, *args, per=[]) -> Any:
-        return Expression(self._graph, Builtins.count, [args, per])
-
-    def sum(self, *args, per=[]) -> Any:
-        return Expression(self._graph, Builtins.sum, [args, per])
-
-    def avg(self, *args, per=[]) -> Any:
-        return Expression(self._graph, Builtins.avg, [args, per])
-
-    def min(self, *args, per=[]) -> Any:
-        return Expression(self._graph, Builtins.min, [args, per])
-
-    def max(self, *args, per=[]) -> Any:
-        return Expression(self._graph, Builtins.max, [args, per])
-
-    def rank_asc(self, *args, per=[]) -> Any:
-        return Expression(self._graph, self.rank_asc_def, [args, per])
-
-    def rank_desc(self, *args, per=[]) -> Any:
-        return Expression(self._graph, self.rank_desc_def, [args, per])
-
-#--------------------------------------------------
 # RuleStack
 #--------------------------------------------------
 
 class RuleStack():
-    def __init__(self):
+    def __init__(self, graph:'Graph'):
         self.items = []
         self.stack = []
+        self._graph = graph
 
     def push(self, item):
         self.stack.append(item)
         self.items.append(("push", item))
 
     def pop(self, item):
         self.stack.pop()
@@ -777,26 +923,38 @@
         if len(self.stack) == 0:
             compacted = self.compact()
             self.items.clear()
             if len(compacted.items):
                 return compacted
 
     def active(self):
-        return self.stack[-1]
+        try:
+            cur = self.stack[-1]
+            if cur is self._graph._temp_rule:
+                Errors.out_of_context(Errors.call_source())
+            return cur
+        except IndexError:
+            Errors.out_of_context(Errors.call_source())
 
     def _expression_start(self, buffer, single_use_vars):
         consume_from = -1
+        if not len(buffer):
+            return consume_from
         # we can only pull vars if their only use is for this condition
         used_vars = set(buffer[-1].requires_provides()[0] & single_use_vars)
         # walk buffer in reverse collecting vars in the action until we get one
         # that doesn't provide a var we care about
         for action in reversed(buffer[:-1]):
             if not isinstance(action, Action):
                 break
-            req, provs = action.requires_provides()
+            req, provs, _ = action.requires_provides()
+            # don't pull in vars the represent root entities even though they're provided
+            # by gets. This prevents scenarios where p = Person() would get pulled in if you
+            # did with p.age > 10:
+            provs = provs - {action.entity}
             if len(used_vars.intersection(provs)):
                 used_vars.update(req & single_use_vars)
                 consume_from -= 1
             else:
                 break
         return consume_from
 
@@ -846,76 +1004,136 @@
                 stack.append(task)
 
             elif op == "pop":
                 cur = stack.pop()
                 cur.items.extend(buffer)
                 buffer.clear()
                 if not len(stack):
-                    cur.normalize()
+                    if not self._graph._config.get("compiler.use_v2", False):
+                        cur.normalize()
                     return cur
                 if isinstance(value, Context) and value._op:
                     stack[-1].items.append(build.call(value._op, [Var(value=value._args), Var(Builtins.Task, value=cur)]))
                 else:
                     stack[-1].items.append(build.call(cur, list(cur.bindings.values())))
 
         raise Exception("No task found")
 
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
+locals = threading.local()
+locals.graph_stack = []
+
+def get_graph():
+    _ensure_stack()
+    if not len(locals.graph_stack):
+        raise Exception("Outside of a model context")
+    return locals.graph_stack[-1]
+
+def _ensure_stack():
+    if not hasattr(locals, "graph_stack"):
+        locals.graph_stack = []
+    return locals.graph_stack
+
+rel = RelationNS([], "")
+global_ns = RelationNS([], "", use_rel_namespaces=True)
+
+def alias(ref:Any, name:str):
+    var = to_var(ref)
+    var.name = name
+    return var
+
+def Vars(count) -> Any:
+    if count == 1:
+        return Instance(get_graph(), ActionType.Get, [], {}, Var(Builtins.Unknown))
+    return [Instance(get_graph(), ActionType.Get, [], {}, Var(Builtins.Unknown)) for _ in range(count)]
+
 class Graph:
     def __init__(self, client, name:str):
         self.name = name
-        self._types = {}
-        self._stack = RuleStack()
-        self._temp_rule = Context(self, source_steps=2)
-        debugging.set_source(self._temp_rule._task, 2)
+        self._stack = RuleStack(self)
+        self._temp_rule = Context(self)
         self._executed = []
         self._client = client
-        self.rel = RelationNS(self, [], "")
-        self.aggregates = Aggregates(self)
+        self._config = client.resources.config
         self.resources = client.resources
+        self._graph_stack = _ensure_stack()
+        self._prop_is_multi = {}
 
+        self._graph_stack.append(self)
         self._stack.push(self._temp_rule)
 
     #--------------------------------------------------
     # Rule stack
     #--------------------------------------------------
 
     def _push(self, item):
+        self._graph_stack.append(self)
         if self._temp_rule:
-            self._pop(self._temp_rule)
+            self._pop(self._temp_rule, is_temp=True)
             self._temp_rule = None
         self._stack.push(item)
 
-    def _pop(self, item):
+    def _pop(self, item, exec=True, is_temp=False):
+        self._graph_stack.pop()
         task = self._stack.pop(item)
-        if task:
+        if exec and task:
             self._exec(item, task)
-
-    def _action(self, action, pre=False):
-        if pre:
-            self._stack.items.insert(-1,action)
-        else:
-            self._stack.items.append(action)
+        if not is_temp and not len(self._stack.stack):
+            self._temp_rule = Context(self)
+            self._graph_stack.append(self)
+            self._stack.push(self._temp_rule)
+
+    def _action(self, action:Action|List[Action]):
+        if isinstance(action, list):
+            for a in action:
+                self._action(a)
+            return
+        self._stack.items.append(action)
 
     def _remove_action(self, action):
         self._stack.items.remove(action)
 
     def _exec(self, context:Context, task):
         if context._exec_type == TaskExecType.Rule:
             self._client.install(f"rule{len(self._executed)}", context._task)
         elif context._exec_type == TaskExecType.Query:
             context.results = self._client.query(context._task)
         elif context._exec_type == TaskExecType.Procedure:
-            self._client.export_udf(context._name, context._inputs, context._outputs, context._task)
+            self._client.export_udf(context._name, context._inputs, context._outputs, context._task, context._engine)
         self._executed.append(context)
 
     #--------------------------------------------------
+    # Property handling
+    #--------------------------------------------------
+
+    def _check_property(self, prop:mProperty, multi_valued=False, unknown_cardinality=False):
+        name = prop.name
+        if name in RESERVED_PROPS:
+            Errors.reserved_property(Errors.call_source(), name)
+
+        if not self._config.get("compiler.use_multi_valued", False):
+            if multi_valued:
+                raise Exception(f"Multi-valued properties aren't enabled. Trying to use a property `{name}` as a multi-valued property")
+            return
+        elif unknown_cardinality:
+            return
+
+        if name in self._prop_is_multi:
+            if self._prop_is_multi[name] != multi_valued:
+                raise Exception(f"Trying to use a property `{name}` as both singular and multi-valued")
+        else:
+            self._prop_is_multi[name] = multi_valued
+        if not multi_valued and Builtins.FunctionAnnotation not in prop.parents:
+            prop.parents.append(Builtins.FunctionAnnotation)
+
+
+    #--------------------------------------------------
     # Public API
     #--------------------------------------------------
 
     def Type(self, name:str):
         return Type(self, name)
 
     def rule(self, **kwargs):
@@ -938,33 +1156,28 @@
 
     def union(self, **kwargs):
         return Context(self, behavior=Behavior.Union, **kwargs)
 
     def ordered_choice(self, **kwargs):
         return Context(self, behavior=Behavior.OrderedChoice, **kwargs)
 
-    def Vars(self, count) -> Any:
-        if count == 1:
-            return Instance(self, ActionType.Get, [], {}, Var(Builtins.Unknown))
-        return [Instance(self, ActionType.Get, [], {}, Var(Builtins.Unknown)) for _ in range(count)]
-
-    def alias(self, ref:Any, name:str):
-        var = to_var(ref)
-        var.name = name
-        return var
+    def read(self, name:str, **kwargs):
+        from relationalai.loaders.loader import read_resource_context # We do the late import to break an dependency cycle
+        return read_resource_context(self, name, **kwargs)
 
     def load_raw(self, path:str):
         if os.path.isfile(path):
             if path.endswith('.rel'):
                 self._client.load_raw_file(path)
         elif os.path.isdir(path):
             for root, _, files in os.walk(path):
                 for file in files:
                     if file.endswith('.rel'):
                         file_path = os.path.join(root, file)
                         self._client.load_raw_file(file_path)
 
-    def exec_raw(self, code:str, readonly=True, raw_results=True):
-        return self._client.exec_raw(code, readonly=readonly, raw_results=raw_results)
+    def exec_raw(self, code:str, readonly=True, raw_results=True, inputs:dict|None = None):
+        return self._client.exec_raw(code, readonly=readonly, raw_results=raw_results, inputs=inputs)
 
     def install_raw(self, code:str, name:str|None=None):
         self._client.install_raw(code, name)
+
```

### Comparing `relationalai-0.1.9/src/relationalai/errors.py` & `relationalai-0.2.0/src/relationalai/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-
-
 import ast
+import io
 import textwrap
 from .metamodel import Action, Task
 from . import debugging
 from rich.console import Console
 
 #--------------------------------------------------
 # Print helpers
 #--------------------------------------------------
 
+def rich_str(string:str, style:str|None = None) -> str:
+    output = io.StringIO()
+    console = Console(file=output, force_terminal=True)
+    console.print(string, style=style)
+    return output.getvalue()
+
 def body_text(console, body:str):
     body = textwrap.dedent(body)
     for line in body.splitlines():
         if not line.startswith("  "):
             console.print(line)
         else:
             console.print(line, soft_wrap=True)
@@ -43,15 +48,15 @@
     body_text(console, content)
     console.print()
     console.print(f'[red]{"-" * 80}')
     console.print()
 
 def print_error(name:str, content:str):
     fixed_content_length = len(name) + 2  # 2 for the spaces around the dash
-    num_dashes = 74 - fixed_content_length
+    num_dashes = 76 - fixed_content_length
     dashes = '-' * num_dashes
     console = Console(width=80)
     console.print(f"[red]--- {name} {dashes}")
     body_text(console, content)
     console.print()
     console.print(f'[red]{"-" * 80}')
     console.print()
@@ -104,20 +109,43 @@
             if hasattr(node, 'type_comment'):
                 expr_node.type_comment = node.type_comment
 
             return expr_node
         return node
 
 #--------------------------------------------------
+# Exceptions
+#--------------------------------------------------
+
+class RAIException(Exception):
+    def __init__(self, message:str):
+        self.message = message
+
+    def __str__(self):
+        return self.message
+
+class RelQueryError(Exception):
+    def __init__(self, problems):
+        super().__init__("Rel query error")
+        self.problems = problems
+
+    def pprint(self):
+        body = "\n\n".join(f'{problem["error_code"]}\n{problem["report"]}\n{problem["message"]}'
+                           for problem in self.problems)
+        return f"Rel query error\n{body}"
+
+#--------------------------------------------------
 # Errors
 #--------------------------------------------------
 
 class Errors:
     @staticmethod
-    def call_source(steps):
+    def call_source(steps=None):
+        if steps is None:
+            return debugging.capture_code_info()
         return debugging.capture_code_info(steps + 1)
 
     #--------------------------------------------------
     # DSL invalid python errors
     #--------------------------------------------------
 
     @staticmethod
@@ -202,14 +230,47 @@
 
         Or maybe you meant [green]==[/green] instead?
 
         {compare}
         """
         print_source_error(source, "Invalid property set", content)
 
+    @staticmethod
+    def invalid_bool(source):
+        marked = mark_source(source, source.line, source.line)
+        content = f"""
+        In a RelationalAI query, the truth values of Producer objects are unknown
+        until the query has been evaluated. You may not use Producers in boolean
+        expressions, such as those involving [green]if[/green], [green]while[/green], [green]and[/green], [green]or[/green], and [green]not[/green]:
+
+        {marked}
+
+        Producer objects include:
+
+        - [green]Instance[/green] objects, such as [green]person[/green].
+        - [green]InstanceProperty[/green] objects, such as [green]person.age[/green].
+        - [green]Expresion[/green] objects, such as [green]person.age >= 18[/green].
+        """
+        print_source_error(source, "Invalid boolean expression with Producer", content)
+
+    #--------------------------------------------------
+    # DSL scope errors
+    #--------------------------------------------------
+
+    @staticmethod
+    def out_of_context(source):
+        marked = mark_source(source, source.line, source.line)
+        content = f"""
+        Looks like this [yellow]object[/yellow] is being used outside of a rule or query.
+
+        {marked}
+        """
+        print_source_error(source, "Outside of context", content)
+        exit()
+
     #--------------------------------------------------
     # DSL reserved errors
     #--------------------------------------------------
 
     @staticmethod
     def reserved_property(source, property_name:str):
         marked = mark_source(source, source.line, source.line)
@@ -229,23 +290,49 @@
     def snowflake_app_missing(app_name):
         content = f"""
         The [yellow]{app_name}[/yellow] app doesn't appear to be installed in this snowflake account.
 
         If it's installed under a different name, run [green]`rai init`[/green] on the command line and you can set the app name.
         """
         print_error("Couldn't find RelationalAI", content)
-        exit(1)
+        raise RAIException("Couldn't find RelationalAI snowflake application") from None
 
     @staticmethod
     def snowflake_import_missing(source, import_name:str, model_name:str):
         marked = mark_source(source, source.line, source.line)
         content = f"""
         The Snowflake object [yellow]{import_name}[/yellow] hasn't been imported into RAI.
 
         {marked}
 
         You can create an import for it using the rai cli:
 
-          [green]rai imports:stream --object {import_name} --model {model_name}[/green]
+          [green]rai imports:stream --source {import_name} --model {model_name}[/green]
         """
         print_source_error(source, "Couldn't find import", content)
-        exit(1)
+        raise RAIException("Couldn't find import") from None
+
+    @staticmethod
+    def snowflake_change_tracking_not_enabled(obj:str, sql:str):
+        content = f"""
+        Change tracking isn't enabled for [yellow]{obj}[/yellow].
+
+        To enable change tracking, you'll need to run the following SQL:
+
+        [green]{sql}[/green]
+        """
+        print_error("Change tracking not enabled", content)
+        raise RAIException("Change tracking not enabled") from None
+
+    #--------------------------------------------------
+    # Engine errors
+    #--------------------------------------------------
+
+    @staticmethod
+    def engine_not_found(name:str, message:str):
+        content = f"""
+        The engine [yellow]{name}[/yellow] isn't available. You can start the engine with the following command:
+
+        [green]rai engines:create --name {name}[/green]
+        """
+        print_error("Engine unavailable", content)
+        raise RAIException(message) from None
```

### Comparing `relationalai-0.1.9/src/relationalai/metagen.py` & `relationalai-0.2.0/src/relationalai/metagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import textwrap
 import time
 from typing import List, Dict, Tuple, Any, Iterable, cast
 from .metamodel import Agent, Base, Namer, Task, Var, Value, Property, Action, ActionType, AllItems, Behavior, Builtins, Type
 from . import debugging
 from .clients import test
+from .clients.config import Config
 import random
 import rich
 import json
 
 DEBUG = False
 
 #--------------------------------------------------
@@ -234,15 +235,15 @@
         types = []
         for t in self.used_types:
             t_name = self.emit(t)
             types.append(f"{t_name} = model.Type(\"{t_name}\")")
         lines = [
             "import relationalai as rai",
             "",
-            "model = rai.clients.test.Graph(\"gentest\")",
+            "model = rai.clients.test.Graph(\"gentest\", config=config)",
             "",
             *types
         ]
         return "\n".join(lines)
 
     def emit_doc(self, tasks:List[Task]) -> str:
         task_code = []
@@ -366,14 +367,15 @@
 class Gen:
     def __init__(self, seed, profile:GenProfile = GenProfile()):
         self.seed = seed
         self.random = random.Random(seed)
         self.eq = Eq()
         self.emitter = PyRelEmitter()
         self.profile = profile
+        self.config = Config()
 
         self.types = []
         for _ in range(self.rand_range(self.profile.types)):
             self.types.append(self.type())
         for t in self.types:
             t.properties = [self.property() for _ in range(self.rand_range(self.profile.type_properties))]
 
@@ -582,18 +584,23 @@
         code = self.emitter.emit_doc([expected])
         stats.emit_time += time.perf_counter() - emit_start
         actual = None
         exception = None
 
         try:
             exec_time = time.perf_counter()
-            exec(code, None, None)
+            exec(code, {"config": self.config}, None)
             result = test.proxied_clients.pop()
             if len(result.blocks):
-                actual = result.blocks[0].task
+                # When use_value_types is active, the first task is installing all the types
+                if self.config.get("compiler.use_value_types", None):
+                    actual = result.blocks[1].task
+                else:
+                    actual = result.blocks[0].task
+                actual.normalize()
             stats.exec_time += time.perf_counter() - exec_time
 
         except Exception:
             output = io.StringIO()
             console = rich.console.Console(file=output, force_terminal=True)
             console.print_exception(extra_lines=0)
             exception = output.getvalue()
@@ -688,15 +695,15 @@
         return True
 
     #--------------------------------------------------
     # Metamodel eq
     #--------------------------------------------------
 
     def type(self, a:Type, b:Type):
-        return self.eq_attrs(a, b, ['name', 'parents'])
+        return self.eq_attrs(a, b, ['name'])
 
     def property(self, a:Property, b:Property):
         # return self.eq_attrs(a, b, ['name', 'type', 'is_input'])
         return self.eq_attrs(a, b, ['name'])
 
     def task(self, task:Task, b:Task):
         return self.eq_attrs(task, b, ["name", "parents", "behavior", "items"])
```

### Comparing `relationalai-0.1.9/src/relationalai/metamodel.py` & `relationalai-0.2.0/src/relationalai/metamodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 UnknownType = Type("Unknown")
 
 @dataclass
 class Property(Base):
     name: str
     type: Type
     is_input: bool = False
+    parents: List[Type] = field(default_factory=list)
 
     def __hash__(self) -> int:
         return self.id
 
     @staticmethod
     def find(name:str, types:List[Type]) -> Optional['Property']:
         found = None
@@ -116,14 +117,39 @@
             if i.action == ActionType.Bind and i.entity.value == Builtins.Return:
                 cols = []
                 for (prop, var) in i.bindings.items():
                     cols.append(namer.get(var) or namer.get(prop))
                 return cols
         return []
 
+    def has_persist(self, seen=None) -> bool:
+        if seen is None:
+            seen = set()
+        for i in self.items:
+            if i.action in [ActionType.Persist, ActionType.Unpersist]:
+                return True
+            vs = i.vars()
+            for v in vs:
+                if v not in seen:
+                    seen.add(v)
+                    if v.value and isinstance(v.value, Task) and v.value.has_persist(seen):
+                        return True
+        return False
+
+    def requires_provides(self, seen = None) -> Tuple[Set['Var'], Set['Var'], Set['Var']]:
+        sub_requires = set()
+        sub_provides = set()
+        refs = set()
+        for i in self.items:
+            r, p, sub_refs = i.requires_provides(seen)
+            sub_requires.update(r)
+            sub_provides.update(p)
+            refs.update(p | sub_refs)
+        return sub_requires - sub_provides, sub_provides, refs
+
     def normalize(self):
         entity_action:Dict[Any, Action] = {}
         seen = set()
         collapsed:List[Action] = []
         for i in self.items:
             if i in seen:
                 continue # prevent duplicates
@@ -156,37 +182,49 @@
                         exists = True
                 if not exists:
                     found.types.extend([x for x in i.types if x not in found.types])
                     found.bindings.update(i.bindings)
                 else:
                     collapsed.append(i)
 
-        try:
-            self.items = Utils.sort(collapsed)
-        except Exception:
-            rich.print("[red bold]Stratification failed[/red bold][red]\nThings may not work correctly. Please send us this program so we can take a look!\n")
+        if self.behavior == Behavior.Query:
+            try:
+                self.items = Utils.sort(collapsed)
+            except Exception:
+                rich.print("[red bold]Stratification failed[/red bold][red]\nThings may not work correctly. Please send us this program so we can take a look!\n")
+                self.items = collapsed
+        else:
             self.items = collapsed
 
 #--------------------------------------------------
 # Var
 #--------------------------------------------------
 
-Value = Union[str, numbers.Number, bool, Task, Property, Type, bytes,
+Value = Union[str, numbers.Number, int, float, bool, Task, Property, Type, bytes,
               datetime, date, List['Value'], List['Var']]
 
 @dataclass
 class Var(Base):
     id: int = field(default_factory=next_id, init=False)
     type: Type = UnknownType
     name: Optional[str] = None
     value: Optional[Value] = None
 
     def __hash__(self) -> int:
         return self.id
 
+    def __eq__(self, other: object) -> bool:
+        if type(other) != Var:
+            return False
+        if super().__eq__(other):
+            return True
+        if other.value is not None and self.value is not None:
+            return other.value is self.value
+        return False
+
     def isa(self, other: Type) -> bool:
         return bool(self.type.isa(other) or (self.value and isinstance(self.value, Type) and self.value.isa(other)))
 
 #--------------------------------------------------
 # Action
 #--------------------------------------------------
 
@@ -195,78 +233,106 @@
     Call = "call"
     Persist = "persist"
     Unpersist = "unpersist"
     Bind = "bind"
     Construct = "construct"
 
     def is_effect(self):
-        return self in [ActionType.Bind, ActionType.Persist, ActionType.Unpersist, ActionType.Construct]
+        return self in [ActionType.Bind, ActionType.Persist, ActionType.Unpersist]
 
 @dataclass
 class Action(Base):
     action: ActionType
     entity: Var
     types: List[Type] = field(default_factory=list)
     bindings: Dict[Property, Var] = field(default_factory=dict)
 
-    def requires_provides(self, seen = None) -> Tuple[Set[Var], Set[Var]]:
+    def requires_provides(self, seen = None) -> Tuple[Set[Var], Set[Var], Set[Var]]:
         requires = set()
         provides = set()
+        refs = set()
         if not seen:
             seen = set()
         if self in seen:
-            return requires, provides
+            return requires, provides, refs
 
         seen.add(self)
-        if isinstance(self.entity.value, Task) and len(self.entity.value.items):
+        is_sub_task = self.is_subtask_call()
+        if is_sub_task:
             sub_requires = set()
             sub_provides = set()
             for i in self.entity.value.items:
-                r, p = i.requires_provides(seen)
+                r, p, sub_refs = i.requires_provides(seen)
                 sub_requires.update(r)
                 sub_provides.update(p)
+                refs.update(p | sub_refs)
             requires.update(sub_requires - sub_provides)
 
         if self.action == ActionType.Get and self.entity.value is None:
             if len(self.types):
                 provides.add(self.entity)
             else:
                 requires.add(self.entity)
         elif self.action != ActionType.Call and self.entity.value is None:
             requires.add(self.entity)
 
-        for k,var in self.bindings.items():
+        items = [*self.bindings.items()]
+        if self.action == ActionType.Construct:
+            provides.add(items[-1][1])
+            items = items[:-1]
+
+        for k,var in items:
             into = provides
-            if self.action == ActionType.Bind:
+            if self.action in [ActionType.Bind, ActionType.Persist, ActionType.Unpersist, ActionType.Construct]:
                 into = requires
             elif k.is_input:
                 into = requires
 
             if var.value is not None and isinstance(var.value, list):
                 for v in var.value:
                     if isinstance(v, Var) and v.value is None:
                         into.add(v)
             elif var.value is None:
                 into.add(var)
 
-        return requires - provides, provides
+        refs.update(requires)
+        return requires - provides, provides, refs
 
-    def vars(self) -> Set[Var]:
+    def vars(self, recursive=False) -> Set[Var]:
         vars = set(self.bindings.values())
         vars.add(self.entity)
+        if recursive:
+            for v in list(vars):
+                if isinstance(v.value, list):
+                    for var in v.value:
+                        if isinstance(var, Var) and var.value is None:
+                            vars.add(var)
         return vars
 
+    def is_subtask_call(self) -> bool:
+        return self.action == ActionType.Call \
+                and isinstance(self.entity.value, Task) \
+                and len(self.entity.value.items) > 0
+
     def append(self, item: Union[Type, Property, Task, Agent, Var], var: Optional[Var] = None):
         if isinstance(item, Type):
             self.types.append(item)
         elif isinstance(item, Property) and var:
             self.bindings[item] = var
         elif isinstance(item, Var):
             self.entity = item
 
+    def equiv(self, other: 'Action') -> bool:
+        if self is other:
+            return True
+        return self.action == other.action \
+                and self.entity == other.entity \
+                and self.types == other.types \
+                and self.bindings == other.bindings
+
     def __hash__(self) -> int:
         return self.id
 
 #--------------------------------------------------
 # All
 #--------------------------------------------------
 
@@ -284,45 +350,57 @@
         self.Any = Type("Any")
         self.String = Type("String", parents=[self.Primitive])
         self.Number = Type("Number", parents=[self.Primitive])
         self.Int = Type("Int", parents=[self.Number])
         self.Decimal = Type("Decimal", parents=[self.Number])
         self.Bool = Type("Bool", parents=[self.Primitive])
         self.Type = Type("Type", parents=[self.Primitive])
+        self.ValueType = Type("ValueType", parents=[self.Type])
         self.Symbol = Type("Type", parents=[self.Primitive])
         self.Relation = Type("Relation", parents=[self.Primitive], properties=[Property(f"v{id}", self.Any) for i in range(1000)])
         self.Anonymous = Type("Anonymous") # A thing we assume to exist in the host DB for which we don't have information.
         self.Task = Type("Task", parents=[self.Type, self.Relation])
         Task._task_builtin = self.Task
+        self.Install = Task("Install", parents=[self.Task], properties=[Property("item", self.Any)])
         self.Return = Type("Return", parents=[self.Relation], properties=[Property(f"v{id}", self.Any) for i in range(20)])
         self.RawCode = Type("RawCode", properties=[Property("code", self.String)])
         self.RawData = Type("RawData", parents=[self.Relation])
-        self.InlineRawData = Type("RawData", parents=[self.RawData])
+        self.Inline = Type("Inline", parents=[])
+        self.Intermediate = Type("Intermediate", parents=[self.Relation])
+        self.InlineRawData = Type("InlineRawData", parents=[self.RawData])
+        self.InlineExpression = Type("InlineExpression", parents=[])
         self.Aggregate = Type("Aggregate", parents=[self.Task])
         self.Extender = Type("Extender", parents=[self.Aggregate])
         self.Quantifier = Type("Quantifier", parents=[self.Task])
         self.Not = Task("Not", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
         self.Exists = Task("Exists", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
         self.Every = Task("Every", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
 
+        self.Annotation = Type("Annotation")
+        self.InlineAnnotation = Type("Inline", parents=[self.Annotation])
+        self.FunctionAnnotation = Type("Function", parents=[self.Annotation])
+
         self.Identity = Type("Identity", parents=[self.String])
         self.make_identity = Task("make_identity", properties=[
             Property("params", self.Any, True),
             Property("identity", self.Any)
         ])
 
         self.Infix = Type("Infix")
+        self.Filter = Type("Filter")
 
         def binary_op(op, with_result=False):
             t = Task(name=op, parents=[self.Infix], properties=[
                 Property("a", self.Number, True),
                 Property("b", self.Number, True),
             ])
             if with_result:
                 t.properties.append(Property("result", self.Number))
+            else:
+                t.parents.append(self.Filter)
             return t
 
         def aggregate(op):
             return Task(name=op, parents=[self.Aggregate], properties=[
                 Property("projection", self.Any, True),
                 Property("group", self.Any, True),
                 Property("result", self.Number),
@@ -374,18 +452,31 @@
 
     def relation_action(self, action_type:ActionType, op:Type|Property, params:Iterable[Any]):
         a = Action(action_type, Var(Builtins.Type, value=op))
         for ix, p in enumerate(params):
             a.append(Builtins.Relation.properties[ix], self.to_var(p))
         return a
 
-    def ident(self, action:Action):
+    def ident(self, action:Action) -> List[Action]:
         params = [Var(value=t.name) for t in action.types]
         params.extend(action.bindings.values())
-        return self.call(Builtins.make_identity, [Var(value=params), action.entity])
+        actions = []
+        ident = action.entity
+        if action.entity.isa(Builtins.ValueType):
+            ident = Var()
+            actions.append(self.construct(action.entity.type, [ident, action.entity]))
+        actions.append(self.call(Builtins.make_identity, [Var(value=params), ident]))
+        actions.reverse()
+        return actions
+
+    def install(self, item:Type|Property):
+        return self.call(Builtins.Install, [item])
+
+    def construct(self, item:Type|Property, params:List[Any]):
+        return self.relation_action(ActionType.Construct, item, params)
 
     def property_named(self, name:str, types:List[Type]):
         found = Property.find(name, types)
         if not found:
             found = Property(name, Builtins.Any)
         for t in types:
             if found not in t.properties:
@@ -561,48 +652,70 @@
         return final
 
 
 #--------------------------------------------------
 # Utils
 #--------------------------------------------------
 
-def _graph_debug(actions, in_degree):
+def _graph_debug(actions, in_degree, vars_provided_by):
     rich.print("\n[yellow bold]STRATIFY CHECK")
     for item in actions:
         print("-------------------------------------------")
         print(in_degree.get(item, 0), item)
-        (requires, provides) = item.requires_provides()
+        (requires, provides, refs) = item.requires_provides()
+        if item.is_subtask_call():
+            for ref in refs:
+                if vars_provided_by.get(ref):
+                    requires.add(ref)
         rich.print("    in:", ", ".join([str(r.id) for r in requires]))
         rich.print("    out:", ", ".join([str(p.id) for p in provides]))
+        rich.print("    refs:", ", ".join([str(r.id) for r in refs]))
 
 class Utils:
 
     @staticmethod
     def action_graph(actions:List[Action]):
         graph:Dict[Action, List[Action]] = defaultdict(list)
         in_degree:Dict[Action, int] = defaultdict(int)
         vars_provided_by:Dict[Var, List[Action]] = defaultdict(list)
         vars_required_by:Dict[Var, List[Action]] = defaultdict(list)
 
+        item_refs = {}
+        cut_vars = set()
 
         for item in actions:
-            (requires, provides) = item.requires_provides()
+            (requires, provides, refs) = item.requires_provides()
+            if item.is_subtask_call():
+                item_refs[item] = refs
             for var in provides:
-                vars_provided_by[var].append(item)
+                if var in cut_vars:
+                    vars_required_by[var].append(item)
+                else:
+                    vars_provided_by[var].append(item)
             for var in requires:
                 vars_required_by[var].append(item)
 
+            if item.entity.isa(Builtins.Aggregate) or item.entity.isa(Builtins.Relation):
+                cut_vars.update(provides)
+
+
+        # ensure that subtasks depend on any var they reference in the outer scope
+        for item, refs in item_refs.items():
+            for ref in refs:
+                if vars_provided_by.get(ref):
+                    vars_required_by[ref].append(item)
+
         for var, requirers in vars_required_by.items():
             providers = vars_provided_by.get(var, [])
             for r in requirers:
                 for provider in providers:
                     graph[provider].append(r)
                     in_degree[r] += 1
 
-        # _graph_debug(actions, in_degree)
+        # _graph_debug(actions, in_degree, vars_provided_by)
 
         return graph, in_degree
 
     #--------------------------------------------------
     # Stratify
     #--------------------------------------------------
 
@@ -628,14 +741,16 @@
                 del graph[item]
                 del in_degree[item]
 
             strata.append(current_stratum)
             current_stratum = []
 
         if graph:
+            # for item in graph:
+            #     rich.print(f"[red bold]Unresolved dependency[/red bold]: {str(item)}")
             raise ValueError("There is a cycle in the graph!")
 
         return strata
 
     #--------------------------------------------------
     # Toposort
     #--------------------------------------------------
@@ -663,8 +778,8 @@
                 if isinstance(v.value, list):
                     for var in v.value:
                         if isinstance(var, Var) and (with_values or var.value is None):
                             vars.add(var)
                 else:
                     if with_values or v.value is None:
                         vars.add(v)
-        return vars
+        return vars
```

### Comparing `relationalai-0.1.9/src/relationalai/analysis/whynot.py` & `relationalai-0.2.0/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/src/relationalai/clients/azure.py` & `relationalai-0.2.0/src/relationalai/clients/azure.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import json
 import textwrap
 from typing import Any, Tuple, List
 import base64
+from urllib.error import HTTPError
 
 from pandas import DataFrame
 import pandas as pd
 
-from ..clients.config import Config
-from ..clients.client import Client, ResourceProvider
+from ..errors import Errors, RAIException
+from ..rel_utils import assert_no_problems
+from ..loaders.loader import emit_delete_import, import_file, list_available_resources
+from .config import Config
+from .types import ImportSource, ImportSourceFile
+from .client import Client, ResourceProvider
 from .. import dsl, rel, metamodel as m
 from railib import api
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
@@ -31,26 +37,42 @@
             self._ctx = api.Context(**self.config.to_rai_config())
         return self._ctx
 
     def reset(self):
         self._ctx = None
 
     #--------------------------------------------------
+    # Generic
+    #--------------------------------------------------
+
+    def get_version(self):
+        raise Exception("Azure version not available")
+
+    #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
     def list_engines(self):
         return api.list_engines(self._api_ctx())
 
+    def get_engine(self, name:str):
+        return api.get_engine(self._api_ctx(), name)
+
     def create_engine(self, name:str, size:str, pool:str=""):
         return api.create_engine_wait(self._api_ctx(), name, size)
 
     def delete_engine(self, name:str):
         return api.delete_engine(self._api_ctx(), name)
 
+    def suspend_engine(self, name:str):
+        return api.suspend_engine(self._api_ctx(), name)
+
+    def resume_engine(self, name:str):
+        return api.resume_engine_wait(self._api_ctx(), name)
+
     #--------------------------------------------------
     # Graphs
     #--------------------------------------------------
 
     def list_graphs(self) -> List[Any]:
         return api.list_databases(self._api_ctx())
 
@@ -69,19 +91,20 @@
 
     def list_models(self, database: str, engine: str):
         return api.list_databases(self._api_ctx())
 
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         lines = []
         for (name, code) in models:
-            code = code.replace("\"", "\\\"")
             name = name.replace("\"", "\\\"")
+            assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
+
             lines.append(textwrap.dedent(f"""
             def delete:rel:catalog:model["{name}"] = rel:catalog:model["{name}"]
-            def insert:rel:catalog:model["{name}"] = \"\"\"{code}\"\"\"
+            def insert:rel:catalog:model["{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
             """))
         rel_code = "\n\n".join(lines)
         results = self.exec_raw(database, engine, rel_code, readonly=False)
         if results.problems:
             return results.problems
         return []
 
@@ -102,68 +125,97 @@
         raise Exception("Azure doesn't support exports")
 
     #--------------------------------------------------
     # Imports
     #--------------------------------------------------
 
     def list_imports(self, model:str):
-        raise Exception("Azure doesn't support imports")
+        return [*list_available_resources(self, model, self.get_default_engine_name()).values()]
 
-    def create_import_stream(self, object:str, model:str, rate = 1):
+    def create_import_stream(self, source:ImportSource, model:str, rate = 1, options: dict|None = None):
         raise Exception("Azure doesn't support import streams")
 
-    def delete_import(self, object:str, model:str):
-        raise Exception("Azure doesn't support imports")
+    def create_import_snapshot(self, source:ImportSource, model:str, options: dict|None = None):
+        assert isinstance(source, ImportSourceFile), "Azure integration only supports loading from files and URLs right now."
+        import_file(self, model, source, **(options or {}))
+
+    def delete_import(self, import_name: str, model:str):
+        res = self.exec_raw(model, self.get_default_engine_name(), emit_delete_import(import_name), False)
+        assert_no_problems(res)
 
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
-    def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True, raw_results=True):
-        return api.exec(self._api_ctx(), database, engine, raw_code, readonly=readonly)
+    def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True, raw_results=True, inputs: dict = {}):
+        try:
+            return api.exec(self._api_ctx(), database, engine, raw_code, readonly=readonly, inputs=inputs)
+        except HTTPError as err:
+            res = json.loads(err.read().decode())
+            # RAI API uses a JSON payload in the body to explain why the request failed
+            # This annotates the error with that to make the exception actually useful.
+            if "engine not found" in res.get('message', ''):
+                print("") # the SDK appears to print some stuff before the error message
+                Errors.engine_not_found(self.config.get("engine", "Unknown"), res.get('message'))
+            raise RAIException(f" {res.get('message', '')} {res.get('details', '')}")
 
     def _has_errors(self, results):
         if len(results.problems):
             for problem in results.problems:
                 if problem.get('is_error') or problem.get('is_exception'):
                     return True
 
-
     def format_results(self, results, task:m.Task) -> Tuple[DataFrame, List[Any]]:
         data_frame = DataFrame()
-        if not self._has_errors(results) and len(results.results):
+        if len(results.results):
             for result in results.results:
                 types = [t for t in result["relationId"].split("/") if t != "" and not t.startswith(":")]
                 result_frame:DataFrame = result["table"].to_pandas()
                 for i, col in enumerate(result_frame.columns):
-                    if types[i] == "UInt128":
+                    if "UInt128" in types[i]:
                         result_frame[col] = result_frame[col].apply(lambda x: base64.b64encode(x.tobytes()).decode()[:-2])
                     if types[i] == "Dates.DateTime":
                         result_frame[col] = pd.to_datetime(result_frame[col] - UNIXEPOCH, unit="ms")
                     if types[i] == "Dates.Date":
                         result_frame[col] = pd.to_datetime(result_frame[col] * MILLISECONDS_PER_DAY - UNIXEPOCH, unit="ms")
                 ret_cols = task.return_cols()
                 if len(ret_cols) and len(result_frame.columns) == len(ret_cols):
                     result_frame.columns = task.return_cols()[0:len(result_frame.columns)]
                 result["table"] = result_frame
                 if ":output" in result["relationId"]:
                     data_frame = pd.concat([data_frame, result_frame], ignore_index=True)
         return (data_frame, results.problems)
 
+    #--------------------------------------------------
+    # Transactions
+    #--------------------------------------------------
+
+    def list_transactions(self, limit:int, only_active=False):
+        raise Exception("Not implemented")
+
+    def cancel_transaction(self, transaction_id):
+        raise Exception("Not implemented")
+
+    def cancel_pending_transactions(self):
+        # all transactions are executed synchronously against azure
+        pass
+
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
-def Graph(name, dry_run=False):
-    client = Client(Resources(), rel.Compiler(), name, dry_run=dry_run)
+def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False):
+    client = Client(Resources(profile, config), rel.Compiler(config), name, dry_run=dry_run)
     client.install("pyrel_base", dsl.build.raw_task("""
         @inline
         def make_identity(x..., z) =
             hash128({x...}, x..., u) and
             hash_value_uint128_convert(u, z)
             from u
 
         @inline
         def pyrel_default[F, c](k..., v) =
             F(k..., v) or (not F(k..., _) and v = c)
+
+        bound __resource
     """))
-    return dsl.Graph(client, name)
+    return dsl.Graph(client, name)
```

### Comparing `relationalai-0.1.9/src/relationalai/clients/client.py` & `relationalai-0.2.0/src/relationalai/clients/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import atexit
 from collections import defaultdict
 from typing import Dict, List, Any, Tuple
 
 from abc import ABC, abstractmethod
 from pandas import DataFrame
-from ..clients.config import Config
-from ..compiler import Compiler
-from .. import dsl, rel, debugging, metamodel as m
 import time
 
+from .types import AvailableModel, Import, ImportSource
+from ..clients.config import Config
+from ..compiler import Compiler
+from .. import dsl, debugging, metamodel as m
 
 #--------------------------------------------------
 # InstallBatch
 #--------------------------------------------------
 
 class InstallBatch:
     def __init__(self):
@@ -53,41 +55,85 @@
 # Resources
 #--------------------------------------------------
 
 class ResourceProvider(ABC):
     def __init__(self, profile: str | None = None, config:Config|None=None):
         super().__init__()
         self.config = config or Config(profile)
+        atexit.register(self.cancel_pending_transactions)
+
+    @property
+    def platform(self):
+        return self.config.get("platform")
 
     @abstractmethod
     def reset(self):
         pass
 
     #--------------------------------------------------
+    # Generic
+    #--------------------------------------------------
+
+    @abstractmethod
+    def get_version(self):
+        pass
+
+    #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
     @abstractmethod
     def list_engines(self) -> List[Any]:
         pass
 
     @abstractmethod
+    def get_engine(self, name: str):
+        pass
+
+    @abstractmethod
     def create_engine(self, name: str, size: str, pool:str=""):
         pass
 
     @abstractmethod
     def delete_engine(self, name: str):
         pass
 
+    @abstractmethod
+    def suspend_engine(self, name: str):
+        pass
+
+    @abstractmethod
+    def resume_engine(self, name: str):
+        pass
+
+    def get_default_engine_name(self) -> str:
+        return self.config.get("engine")
+
+    #--------------------------------------------------
+    # Transactions
+    #--------------------------------------------------
+
+    @abstractmethod
+    def list_transactions(self, limit:int, only_active=False) -> List[dict]:
+        pass
+
+    @abstractmethod
+    def cancel_transaction(self, transaction_id):
+        pass
+
+    @abstractmethod
+    def cancel_pending_transactions(self):
+        pass
+
     #--------------------------------------------------
     # Graphs
     #--------------------------------------------------
 
     @abstractmethod
-    def list_graphs(self) -> List[Any]:
+    def list_graphs(self) -> List[AvailableModel]:
         pass
 
     @abstractmethod
     def get_graph(self, name:str):
         pass
 
     @abstractmethod
@@ -111,15 +157,15 @@
         pass
 
     @abstractmethod
     def delete_model(self, database: str, engine: str, name: str):
         pass
 
     #--------------------------------------------------
-    # EXports
+    # Exports
     #--------------------------------------------------
 
     @abstractmethod
     def list_exports(self, database: str, engine: str):
         pass
 
     @abstractmethod
@@ -131,117 +177,131 @@
         pass
 
     #--------------------------------------------------
     # Imports
     #--------------------------------------------------
 
     @abstractmethod
-    def list_imports(self, model:str):
+    def list_imports(self, model: str) -> list[Import]:
+        pass
+
+    @abstractmethod
+    def create_import_stream(self, source: ImportSource, model: str, rate: int, options: dict|None):
         pass
 
     @abstractmethod
-    def create_import_stream(self, object:str, model:str, rate:int):
+    def create_import_snapshot(self, source: ImportSource, model: str, options: dict|None):
         pass
 
     @abstractmethod
-    def delete_import(self, object:str, model:str):
+    def delete_import(self, import_name: str, model: str):
         pass
 
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
     @abstractmethod
-    def exec_raw(self, database: str, engine: str, raw_code: str, readonly: bool = True):
+    def exec_raw(self, database: str, engine: str, raw_code: str, readonly: bool = True, inputs={}) -> Any: # @FIXME: Better type annotation
         pass
 
     @abstractmethod
     def format_results(self, results, task:m.Task|None=None) -> Tuple[DataFrame, List[Any]]:
         pass
 
 
 #--------------------------------------------------
-# Executor
+# Client
 #--------------------------------------------------
 
 class Client():
     def __init__(self, resources:ResourceProvider, compiler:Compiler, database:str, dry_run=False):
         self.dry_run = dry_run
         self._database = database
-        self.compiler = rel.Compiler()
+        self.compiler = compiler
         self._install_batch = InstallBatch()
         self.resources = resources
 
         if not self.dry_run:
             start = time.perf_counter()
             existing = self.resources.get_graph(self._database)
             if not existing:
                 self.resources.create_graph(self._database)
                 debugging.time("create_database", time.perf_counter() - start)
 
-    def get_engine(self, name:str|None=None) -> str:
+    def get_engine_name(self, name:str|None=None) -> str:
         return str(name or self.resources.config.get("engine"))
 
-    def report_errors(self, errors:List[Any]):
-        abort = False
+    def report_errors(self, errors:List[Any], abort_on_error=True):
+        maybe_abort = False
         if len(errors):
             for problem in errors:
                 if problem.get("is_error") or problem.get("is_exception"):
-                    abort = True
+                    maybe_abort = True
                     if "message" in problem:
                         print(problem["message"])
                     if "report" in problem:
                         print(problem["report"])
-        if abort:
-            raise Exception("Rel query error")
+        if abort_on_error and maybe_abort:
+            from relationalai.errors import RelQueryError
+            raise RelQueryError(errors)
 
     def load_raw_file(self, path:str):
         content = open(path).read()
         code = self.compiler.compile(dsl.build.raw_task(content))
         self._install_batch.set(path, code)
 
-    def exec_raw(self, code:str, readonly=True, raw_results=True):
-        return self.query(dsl.build.raw_task(code), readonly=readonly, raw_results=raw_results)
+    def exec_raw(self, code:str, readonly=True, raw_results=True, inputs={}):
+        return self.query(dsl.build.raw_task(code), readonly=readonly, raw_results=raw_results, inputs=inputs)
 
     def install_raw(self, code:str, name:str="pyrel_batch_0"):
         if not name:
             name = "pyrel_batch_0"
         self.compiler.compile(dsl.build.raw_task(code))
         self._install_batch.append(name, code)
 
-    def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False) -> DataFrame|Any:
+    def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False, inputs={}) -> DataFrame|Any:
         if self._install_batch.is_dirty():
             self._install_batch_flush()
 
-        code = self.compiler.compile(task)
-        if not self.dry_run:
+        with debugging.span("query", model=self._database, task=task):
+            code = self.compiler.compile(task)
+            if task.has_persist():
+                readonly = False
+            if self.dry_run:
+                return DataFrame()
+
             start = time.perf_counter()
-            results = self.resources.exec_raw(self._database, self.get_engine(), code, readonly=readonly)
+            results = self.resources.exec_raw(self._database, self.get_engine_name(), code, readonly=readonly, inputs=inputs)
             dataframe, errors = self.resources.format_results(results, task)
             if raw_results:
                 debugging.time("query", time.perf_counter() - start, DataFrame())
+                self.report_errors(errors, abort_on_error=False)
                 return results
             self.report_errors(errors)
             debugging.time("query", time.perf_counter() - start, dataframe)
             return dataframe
-        return DataFrame()
 
     def _install_batch_flush(self):
         if not self.dry_run:
-            start = time.perf_counter()
-            code = self._install_batch.flush()
-            errors = self.resources.create_models(self._database, self.get_engine(), code)
-            self.report_errors(errors)
-            debugging.time("install_batch", time.perf_counter() - start, code="\n".join([c[1] for c in code]))
+            with debugging.span("install_batch", model=self._database):
+                start = time.perf_counter()
+                code = self._install_batch.flush()
+                errors = self.resources.create_models(self._database, self.get_engine_name(), code)
+                self.report_errors(errors)
+                debugging.time("install_batch", time.perf_counter() - start, code="\n".join([c[1] for c in code]))
 
     def install(self, name, task:m.Task):
-        code = self.compiler.compile(task)
-        self._install_batch.append("pyrel_batch_0", code)
+        with debugging.span("rule", model=self._database, task=task, name=name):
+            code = self.compiler.compile(task)
+            self._install_batch.append("pyrel_batch_0", code)
 
-    def export_udf(self, name, inputs:List[Tuple[str, m.Var, Any]], outputs, task:m.Task):
+    def export_udf(self, name, inputs:List[Tuple[str, m.Var, Any]], outputs, task:m.Task, engine=""):
         cols = task.return_cols()
         if len(outputs) != len(cols):
             raise Exception(f"Expected {len(outputs)} outputs, got {len(cols)}")
         emitted_inputs = [(name, self.compiler.emitter.emit(var), type) for (name, var, type) in inputs]
         outputs = list(zip(cols, outputs))
+        if not engine:
+            engine = self.get_engine_name()
         if not self.dry_run:
-            self.resources.create_export(self._database, self.get_engine(), name, emitted_inputs, outputs, self.compiler.compile(task))
+            self.resources.create_export(self._database, engine, name, emitted_inputs, outputs, self.compiler.compile(task))
```

### Comparing `relationalai-0.1.9/src/relationalai/clients/snowflake.py` & `relationalai-0.2.0/src/relationalai/clients/snowflake.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 from pandas import DataFrame
 
 from relationalai.clients.azure import MILLISECONDS_PER_DAY, UNIXEPOCH
 
 from ..tools.cli_controls import Spinner
 
+from ..clients.types import AvailableModel, Import, ImportSource, ImportSourceTable
 from ..clients.config import Config
 from ..clients.client import Client, ResourceProvider
 from .. import dsl, rel, metamodel as m
-from ..errors import Errors
+from ..errors import Errors, RAIException
+from .. import std
 import re
 
 USE_EXEC_ASYNC = True
 
 #--------------------------------------------------
 # Helpers
 #--------------------------------------------------
@@ -77,72 +79,103 @@
 APP_NAME = "___RAI_APP___"
 
 class Resources(ResourceProvider):
     def __init__(self, profile:str|None=None, config:Config|None=None):
         super().__init__(profile, config=config)
         self._conn = None
         self._app_name = "relationalai"
+        self._pending_transactions: list[str] = []
 
-    def _exec(self, code:str):
+    def _exec(self, code:str, params:List[Any]|None = None):
         if not self._conn:
             self._conn = snowflake.connector.connect(
-                user=self.config.get('snowsql_user'),
-                password=self.config.get('snowsql_pwd'),
+                user=self.config.get('user'),
+                password=self.config.get('password'),
                 account=self.config.get('account'),
                 warehouse=self.config.get('warehouse', ""),
                 # database=self.config.get('database', ""),
                 # schema=self.config.get('schema', ""),
                 role=self.config.get('role', ""),
+                client_store_temporary_credential=True,
+                client_request_mfa_token=True,
             )
             self._app_name = self.config.get('rai_app_name', "relationalai")
         try:
-            return self._conn.cursor().execute(code.replace(APP_NAME, self._app_name))
+            return self._conn.cursor().execute(code.replace(APP_NAME, self._app_name), params)
         except Exception as e:
-            if re.search(r"Database '(.+)' does not exist or not authorized\.", str(e)):
+            orig_message = str(e).lower()
+            rai_app = self.config.get("rai_app_name", "")
+            if re.search(f"database '{rai_app}' does not exist or not authorized.".lower(), orig_message):
                 print("\n")
-                name = re.search(r"Database '(.+)' does not exist or not authorized\.", str(e)).group(1) #type: ignore
-                Errors.snowflake_app_missing(name)
-            else:
-                raise e
+                Errors.snowflake_app_missing(rai_app)
+            elif re.search(r"JavaScript execution error", orig_message):
+                match = re.search(r"\"message\":\"(.*)\"", orig_message)
+                if match:
+                    message = match.group(1)
+                    if "engine was deleted" in message or "engine not found" in message:
+                        Errors.engine_not_found(self.config.get('engine', "Unknown"), message)
+                    else:
+                        raise RAIException(message) from None
+            raise e
 
 
     def reset(self):
         self._conn = None
 
     #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
     def list_engines(self):
-        results = self._exec(f"SELECT * FROM {APP_NAME}.api.engines")
+        results = self._exec(f"select NAME, SIZE, STATUS from {APP_NAME}.api.engines")
         if not results:
             return []
         return [{"name":name, "size":size, "state":state}
                 for (name, size, state) in results.fetchall()]
 
+    def get_engine(self, name:str):
+        results = self._exec(f"select NAME, SIZE, STATUS from {APP_NAME}.api.engines WHERE NAME='{name}'")
+        if not results:
+            return None
+        return [{"name":name, "size":size, "state":state}
+                for (name, size, state) in results.fetchall()][0]
+
     def create_engine(self, name:str, size:str, pool:str = ""):
         if not pool:
             raise ValueError("Pool is required")
-        self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
+        try:
+            self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
+        except Exception as e:
+            raise Exception("Failed to create engine") from e
 
     def delete_engine(self, name:str):
         self._exec(f"call {APP_NAME}.api.delete_engine('{name}');")
 
+    def suspend_engine(self, name:str):
+        raise Exception("Not implemented")
+
+    def resume_engine(self, name:str):
+        raise Exception("Not implemented")
+
     #--------------------------------------------------
     # Graphs
     #--------------------------------------------------
 
-    def list_graphs(self) -> List[Any]:
-        results = self._exec(f"SELECT * FROM {APP_NAME}.api.databases")
+    def list_graphs(self) -> List[AvailableModel]:
+        results = self._exec(f"select NAME from {APP_NAME}.api.databases WHERE state <> 'DELETED'")
         if not results:
             return []
-        return [x[1] for x in results.fetchall()]
+        return [{"name": name} for (name,) in results.fetchall()]
 
     def get_graph(self, name:str):
-        results = self._exec(f"SELECT * FROM {APP_NAME}.api.databases WHERE name='{name}'")
+        results = self._exec(f"""
+            select ID, NAME, CREATED_ON, DELETED_ON, STATE
+            from {APP_NAME}.api.databases
+            where name='{name}' AND state <> 'DELETED'
+        """)
         if not results:
             return None
         return results.fetchone()
 
     def create_graph(self, name: str):
         self._exec(f"call {APP_NAME}.api.create_database('{name}');")
 
@@ -155,19 +188,20 @@
 
     def list_models(self, database: str, engine: str):
         pass
 
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         lines = []
         for (name, code) in models:
-            code = code.replace("\"", "\\\"")
             name = name.replace("\"", "\\\"")
+            assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
+
             lines.append(textwrap.dedent(f"""
             def delete:rel:catalog:model["{name}"] = rel:catalog:model["{name}"]
-            def insert:rel:catalog:model["{name}"] = \"\"\"{code}\"\"\"
+            def insert:rel:catalog:model["{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
             """))
         rel_code = "\n\n".join(lines)
         self.exec_raw(database, engine, rel_code, readonly=False)
         # TODO: handle SPCS errors once they're figured out
         return []
 
     def delete_model(self, database:str, engine:str, name:str):
@@ -227,45 +261,102 @@
     def delete_export(self, model: str, engine: str, export: str):
         pass
 
     #--------------------------------------------------
     # Imports
     #--------------------------------------------------
 
-    def list_imports(self, model:str):
-        results = self._exec(f"select * from {APP_NAME}.api.data_streams where RAI_DATABASE='{model}';")
-        if not results:
-            return []
-        return [{"name":row[6]}
-                for row in results.fetchall()]
+    def list_imports(self, model:str) -> list[Import]:
+        # this is roughly copied from the native app code because we don't have a way to
+        # get the status of multiple streams at once and doing them individually is way
+        # too slow
+        results = self._exec(f"""
+        select FQ_OBJECT_NAME, nextBatch.status, nextBatch.pending_batches_count,
+            from {APP_NAME}.api.data_streams as ds
+            left JOIN (
+            select
+                data_stream_id,
+                min_by(status, unloaded) as status,
+                min_by(batch_details, unloaded) as batch_details,
+                min(unloaded) as unloaded,
+                count(*) as pending_batches_count
+            from {APP_NAME}.api.data_stream_batches
+            where status !in ('loaded')
+            group by data_stream_id
+            ) nextBatch
+            ON ds.id = nextBatch.data_stream_id
+            where RAI_DATABASE='{model}';
+        """)
+        items = []
+        if results:
+            for stream in results.fetchall():
+                (name, status, pending_batches_count) = stream
+                if not status and not pending_batches_count:
+                    status = "SYNCED"
+                if pending_batches_count:
+                    status = "SYNCING"
+                items.append(cast(Import, {"name": name, "type": "Snowflake object", "status": status}))
+        return items
+
+    def create_import_stream(self, source:ImportSource, model:str, rate = 1, options: dict|None = None):
+        assert isinstance(source, ImportSourceTable), "Snowflake integration only supports loading from SF Tables right now. Try loading your data as a table via the snowflake interface first."
+        object = source.fqn
 
-    def create_import_stream(self, object:str, model:str, rate = 1):
         if object.lower() in [x["name"].lower() for x in self.list_imports(model)]:
             return
 
-        self._exec(f"call {APP_NAME}.api.setup_cdc('{self.config.get('engine')}');")
-        self._exec(f"ALTER TABLE {object} SET CHANGE_TRACKING = TRUE;")
-        self._exec(f"""call {APP_NAME}.api.create_data_stream(
-             {APP_NAME}.api.object_reference('TABLE', '{object}'),
-             '{model}',
-             '{object.replace('.', '_')}');""")
+        try:
+            self._exec(f"call {APP_NAME}.api.setup_cdc('{self.config.get('engine')}');")
+        except Exception:
+           pass
+
+        info = self._exec(f"SHOW OBJECTS like %s in {source.database}.{source.schema}", [source.table])
+        if not info:
+            raise ValueError(f"Object {source.table} not found in {source.database}.{source.schema}")
+        else:
+            # (time, name, db_name, schema_name, kind, *rest)
+            kind = info.fetchone()[4]
+
+        try:
+            self._exec(f"ALTER {kind} {object} SET CHANGE_TRACKING = TRUE;")
+        except Exception:
+            pass
+
+        command = f"""call {APP_NAME}.api.create_data_stream(
+            {APP_NAME}.api.object_reference('{kind}', '{object}'),
+            '{model}',
+            '{object.replace('.', '_').lower()}');"""
+        try:
+            self._exec(command)
+        except Exception as e:
+            if "ensure that CHANGE_TRACKING is enabled on the source object" in str(e):
+                print("\n")
+                Errors.snowflake_change_tracking_not_enabled(object, f"ALTER TABLE {object} SET CHANGE_TRACKING = TRUE;")
+            raise e
+
         return
 
-    def delete_import(self, object:str, model:str):
+    def create_import_snapshot(self, source:ImportSource, model:str, _: dict|None = None):
+        raise Exception("Snowflake integration doesn't support snapshot imports yet")
+
+    def delete_import(self, import_name:str, model:str):
         self._exec(f"""call {APP_NAME}.api.delete_data_stream(
-             '{object}',
+             '{import_name}',
              '{model}'
         );""")
         return
 
     #--------------------------------------------------
     # Exec Sync
     #--------------------------------------------------
 
-    def _exec_sync_raw(self, database:str, engine:str, raw_code:str, readonly=True):
+    def _exec_sync_raw(self, database:str, engine:str, raw_code:str, readonly=True, inputs = {}):
+        if inputs:
+            raise Exception("Inputs aren't currently supported using exec_sync in SPCS.")
+
         return self._exec(f"select {APP_NAME}.api.exec('{database}','{engine}','{raw_code}', {readonly});")
 
     def _format_results_sync(self, results, task:m.Task) -> Tuple[DataFrame, List[Any]]:
         parsed_results = []
         parsed_problems = []
         if results:
             for row in results:
@@ -325,25 +416,32 @@
                 schema = reader.schema
                 batches = [batch for batch in reader]
                 table = pa.Table.from_batches(batches=batches, schema=schema)
                 results.append({"relationId": file_name, "table": table})
 
         return results
 
-    def _exec_async_raw(self, database:str, engine:str, raw_code:str, readonly=True):
+    def _exec_async_raw(self, database:str, engine:str, raw_code:str, readonly=True, inputs={}):
+        if inputs:
+            raise Exception("Inputs aren't currently supported using exec_async in SPCS.")
+
         response = self._exec(f"CALL {APP_NAME}.api.exec_async('{database}','{engine}','{raw_code}', {readonly});")
         if not response:
             raise Exception("No results from exec_async")
 
         # Grab the txn_id from the response
         txn_id, status = next(iter(response))
+        debugging.event("transaction", txn_id=txn_id)
         # Wait for completion or failure
         if status != "COMPLETED":
+            self._pending_transactions.append(txn_id)
             poll_with_specified_overhead(lambda: self._check_exec_async_status(txn_id), 0.2)
 
+        self._pending_transactions.remove(txn_id)
+
         # List the result artifacts (and the URLs to retrieve them)
         artifact_urls = self._list_exec_async_artifacts(txn_id)
         # Actually retrieve them
         artifacts = self._fetch_exec_async_artifacts(artifact_urls)
 
         meta = _parse_metadata_proto(artifacts["metadata.proto"])
         meta_json = artifacts["metadata.json"]
@@ -375,20 +473,20 @@
             for problem in results.problems:
                 if problem['is_error'] or problem['is_exception']:
                     return True
 
     # Copied directly from azure.py
     def _format_results_async(self, results, task:m.Task) -> Tuple[DataFrame, List[Any]]:
         data_frame = DataFrame()
-        if not self._has_errors(results) and len(results.results):
+        if len(results.results):
             for result in results.results:
                 types = [t for t in result["relationId"].split("/") if t != "" and not t.startswith(":")]
                 result_frame:DataFrame = result["table"].to_pandas()
                 for i, col in enumerate(result_frame.columns):
-                    if types[i] == "UInt128":
+                    if "UInt128" in types[i]:
                         result_frame[col] = result_frame[col].apply(lambda x: base64.b64encode(x.tobytes()).decode()[:-2])
                     if types[i] == "Dates.DateTime":
                         result_frame[col] = pd.to_datetime(result_frame[col] - UNIXEPOCH, unit="ms")
                     if types[i] == "Dates.Date":
                         result_frame[col] = pd.to_datetime(result_frame[col] * MILLISECONDS_PER_DAY - UNIXEPOCH, unit="ms")
                 ret_cols = task.return_cols()
                 if len(ret_cols) and len(result_frame.columns) == len(ret_cols):
@@ -398,31 +496,64 @@
                     data_frame = pd.concat([data_frame, result_frame], ignore_index=True)
         return (data_frame, results.problems)
 
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
-    def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True):
+    def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True, inputs: dict = {}):
         raw_code = raw_code.replace("'", "\\'") # @NOTE: If collapsing to a single exec, make sure to copy this line into it.
         if USE_EXEC_ASYNC:
-            return self._exec_async_raw(database, engine, raw_code, readonly)
+            return self._exec_async_raw(database, engine, raw_code, readonly, inputs=inputs)
         else:
-            return self._exec_sync_raw(database, engine, raw_code, readonly)
+            return self._exec_sync_raw(database, engine, raw_code, readonly, inputs=inputs)
 
     def format_results(self, results, task:m.Task) -> Tuple[DataFrame, List[Any]]:
         if USE_EXEC_ASYNC:
             return self._format_results_async(results, task)
         else:
             return self._format_results_sync(results, task)
 
     #--------------------------------------------------
+    # Transactions
+    #--------------------------------------------------
+
+    def list_transactions(self, limit:int, only_active=False):
+        where = "WHERE state <> 'COMPLETED'" if only_active else ""
+        field_names = [
+            "id", "database_name", "state", "abort_reason", "read_only", "created_by",
+            "duration", "created_on", "finished_at"
+        ]
+        sql_fields = ", ".join([f.upper() for f in field_names])
+        results = self._exec(f"select {sql_fields} from {APP_NAME}.api.transactions {where} LIMIT %s", [limit])
+        if not results:
+            return []
+        map = {"database_name": "database"}
+        mapped = [map.get(f, f) for f in field_names]
+        return [dict(zip(mapped, row)) for row in results.fetchall()]
+
+    def cancel_transaction(self, transaction_id):
+        self._exec(f"CALL {APP_NAME}.api.CANCEL_TRANSACTION(%s);", [transaction_id])
+        if transaction_id in self._pending_transactions:
+            self._pending_transactions.remove(transaction_id)
+
+    def cancel_pending_transactions(self):
+        for txn_id in self._pending_transactions:
+            self.cancel_transaction(txn_id)
+
+    #--------------------------------------------------
     # Snowflake specific
     #--------------------------------------------------
 
+    def get_version(self):
+        results = self._exec(f"SELECT {APP_NAME}.app.get_release()")
+        if not results:
+            return None
+        return results.fetchone()[0]
+
     def list_warehouses(self):
         results = self._exec("SHOW WAREHOUSES")
         if not results:
             return []
         return [{"name":name}
                 for (name, *rest) in results.fetchall()]
 
@@ -430,19 +561,23 @@
         results = self._exec("SHOW COMPUTE POOLS")
         if not results:
             return []
         return [{"name":name}
                 for (name, *rest) in results.fetchall()]
 
     def list_roles(self):
-        results = self._exec("SHOW ROLES")
+        results = self._exec("SELECT CURRENT_AVAILABLE_ROLES()")
         if not results:
             return []
-        return [{"name":name}
-                for (name, *rest) in results.fetchall()]
+        # the response is a single row with a single column containing
+        # a stringified JSON array of role names:
+        row = results.fetchone()
+        if not row:
+            return []
+        return [{"name": name} for name in json.loads(row[0])]
 
     def list_apps(self):
         results = self._exec("SHOW APPLICATIONS")
         if not results:
             return []
         return [{"name":name}
                 for (time, name, *rest) in results.fetchall()]
@@ -458,31 +593,31 @@
         results = self._exec(f"SHOW SCHEMAS IN {database}")
         if not results:
             return []
         return [{"name":name}
                 for (time, name, *rest) in results.fetchall()]
 
     def list_tables(self, database:str, schema:str):
-        results = self._exec(f"SHOW TABLES IN {database}.{schema}")
-        if not results:
-            return []
-        return [{"name":name}
-                for (time, name, *rest) in results.fetchall()]
-
+        results = self._exec(f"SHOW OBJECTS IN {database}.{schema}")
+        items = []
+        if results:
+            for (time, name, db_name, schema_name, kind, *rest) in results.fetchall():
+                items.append({"name":name, "kind":kind.lower()})
+        return items
 
     def schema_info(self, database:str, schema:str, tables:Iterable[str]):
         pks = self._exec(f"SHOW PRIMARY KEYS IN SCHEMA {database}.{schema};")
         fks = self._exec(f"SHOW IMPORTED KEYS IN SCHEMA {database}.{schema};")
         tables = ", ".join([f"'{x.upper()}'" for x in tables])
         columns = self._exec(f"""
-            SELECT TABLE_NAME, COLUMN_NAME, DATA_TYPE
-            FROM {database.upper()}.INFORMATION_SCHEMA.COLUMNS
-            WHERE TABLE_SCHEMA = '{schema.upper()}'
-            AND TABLE_NAME in ({tables})
-            AND TABLE_CATALOG = '{database.upper()}';
+            select TABLE_NAME, COLUMN_NAME, DATA_TYPE
+            from {database.upper()}.INFORMATION_SCHEMA.COLUMNS
+            where TABLE_SCHEMA = '{schema.upper()}'
+            and TABLE_NAME in ({tables})
+            and TABLE_CATALOG = '{database.upper()}';
         """)
         results = defaultdict(lambda: {"pks": [], "fks": {}, "columns": {}})
         if pks:
             for row in pks:
                 results[row[3].lower()]["pks"].append(row[4].lower()) # type: ignore
         if fks:
             for row in fks:
@@ -505,20 +640,20 @@
         self._auto_import = auto_import
         if not isinstance(model._client.resources, Resources):
             raise ValueError("Snowflake model must be used with a snowflake config")
         self._dbs = {}
         imports = model._client.resources.list_imports(model.name)
         self._import_structure(imports)
 
-    def _import_structure(self, imports):
+    def _import_structure(self, imports: list[Import]):
         tree = self._dbs
         # pre-create existing imports
         schemas = set()
         for item in imports:
-            database_name, schema_name, table_name = item['name'].lower().split('.')
+            database_name, schema_name, table_name = item["name"].lower().split('.')
             database = getattr(self, database_name)
             schema = getattr(database, schema_name)
             schemas.add(schema)
             schema._add(table_name, is_imported=True)
         for schema in schemas:
             schema._finalize()
         return tree
@@ -578,44 +713,46 @@
         self._name = name
         self._model = parent._model
         self._parent = parent
         self._aliases = {}
         self._finalzed = False
         if not is_imported and self._parent._parent._parent._auto_import:
             with Spinner(f"Creating stream for {self.fqname()}", f"Stream created for {self.fqname()}"):
-                self._model._client.resources.create_import_stream(self.fqname(), self._model.name)
+                db_name = parent._parent._name
+                schema_name = parent._name
+                self._model._client.resources.create_import_stream(ImportSourceTable(db_name, schema_name, name), self._model.name)
             print("")
             parent._tables[name] = self
             parent._finalize()
         elif not is_imported:
             Errors.snowflake_import_missing(debugging.capture_code_info(4), self.fqname(), self._model.name)
 
 
     def _finalize(self):
         if self._finalzed:
             return
 
         self._finalzed = True
         self._schema = self._parent._table_info[self._name]
-        relation_name = self.fqname().replace(".", "_")
+        relation_name = self.fqname().replace(".", "_").lower()
         model:dsl.Graph = self._model
         model.install_raw(f"bound {relation_name}")
 
         with model.rule(dynamic=True):
-            prop, id, val = model.Vars(3)
+            prop, id, val = std.Vars(3)
             if self._schema["pks"]:
-                getattr(getattr(model.rel, relation_name), self._schema["pks"][0].upper())(id, val)
+                getattr(getattr(std.rel, relation_name), self._schema["pks"][0].upper())(id, val)
             else:
-                getattr(model.rel, relation_name)(prop, id, val)
+                getattr(std.rel, relation_name)(prop, id, val)
             self.add(snowflake_id=id)
 
         for prop, prop_type in self._schema["columns"].items():
             with model.rule():
-                id, val = model.Vars(2)
-                getattr(getattr(model.rel, relation_name), prop.upper())(id, val)
+                id, val = std.Vars(2)
+                getattr(getattr(std.rel, relation_name), prop.upper())(id, val)
                 self(snowflake_id=id).set(**{prop.lower(): val})
 
     def namespace(self):
         return f"{self._parent._parent._name}.{self._parent._name}"
 
     def fqname(self):
         return f"{self.namespace()}.{self._name}"
@@ -641,16 +778,16 @@
                 raise ValueError(f"Invalid column {k}={v}")
         return self
 
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
-def Graph(name, dry_run=False):
-    client = Client(Resources(), rel.Compiler(), name, dry_run=dry_run)
+def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False):
+    client = Client(Resources(profile, config), rel.Compiler(config), name, dry_run=dry_run)
     client.install("pyrel_base", dsl.build.raw_task("""
         @inline
         def make_identity(x..., z) =
             hash128({x...}, x..., u) and
             hash_value_uint128_convert(u, z)
             from u
```

### Comparing `relationalai-0.1.9/src/relationalai/clients/test.py` & `relationalai-0.2.0/src/relationalai/clients/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,52 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import Any, cast
+from relationalai.analysis.mechanistic import Mechanism
 
 from pandas import DataFrame
 from ..clients.client import Client
 from .. import debugging
 from .. import dsl, rel, metamodel as m
 
 @dataclass
 class Query:
     task: m.Task
     ix: int
     code: str|None = None
     err: Exception|None = None
     result: Any = None
+    mech: Mechanism|None = None
+
+    def to_json(self):
+        return {
+            "task": str(self.task),
+            "ix": self.ix,
+            "code": self.code,
+            "err": str(self.err),
+            "mech": self.mech.stack[-1] if self.mech else None
+        }
 
 
 @dataclass
 class Install:
     task: m.Task
     name: str|None = None
     code: str|None = None
     err: Exception|None = None
+    mech: Mechanism|None = None
+
+    def to_json(self):
+        return {
+            "task": str(self.task),
+            "name": self.name,
+            "code": self.code,
+            "err": str(self.err),
+            "mech": self.mech.stack[-1] if self.mech else None
+        }
 
 
 class Document():
     blocks: list[Query | Install]
     query_count: int
 
     def __init__(self):
@@ -45,18 +66,22 @@
                 case Install():
                     h = f"----[ Rule {block.name} ]"
                     parts.append(f"{h}{'-'*(80 - len(h))}")
                     parts.append(str(block.task))
 
         return "\n".join(parts)
 
+class Config():
+    def get(self, key:str, default:Any=None):
+        return default
 
 class NoopClient():
-    def __init__(self, *_args, **_kwargs):
-        self.compiler = rel.Compiler()
+    def __init__(self, *_args, config=None, **_kwargs):
+        self.compiler = rel.Compiler(config or Config())
+        self.resources = Resources(config or Config())
 
     def query(self, task: m.Task, *args, **kwargs):
         self.compiler.compile(task)
         return DataFrame()
 
     def install(self, name: str, task: m.Task, *args, **kwargs):
         self.compiler.compile(task)
@@ -68,22 +93,24 @@
         raise Exception("Cannot exec raw code in test executor")
 
     def load_raw_file(self, path:str):
         raise Exception("Cannot load raw file in test executor")
 
 proxied_clients: list[Document] = []
 
+class Resources():
+    def __init__(self, config:Config):
+        self.config = config
 
 def proxy_client(client_class, throw_on_error = True):
     class ProxiedClient(client_class, Document):
         def __init__(self, *args, throw_on_error = True, **kwargs):
             self.blocks: list[Query | Install] = []
             self.query_count = 0
             self.throw_on_error = throw_on_error
-            self.resources = {}
             # self.capture_handler = CaptureHandler()
 
             # debugging.logger.addHandler(self.capture_handler)
             super().__init__(*args, **kwargs)
             proxied_clients.append(self)
 
         # def __del__(self):
@@ -108,35 +135,39 @@
             msgs[0]["emitted"] if len(msgs) > 0 and msgs[0]["event"] == "compilation" else None
 
         def query(self, task:m.Task, *args, **kwargs):
             ix = self.query_count
             self.query_count += 1
             res = None
             with self.capture_debugging() as msgs:
+                mech = None
                 try:
+                    mech = Mechanism(task)
                     res = super().query(task, *args, **kwargs)
-                    self.blocks.append(Query(task, ix, self.get_emitted(msgs), None, res))
+                    self.blocks.append(Query(task, ix, self.get_emitted(msgs), None, res, mech))
 
                 except Exception as err:
-                    self.blocks.append(Query(task, ix, self.get_emitted(msgs), err))
+                    self.blocks.append(Query(task, ix, self.get_emitted(msgs), err, None, mech))
                     if self.throw_on_error:
                         raise
 
             return res
 
         def install(self, name, task:m.Task, *args, **kwargs):
             with self.capture_debugging() as msgs:
+                mech = None
                 try:
+                    mech = Mechanism(task)
                     super().install(name, task, *args, **kwargs)
-                    self.blocks.append(Install(task, name, self.get_emitted(msgs)))
+                    self.blocks.append(Install(task, name, self.get_emitted(msgs), None, mech))
                 except Exception as err:
-                    self.blocks.append(Install(task, name, self.get_emitted(msgs), err))
+                    self.blocks.append(Install(task, name, self.get_emitted(msgs), err, mech))
                     if self.throw_on_error:
                         raise
 
     return ProxiedClient
 
 Executor = proxy_client(NoopClient, throw_on_error=False)
 
-def Graph(name, engine:str|None=None, dry_run=False):
-    client = cast(Client, Executor(name, engine, dry_run))
+def Graph(name, engine:str|None=None, dry_run=False, config=None):
+    client = cast(Client, Executor(name, engine, dry_run, config=config or Config()))
     return dsl.Graph(client, name)
```

### Comparing `relationalai-0.1.9/src/relationalai/graphs/lib.py` & `relationalai-0.2.0/src/relationalai/std/graphs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 from copy import deepcopy
 from typing import Any
 from .. import dsl, errors
 import gravis as gv
+from . import rel, Vars
 
 #--------------------------------------------------
 # Errors
 #--------------------------------------------------
 
 def invalid_param(param:str, message:str):
     source = errors.Errors.call_source(4)
@@ -28,175 +29,263 @@
         invalid_param(param, f"must be between {min} and {max}")
 
 def positive(param:str, value):
     if value <= 0:
         invalid_param(param, "must be positive")
 
 #--------------------------------------------------
-# Graph
+# Algos
 #--------------------------------------------------
 
 class Compute:
     def __init__(self, graph:'Graph'):
         self._graph = graph
-        self._lib = self._graph.model.rel.rel.graph
-        self._old_lib = getattr(self._graph.model.rel, self._graph._lib_ref())
+        self._lib = dsl.global_ns.graphlib
+        self._module_lib = rel.rel.graph
+        self._old_lib = getattr(rel, self._graph._lib_ref())
 
     def _config(self, **kwargs):
         return dsl.InlineRelation(self._graph.model, [
             *[(dsl.Symbol(k), v) for k, v in kwargs.items()],
         ])
 
+    # --------------------------------------------------
+    # Degree
+    # --------------------------------------------------
+
+    # TODO: these are still in the old style graph lib
+    def degree(self, node, weight=None):
+        if not weight:
+            return self._old_lib.degree(node)
+        return self._old_lib.weighted_degree(node)
+
+    def indegree(self, node):
+        return self._lib.indegree(self._graph, node)
+
+    def outdegree(self, node):
+        return self._lib.outdegree(self._graph, node)
+
+    # --------------------------------------------------
+    # Similarity
+    # --------------------------------------------------
+
+    def cosine_similarity(self, node1, node2):
+        if not self._graph.undirected:
+            invalid_param("graph", "must be undirected")
+        return self._module_lib.similarity.cosine_similarity(self._graph, node1, node2)
+
+    def jaccard_similarity(self, node1, node2):
+        return self._module_lib.similarity.jaccard_similarity(self._graph, node1, node2)
+
+    # --------------------------------------------------
+    # Centrality
+    # --------------------------------------------------
+
     def pagerank(self, node, damping_factor=0.85, tolerance=1e-6, max_iter=20):
         between("damping_factor", damping_factor, 0, 1)
         positive("tolerance", tolerance)
         positive("max_iter", max_iter)
 
         config = self._config(
             graph=self._graph,
             damping_factor=damping_factor,
             tolerance=tolerance,
             max_iter=max_iter,
         )
-        return self._lib.centrality.pagerank(config, node)
-
-    #TODO: these are still in the old style graph lib
-    def degree(self, node, weight=None):
-        if not weight:
-            return self._old_lib.degree(node)
-        return self._old_lib.weighted_degree(node)
+        return self._lib.pagerank(config, node)
 
+    # TODO: these are still in the old style graph lib
     def betweenness_centrality(self, node):
         return self._old_lib.betweenness_centrality(node)
 
     def degree_centrality(self, node):
         return self._old_lib.degree_centrality(node)
 
+    def eigenvector_centrality(self, node):
+        if not self._graph.undirected:
+            invalid_param("graph", "must be undirected")
+        return self._old_lib.eigenvector_centrality(node)
+
+    # --------------------------------------------------
+    # Community Detection
+    # --------------------------------------------------
+
     def label_propagation(self, node):
         return self._old_lib.label_propagation(node)
 
     def weakly_connected_component(self, node):
         return self._old_lib.weakly_connected_component(node)
 
-class Nodes:
-    def __init__(self, graph:'Graph'):
-        self._graph = graph
-        self._type = dsl.RawRelation(self._graph.model, f"graph{self._graph.id}_nodes", 1)
-        self._props = {}
+    def triangle_community(self, node):
+        return self._old_lib.triangle_community(node)
 
-    def _prop(self, name:str):
-        if name not in self._props:
-            self._props[name] = dsl.RawRelation(self._graph.model, f"graph{self._graph.id}_node_{name}", 2)
-        return self._props[name]
+    def infomap(self, node):
+        config = self._config(graph=self._graph)
+        return self._lib.infomap(config, node)
+
+    def louvain(self, node):
+        config = self._config(graph=self._graph)
+        return self._lib.louvain(config, node)
 
-    def extend(self, type:dsl.Type, **kwargs):
-        with self._graph.model.rule():
-            t = type()
-            self.add(t, **kwargs)
+#--------------------------------------------------
+# Edge
+#--------------------------------------------------
 
-    def add(self, node, **kwargs):
-        self._type.add(node)
+class EdgeInstance:
+    def __init__(self, edge:'Edge', from_:Any, to:Any, kwargs:dict={}):
+        self._edge = edge
+        self._graph = edge._graph
+        self.from_ = from_
+        self.to = to
         for k, v in kwargs.items():
-            if isinstance(v, dsl.Property):
-                v = getattr(node, v._name)
-            self._prop(k).add(node, v)
+            self._edge._prop(k)(from_, to, v)
 
-    def __getattribute__(self, __name: str) -> Any:
-        if __name in ["add", "extend"] or __name.startswith("_"):
-            return super().__getattribute__(__name)
-        return self._props[__name]
+    def __getattr__(self, name:str):
+        v = Vars(1)
+        self._edge._prop(name)(self.from_, self.to, v)
+        return v
+
+    def set(self, **kwargs):
+        for k, v in kwargs.items():
+            self._edge._prop(k).add(self.from_, self.to, v)
+
+    def _to_var(self):
+        raise Exception("Edges can't be returned directly, you can return the from_ and to properties individually")
 
-class Edges:
+class Edge:
     def __init__(self, graph:'Graph'):
         self._graph = graph
         self._type = dsl.RawRelation(self._graph.model, f"graph{self._graph.id}_edges", 2)
         self._props = {}
 
     def _prop(self, name:str):
         if name not in self._props:
             self._props[name] = dsl.RawRelation(self._graph.model, f"graph{self._graph.id}_edge_{name}", 3)
         return self._props[name]
 
-    def extend(self, prop:'dsl.Property|Edge', **kwargs):
+    def _is_weighted(self):
+        return "weight" in self._props
+
+    def extend(self, prop:'dsl.Property', **kwargs):
         type = prop._provider
         with self._graph.model.rule():
             t = type()
             self.add(t, getattr(t, prop._name), **kwargs)
 
     def add(self, from_:Any, to:Any, **kwargs):
         self._type.add(from_, to)
         for k, v in kwargs.items():
             self._prop(k).add(from_, to, v)
+        return EdgeInstance(self, from_, to, {})
+
+    def __call__(self, from_:Any=None, to:Any=None, **kwargs):
+        if from_ is None:
+            from_ = Vars(1)
+        if to is None:
+            to = Vars(1)
+        self._type(from_, to)
+        return EdgeInstance(self, from_, to, kwargs)
 
     def __getattribute__(self, __name: str) -> Any:
         if __name in ["add", "extend"] or __name.startswith("_"):
             return super().__getattribute__(__name)
         return self._props[__name]
 
+#--------------------------------------------------
+# Graph
+#--------------------------------------------------
+
 class Graph:
-    def __init__(self, model:dsl.Graph, undirected=False):
+    def __init__(self, model:dsl.Graph, undirected=False, weighted=False, default_weight=1.0):
         self.model = model
         self.id = dsl.next_id()
         self.compute = Compute(self)
-        self.nodes = Nodes(self)
-        self.edges = Edges(self)
+        self.Node = dsl.Type(model, "nodes", scope=f"graph{self.id}_")
+        self.Edge = Edge(self)
         self.undirected = undirected
+        self.weighted = weighted
+        self.default_weight=default_weight
         self._last_fetch = None
 
-        graph_type = "undirected_graph" if undirected else "directed_graph"
+        graph_type = "::graphlib::undirected_graph" if undirected else "::graphlib::directed_graph"
+        if weighted:
+            create_graph = f"""{graph_type}[{self.Edge._prop("weight")._name}]"""
+        else:
+            create_graph = f"{graph_type}[{self.Edge._type._name}]"
+
         self.model.install_raw(f"""
-        bound {self.edges._type._name}
-        def {self._graph_ref()} = {graph_type}[{self.edges._type._name}]
+        bound {self.Node._type.name}
+        bound {self.Edge._type._name}
+        {f"bound {self.Edge._prop('weight')._name}" if weighted else ""}
+        def {self._graph_ref()} = {create_graph}
         @inline
         def {self._lib_ref()} = rel:graphlib[{self._graph_ref()}]
         """)
 
+        # Add a rule that makes all nodes used in edges are also added to
+        # the nodes relation
+        with model.rule():
+            a, b = dsl.Vars(2)
+            self.Edge._type(a, b)
+            self.Node.add(a)
+            self.Node.add(b)
+
     def _graph_ref(self):
         return f"graph{self.id}"
 
     def _lib_ref(self):
         return f"graphlib{self.id}"
 
     def _to_var(self):
-        return getattr(self.model.rel, self._graph_ref())._to_var()
+        return getattr(rel, self._graph_ref())._to_var()
+
+    def _is_weighted(self):
+        return self.weighted
+        # return self.edges._is_weighted()
 
     #--------------------------------------------------
     # Fetch
     #--------------------------------------------------
 
     def fetch(self):
         code = []
-        code.append(f"def output:nodes(n) = {self.nodes._type._name}(n)")
-        for name, prop in self.nodes._props.items():
-            code.append(f"def output:nodes:{name}(n, v) = {prop._name}(n, v)")
-        code.append(f"def output:edges(a,b) = {self.edges._type._name}(a,b)")
-        for name, prop in self.edges._props.items():
+        code.append(f"def output:nodes(n) = {self.Node._type.name}(n)")
+        for prop in self.Node._type.properties:
+            code.append(f"def output:nodes:{prop.name.split('_')[-1]}(n, v) = {prop.name}(n, v)")
+        code.append(f"def output:edges(a,b) = {self.Edge._type._name}(a,b)")
+        for name, prop in self.Edge._props.items():
             code.append(f"def output:edges:{name}(a,b,v) = {prop._name}(a,b,v)")
 
         output = {"nodes": defaultdict(dict), "edges": defaultdict(dict)}
         results = self.model.exec_raw("\n".join(code), raw_results=True)
-        for set in results.results:
-            path = [v[1:] for v in set["relationId"].split("/")[2:] if v[0] == ":"]
+        for set_ in results.results:
+            path = [v[1:] for v in set_["relationId"].split("/")[2:] if v[0] == ":"]
             if path[0] not in ["nodes", "edges"]:
                 continue
             cur = output[path[0]]
             if path[0] == "nodes":
                 if len(path) == 1:
-                    for (n,) in set["table"].itertuples(index=False):
+                    for (n,) in set_["table"].itertuples(index=False):
                         cur[n]
                 else:
-                    for (n,v) in set["table"].itertuples(index=False):
+                    for (n, v) in set_["table"].itertuples(index=False):
                         cur[n][path[1]] = v
             elif path[0] == "edges":
                 if len(path) == 1:
-                    for (a,b) in set["table"].itertuples(index=False):
-                        cur[(a,b)]
+                    for (a, b) in set_["table"].itertuples(index=False):
+                        # If the graph is undirected, normalize the order of
+                        # the source and target nodes.
+                        if self.undirected and a > b:
+                            a, b = b, a
+                        cur[(a, b)]
                 else:
-                    for (a,b,v) in set["table"].itertuples(index=False):
-                        cur[(a,b)][path[1]] = v
+                    for (a, b, v) in set_["table"].itertuples(index=False):
+                        if self.undirected and a > b:
+                            a, b = b, a
+                        cur[(a, b)][path[1]] = v
             else:
                 raise Exception(f"Unexpected path: {path}")
         self._last_fetch = output
         return output
 
     #--------------------------------------------------
     # Visualize
@@ -228,41 +317,41 @@
     }
 
     _style_map = {
         "arrow_size": "arrow_size",
         "arrow_color": "arrow_color",
     }
 
-
     def _visual_props(self, prop_def, metadata):
         for k, v in prop_def.items():
             if callable(v):
                 metadata[k] = v(metadata)
         return metadata
 
-    def visualize(self, three=False, style={"node": {}, "edge": {}}, **kwargs):
-        data = self._last_fetch
+    def _visual_dict(self, style: dict, use_cache = False) -> dict:
+        data = self._last_fetch if use_cache else None
         if not data:
             data = self.fetch()
-
         style = deepcopy(style)
         if "node" not in style:
             style["node"] = {}
         if "edge" not in style:
             style["edge"] = {}
         merged_style = deepcopy(self.default_visual_props)
         for category in ["node", "edge"]:
             for k, v in style.get(category, {}).items():
                 if not callable(v):
                     merged_style[category][k] = v
-        flat_style = {self._style_map.get(k, f"{type}_{k}"): v
-                        for type, category in merged_style.items()
-                        for k, v in category.items()}
+        flat_style = {
+            self._style_map.get(k, f"{type}_{k}"): v
+            for type, category in merged_style.items()
+            for k, v in category.items()
+        }
 
-        graph1 = {
+        return {
             "graph": {
                 "directed": not self.undirected,
                 "metadata": flat_style,
                 "nodes": {
                     node_id: {
                         **({"label": info["label"]} if "label" in info else {}),
                         "metadata": self._visual_props(style["node"], info),
@@ -272,42 +361,38 @@
                 "edges": [
                     {"source": source, "target": target, "metadata": self._visual_props(style["edge"], info)}
                     for ((source, target), info) in data["edges"].items()
                 ],
             }
         }
 
+    def visualize(self, three=False, style: dict | None = None, use_cache = False, **kwargs):
+        style = style if style is not None else {"node": {}, "edge": {}}
         vis = gv.vis if not three else gv.three
-        fig = vis(graph1, edge_label_data_source='label', node_label_data_source='label', edge_curvature=0.4, **kwargs)
+        graph_dict = self._visual_dict(style=style, use_cache=use_cache)
+        # Use defaults for the following kwargs if not provided
+        new_kwargs = {
+            "node_label_data_source": "label",
+            "edge_label_data_source": "label",
+            "edge_curvature": 0.4,
+        } | kwargs
+        fig = vis(graph_dict, **new_kwargs)
         return fig
 
-
-#--------------------------------------------------
-# Edge
-#--------------------------------------------------
-
-class Edge:
-    def __init__(self, type:Any, from_:Any, to:Any):
-        # raise NotImplementedError()
-        pass
-
-    def __call__(self, *args, **kwargs):
-        return self
-
-    def __getattribute__(self, __name: str) -> Any:
-        pass
-
-    def __getitem__(self, item):
-        return self
-
 #--------------------------------------------------
 # Path
 #--------------------------------------------------
 
 class Path:
     def __init__(self, *args):
         self.edges = []
         self.nodes = []
         pass
 
     def __getitem__(self, item):
         return self
+
+#--------------------------------------------------
+# Exports
+#--------------------------------------------------
+
+__all__ = ["Graph", "Path"]
```

### Comparing `relationalai-0.1.9/src/relationalai/tools/debugger.py` & `relationalai-0.2.0/src/relationalai/tools/debugger.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 last_mod_time = None
 current_json_objects = []
 active_ix = None
 active_item = None
 
 def set_item(ix):
     global active_item, active_ix
-    active_ix = ix
-    active_item = current_json_objects[ix]
-    my_stuff.refresh()
-    details.refresh()
+    if active_ix != ix:
+        active_ix = ix
+        active_item = current_json_objects[ix]
+        my_stuff.refresh()
+        details.refresh()
 
 def format_time(t):
     if t > 1:
         return f"{t:.1f}s"
     elif t > 0.001:
         return f"{t*1000:.1f}ms"
     elif t > 0.0001:
@@ -82,37 +83,49 @@
                 code(active_item["code"])
             # ui.label(f"{active_item['results']['values']}").style('white-space: pre;')
 
 @ui.refreshable
 def my_stuff():
     total_time = 0
     with ui.column():
+
         for (ix, obj) in enumerate(current_json_objects):
+            if 'span' in obj['event']:
+                continue
+
             if obj['event'] == "compilation":
                 me = code(obj["source"]["block"] or obj["emitted"])
                 total_time += obj["emit_time"]
                 for p in obj['passes']:
                     total_time += p['elapsed']
             elif obj['event'] == "time":
                 total_time += obj['elapsed']
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['type']}")
                     ui.label(format_time(obj['elapsed']))
                     if obj.get('results'):
                         ui.label(f"{obj['results']['count']}")
-            else:
-                total_time += obj['elapsed']
+            elif obj['event'] == "transaction":
+                with ui.row() as me:
+                    me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
+                    ui.label(f"{obj['event']}")
+                    ui.label(obj["txn_id"])
+            elif obj.get('type'):
+                total_time += obj.get('elapsed', 0)
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['type']}")
-                    ui.label(format_time(obj['elapsed']))
+                    ui.label(format_time(obj.get('elapsed', 0)))
                     if obj.get('results'):
                         ui.label(f"{obj['results']['count']}")
-
+            else:
+                with ui.row() as me:
+                    me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
+                    ui.label(f"{obj['event']}")
 
             me.classes("w-full")
             me.on("click", lambda ix=ix: set_item(ix))
             if ix != active_ix:
                 me.style('opacity: 0.5')
         with ui.row() as me:
             me.style("padding: 5px 10px; border: 1px solid #445; border-radius: 5px; background:#223; opacity: 0.5;")
@@ -147,22 +160,22 @@
                 active_item = current_json_objects[active_ix]
             # Refresh the UI with the new objects
             my_stuff.refresh()
             details.refresh()
     except FileNotFoundError:
         pass
 
-def main():
+def main(port=8080):
     ui.dark_mode().enable()
     with ui.row():
         with ui.column() as c:
             c.style("cursor: pointer;")
             my_stuff()
         with ui.column() as c:
             c.style("padding-left: 2em;")
             details()
 
     ui.timer(1, poll)
-    ui.run(reload=False)
+    ui.run(reload=False, port=port)
 
 if __name__ == "__main__":
     main()
```

### Comparing `relationalai-0.1.9/src/relationalai/tools/dev.py` & `relationalai-0.2.0/src/relationalai/tools/dev.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,28 @@
 # Watch
 #--------------------------------------------------
 
 def clear():
     os.system('cls' if os.name == 'nt' else 'clear')
 
 class ChangeHandler(PatternMatchingEventHandler):
-    patterns = ["*.py", "*.rel"]
+    patterns = ["*.py", "*.rel", "raiconfig.toml"]
 
     def __init__(self):
         super().__init__()
         self.script = None
         self.process = None
         self.event_lock = threading.Lock()
         self.has_queued_events = False
 
     def check_event(self, event):
-        if "examples/" in event.src_path and event.src_path.endswith(".py"):
+        if not event.src_path.endswith(".py"):
+            return
+
+        if "examples/" in event.src_path or "tests/end2end/test_cases/" in event.src_path:
             self.script = event.src_path
 
     def on_any_event(self, event):
         self.check_event(event)
         with self.event_lock:
             if self.process and self.process.poll() is None:
                 # Mark that there are queued events
@@ -119,37 +122,43 @@
         return cast(int, total_lines)
     except Exception as e:
         print(f"Error while parsing cloc output: {e}")
         return 0
 
 @cli.command()
 def stats():
-    core = cloc(["compiler.py", "dsl.py", "metamodel.py", "rel.py"])
     dsl = cloc(["dsl.py"])
     compiler = cloc(["compiler.py"])
     metamodel = cloc(["metamodel.py"])
+    emitter = cloc(["rel_emitter.py"])
     rel = cloc(["rel.py"])
+    rel2 = cloc(["rel2.py"])
     metagen = cloc(["metagen.py"])
     gentest = cloc(["../gentest", "metagen.py"])
     tools = cloc(["tools/"])
     clients = cloc(["clients/"])
+    std = cloc(["std/"])
     non_test_total = cloc(["."]) - metagen
     total = non_test_total + gentest
+    core = dsl + compiler + metamodel + emitter + rel + rel2
 
     max_width = len(f"{total:,}")
 
     # Print statements with numbers right-aligned
     divider()
     rich.print(f"[yellow]RelationalAI  {non_test_total:>{max_width},} loc")
     rich.print(f"[yellow]  Core        {core:>{max_width},} loc")
     rich.print(f"[yellow]    dsl       {dsl:>{max_width},} loc")
     rich.print(f"[yellow]    rel       {rel:>{max_width},} loc")
+    rich.print(f"[yellow]    rel2      {rel2:>{max_width},} loc")
+    rich.print(f"[yellow]    emitter   {emitter:>{max_width},} loc")
     rich.print(f"[yellow]    metamodel {metamodel:>{max_width},} loc")
     rich.print(f"[yellow]    compiler  {compiler:>{max_width},} loc")
     rich.print(f"[yellow]  Clients     {clients:>{max_width},} loc")
+    rich.print(f"[yellow]  Std         {std:>{max_width},} loc")
     rich.print(f"[yellow]  Tools       {tools:>{max_width},} loc")
     rich.print("")
     rich.print(f"[cyan]Gentest       {gentest:>{max_width},} loc")
     rich.print("")
     rich.print(f"[magenta]All           {total:>{max_width},} loc")
     divider()
```

### Comparing `relationalai-0.1.9/tests/conftest.py` & `relationalai-0.2.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from _pytest._io.wcwidth import wcswidth
 from _pytest.terminal import TerminalReporter
 from gentest.util import condense_traceback
-from gentest.validate.errors import GenException
-from gentest.validate.roundtrip import fmt_err
 import pytest
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     term: TerminalReporter = item.config.pluginmanager.getplugin("terminalreporter")
     write_status(term)
 
@@ -27,18 +25,14 @@
     return line if ix == -1 else line[0:ix]
 
 
 
 def custom_repr_failure(self, excinfo: pytest.ExceptionInfo, style=None):
     err = excinfo.value
     match err:
-        case ExceptionGroup():
-            return fmt_err(err, None, getattr(err, "key_hash"))
-        case GenException():
-            return fmt_err(err, None, getattr(err, "key_hash"))
         case Exception():
             return str(err) + "\n\n" + condense_traceback(err)
         case _:
             raise err
     # return str(excinfo.value)
     # print("hi", excinfo)
```

### Comparing `relationalai-0.1.9/tests/roundtrip/test_document.py` & `relationalai-0.2.0/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/tests/roundtrip/test_task.py` & `relationalai-0.2.0/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.9/PKG-INFO` & `relationalai-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: relationalai
-Version: 0.1.9
+Version: 0.2.0
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
-Requires-Dist: docutils
 Requires-Dist: gravis
 Requires-Dist: inquirerpy
 Requires-Dist: nicegui
+Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pyarrow
 Requires-Dist: rai-sdk
-Requires-Dist: snowflake-connector-python
-Requires-Dist: sqlean
+Requires-Dist: requests
+Requires-Dist: rich
+Requires-Dist: snowflake-connector-python[secure-local-storage]
+Requires-Dist: toml
+Requires-Dist: tomlkit
+Requires-Dist: websockets
 Provides-Extra: dev
 Requires-Dist: argcomplete; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
+Requires-Dist: coverage; extra == 'dev'
+Requires-Dist: ddtrace; extra == 'dev'
 Requires-Dist: faker; extra == 'dev'
 Requires-Dist: hupper; extra == 'dev'
 Requires-Dist: hypothesis; extra == 'dev'
+Requires-Dist: pexpect; extra == 'dev'
 Requires-Dist: prompt-toolkit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-snapshot; extra == 'dev'
-Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
-Requires-Dist: tabulate; extra == 'dev'
 Requires-Dist: watchdog; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # The RelationalAI Python Library
 
 The Python library for building and querying knowledge graphs with RelationalAI.
```

