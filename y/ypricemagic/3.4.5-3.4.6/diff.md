# Comparing `tmp/ypricemagic-3.4.5.tar.gz` & `tmp/ypricemagic-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-3.4.5.tar", last modified: Tue Apr  2 08:01:15 2024, max compression
+gzip compressed data, was "ypricemagic-3.4.6.tar", last modified: Mon Apr  8 16:03:27 2024, max compression
```

## Comparing `ypricemagic-3.4.5.tar` & `ypricemagic-3.4.6.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.385708 ypricemagic-3.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.393709 ypricemagic-3.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.393709 ypricemagic-3.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.385708 ypricemagic-3.4.5/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.385708 ypricemagic-3.4.5/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.393709 ypricemagic-3.4.5/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/scripts/debug-curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/scripts/debug-price.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/test_uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/test_velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.401708 ypricemagic-3.4.5/y/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.401708 ypricemagic-3.4.5/y/_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/_db/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/_ep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/price.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/classes/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/velov2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13900 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/mooniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/solidly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    31130 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/rkp3r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/solidex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/y/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.181417 ypricemagic-3.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.149417 ypricemagic-3.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.153417 ypricemagic-3.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-08 16:03:27.181417 ypricemagic-3.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.153417 ypricemagic-3.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.149417 ypricemagic-3.4.6/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.149417 ypricemagic-3.4.6/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.157417 ypricemagic-3.4.6/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.157417 ypricemagic-3.4.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/scripts/debug-curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/scripts/debug-price.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 16:03:27.181417 ypricemagic-3.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.157417 ypricemagic-3.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.157417 ypricemagic-3.4.6/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.157417 ypricemagic-3.4.6/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.161417 ypricemagic-3.4.6/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/dex/test_uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/dex/test_velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.161417 ypricemagic-3.4.6/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.161417 ypricemagic-3.4.6/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.161417 ypricemagic-3.4.6/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.161417 ypricemagic-3.4.6/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.161417 ypricemagic-3.4.6/y/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/_db/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/_ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/_db/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.165417 ypricemagic-3.4.6/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.169417 ypricemagic-3.4.6/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/interfaces/uniswap/velov2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.169417 ypricemagic-3.4.6/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.169417 ypricemagic-3.4.6/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.169417 ypricemagic-3.4.6/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/mooniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/solidly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.173417 ypricemagic-3.4.6/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/uniswap/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/dex/velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.173417 ypricemagic-3.4.6/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.173417 ypricemagic-3.4.6/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/rkp3r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/solidex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.173417 ypricemagic-3.4.6/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.173417 ypricemagic-3.4.6/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.177417 ypricemagic-3.4.6/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.177417 ypricemagic-3.4.6/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.177417 ypricemagic-3.4.6/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-08 16:03:04.000000 ypricemagic-3.4.6/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:03:27.177417 ypricemagic-3.4.6/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-08 16:03:27.000000 ypricemagic-3.4.6/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-08 16:03:27.000000 ypricemagic-3.4.6/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:03:27.000000 ypricemagic-3.4.6/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 16:03:27.000000 ypricemagic-3.4.6/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 16:03:27.000000 ypricemagic-3.4.6/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-3.4.5/.github/workflows/codeql-analysis.yml` & `ypricemagic-3.4.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/.github/workflows/deploy-docs.yml` & `ypricemagic-3.4.6/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/.github/workflows/pytest.yaml` & `ypricemagic-3.4.6/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/.github/workflows/release.yaml` & `ypricemagic-3.4.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/CONTRIBUTING.md` & `ypricemagic-3.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/LICENSE.txt` & `ypricemagic-3.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/Makefile` & `ypricemagic-3.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/PKG-INFO` & `ypricemagic-3.4.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypricemagic
-Version: 3.4.5
+Version: 3.4.6
 Summary: Use this tool to extract historical on-chain price data from an archive node. Shoutout to @bantg and @nymmrx for their awesome work on yearn-exporter that made this library possible.
 Home-page: https://github.com/BobTheBuidler/ypricemagic
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 License-File: LICENSE.txt
 Requires-Dist: bobs_lazy_logging==0.0.4
```

### Comparing `ypricemagic-3.4.5/README.md` & `ypricemagic-3.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/Makefile` & `ypricemagic-3.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/alabaster.css` & `ypricemagic-3.4.6/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/basic.css` & `ypricemagic-3.4.6/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/doctools.js` & `ypricemagic-3.4.6/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/language_data.js` & `ypricemagic-3.4.6/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/pygments.css` & `ypricemagic-3.4.6/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/searchtools.js` & `ypricemagic-3.4.6/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/_build/html/_static/sphinx_highlight.js` & `ypricemagic-3.4.6/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/conf.py` & `ypricemagic-3.4.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/docs/make.bat` & `ypricemagic-3.4.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/scripts/debug-curve.py` & `ypricemagic-3.4.6/scripts/debug-curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/scripts/debug-price.py` & `ypricemagic-3.4.6/scripts/debug-price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/setup.py` & `ypricemagic-3.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/classes/test_erc20.py` & `ypricemagic-3.4.6/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/classes/test_singleton.py` & `ypricemagic-3.4.6/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/fixtures.py` & `ypricemagic-3.4.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/dex/test_balancer.py` & `ypricemagic-3.4.6/tests/prices/dex/test_balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/dex/test_uniswap.py` & `ypricemagic-3.4.6/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/lending/test_aave.py` & `ypricemagic-3.4.6/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/lending/test_compound.py` & `ypricemagic-3.4.6/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/test_chainlink.py` & `ypricemagic-3.4.6/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/test_magic.py` & `ypricemagic-3.4.6/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/test_popsicle.py` & `ypricemagic-3.4.6/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/test_synthetix.py` & `ypricemagic-3.4.6/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/test_yearn.py` & `ypricemagic-3.4.6/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/tests/prices/utils/test_buckets.py` & `ypricemagic-3.4.6/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/ENVIRONMENT_VARIABLES.py` & `ypricemagic-3.4.6/y/ENVIRONMENT_VARIABLES.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/__init__.py` & `ypricemagic-3.4.6/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/__init__.py` & `ypricemagic-3.4.6/y/_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/common.py` & `ypricemagic-3.4.6/y/_db/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/config.py` & `ypricemagic-3.4.6/y/_db/config.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/decorators.py` & `ypricemagic-3.4.6/y/_db/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/entities.py` & `ypricemagic-3.4.6/y/_db/entities.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/exceptions.py` & `ypricemagic-3.4.6/y/_db/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/structs.py` & `ypricemagic-3.4.6/y/_db/structs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/_ep.py` & `ypricemagic-3.4.6/y/_db/utils/_ep.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/bulk.py` & `ypricemagic-3.4.6/y/_db/utils/bulk.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/contract.py` & `ypricemagic-3.4.6/y/_db/utils/contract.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/logs.py` & `ypricemagic-3.4.6/y/_db/utils/logs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/price.py` & `ypricemagic-3.4.6/y/_db/utils/price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/token.py` & `ypricemagic-3.4.6/y/_db/utils/token.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/traces.py` & `ypricemagic-3.4.6/y/_db/utils/traces.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/_db/utils/utils.py` & `ypricemagic-3.4.6/y/_db/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/classes/common.py` & `ypricemagic-3.4.6/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/classes/singleton.py` & `ypricemagic-3.4.6/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/constants.py` & `ypricemagic-3.4.6/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/contracts.py` & `ypricemagic-3.4.6/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/datatypes.py` & `ypricemagic-3.4.6/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/decorators.py` & `ypricemagic-3.4.6/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/erc20.py` & `ypricemagic-3.4.6/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/exceptions.py` & `ypricemagic-3.4.6/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/ERC20.py` & `ypricemagic-3.4.6/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-3.4.6/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/compound/unitroller.py` & `ypricemagic-3.4.6/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-3.4.6/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/multicall2.py` & `ypricemagic-3.4.6/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-3.4.6/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-3.4.6/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/interfaces/uniswap/velov2.py` & `ypricemagic-3.4.6/y/interfaces/uniswap/velov2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/networks.py` & `ypricemagic-3.4.6/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/band.py` & `ypricemagic-3.4.6/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/chainlink.py` & `ypricemagic-3.4.6/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/convex.py` & `ypricemagic-3.4.6/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/balancer/balancer.py` & `ypricemagic-3.4.6/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/balancer/v1.py` & `ypricemagic-3.4.6/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/balancer/v2.py` & `ypricemagic-3.4.6/y/prices/dex/balancer/v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,19 @@
             self.contract
     
     @a_sync_cache
     @stuck_coro_debugger
     async def list_pools(self, block: Optional[Block] = None) -> List["BalancerV2Pool"]:
         return [pool async for pool in self._events.events(to_block=block)]
 
+    async def pools_for_token(self, token: Address, block: Optional[Block] = None) -> AsyncIterator["BalancerV2Pool"]:
+        async for pool, info in a_sync.map(lambda pool: pool.tokens(block=block, sync=False), self._events.events(to_block=block)):
+            if token in info:
+                yield pool
+                
     @a_sync_cache
     @stuck_coro_debugger
     async def get_pool_tokens(self, pool_id: HexBytes, block: Optional[Block] = None):
         contract = await contracts.Contract.coroutine(self.address)
         return await contract.getPoolTokens.coroutine(pool_id, block_identifier = block)
     
     @a_sync_cache
@@ -83,28 +88,23 @@
         ])
     
     @a_sync_cache
     @stuck_coro_debugger
     async def deepest_pool_for(self, token_address: Address, block: Optional[Block] = None) -> Tuple[Optional["BalancerV2Pool"], int]:
         logger = get_price_logger(token_address, block, 'balancer.v2')
         deepest_pool, deepest_balance = None, 0
-        async for pool in self._yield_pools_for(token_address, block=block):
+        async for pool in self.pools_for_token(token_address, block=block):
             info: Dict[ERC20, WeiBalance]
             if info := await pool.get_balances(block=block, sync=False):
                 pool_balance = info[token_address].balance
                 if pool_balance > deepest_balance:
                     deepest_pool = pool
         logger.debug("deepest pool %s balance %s", deepest_pool, deepest_balance)
         return deepest_pool, deepest_balance
 
-    async def _yield_pools_for(self, token: Address, block: Optional[Block] = None) -> AsyncIterator["BalancerV2Pool"]:
-        async for pool, info in a_sync.map(lambda pool: pool.tokens(block=block, sync=False), self._events.events(to_block=block)):
-            if token in info:
-                yield pool
-
 class BalancerEvents(ProcessedEvents[Tuple[HexBytes, EthAddress, Block]]):
     __slots__ = "asynchronous", 
     def __init__(self, *args, asynchronous: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
         self.asynchronous = asynchronous
     def _include_event(self, event: _EventItem) -> bool:
         # NOTE: For some reason the Balancer fork on Fantom lists "0x3e522051A9B1958Aa1e828AC24Afba4a551DF37d"
```

### Comparing `ypricemagic-3.4.5/y/prices/dex/genericamm.py` & `ypricemagic-3.4.6/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/mooniswap.py` & `ypricemagic-3.4.6/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/solidly.py` & `ypricemagic-3.4.6/y/prices/dex/solidly.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-3.4.6/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/uniswap/v1.py` & `ypricemagic-3.4.6/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/uniswap/v2.py` & `ypricemagic-3.4.6/y/prices/dex/uniswap/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,15 @@
         except Exception as e:
             e.args = (*e.args, self.__repr__(), token, block, ignore_pools)
             raise e
     
     @cached_property
     def _supports_uniswap_helper(self) -> bool:
         """returns True if our uniswap helper contract is supported, False if not"""
-        return FACTORY_HELPER and self.label and self.label not in {"zipswap"}
+        return chain.id != Network.Mainnet and FACTORY_HELPER and self.label and self.label not in {"zipswap"}
 
 
     def _smol_brain_path_selector(self, token_in: AddressOrContract, token_out: AddressOrContract, paired_against: AddressOrContract) -> Path:
         # sourcery skip: assign-if-exp, lift-return-into-if, merge-duplicate-blocks, merge-else-if-into-elif, remove-redundant-if, remove-unnecessary-cast
         '''Chooses swap path to use for quote'''
         # NOTE: can we just delete this now? probably, must test
         token_in, token_out, paired_against = str(token_in), str(token_out), str(paired_against)
```

### Comparing `ypricemagic-3.4.5/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-3.4.6/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/dex/uniswap/v3.py` & `ypricemagic-3.4.6/y/prices/dex/uniswap/v3.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -115,32 +115,45 @@
             raise UnsupportedNetwork('compound is not supported on this network')
         self.fee_tiers = addresses[chain.id]['fee_tiers']
         self.loading = False
         self._pools = {}
 
     def __contains__(self, asset) -> bool:
         return chain.id in addresses
+    
+    @cached_property
+    def loaded(self) -> a_sync.Event:
+        return a_sync.Event(name=self)
 
     @a_sync.aka.property
     async def factory(self) -> Contract:
         return await Contract.coroutine(addresses[chain.id]['factory'])
     __factory__: HiddenMethodDescriptor[Self, Contract]
     
-    @cached_property
-    def loaded(self) -> a_sync.Event:
-        return a_sync.Event(name=self)
-    
     @a_sync.aka.cached_property
     async def quoter(self) -> Contract:
         quoter = addresses[chain.id]['quoter']
         try:
             return await Contract.coroutine(quoter)
         except ContractNotVerified:
             return Contract.from_abi("Quoter", quoter, UNIV3_QUOTER_ABI)
     __quoter__: HiddenMethodDescriptor[Self, Contract]
+
+    @a_sync.aka.cached_property
+    @stuck_coro_debugger
+    async def pools(self) -> List[UniswapV3Pool]:
+        factory = await self.__factory__
+        return UniV3Pools(factory, asynchronous=self.asynchronous)
+    __pools__: HiddenMethodDescriptor[Self, "UniV3Pools"]
+
+    async def pools_for_token(self, token: Address, block: Block) -> AsyncIterator[UniswapV3Pool]:
+        pools = await self.__pools__
+        async for pool in pools.objects(to_block=block):
+            if token in pool:
+                yield pool
     
     @stuck_coro_debugger
     @a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_price(
         self, 
         token: Address, 
         block: Optional[Block] = None,
@@ -173,21 +186,14 @@
             (amount if isinstance(amount, int) else amount[0]) / _undo_fees(path) / 1e6
             for amount, path in zip(results, paths)
             if amount
         ]
         logger.debug("outputs: %s", outputs)
         return UsdPrice(max(outputs)) if outputs else None
 
-    @a_sync.aka.cached_property
-    @stuck_coro_debugger
-    async def pools(self) -> List[UniswapV3Pool]:
-        factory = await self.__factory__
-        return UniV3Pools(factory, asynchronous=self.asynchronous)
-    __pools__: HiddenMethodDescriptor[Self, "UniV3Pools"]
-
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
     async def check_liquidity(self, token: Address, block: Block, ignore_pools: Tuple[Pool, ...] = ()) -> int:
         logger.debug("checking %s liquidity for %s at %s", self, token, block)
         if chain.id == Network.Mainnet and token == "0x6DEA81C8171D0bA574754EF6F8b412F2Ed88c54D":
             # LQTY, TODO refactor this somehow
             return 0
@@ -223,20 +229,14 @@
                 logger.debug("insufficient liquidity for %s", pool)
                 token_in_tasks.pop(pool)
 
         liquidity = max(await asyncio.gather(*token_in_tasks.values())) if token_in_tasks else 0
         logger.debug("%s liquidity for %s at %s is %s", self, token, block, liquidity)
         return liquidity
 
-    async def pools_for_token(self, token: Address, block: Block) -> AsyncIterator[UniswapV3Pool]:
-        pools = await self.__pools__
-        async for pool in pools.objects(to_block=block):
-            if token in pool:
-                yield pool
-
 def _encode_path(path) -> bytes:
     types = [type for _, type in zip(path, cycle(['address', 'uint24']))]
     return encode_abi_packed(types, path)
 
 def _undo_fees(path) -> float:
     fees = [1 - fee / FEE_DENOMINATOR for fee in path if isinstance(fee, int)]
     return math.prod(fees)
```

### Comparing `ypricemagic-3.4.5/y/prices/dex/velodrome.py` & `ypricemagic-3.4.6/y/prices/dex/velodrome.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/eth_derivs/creth.py` & `ypricemagic-3.4.6/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/eth_derivs/wsteth.py` & `ypricemagic-3.4.6/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/gearbox.py` & `ypricemagic-3.4.6/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/lending/aave.py` & `ypricemagic-3.4.6/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/lending/compound.py` & `ypricemagic-3.4.6/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/lending/ib.py` & `ypricemagic-3.4.6/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/magic.py` & `ypricemagic-3.4.6/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/one_to_one.py` & `ypricemagic-3.4.6/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/popsicle.py` & `ypricemagic-3.4.6/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/rkp3r.py` & `ypricemagic-3.4.6/y/prices/rkp3r.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/solidex.py` & `ypricemagic-3.4.6/y/prices/solidex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/stable_swap/belt.py` & `ypricemagic-3.4.6/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/stable_swap/curve.py` & `ypricemagic-3.4.6/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/stable_swap/ellipsis.py` & `ypricemagic-3.4.6/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/stable_swap/froyo.py` & `ypricemagic-3.4.6/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-3.4.6/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/stable_swap/saddle.py` & `ypricemagic-3.4.6/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/synthetix.py` & `ypricemagic-3.4.6/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-3.4.6/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/tokenized_fund/gelato.py` & `ypricemagic-3.4.6/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/tokenized_fund/piedao.py` & `ypricemagic-3.4.6/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-3.4.6/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/utils/buckets.py` & `ypricemagic-3.4.6/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/utils/sense_check.py` & `ypricemagic-3.4.6/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/utils/ypriceapi.py` & `ypricemagic-3.4.6/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/prices/yearn.py` & `ypricemagic-3.4.6/y/prices/yearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if chain.id == Network.Arbitrum and self.address == '0x57c7E0D43C05bCe429ce030132Ca40F6FA5839d7':
             return ERC20(await raw_call(self.address, 'usdl()', output='address', sync=False), asynchronous=self.asynchronous)
 
         try:
             underlying = await probe(self.address, underlying_methods)
         except AssertionError:
             # special handler for some strange beefy vaults
-            if not (method := {"BeefyVaultV6Matic": "wmatic()", "BeefyVenusVaultBNB": "wbnb()"}.get(self.build_name)):
+            if not (method := {"BeefyVaultV6Matic": "wmatic()", "BeefyVenusVaultBNB": "wbnb()"}.get(await self.__build_name__)):
                 raise
             underlying = await raw_call(self.address, method, output='address', sync=False)
         
         if not underlying:
             # certain reaper vaults
             lend_platform = await self.has_method('lendPlatform()(address)', return_response=True, sync=False)
             if lend_platform:
```

### Comparing `ypricemagic-3.4.5/y/time.py` & `ypricemagic-3.4.6/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/client.py` & `ypricemagic-3.4.6/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/events.py` & `ypricemagic-3.4.6/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/fakes.py` & `ypricemagic-3.4.6/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/gather.py` & `ypricemagic-3.4.6/y/utils/gather.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/logging.py` & `ypricemagic-3.4.6/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/middleware.py` & `ypricemagic-3.4.6/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/multicall.py` & `ypricemagic-3.4.6/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/y/utils/raw_calls.py` & `ypricemagic-3.4.6/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/ypricemagic/magic.py` & `ypricemagic-3.4.6/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.5/ypricemagic.egg-info/PKG-INFO` & `ypricemagic-3.4.6/ypricemagic.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypricemagic
-Version: 3.4.5
+Version: 3.4.6
 Summary: Use this tool to extract historical on-chain price data from an archive node. Shoutout to @bantg and @nymmrx for their awesome work on yearn-exporter that made this library possible.
 Home-page: https://github.com/BobTheBuidler/ypricemagic
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 License-File: LICENSE.txt
 Requires-Dist: bobs_lazy_logging==0.0.4
```

### Comparing `ypricemagic-3.4.5/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-3.4.6/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

