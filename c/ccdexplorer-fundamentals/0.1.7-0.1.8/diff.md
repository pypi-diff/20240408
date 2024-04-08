# Comparing `tmp/ccdexplorer-fundamentals-0.1.7.tar.gz` & `tmp/ccdexplorer-fundamentals-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdexplorer-fundamentals-0.1.7.tar", last modified: Thu Mar 21 17:39:18 2024, max compression
+gzip compressed data, was "ccdexplorer-fundamentals-0.1.8.tar", last modified: Mon Apr  8 17:48:33 2024, max compression
```

## Comparing `ccdexplorer-fundamentals-0.1.7.tar` & `ccdexplorer-fundamentals-0.1.8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.885500 ccdexplorer-fundamentals-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-21 17:39:18.885500 ccdexplorer-fundamentals-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.869500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.873500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.873500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/CCD_Types/
--rw-r--r--   0 runner    (1001) docker     (127)    38515 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.873500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.873500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/health/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.873500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/v2/
--rw-r--r--   0 runner    (1001) docker     (127)   190426 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.881500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    38653 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    99596 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   131737 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   198939 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/wadze.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.881500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    40923 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/cis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/cns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.885500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_store_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/tooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    46983 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/user_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.885500 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-21 17:39:18.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-21 17:39:18.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 17:39:18.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-21 17:39:18.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-21 17:39:18.000000 ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 17:39:18.885500 ccdexplorer-fundamentals-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:18.885500 ccdexplorer-fundamentals-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:39:09.000000 ccdexplorer-fundamentals-0.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.738663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.742663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.742663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/CCD_Types/
+-rw-r--r--   0 runner    (1001) docker     (127)    38515 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.742663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.742663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/health/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.742663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)   190426 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.746663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38653 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    99596 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131737 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198939 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/wadze.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41164 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/cis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/cns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_store_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/tooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46983 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/user_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-08 17:48:33.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-08 17:48:33.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:48:33.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:48:33.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 17:48:33.000000 ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:33.750663 ccdexplorer-fundamentals-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:48:29.000000 ccdexplorer-fundamentals-0.1.8/tests/__init__.py
```

### Comparing `ccdexplorer-fundamentals-0.1.7/LICENSE.md` & `ccdexplorer-fundamentals-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/PKG-INFO` & `ccdexplorer-fundamentals-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdexplorer-fundamentals
-Version: 0.1.7
+Version: 0.1.8
 Summary: Shared code for CCDExplorer.io and its Notification Bot.
 Home-page: https://github.com/ccdexplorer/ccdexplorer-fundamentals
 Author: Sander de Ruiter
 Author-email: sdr@ccdexplorer.io
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ccdexplorer-fundamentals-0.1.7/README.md` & `ccdexplorer-fundamentals-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/__init__.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/health_pb2.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/health_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/service_pb2.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/types_pb2.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/GRPCClient/wadze.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/GRPCClient/wadze.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/block.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/block.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_search.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_search.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/cis.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/cis.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,17 +539,17 @@
         except:  # noqa: E722
             console.log(
                 f"""{result.tag}: {result.from_address} is not listed as 
                 token holder for {token_address}?"""
             )
             # exit
 
-    def save_logged_event(
+    def formulate_logged_event(
         self,
-        db_to_use,
+        slot_time: dt.datetime,
         tag_: int,
         result: Union[
             mintEvent, burnEvent, transferEvent, updateOperatorEvent, tokenMetadataEvent
         ],
         instance_address: str,
         event: str,
         height: int,
@@ -563,15 +563,15 @@
                 token_address = f"{instance_address}-operator"
             elif tag_ == 250:
                 token_address = f"{instance_address}-nonce"
             else:
                 token_address = f"{instance_address}-{result.token_id}"
             _id = f"{height}-{token_address}-{event}-{_id_postfix}"
             if result:
-                result_dict = result.dict()
+                result_dict = result.model_dump()
             else:
                 result_dict = {}
             if "token_amount" in result_dict:
                 result_dict["token_amount"] = str(result_dict["token_amount"])
 
             d = {
                 "_id": _id,
@@ -581,23 +581,27 @@
                 "event_type": LoggedEvents(tag_).name,
                 "block_height": height,
                 "tx_hash": tx_hash,
                 "tx_index": tx_index,
                 "ordering": ordering,
                 "token_address": token_address,
                 "contract": instance_address,
+                "date": f"{slot_time:%Y-%m-%d}",
             }
-            return ReplaceOne(
-                {"_id": _id},
-                replacement=d,
-                upsert=True,
+            return (
+                MongoTypeLoggedEvent(**d),
+                ReplaceOne(
+                    {"_id": _id},
+                    replacement=d,
+                    upsert=True,
+                ),
             )
 
         else:
-            return None
+            return (None, None)
 
     # not used
     def execute_logged_event(
         self,
         db_to_use,
         tag_: int,
         result: Union[mintEvent, burnEvent, transferEvent, tokenMetadataEvent],
@@ -618,15 +622,15 @@
         elif tag_ == 251:
             self.save_metadata(db_to_use, instance_address, result, height)
         elif tag_ == 250:
             pass  # nonceEvent
 
     def process_event(
         self,
-        db_to_use,
+        slot_time: dt.datetime,
         instance_address: str,
         event: str,
         height: int,
         tx_hash: str,
         tx_index: int,
         ordering: int,
         _id_postfix: str,
@@ -635,28 +639,28 @@
         logged_event = None
         token_address = None
         if result:
             # if tag_ in [255, 254, 253, 252, 251, 250]:
             if tag_ in [255, 254, 253, 251]:
                 token_address = f"{instance_address}-{result.token_id}"
 
-                logged_event = self.save_logged_event(
-                    db_to_use,
+                (logged_event, logged_event_for_queue) = self.formulate_logged_event(
+                    slot_time,
                     tag_,
                     result,
                     instance_address,
                     event,
                     height,
                     tx_hash,
                     tx_index,
                     ordering,
                     _id_postfix,
                 )
 
-        return tag_, logged_event, token_address
+        return tag_, logged_event, logged_event_for_queue, token_address
 
     ###############
 
     def standard_identifier(self, identifier: StandardIdentifiers) -> bytes:
         si = io.BytesIO()
         # write the length of ASCII characters for the identifier
         number = len(identifier.value)
```

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/cns.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/cns.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/credential.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/credential.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/env.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/env.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # ruff: noqa :E501, F405
+import datetime as dt
 from enum import Enum
-from ccdexplorer_fundamentals.mongodb_queries._search_transfers import (
-    Mixin as _search_transfers,
-)
-from ccdexplorer_fundamentals.mongodb_queries._subscriptions import (
-    Mixin as _subscriptions,
-)
-from ccdexplorer_fundamentals.mongodb_queries._baker_distributions import (
-    Mixin as _distributions,
-)
-from ccdexplorer_fundamentals.mongodb_queries._store_block import Mixin as _store_block
-from ccdexplorer_fundamentals.mongodb_queries._apy_calculations import (
-    Mixin as _apy_calculations,
-)
-from ccdexplorer_fundamentals.GRPCClient.CCD_Types import *  # noqa: F403
-from ccdexplorer_fundamentals.env import MONGO_URI
+from typing import Dict, Optional, Union
+
 import motor.motor_asyncio
 from motor.motor_asyncio import AsyncIOMotorCollection
+from pydantic import BaseModel, ConfigDict, Field
 from pymongo import MongoClient
 from pymongo.collection import Collection
-
 from rich.console import Console
-from typing import Dict, Optional, Union
-from ccdexplorer_fundamentals.tooter import Tooter, TooterType, TooterChannel
-from pydantic import BaseModel, Field, ConfigDict
-import datetime as dt
 
+from ccdexplorer_fundamentals.env import MONGO_URI
+from ccdexplorer_fundamentals.GRPCClient.CCD_Types import *  # noqa: F403
+from ccdexplorer_fundamentals.mongodb_queries._apy_calculations import (
+    Mixin as _apy_calculations,
+)
+from ccdexplorer_fundamentals.mongodb_queries._baker_distributions import (
+    Mixin as _distributions,
+)
+from ccdexplorer_fundamentals.mongodb_queries._search_transfers import (
+    Mixin as _search_transfers,
+)
+from ccdexplorer_fundamentals.mongodb_queries._store_block import Mixin as _store_block
+from ccdexplorer_fundamentals.mongodb_queries._subscriptions import (
+    Mixin as _subscriptions,
+)
+from ccdexplorer_fundamentals.tooter import Tooter, TooterChannel, TooterType
 
 console = Console()
 
 
 class MongoLabeledAccount(BaseModel):
     id: str = Field(..., alias="_id")
     account_index: Optional[CCD_AccountIndex] = None
@@ -71,14 +71,26 @@
     effect_type: str
     balance_movement: Optional[AccountStatementEntryType] = None
     block_height: int
     included_in_flow: Optional[bool] = None
     date: Optional[str] = None
 
 
+class MongoTokensImpactedAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+    id: str = Field(..., alias="_id")
+    tx_hash: str
+    impacted_address: str
+    impacted_address_canonical: str
+    event_type: str
+    token_address: str
+    block_height: int
+    date: str
+
+
 class MongoTypeBlockPerDay(BaseModel):
     """
     Block Per Day. This type is stored in the collection `blocks_per_day`.
 
     :Parameters:
     - `_id`: the date of the day that ended
     - `date`: the date of the day that ended
@@ -354,16 +366,18 @@
     impacted_addresses_all_top_list = "impacted_addresses_all_top_list"
     # statistics and pre-renders
     pre_tokens_overview = "pre_tokens_overview"
     pre_addresses_by_contract_count = "pre_addresses_by_contract_count"
     pre_tokens_by_address = "pre_tokens_by_address"
     statistics = "statistics"
     pre_render = "pre_render"
+
     # addresses and contracts per net per usecase
     usecases = "usecases"
+    tokens_impacted_addresses = "tokens_impacted_addresses"
 
 
 class CollectionsUtilities(Enum):
     labeled_accounts = "labeled_accounts"
     labeled_accounts_metadata = "labeled_accounts_metadata"
     users_prod = "users_prod"
     users_dev = "users_dev"
```

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_store_block.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_store_block.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/node.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/node.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/pool.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/pool.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/tooter.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/tooter.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/transaction.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/transaction.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals/user_v2.py` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals/user_v2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/PKG-INFO` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdexplorer-fundamentals
-Version: 0.1.7
+Version: 0.1.8
 Summary: Shared code for CCDExplorer.io and its Notification Bot.
 Home-page: https://github.com/ccdexplorer/ccdexplorer-fundamentals
 Author: Sander de Ruiter
 Author-email: sdr@ccdexplorer.io
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ccdexplorer-fundamentals-0.1.7/ccdexplorer_fundamentals.egg-info/SOURCES.txt` & `ccdexplorer-fundamentals-0.1.8/ccdexplorer_fundamentals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdexplorer-fundamentals-0.1.7/setup.py` & `ccdexplorer-fundamentals-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="ccdexplorer-fundamentals",
-    version="0.1.7",
+    version="0.1.8",
     author="Sander de Ruiter",
     author_email="sdr@ccdexplorer.io",
     description="Shared code for CCDExplorer.io and its Notification Bot.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ccdexplorer/ccdexplorer-fundamentals",
     project_urls={},
```

