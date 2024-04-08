# Comparing `tmp/original_metaplex_python-0.0.1a1.tar.gz` & `tmp/original_metaplex_python-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "original_metaplex_python-0.0.1a1.tar", last modified: Mon Mar 25 10:49:26 2024, max compression
+gzip compressed data, was "original_metaplex_python-0.0.1a2.tar", last modified: Mon Apr  8 11:17:51 2024, max compression
```

## Comparing `original_metaplex_python-0.0.1a1.tar` & `original_metaplex_python-0.0.1a2.tar`

### file list

```diff
@@ -1,260 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.314678 original_metaplex_python-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-25 10:49:26.314678 original_metaplex_python-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.278677 original_metaplex_python-0.0.1a1/original_metaplex_python/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/__pkg__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/core_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/core_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/core_plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/irys_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/metaplex_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/program_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/read_api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/sdk_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/identity_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/identity_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/identity_module/identity_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/identity_module/identity_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/identity_module/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/irys_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/irys_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/irys_storage/irys_storage_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/irys_storage/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/keypair_identity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/keypair_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/keypair_identity/keypair_identity_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/keypair_identity/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/metaplex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.286677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/delegate_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/delegate_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.286677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/json_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/nft_edition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/nft_builders_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/nft_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/nft_pdas_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.286677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/create_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/create_sft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/delete_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/find_nft_by_mint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/mint_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/transfer_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/unverify_nft_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/update_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/verify_nft_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/verify_nft_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/operation_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/operation_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/operation_module/operation_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/operation_module/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/program_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/program_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/program_module/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/program_module/program_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/rpc_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/rpc_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/rpc_module/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/rpc_module/rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/metaplex_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/operations/create_account.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/operations/transfer_sol.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/system_builders_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/system_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.290677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/models/mint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/models/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/program.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/token_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/token_pdas_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.294677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/pda.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/program.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/read_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.294677 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/read_api_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/transaction_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.294677 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.294677 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.298678 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/collection_authority_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/edition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/edition_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/edition_marker_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/master_edition_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/master_edition_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/metadata_delegate_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/token_owned_escrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/token_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/use_authority_record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.298678 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    61208 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.298678 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/idl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/idl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.306677 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/approve_collection_authority.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/approve_use_authority.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/bubblegum_set_collection_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/burn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/burn_edition_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/burn_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/close_escrow_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/convert_master_edition_v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_escrow_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_master_edition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_master_edition_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_master_edition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_new_edition_from_master_edition_via_printing_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens_via_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_set_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/freeze_delegated_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/mint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_vault_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/print.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/puff_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/remove_creator_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/revoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/revoke_collection_authority.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/revoke_use_authority.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_sized_collection_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_collection_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_token_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/sign_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/thaw_delegated_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/transfer_out_of_escrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unverify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unverify_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unverify_sized_collection_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update_primary_sale_happened_via_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/utilize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/verify_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/verify_sized_collection_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/program_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.314678 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/approve_use_authority_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/asset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/authority_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/authorization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/burn_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection_details_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/create_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/create_master_edition_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/create_metadata_account_args_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/data_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32281 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/delegate_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/escrow_authority.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/lock_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/metadata_delegate_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/migration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/mint_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/mint_new_edition_from_master_edition_via_token_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/payload_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/payload_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/print_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/print_supply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/programmable_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/proof_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/reservation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/revoke_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/rule_set_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/seeds_vec.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/set_collection_size_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/token_delegate_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/token_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/token_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/transfer_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/transfer_out_of_escrow_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/unlock_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    41245 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/update_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/update_metadata_account_args_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/use_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/use_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/uses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/uses_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/utilize_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/verification_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:49:26.282678 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-25 10:49:26.000000 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-03-25 10:49:26.000000 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:49:26.000000 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:49:26.000000 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-25 10:49:26.000000 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 10:49:26.000000 original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 10:49:26.314678 original_metaplex_python-0.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-25 10:49:18.000000 original_metaplex_python-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.572954 original_metaplex_python-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-08 11:17:51.572954 original_metaplex_python-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.536954 original_metaplex_python-0.0.1a2/original_metaplex_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/__pkg__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.536954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.540954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/core_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/core_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/core_plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.540954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/irys_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/metaplex_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/program_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/read_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/sdk_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.540954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/identity_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/identity_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/identity_module/identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/identity_module/identity_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/identity_module/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.540954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/irys_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/irys_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/irys_storage/irys_storage_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/irys_storage/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.540954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/keypair_identity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/keypair_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/keypair_identity/keypair_identity_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/keypair_identity/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/metaplex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.544954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/delegate_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/delegate_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.544954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/json_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/nft_edition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/nft_builders_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/nft_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/nft_pdas_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.544954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/approve_nft_collection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/approve_nft_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/create_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/create_sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/delete_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/find_nft_by_mint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/mint_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/revoke_nft_collection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/revoke_nft_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/transfer_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/unverify_nft_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/update_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/verify_nft_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/verify_nft_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.544954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/operation_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/operation_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/operation_module/operation_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/operation_module/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/program_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/program_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/program_module/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/program_module/program_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/rpc_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/rpc_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/rpc_module/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/rpc_module/rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/metaplex_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/operations/create_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/operations/transfer_sol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/system_builders_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/system_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.548954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/models/mint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/token_pdas_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.552954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/pda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.552954 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/read_api_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/transaction_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.552954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.552954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.552954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/collection_authority_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/edition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/edition_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/edition_marker_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/master_edition_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/master_edition_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/metadata_delegate_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/token_owned_escrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/token_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/use_authority_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.556954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61208 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.556954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/idl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/idl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.564954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/approve_collection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/approve_use_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/bubblegum_set_collection_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/burn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/burn_edition_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/burn_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/close_escrow_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/convert_master_edition_v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_escrow_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_master_edition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_master_edition_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_master_edition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_new_edition_from_master_edition_via_printing_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens_via_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_set_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/freeze_delegated_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/mint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_vault_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/puff_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/remove_creator_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/revoke_collection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/revoke_use_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_sized_collection_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_collection_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_token_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/sign_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/thaw_delegated_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/transfer_out_of_escrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unverify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unverify_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unverify_sized_collection_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update_primary_sale_happened_via_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/utilize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/verify_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/verify_sized_collection_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/program_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.572954 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/approve_use_authority_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/asset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/authority_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/authorization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/burn_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection_details_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/create_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/create_master_edition_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/create_metadata_account_args_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/data_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32281 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/delegate_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/escrow_authority.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/lock_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/metadata_delegate_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/migration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/mint_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/mint_new_edition_from_master_edition_via_token_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/payload_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/payload_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/print_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/print_supply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/programmable_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/proof_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/reservation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/revoke_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/rule_set_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/seeds_vec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/set_collection_size_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/token_delegate_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/token_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/token_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/transfer_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/transfer_out_of_escrow_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/unlock_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41245 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/update_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/update_metadata_account_args_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/use_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/use_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/uses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/uses_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/utilize_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/verification_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:51.536954 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-08 11:17:51.000000 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-04-08 11:17:51.000000 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:17:51.000000 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:17:51.000000 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 11:17:51.000000 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 11:17:51.000000 original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:17:51.572954 original_metaplex_python-0.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 11:17:39.000000 original_metaplex_python-0.0.1a2/setup.py
```

### Comparing `original_metaplex_python-0.0.1a1/LICENSE` & `original_metaplex_python-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/PKG-INFO` & `original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: original_metaplex_python
-Version: 0.0.1a1
+Name: original-metaplex-python
+Version: 0.0.1a2
 Summary: Python port of Metaplex JS SDK - https://github.com/metaplex-foundation/js
 Home-page: https://github.com/getoriginal/original-metaplex-python
 Author: Original
 Author-email: support@getoriginal.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `original_metaplex_python-0.0.1a1/README.md` & `original_metaplex_python-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/core_plugins/plugin.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/core_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/irys_error.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/irys_error.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/metaplex_error.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/metaplex_error.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/program_error.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/program_error.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/rpc_error.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/errors/sdk_error.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/errors/sdk_error.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/identity_module/identity_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/identity_module/identity_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/keypair_identity/keypair_identity_driver.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/keypair_identity/keypair_identity_driver.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/metaplex.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/metaplex.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/authorization.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/authorization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional, Union, cast
 
 from solders.pubkey import Pubkey
 
 from original_metaplex_python.metaplex.nft_module.delegate_input import (
+    MetadataDelegateInputWithData,
+    TokenDelegateInputWithData,
     TokenMetadataDelegateInput,
     parse_token_metadata_delegate_input,
 )
 from original_metaplex_python.metaplex.types.program import Program
 from original_metaplex_python.metaplex.types.signer import Signer, get_public_key
 from original_metaplex_python.token_metadata.generated.types import AuthorizationData
 
@@ -63,18 +65,19 @@
     TokenMetadataAuthorityHolder,
     TokenMetadataAuthorityMetadataDelegate,
     TokenMetadataAuthorityTokenDelegate,
 ]
 
 
 class AuthorityType(Enum):
-    Metadata = 0
-    MetadataDelegate = 1
-    TokenDelegate = 2
-    Holder = 3
+    None_ = 0
+    Metadata = 1
+    Holder = 2
+    MetadataDelegate = 3
+    TokenDelegate = 4
 
 
 @dataclass
 class TokenMetadataAuthorizationDetails:
     rules: Pubkey
     data: Optional[AuthorizationData] = None
 
@@ -144,15 +147,18 @@
             owner=input.authority.update_authority,
             delegate=input.authority.delegate,
             token=None,
             update_authority=input.authority.update_authority,
             type=input.authority.type,
         )
         delegate_output = parse_token_metadata_delegate_input(
-            metaplex, input.mint, delegate_input, input.programs
+            metaplex=metaplex,
+            mint=input.mint,
+            input=cast(MetadataDelegateInputWithData, delegate_input),
+            programs=input.programs,
         )
         delegate_record = delegate_output.delegate_record
         approver = delegate_output.approver
 
         auth.accounts.authority = get_public_key(input.authority.delegate)
         auth.accounts.delegate_record = delegate_record
         auth.accounts.approver = approver
@@ -164,15 +170,18 @@
             delegate=input.authority.delegate,
             token=input.authority.token,
             update_authority=None,
             type=input.authority.type,
         )
 
         delegate_output = parse_token_metadata_delegate_input(
-            metaplex, input.mint, delegate_input, input.programs
+            metaplex=metaplex,
+            mint=input.mint,
+            input=cast(TokenDelegateInputWithData, delegate_input),
+            programs=input.programs,
         )
 
         delegate_record = delegate_output.delegate_record
         approver = delegate_output.approver
         token_account = delegate_output.token_account
 
         auth.accounts.authority = get_public_key(input.authority.delegate)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/delegate_input.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/delegate_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Optional, cast
+from typing import Any, Optional, Union, cast
 
 from solders.pubkey import Pubkey
 
 from original_metaplex_python.metaplex.nft_module.nft_pdas_client import (
     MetadataDelegateRecordPdaInput,
     TokenRecordPdaInput,
 )
@@ -28,18 +28,40 @@
     is_token_delegate: bool
     delegate: Signer
     approver: Pubkey
     delegate_record: Pubkey
     token_account: Optional[Pubkey] = None
 
 
+@dataclass
+class MetadataDelegateInputWithData:
+    delegate: Signer
+    update_authority: Pubkey
+    type: str
+    data: Optional[Any] = None
+    __kind: Optional[Any] = None
+
+
+@dataclass
+class TokenDelegateInputWithData:
+    delegate: Signer
+    owner: Pubkey
+    type: str
+    data: Any
+    __kind: Any
+    token: Optional[Pubkey] = None
+
+
+DelegateInputWithData = Union[MetadataDelegateInputWithData, TokenDelegateInputWithData]
+
+
 def parse_token_metadata_delegate_input(
     metaplex,
     mint: Pubkey,
-    input: TokenMetadataDelegateInput,
+    input: DelegateInputWithData,
     programs: Optional[list[Program]] = None,
 ):
     if hasattr(input, "update_authority"):
         return TokenMetadataDelegateOutput(
             is_token_delegate=False,
             delegate=input.delegate,
             approver=cast(Pubkey, input.update_authority),
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/json_metadata.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/json_metadata.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/metadata.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/metadata.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/nft_edition.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/nft_edition.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/models/sft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/models/sft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/nft_builders_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/nft_builders_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from typing import Optional
 
 from ..utils.transaction_builder import TransactionBuilderOptions
+from .operations.approve_nft_collection_authority import (
+    ApproveNftCollectionAuthorityBuilderParams,
+    approve_nft_collection_authority_builder,
+)
+from .operations.approve_nft_delegate import (
+    ApproveNftDelegateBuilderParams,
+    approve_nft_delegate_builder,
+)
 from .operations.create_nft import CreateNftBuilderParams, create_nft_builder
 from .operations.create_sft import CreateSftBuilderParams, create_sft_builder
 from .operations.delete_nft import DeleteNftBuilderParams, delete_nft_builder
 from .operations.mint_nft import MintNftBuilderParams, mint_nft_builder
+from .operations.revoke_nft_collection_authority import (
+    RevokeNftCollectionAuthorityBuilderParams,
+    revoke_nft_collection_authority_builder,
+)
 from .operations.transfer_nft import TransferNftBuilderParams, transfer_nft_builder
 from .operations.unverify_nft_collection import (
     UnverifyNftCollectionBuilderParams,
     unverify_nft_collection_builder,
 )
 from .operations.update_nft import UpdateNftBuilderParams, update_nft_builder
 from .operations.verify_nft_collection import (
@@ -72,20 +84,49 @@
     def unverify_collection(
         self,
         input: UnverifyNftCollectionBuilderParams,
         options: Optional[TransactionBuilderOptions] = None,
     ):
         return unverify_nft_collection_builder(self.metaplex, input, options)
 
+    def approve_collection_authority(
+        self,
+        input: ApproveNftCollectionAuthorityBuilderParams,
+        options: Optional[TransactionBuilderOptions] = None,
+    ):
+        return approve_nft_collection_authority_builder(self.metaplex, input, options)
+
+    def revoke_collection_authority(
+        self,
+        input: RevokeNftCollectionAuthorityBuilderParams,
+        options: Optional[TransactionBuilderOptions] = None,
+    ):
+        return revoke_nft_collection_authority_builder(self.metaplex, input, options)
+
     def delete(
         self,
         input: DeleteNftBuilderParams,
         options: Optional[TransactionBuilderOptions] = None,
     ):
         return delete_nft_builder(self.metaplex, input, options)
 
     def update(
         self,
         input: UpdateNftBuilderParams,
         options: Optional[TransactionBuilderOptions] = None,
     ):
         return update_nft_builder(self.metaplex, input, options)
+
+    def delegate(
+        self,
+        input: ApproveNftDelegateBuilderParams,
+        options: Optional[TransactionBuilderOptions] = None,
+    ):
+        return approve_nft_delegate_builder(self.metaplex, input, options)
+
+    # TODO_ORIGINAL: Not used yet
+    # def revoke(
+    #         self,
+    #         input: RevokeNftDelegateBuilderParams,
+    #         options: Optional[TransactionBuilderOptions] = None
+    # ):
+    #     return revokeNftDelegateBuilder(self.metaplex, input, options);
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/nft_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/nft_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/nft_pdas_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/nft_pdas_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/create_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/create_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/create_sft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/create_sft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/delete_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/delete_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/find_nft_by_mint.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/find_nft_by_mint.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/mint_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/mint_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/transfer_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/transfer_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/unverify_nft_collection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/unverify_nft_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from original_metaplex_python.metaplex.nft_module.nft_pdas_client import (
     CollectionAuthorityRecordPdaInput,
     MetadataDelegateRecordPdaInput,
     MintAddressPdaInput,
 )
 from original_metaplex_python.metaplex.types.signer import Signer, get_public_key
 from original_metaplex_python.metaplex.utils.transaction_builder import (
+    InstructionWithSigners,
     TransactionBuilder,
     TransactionBuilderOptions,
 )
 from original_metaplex_python.token_metadata.generated.instructions import (
     UnverifyAccounts,
     UnverifyArgs,
     UnverifyCollectionAccounts,
@@ -132,19 +133,19 @@
             )
         )
 
         return (
             TransactionBuilder.make()
             .set_fee_payer(payer)
             .add(
-                {
-                    "instruction": instruction,
-                    "signers": [payer, collection_authority],
-                    "key": params.instruction_key or "unverify_collection",
-                }
+                InstructionWithSigners(
+                    instruction=instruction,
+                    signers=[payer, collection_authority],
+                    key=params.instruction_key or "unverify_collection",
+                )
             )
         )
 
     delegate_record = (
         metaplex.nfts()
         .pdas()
         .metadata_delegate_record(
@@ -160,25 +161,25 @@
         else None
     )
 
     return (
         TransactionBuilder.make()
         .set_fee_payer(payer)
         .add(
-            {
-                "instruction": unverify(
+            InstructionWithSigners(
+                instruction=unverify(
                     accounts=UnverifyAccounts(
                         authority=get_public_key(collection_authority),
                         delegate_record=delegate_record,
                         metadata=metadata,
                         collection_mint=collection_mint_address,
                         collection_metadata=collection_metadata,
                         sysvar_instructions=SYSVAR_INSTRUCTIONS_PUBKEY,
                     ),
                     args=UnverifyArgs(verification_args=CollectionV1()),
                     program_id=token_metadata_program.address,
                 ),
-                "signers": [collection_authority],
-                "key": params.instruction_key or "unverify_collection",
-            }
+                signers=[collection_authority],
+                key=params.instruction_key or "unverify_collection",
+            )
         )
     )
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/update_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/update_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/verify_nft_collection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/verify_nft_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,19 +128,19 @@
             )
         )
 
         return (
             TransactionBuilder.make()
             .set_fee_payer(payer)
             .add(
-                {
-                    "instruction": instruction,
-                    "signers": [payer, collection_authority],
-                    "key": params.instruction_key or "verifyCollection",
-                }
+                InstructionWithSigners(
+                    instruction=instruction,
+                    signers=[payer, collection_authority],
+                    key=params.instruction_key or "verify_collection",
+                )
             )
         )
 
     delegate_record = (
         metaplex.nfts()
         .pdas()
         .metadata_delegate_record(
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/operations/verify_nft_creator.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/operations/verify_nft_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from solders.sysvar import INSTRUCTIONS as SYSVAR_INSTRUCTIONS_PUBKEY
 
 from original_metaplex_python.metaplex.nft_module.nft_pdas_client import (
     MintAddressPdaInput,
 )
 from original_metaplex_python.metaplex.types.signer import Signer, get_public_key
 from original_metaplex_python.metaplex.utils.transaction_builder import (
+    InstructionWithSigners,
     TransactionBuilder,
     TransactionBuilderOptions,
 )
 from original_metaplex_python.token_metadata.generated.instructions import (
     VerifyAccounts,
     VerifyArgs,
     verify,
@@ -46,16 +47,16 @@
     creator = params.creator or metaplex.identity()
 
     # Programs
     token_metadata_program = metaplex.programs().get_token_metadata(programs)
 
     transaction_builder = TransactionBuilder.make().set_fee_payer(payer)
     transaction_builder.add(
-        {
-            "instruction": verify(
+        InstructionWithSigners(
+            instruction=verify(
                 accounts=VerifyAccounts(
                     authority=get_public_key(creator),
                     metadata=metaplex.nfts()
                     .pdas()
                     .metadata(
                         MintAddressPdaInput(mint=mint_address, programs=programs)
                     ),
@@ -66,13 +67,13 @@
                     collection_master_edition=None,
                 ),
                 args=VerifyArgs(
                     verification_args=cast(VerificationArgsKind, CreatorV1())
                 ),
                 program_id=token_metadata_program.address,
             ),
-            "signers": [creator],
-            "key": params.instruction_key or "verify_creator",
-        }
+            signers=[creator],
+            key=params.instruction_key or "verify_creator",
+        )
     )
 
     return transaction_builder
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/nft_module/plugin.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/nft_module/plugin.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/operation_module/operation_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/operation_module/operation_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/program_module/program_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/program_module/program_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/rpc_module/rpc_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/rpc_module/rpc_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/metaplex_file.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/metaplex_file.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/storage_module/storage_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/storage_module/storage_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/operations/create_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/operations/create_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/plugin.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/plugin.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/system_builders_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/system_builders_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/system_module/system_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/system_module/system_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/models/mint.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/models/mint.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/models/token.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/models/token.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/plugin.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/plugin.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/token_module/token_pdas_client.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/token_module/token_pdas_client.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/amount.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/amount.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/cluster.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/cluster.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/operation.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/operation.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/pda.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/pda.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/program.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/program.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/read_api.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/read_api.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/types/signer.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/types/signer.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/common.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/common.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/read_api_connection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/read_api_connection.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/metaplex/utils/transaction_builder.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/metaplex/utils/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/__init__.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/collection_authority_record.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/collection_authority_record.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/edition.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/edition.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/edition_marker.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/edition_marker.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/edition_marker_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/edition_marker_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/master_edition_v1.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/master_edition_v1.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/master_edition_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/master_edition_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/metadata.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/metadata.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/metadata_delegate_record.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/metadata_delegate_record.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v1.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v1.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/reservation_list_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/token_owned_escrow.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/token_owned_escrow.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/token_record.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/token_record.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/accounts/use_authority_record.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/accounts/use_authority_record.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/__init__.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/anchor.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/anchor.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/errors/custom.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/errors/custom.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/__init__.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/approve_collection_authority.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/approve_collection_authority.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,11 +46,17 @@
             AccountMeta(pubkey=RENT, is_signer=False, is_writable=False)
             if RENT
             else AccountMeta(pubkey=program_id, is_signer=False, is_writable=False)
         ),
     ]
     if remaining_accounts is not None:
         keys += remaining_accounts
-    identifier = b"\xfe\x88\xd0'AB\x1bo"
+
+    # DON 4-Apr-2024 - TODO_ORIGINAL The original code uses this byte string as the identifier, however it doesn't work
+    # and raises an error - "Transaction simulation failed: Error processing Instruction 0: invalid instruction data"
+    #
+    # We use the below descriminator of 23 instead which is taken from the javascript SDK.
+    # identifier = b"\xfe\x88\xd0'AB\x1bo"
+    identifier = bytes([23])
     encoded_args = b""
     data = identifier + encoded_args
     return Instruction(program_id, data, keys)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/approve_use_authority.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/approve_use_authority.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/bubblegum_set_collection_size.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/bubblegum_set_collection_size.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/burn.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/burn.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/burn_edition_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/burn_edition_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/burn_nft.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/burn_nft.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/close_escrow_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/close_escrow_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/collect.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/collect.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/convert_master_edition_v1_to_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/convert_master_edition_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_escrow_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_escrow_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_master_edition.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_master_edition.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_master_edition_v3.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_master_edition_v3.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v3.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/create_metadata_account_v3.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/delegate.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,17 @@
             )
             if accounts["authorization_rules"]
             else AccountMeta(pubkey=program_id, is_signer=False, is_writable=False)
         ),
     ]
     if remaining_accounts is not None:
         keys += remaining_accounts
-    identifier = b"Z\x93K\xb2UX\x04\x89"
+    # TODO_ORIGINAL
+    # identifier = b"Z\x93K\xb2UX\x04\x89"
+    identifier = bytes([44])
     encoded_args = layout.build(
         {
             "delegate_args": args["delegate_args"].to_encodable(),
         }
     )
     data = identifier + encoded_args
     return Instruction(program_id, data, keys)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_master_edition.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_master_edition.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_reservation_list.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_create_reservation_list.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_new_edition_from_master_edition_via_printing_token.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_new_edition_from_master_edition_via_printing_token.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens_via_token.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_mint_printing_tokens_via_token.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/deprecated_set_reservation_list.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/deprecated_set_reservation_list.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/freeze_delegated_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/freeze_delegated_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/lock.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/lock.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/migrate.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/migrate.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/mint.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/mint.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_token.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_token.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_vault_proxy.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/mint_new_edition_from_master_edition_via_vault_proxy.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/print.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/print.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/puff_metadata.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/puff_metadata.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/remove_creator_verification.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/remove_creator_verification.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/revoke.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/revoke.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/revoke_collection_authority.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unverify_collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,52 @@
 
 from solders.instruction import AccountMeta, Instruction
 from solders.pubkey import Pubkey
 
 from ..program_id import PROGRAM_ID
 
 
-class RevokeCollectionAuthorityAccounts(typing.TypedDict):
-    collection_authority_record: Pubkey
-    delegate_authority: Pubkey
-    revoke_authority: Pubkey
+class UnverifyCollectionAccounts(typing.TypedDict):
     metadata: Pubkey
-    mint: Pubkey
+    collection_authority: Pubkey
+    collection_mint: Pubkey
+    collection: Pubkey
+    collection_master_edition_account: Pubkey
+    collection_authority_record: typing.Optional[Pubkey]
 
 
-def revoke_collection_authority(
-    accounts: RevokeCollectionAuthorityAccounts,
+def unverify_collection(
+    accounts: UnverifyCollectionAccounts,
     program_id: Pubkey = PROGRAM_ID,
     remaining_accounts: typing.Optional[typing.List[AccountMeta]] = None,
 ) -> Instruction:
     keys: list[AccountMeta] = [
+        AccountMeta(pubkey=accounts["metadata"], is_signer=False, is_writable=True),
         AccountMeta(
-            pubkey=accounts["collection_authority_record"],
-            is_signer=False,
-            is_writable=True,
+            pubkey=accounts["collection_authority"], is_signer=True, is_writable=True
         ),
         AccountMeta(
-            pubkey=accounts["delegate_authority"], is_signer=False, is_writable=True
+            pubkey=accounts["collection_mint"], is_signer=False, is_writable=False
         ),
+        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=False),
         AccountMeta(
-            pubkey=accounts["revoke_authority"], is_signer=True, is_writable=True
+            pubkey=accounts["collection_master_edition_account"],
+            is_signer=False,
+            is_writable=False,
+        ),
+        (
+            AccountMeta(
+                pubkey=accounts["collection_authority_record"],
+                is_signer=False,
+                is_writable=False,
+            )
+            if accounts["collection_authority_record"]
+            else AccountMeta(pubkey=program_id, is_signer=False, is_writable=False)
         ),
-        AccountMeta(pubkey=accounts["metadata"], is_signer=False, is_writable=False),
-        AccountMeta(pubkey=accounts["mint"], is_signer=False, is_writable=False),
     ]
     if remaining_accounts is not None:
         keys += remaining_accounts
-    identifier = b"\x1f\x8b\x87\xc6\x1d0\xa0\x9a"
+    # identifier = b"\xfa\xfb*j)\x89\xba\xa8"
+    identifier = bytes([22])
     encoded_args = b""
     data = identifier + encoded_args
     return Instruction(program_id, data, keys)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/revoke_use_authority.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/revoke_use_authority.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_collection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_collection.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_sized_collection_item.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_and_verify_sized_collection_item.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_collection_size.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_collection_size.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/set_token_standard.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/set_token_standard.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/sign_metadata.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/sign_metadata.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/thaw_delegated_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/thaw_delegated_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/transfer.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/transfer.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/transfer_out_of_escrow.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/transfer_out_of_escrow.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unlock.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unlock.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unverify.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unverify.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unverify_collection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/unverify_sized_collection_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 
 from solders.instruction import AccountMeta, Instruction
 from solders.pubkey import Pubkey
 
 from ..program_id import PROGRAM_ID
 
 
-class UnverifyCollectionAccounts(typing.TypedDict):
+class UnverifySizedCollectionItemAccounts(typing.TypedDict):
     metadata: Pubkey
     collection_authority: Pubkey
+    payer: Pubkey
     collection_mint: Pubkey
     collection: Pubkey
     collection_master_edition_account: Pubkey
     collection_authority_record: typing.Optional[Pubkey]
 
 
-def unverify_collection(
-    accounts: UnverifyCollectionAccounts,
+def unverify_sized_collection_item(
+    accounts: UnverifySizedCollectionItemAccounts,
     program_id: Pubkey = PROGRAM_ID,
     remaining_accounts: typing.Optional[typing.List[AccountMeta]] = None,
 ) -> Instruction:
     keys: list[AccountMeta] = [
         AccountMeta(pubkey=accounts["metadata"], is_signer=False, is_writable=True),
         AccountMeta(
-            pubkey=accounts["collection_authority"], is_signer=True, is_writable=True
+            pubkey=accounts["collection_authority"], is_signer=True, is_writable=False
         ),
+        AccountMeta(pubkey=accounts["payer"], is_signer=True, is_writable=True),
         AccountMeta(
             pubkey=accounts["collection_mint"], is_signer=False, is_writable=False
         ),
-        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=False),
+        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=True),
         AccountMeta(
             pubkey=accounts["collection_master_edition_account"],
             is_signer=False,
             is_writable=False,
         ),
         (
             AccountMeta(
@@ -44,12 +46,13 @@
             )
             if accounts["collection_authority_record"]
             else AccountMeta(pubkey=program_id, is_signer=False, is_writable=False)
         ),
     ]
     if remaining_accounts is not None:
         keys += remaining_accounts
-    # identifier = b"\xfa\xfb*j)\x89\xba\xa8"
-    identifier = bytes([22])
+    # identifier = b"\xa1\xbb\xc2\x9c\x9e\x9a\x90\xdd"
+    identifier = bytes([31])
+
     encoded_args = b""
     data = identifier + encoded_args
     return Instruction(program_id, data, keys)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/unverify_sized_collection_item.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/verify_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 
 from solders.instruction import AccountMeta, Instruction
 from solders.pubkey import Pubkey
 
 from ..program_id import PROGRAM_ID
 
 
-class UnverifySizedCollectionItemAccounts(typing.TypedDict):
+class VerifyCollectionAccounts(typing.TypedDict):
     metadata: Pubkey
     collection_authority: Pubkey
     payer: Pubkey
     collection_mint: Pubkey
     collection: Pubkey
     collection_master_edition_account: Pubkey
     collection_authority_record: typing.Optional[Pubkey]
 
 
-def unverify_sized_collection_item(
-    accounts: UnverifySizedCollectionItemAccounts,
+def verify_collection(
+    accounts: VerifyCollectionAccounts,
     program_id: Pubkey = PROGRAM_ID,
     remaining_accounts: typing.Optional[typing.List[AccountMeta]] = None,
 ) -> Instruction:
     keys: list[AccountMeta] = [
         AccountMeta(pubkey=accounts["metadata"], is_signer=False, is_writable=True),
         AccountMeta(
-            pubkey=accounts["collection_authority"], is_signer=True, is_writable=False
+            pubkey=accounts["collection_authority"], is_signer=True, is_writable=True
         ),
         AccountMeta(pubkey=accounts["payer"], is_signer=True, is_writable=True),
         AccountMeta(
             pubkey=accounts["collection_mint"], is_signer=False, is_writable=False
         ),
-        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=True),
+        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=False),
         AccountMeta(
             pubkey=accounts["collection_master_edition_account"],
             is_signer=False,
             is_writable=False,
         ),
         (
             AccountMeta(
@@ -46,13 +46,17 @@
             )
             if accounts["collection_authority_record"]
             else AccountMeta(pubkey=program_id, is_signer=False, is_writable=False)
         ),
     ]
     if remaining_accounts is not None:
         keys += remaining_accounts
-    # identifier = b"\xa1\xbb\xc2\x9c\x9e\x9a\x90\xdd"
-    identifier = bytes([31])
+
+    # DON 29-Jan-2024 - TODO_ORIGINAL The original code uses this byte string as the identifier, however it doesn't work
+    # We use the below descriminator of 42 instead which is taken from the javascript SDK.
+
+    # identifier = b"8qe\xfdO7z\xa9"
+    identifier = bytes([18])
 
     encoded_args = b""
     data = identifier + encoded_args
     return Instruction(program_id, data, keys)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update_metadata_account_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/update_primary_sale_happened_via_token.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/update_primary_sale_happened_via_token.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/use.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/use.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/utilize.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/utilize.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/verify.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/verify.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/instructions/verify_collection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/instructions/verify_sized_collection_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 
 from solders.instruction import AccountMeta, Instruction
 from solders.pubkey import Pubkey
 
 from ..program_id import PROGRAM_ID
 
 
-class VerifyCollectionAccounts(typing.TypedDict):
+class VerifySizedCollectionItemAccounts(typing.TypedDict):
     metadata: Pubkey
     collection_authority: Pubkey
     payer: Pubkey
     collection_mint: Pubkey
     collection: Pubkey
     collection_master_edition_account: Pubkey
     collection_authority_record: typing.Optional[Pubkey]
 
 
-def verify_collection(
-    accounts: VerifyCollectionAccounts,
+def verify_sized_collection_item(
+    accounts: VerifySizedCollectionItemAccounts,
     program_id: Pubkey = PROGRAM_ID,
     remaining_accounts: typing.Optional[typing.List[AccountMeta]] = None,
 ) -> Instruction:
     keys: list[AccountMeta] = [
         AccountMeta(pubkey=accounts["metadata"], is_signer=False, is_writable=True),
         AccountMeta(
-            pubkey=accounts["collection_authority"], is_signer=True, is_writable=True
+            pubkey=accounts["collection_authority"], is_signer=True, is_writable=False
         ),
         AccountMeta(pubkey=accounts["payer"], is_signer=True, is_writable=True),
         AccountMeta(
             pubkey=accounts["collection_mint"], is_signer=False, is_writable=False
         ),
-        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=False),
+        AccountMeta(pubkey=accounts["collection"], is_signer=False, is_writable=True),
         AccountMeta(
             pubkey=accounts["collection_master_edition_account"],
             is_signer=False,
             is_writable=False,
         ),
         (
             AccountMeta(
@@ -49,14 +49,14 @@
         ),
     ]
     if remaining_accounts is not None:
         keys += remaining_accounts
 
     # DON 29-Jan-2024 - TODO_ORIGINAL The original code uses this byte string as the identifier, however it doesn't work
     # We use the below descriminator of 42 instead which is taken from the javascript SDK.
+    # identifier = b"Vo\xdfD\x11c\xb4\x93"
 
-    # identifier = b"8qe\xfdO7z\xa9"
-    identifier = bytes([18])
+    identifier = bytes([30])
 
     encoded_args = b""
     data = identifier + encoded_args
     return Instruction(program_id, data, keys)
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/__init__.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/__init__.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/approve_use_authority_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/approve_use_authority_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/asset_data.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/asset_data.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/authority_type.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/authority_type.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/authorization_data.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/authorization_data.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/burn_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/burn_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection_details.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection_details.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection_details_toggle.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection_details_toggle.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/collection_toggle.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/collection_toggle.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/create_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/create_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/create_master_edition_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/create_master_edition_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/create_metadata_account_args_v3.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/create_metadata_account_args_v3.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/creator.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/creator.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/data.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/data.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/data_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/data_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/delegate_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/delegate_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/escrow_authority.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/escrow_authority.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/key.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/key.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/lock_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/lock_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/metadata_delegate_role.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/metadata_delegate_role.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/migration_type.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/migration_type.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/mint_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/mint_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/mint_new_edition_from_master_edition_via_token_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/mint_new_edition_from_master_edition_via_token_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/payload.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/payload.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/payload_key.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/payload_key.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/payload_type.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/payload_type.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/print_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/print_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/print_supply.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/print_supply.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/programmable_config.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/programmable_config.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/proof_info.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/proof_info.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/reservation.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/reservation.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/reservation_v1.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/reservation_v1.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/revoke_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/revoke_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/rule_set_toggle.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/rule_set_toggle.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/seeds_vec.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/seeds_vec.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/set_collection_size_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/set_collection_size_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/token_delegate_role.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/token_delegate_role.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/token_standard.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/token_standard.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/token_state.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/token_state.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/transfer_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/transfer_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/transfer_out_of_escrow_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/transfer_out_of_escrow_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/unlock_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/unlock_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/update_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/update_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/update_metadata_account_args_v2.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/update_metadata_account_args_v2.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/use_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/use_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/use_method.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/use_method.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/uses.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/uses.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/uses_toggle.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/uses_toggle.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/utilize_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/utilize_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python/token_metadata/generated/types/verification_args.py` & `original_metaplex_python-0.0.1a2/original_metaplex_python/token_metadata/generated/types/verification_args.py`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/PKG-INFO` & `original_metaplex_python-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: original-metaplex-python
-Version: 0.0.1a1
+Name: original_metaplex_python
+Version: 0.0.1a2
 Summary: Python port of Metaplex JS SDK - https://github.com/metaplex-foundation/js
 Home-page: https://github.com/getoriginal/original-metaplex-python
 Author: Original
 Author-email: support@getoriginal.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/SOURCES.txt` & `original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,35 @@
 original_metaplex_python/metaplex/keypair_identity/__init__.py
 original_metaplex_python/metaplex/keypair_identity/keypair_identity_driver.py
 original_metaplex_python/metaplex/keypair_identity/plugin.py
 original_metaplex_python/metaplex/nft_module/__init__.py
 original_metaplex_python/metaplex/nft_module/authorization.py
 original_metaplex_python/metaplex/nft_module/delegate_input.py
 original_metaplex_python/metaplex/nft_module/delegate_type.py
+original_metaplex_python/metaplex/nft_module/errors.py
 original_metaplex_python/metaplex/nft_module/nft_builders_client.py
 original_metaplex_python/metaplex/nft_module/nft_client.py
 original_metaplex_python/metaplex/nft_module/nft_pdas_client.py
 original_metaplex_python/metaplex/nft_module/plugin.py
 original_metaplex_python/metaplex/nft_module/models/__init__.py
 original_metaplex_python/metaplex/nft_module/models/json_metadata.py
 original_metaplex_python/metaplex/nft_module/models/metadata.py
 original_metaplex_python/metaplex/nft_module/models/nft.py
 original_metaplex_python/metaplex/nft_module/models/nft_edition.py
 original_metaplex_python/metaplex/nft_module/models/sft.py
 original_metaplex_python/metaplex/nft_module/operations/__init__.py
+original_metaplex_python/metaplex/nft_module/operations/approve_nft_collection_authority.py
+original_metaplex_python/metaplex/nft_module/operations/approve_nft_delegate.py
 original_metaplex_python/metaplex/nft_module/operations/create_nft.py
 original_metaplex_python/metaplex/nft_module/operations/create_sft.py
 original_metaplex_python/metaplex/nft_module/operations/delete_nft.py
 original_metaplex_python/metaplex/nft_module/operations/find_nft_by_mint.py
 original_metaplex_python/metaplex/nft_module/operations/mint_nft.py
+original_metaplex_python/metaplex/nft_module/operations/revoke_nft_collection_authority.py
+original_metaplex_python/metaplex/nft_module/operations/revoke_nft_delegate.py
 original_metaplex_python/metaplex/nft_module/operations/transfer_nft.py
 original_metaplex_python/metaplex/nft_module/operations/unverify_nft_collection.py
 original_metaplex_python/metaplex/nft_module/operations/update_nft.py
 original_metaplex_python/metaplex/nft_module/operations/verify_nft_collection.py
 original_metaplex_python/metaplex/nft_module/operations/verify_nft_creator.py
 original_metaplex_python/metaplex/operation_module/__init__.py
 original_metaplex_python/metaplex/operation_module/operation_client.py
```

### Comparing `original_metaplex_python-0.0.1a1/original_metaplex_python.egg-info/requires.txt` & `original_metaplex_python-0.0.1a2/original_metaplex_python.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/pyproject.toml` & `original_metaplex_python-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `original_metaplex_python-0.0.1a1/setup.py` & `original_metaplex_python-0.0.1a2/setup.py`

 * *Files identical despite different names*

