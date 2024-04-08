# Comparing `tmp/climate_finance-1.0.1.tar.gz` & `tmp/climate_finance-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_finance-1.0.1.tar", max compression
+gzip compressed data, was "climate_finance-1.1.0.tar", max compression
```

## Comparing `climate_finance-1.0.1.tar` & `climate_finance-1.1.0.tar`

### file list

```diff
@@ -1,76 +1,79 @@
--rw-r--r--   0        0        0     1069 2024-04-04 09:35:24.926246 climate_finance-1.0.1/LICENSE
--rw-r--r--   0        0        0     3001 2024-04-04 09:35:24.926246 climate_finance-1.0.1/README.md
--rw-r--r--   0        0        0       11 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/.raw_data/README.md
--rw-r--r--   0        0        0       26 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/.raw_data/data_updates.json
--rw-r--r--   0        0        0       66 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/.raw_data/imputed_missing.csv
--rw-r--r--   0        0        0    16080 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/README.md
--rw-r--r--   0        0        0      499 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/__init__.py
--rw-r--r--   0        0        0     7222 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/analysis_tools.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/cleaning_tools.py
--rw-r--r--   0        0        0     9505 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/common/schema.py
--rw-r--r--   0        0        0     1120 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/config.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/__init__.py
--rw-r--r--   0        0        0    25777 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/data.py
--rw-r--r--   0        0        0     3817 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/deflators.py
--rw-r--r--   0        0        0     4466 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/dtypes.py
--rw-r--r--   0        0        0     3081 2024-04-04 09:35:24.926246 climate_finance-1.0.1/climate_finance/core/enums.py
--rw-r--r--   0        0        0     3366 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/core/loaders.py
--rw-r--r--   0        0        0    12444 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/core/tools.py
--rw-r--r--   0        0        0     2582 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/core/validation.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/bilateral/__init__.py
--rw-r--r--   0        0        0    10180 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/bilateral/bilateral_methodologies.py
--rw-r--r--   0        0        0     4589 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/bilateral/tools.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/__init__.py
--rw-r--r--   0        0        0    19795 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/crs_tools.py
--rw-r--r--   0        0        0    10482 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/multilateral_spending_data.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/__init__.py
--rw-r--r--   0        0        0     6969 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py
--rw-r--r--   0        0        0     2620 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/__init__.py
--rw-r--r--   0        0        0     5781 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py
--rw-r--r--   0        0        0     1037 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/imputations.py
--rw-r--r--   0        0        0      308 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/shares.py
--rw-r--r--   0        0        0     9869 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/multilateral/tools.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/__init__.py
--rw-r--r--   0        0        0     8157 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/crdf.py
--rw-r--r--   0        0        0    13352 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/crdf_crs.py
--rw-r--r--   0        0        0     5679 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/crs.py
--rw-r--r--   0        0        0     6329 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/methodologies/spending/tools.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/__init__.py
--rw-r--r--   0        0        0    19065 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv
--rw-r--r--   0        0        0     7484 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/names.py
--rw-r--r--   0        0        0    23354 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_agency_names.feather
--rw-r--r--   0        0        0     5570 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_names.feather
--rw-r--r--   0        0        0     5370 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/recipient_names.feather
--rw-r--r--   0        0        0     1436 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/settings.py
--rw-r--r--   0        0        0    14959 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/tools.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/__init__.py
--rw-r--r--   0        0        0     4144 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/provider_perspective.py
--rw-r--r--   0        0        0     4144 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/recipient_perspective.py
--rw-r--r--   0        0        0     3579 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crdf/tools.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crs/__init__.py
--rw-r--r--   0        0        0    13296 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crs/add_crs_data.py
--rw-r--r--   0        0        0     9598 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/crs/get_data.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.930246 climate_finance-1.0.1/climate_finance/oecd/multisystem/__init__.py
--rw-r--r--   0        0        0     4492 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/oecd/multisystem/crs_channel_mapping.csv
--rw-r--r--   0        0        0     2709 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/oecd/multisystem/get_data.py
--rw-r--r--   0        0        0    22597 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/README.md
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/__init__.py
--rw-r--r--   0        0        0     7981 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/tools.py
--rw-r--r--   0        0        0     3705 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json
--rw-r--r--   0        0        0     3439 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/validation.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/__init__.py
--rw-r--r--   0        0        0    17282 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/download_data.py
--rw-r--r--   0        0        0     9534 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/get_data.py
--rw-r--r--   0        0        0     3413 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/download/pre_process.py
--rw-r--r--   0        0        0     6309 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/get_unfccc_data.py
--rw-r--r--   0        0        0        0 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/__init__.py
--rw-r--r--   0        0        0     2966 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/get_data.py
--rw-r--r--   0        0        0    11767 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/pre_process.py
--rw-r--r--   0        0        0     1165 2024-04-04 09:35:24.934246 climate_finance-1.0.1/climate_finance/unfccc/manual/read_files.py
--rw-r--r--   0        0        0      660 2024-04-04 09:35:24.934246 climate_finance-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 climate_finance-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-08 11:54:43.351917 climate_finance-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3001 2024-04-08 11:54:43.351917 climate_finance-1.1.0/README.md
+-rw-r--r--   0        0        0       11 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/.raw_data/README.md
+-rw-r--r--   0        0        0       26 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/.raw_data/data_updates.json
+-rw-r--r--   0        0        0       66 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/.raw_data/imputed_missing.csv
+-rw-r--r--   0        0        0    17698 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/README.md
+-rw-r--r--   0        0        0      499 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/common/__init__.py
+-rw-r--r--   0        0        0     7222 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/common/analysis_tools.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/common/cleaning_tools.py
+-rw-r--r--   0        0        0     9505 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/common/schema.py
+-rw-r--r--   0        0        0     1120 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/config.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/core/__init__.py
+-rw-r--r--   0        0        0    26092 2024-04-08 11:54:43.351917 climate_finance-1.1.0/climate_finance/core/data.py
+-rw-r--r--   0        0        0     3817 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/deflators.py
+-rw-r--r--   0        0        0     4466 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/dtypes.py
+-rw-r--r--   0        0        0     3081 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/enums.py
+-rw-r--r--   0        0        0     3366 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/loaders.py
+-rw-r--r--   0        0        0    13459 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/oecd_classification.csv
+-rw-r--r--   0        0        0    15208 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/tools.py
+-rw-r--r--   0        0        0     2582 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/core/validation.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/bilateral/__init__.py
+-rw-r--r--   0        0        0    10180 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/bilateral/bilateral_methodologies.py
+-rw-r--r--   0        0        0     4589 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/bilateral/tools.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/__init__.py
+-rw-r--r--   0        0        0    19795 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/crs_tools.py
+-rw-r--r--   0        0        0    10482 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/multilateral_spending_data.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/oecd_multilateral/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py
+-rw-r--r--   0        0        0     2620 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/__init__.py
+-rw-r--r--   0        0        0     5781 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/imputations/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/imputations/spending.py
+-rw-r--r--   0        0        0     1037 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/imputations.py
+-rw-r--r--   0        0        0      308 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/shares.py
+-rw-r--r--   0        0        0     9869 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/multilateral/tools.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/spending/__init__.py
+-rw-r--r--   0        0        0     8157 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/spending/crdf.py
+-rw-r--r--   0        0        0    13352 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/spending/crdf_crs.py
+-rw-r--r--   0        0        0     5679 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/spending/crs.py
+-rw-r--r--   0        0        0     6329 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/methodologies/spending/tools.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0    19065 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     7484 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/names.py
+-rw-r--r--   0        0        0    23354 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/provider_agency_names.feather
+-rw-r--r--   0        0        0     5570 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/provider_names.feather
+-rw-r--r--   0        0        0     5370 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/recipient_names.feather
+-rw-r--r--   0        0        0     1436 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/settings.py
+-rw-r--r--   0        0        0    14959 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/tools.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/crdf/__init__.py
+-rw-r--r--   0        0        0     4144 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/crdf/provider_perspective.py
+-rw-r--r--   0        0        0     4144 2024-04-08 11:54:43.355917 climate_finance-1.1.0/climate_finance/oecd/crdf/recipient_perspective.py
+-rw-r--r--   0        0        0     3579 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/crdf/tools.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/crs/__init__.py
+-rw-r--r--   0        0        0    13296 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/crs/add_crs_data.py
+-rw-r--r--   0        0        0     9598 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/crs/get_data.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/multisystem/__init__.py
+-rw-r--r--   0        0        0     4492 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/multisystem/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     2709 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/oecd/multisystem/get_data.py
+-rw-r--r--   0        0        0    22597 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0     7981 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/tools.py
+-rw-r--r--   0        0        0     3705 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json
+-rw-r--r--   0        0        0     3439 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/validation.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/download/__init__.py
+-rw-r--r--   0        0        0    17282 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/download/download_data.py
+-rw-r--r--   0        0        0     9534 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/download/get_data.py
+-rw-r--r--   0        0        0     3413 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/download/pre_process.py
+-rw-r--r--   0        0        0     6309 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/get_unfccc_data.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/manual/__init__.py
+-rw-r--r--   0        0        0     2966 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/manual/get_data.py
+-rw-r--r--   0        0        0    11767 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/manual/pre_process.py
+-rw-r--r--   0        0        0     1165 2024-04-08 11:54:43.359917 climate_finance-1.1.0/climate_finance/unfccc/manual/read_files.py
+-rw-r--r--   0        0        0      660 2024-04-08 11:54:43.359917 climate_finance-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 climate_finance-1.1.0/PKG-INFO
```

### Comparing `climate_finance-1.0.1/LICENSE` & `climate_finance-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/README.md` & `climate_finance-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/README.md` & `climate_finance-1.1.0/climate_finance/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 
 #### Creating an instance of `ClimateData`
 
 The first step when using the `ClimateData` class is to create an instance of it.
 You can define a number of parameters when creating the instance:
 
 - _years_: a list of years (or a range) to get data for.
-- _providers_: a list of provider codes (or a single one) for whom to get data.
-  For now, only 'OECD' codes are supported. If `None` are provided, all available providers
-  are included.
+- _providers_: a list of provider codes, names, or ISO3 codes (or a single one) for whom to get data.
+  If `None` are provided, all available providers are included. To get a list of available
+    providers, you can call `ClimateData.available_providers()`.
 - _recipients_: a list of recipient codes (or a single one) for whom to get data.
   For now, only 'OECD' codes are supported. If `None` are provided, all available recipients
   are included.
 - _currency_: the currency used for the data. The default is 'USD'. Available options
   include 'USD', 'EUR', 'GBP','CAD'. Others can be added by request.
 - _prices_: the price type to use. The default is 'current'. The data can also be
   converted to constant prices. In that case DAC deflators are used by default, though
@@ -261,65 +261,14 @@
 df = climate_data.get_data()
 ```
 
 In this example, the data will be returned for providers 4 and 12, for all recipients,
 for the years 2018, 2019, 2020 and 2021, in constant 2022 Euros.
 
 
-#### Other functionality
-
-##### Specifying a custom methodology
-The `ClimateData` class also allows the user to specify a custom methodology.
-
-This can be done using the `set_custom_spending_methodology` method. 
-
-This method takes a
-tuple of two coefficients (as integers or floats) as the 'coefficient' parameter. They
-are for (significant, principal) activities. For reference, the OECD uses (1, 1) and 
-ONE uses (0.4, 1).
-
-This method also takes a `highest_marker` parameter, which is a boolean set to `True` if
-the highest marker rule should be applied, and `False` otherwise.
-
-```python
-
-from climate_finance import ClimateData, set_climate_finance_data_path
-
-# As always, start by setting the data path
-set_climate_finance_data_path('path/to/your/data')
-
-# Create an instance of the ClimateData class
-# In this example, it will be set for the years 2018, 2019, 2020 and 2022, for 
-# all providers in current USD
-climate_data = ClimateData(
-  years=range(2018, 2022),
-  providers=[4, 12]
-)
-
-# Set a custom methodology. 
-# In this example, principal activities are counted at 30% of their value, significant
-# at 80%, and the highest marker rule is applied.
-climate_data.set_custom_spending_methodology(
-  coefficients=(0.3, 0.8),
-  highest_marker=True
-)
-
-# Load disbursements spending data using the custom methodology and
-# focusing on CRS allocable data
-climate_data.load_spending_data(
-  methodology='custom',
-  source='OECD_CRS_ALLOCABLE',
-  flows='commitments'
-)
-
-# Get the data as a DataFrame
-df = climate_data.get_data()
-
-```
-
 ## Multilateral imputations
 
 A significant portion of climate finance is provided through the multilateral system.
 The sums provided by multilateral institutions can be accessed through the approach
 outlined above, using data released by the OECD through the CRDF.
 
 Bilateral providers support the core operating budgets of multilateral institutions.
@@ -330,29 +279,29 @@
 Through the "Provider Perspective" of the CRDF, providers report imputed climate finance
 that is provided through the multilateral system. The quality and coverage of this data
 is imperfect, as we note in our methodology note.
 
 The OECD also releases data on the "shares" of multilateral spending that is considered
 climate finance. These shares can be used, together with data on multilateral contributions
 from bilateral providers, to impute the climate finance that is provided through the
-multilateral system. This data is reported at a very aggregate level, it is based on 
+multilateral system. This data is reported at a very aggregate level, it is based on
 commitments, and is presented as 2-year averages.
 
 The `ClimateData` class provides tools to calculate spending shares following
 whichever methodology the user prefers. It also provides tools to calculate imputations
 based on these shares.
 
 The easiest way to get imputed amounts for bilateral providers is through the
 `load_multilateral_imputations_data` method
 
 ### Using the `load_multilateral_imputations_data` method
 
 To load the multilateral imputations data a few parameters should
 be defined:
-- _spending_methodology_: a string defining the 'spending' methodology to use. This is applied 
+- _spending_methodology_: a string defining the 'spending' methodology to use. This is applied
   to the spending data of multilateral agencies. The default is 'ONE' but 'OECD'
   and 'custom' are also available. The 'custom' methodology allows you to define a specific
   methodology to discount 'principal' and 'significant' climate activities. You can call
   `.available_methodologies` for a full list of available methodologies.
 - _rolling_years_spending_: if needed, the spending data can be smoothed over a certain
   number of years. The default, 1, means no smoothing.
 - _flows_': one, or a list of supported flows: gross_disbursements, commitments,
@@ -368,66 +317,159 @@
   calculated for a year/provider/agency/flow_type level.
 
 
 As in the case of spending data, the combination of spending methodology and source are key
 in determining the data that is returned.
 
 A few things happen when you load the multilateral imputations data:
-- Spending data is loaded for multilateral agencies. This data is transformed into 
+- Spending data is loaded for multilateral agencies. This data is transformed into
   climate finance shares using the methodology specified (including smoothing if requested.)
 - Core contributions from bilateral providers to multilateral agencies are loaded and matched
   to the multilateral spending shares data.
 - The imputed climate finance is calculated by multiplying the shares by the core contributions.
 
 This all happens based on the parameters you provide. For example:
 
 ```python
 from climate_finance import ClimateData, set_climate_finance_data_path
 
 # As always, start by setting the data path
 set_climate_finance_data_path('path/to/your/data')
 
 # Create an instance of the ClimateData class
-# In this example, it will be set for the years 2018, 2019, 2020 and 2021, for
+# In this example, it will be set for the years 2018, 2019, 2020, 2021 and 2022, for
 # providers 4 and 12 (France and the UK), for all recipients, in constant 2022 Euros.
 climate_data = ClimateData(
-        years=range(2018, 2022),                  
+        years=range(2018, 2023),                  
         providers=[4, 12],
         recipients=None, # which means getting all available
         currency='EUR',
         prices='constant',
         base_year=2022
     )
 
 # Load the multilateral imputations data using the 'ONE' methodology
 climate_data.load_multilateral_imputations_data(
-  spending_methodology="ONE",
+  spending_methodology="OECD",
   source="OECD_CRDF_CRS_ALLOCABLE",
   rolling_years_spending=2,
   flows=["gross_disbursements"],
-  groupby=[
+  shareby=[
     "year",
     "oecd_provider_code",
     "provider",
-    "indicator",
     "flow_type",
     "currency",
     "prices",
   ],
-  shareby=[
+  groupby=[
     "year",
     "oecd_provider_code",
     "provider",
+    "indicator",
     "flow_type",
     "currency",
     "prices",
   ],
 )
 
 
 # Get the data as a DataFrame
 df = climate_data.get_data()
 
 ```
 
+In this example, multilateral imputations will be returned for providers 4 and 12, for all
+recipients, for the years 2018, 2019, 2020, 2021 and 2022, in constant 2022 Euros.
+
+The multilateral spending shares used to create the imputations are calculated for a 2-year
+rolling average.
+
+The imputed data is grouped by year, provider, indicator, flow type, currency
+and prices.
+
+The `shareby` setting is quite important, as it determines the level of aggregation used
+to calculate the spending shares, and therefore the level of detail at which the imputed
+data is returned.
+
+# Other functionality
+
+## Specifying a custom methodology
+The `ClimateData` class also allows the user to specify a custom methodology.
+
+This can be done using the `set_custom_spending_methodology` method. 
+
+This method takes a
+tuple of two coefficients (as integers or floats) as the 'coefficient' parameter. They
+are for (significant, principal) activities. For reference, the OECD uses (1, 1) and 
+ONE uses (0.4, 1).
+
+This method also takes a `highest_marker` parameter, which is a boolean set to `True` if
+the highest marker rule should be applied, and `False` otherwise.
+
+```python
+
+from climate_finance import ClimateData, set_climate_finance_data_path
+
+# As always, start by setting the data path
+set_climate_finance_data_path('path/to/your/data')
+
+# Create an instance of the ClimateData class
+# In this example, it will be set for the years 2018, 2019, 2020 and 2022, for 
+# all providers in current USD
+climate_data = ClimateData(
+  years=range(2018, 2022),
+  providers=[4, 12]
+)
+
+# Set a custom methodology. 
+# In this example, principal activities are counted at 30% of their value, significant
+# at 80%, and the highest marker rule is applied.
+climate_data.set_custom_spending_methodology(
+  coefficients=(0.3, 0.8),
+  highest_marker=True
+)
+
+# Load disbursements spending data using the custom methodology and
+# focusing on CRS allocable data
+climate_data.load_spending_data(
+  methodology='custom',
+  source='OECD_CRS_ALLOCABLE',
+  flows='commitments'
+)
+
+# Get the data as a DataFrame
+df = climate_data.get_data()
+
+```
+
+## Getting available providers
+
+The `ClimateData` class also provides a method to get a list of available providers.
+
+```python
+from climate_finance import ClimateData
+
+# Get a dictionary of available providers (code: name)
+# By default, private providers are excluded
+providers = ClimateData.available_providers(include_private=False)
+
+```
+
+You can also get lists of groups of providers, such as DAC members, Non-DAC members, Multilateral providers, and Private providers.
+
+```python
+from climate_finance import ClimateData
+
+# Get a list of DAC providers, excluding EU institutions
+dac_members = ClimateData.get_dac_providers(include_eui=False)
+
+# Get a list of Non-DAC providers
+non_dac_members = ClimateData.get_non_dac_providers()
+
+# Get a list of Multilateral providers, including EU institutions
+multilateral_providers = ClimateData.get_multilateral_providers(include_eui=True)
 
+# Get a list of Private providers
+private_providers = ClimateData.get_private_providers()
 
+```
```

### Comparing `climate_finance-1.0.1/climate_finance/common/analysis_tools.py` & `climate_finance-1.1.0/climate_finance/common/analysis_tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/common/schema.py` & `climate_finance-1.1.0/climate_finance/common/schema.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/config.py` & `climate_finance-1.1.0/climate_finance/config.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/core/data.py` & `climate_finance-1.1.0/climate_finance/core/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
-from oda_data import set_data_path, ODAData
+from oda_data import set_data_path
 from oda_data.clean_data.channels import add_multi_channel_codes
 
-from climate_finance.common.schema import ClimateSchema
 from climate_finance.config import logger, ClimateDataPath
 from climate_finance.core import loaders
 from climate_finance.core.deflators import oecd_deflator
 from climate_finance.core.enums import (
     ValidPrices,
     ValidCurrencies,
     SpendingMethodologies,
@@ -23,14 +22,17 @@
     align_oda_data_names,
     validate_multi_shares_groupers,
     validate_multi_groupby,
     merge_spending_and_contributions,
     calculate_imputations,
     remove_channel_name_from_spending_data,
     groupby_sum,
+    get_oecd_classification,
+    get_available_providers,
+    match_providers,
 )
 from climate_finance.core.validation import (
     validate_prices_and_base_year,
     validate_methodology,
     validate_list_of_str,
     validate_source,
 )
@@ -94,14 +96,18 @@
         self.currency: ValidCurrencies | str = ValidCurrencies(currency)
         self.prices: ValidPrices | str = ValidPrices(prices)
         self.base_year = base_year
 
         # Validate the prices and base year
         validate_prices_and_base_year(prices=self.prices, base_year=self.base_year)
 
+        # Validate providers
+        if not all(isinstance(provider, int) for provider in self.providers):
+            self.providers = match_providers(self.providers)
+
         # By default, the data is not loaded
         self.data: dict[str, pd.DataFrame] = {}
 
         # By default, raw data sources are not loaded
         self._data: dict[str, pd.DataFrame] = {}
 
         # Other data attributes
@@ -146,14 +152,56 @@
         ValidPrices.print_available(name="prices")
 
     @staticmethod
     def available_currencies():
         """Print all the valid, available flows"""
         ValidCurrencies.print_available(name="currencies")
 
+    @staticmethod
+    def available_providers(include_private: bool = False):
+        """return a list of available providers"""
+
+        return get_available_providers(include_private=include_private)
+
+    @staticmethod
+    def get_dac_providers(include_eui: bool = False) -> dict:
+        """return a list of DAC providers
+
+        Args:
+            include_eui: Optional. A boolean specifying whether to include the EU institutions.
+            Defaults to False.
+
+        """
+        dac = get_oecd_classification()["DAC member"]
+
+        if not include_eui:
+            dac = {k: v for k, v in dac.items() if k != 918}
+
+        return dac
+
+    @staticmethod
+    def get_non_dac_providers() -> dict:
+        """return a list of non DAC providers"""
+        return get_oecd_classification()["Non-DAC member"]
+
+    @staticmethod
+    def get_multilateral_providers(include_eui: bool = True) -> dict:
+        """return a list of multilateral providers"""
+        multi = get_oecd_classification()["Multilateral donor"]
+
+        if include_eui:
+            return multi | {918: "EU Institutions"}
+
+        return multi
+
+    @staticmethod
+    def get_private_providers() -> dict:
+        """return a list of private providers"""
+        return get_oecd_classification()["Private donor"]
+
     def __repr__(self):
         message: str = f"ClimateData object for {self._years_str}. "
 
         if self.data is None:
             message += "No data has been loaded yet. "
 
         return message
@@ -542,14 +590,16 @@
         data = calculate_imputations(data)
 
         # Group to the desired level
         data = groupby_sum(data=data, groupby=groupby)
 
         self.data = {"Multilateral Imputations": data}
 
+        return self
+
     def convert_to_shares(
         self,
         rolling_years: int = 1,
         groupby: list[str] | str | None = None,
         shareby: list[str] | str | None = None,
     ) -> "ClimateData":
         """
@@ -640,55 +690,7 @@
         else:
             loaded_data = loaded_data.assign(
                 currency=self.currency,
                 prices=self.prices,
             )
 
         return loaded_data
-
-
-if __name__ == "__main__":
-    climate = ClimateData(
-        years=range(2016, 2022),
-        providers=[4, 12],
-        currency="EUR",
-        prices="constant",
-        base_year=2021,
-    )
-    #
-    # climate.load_spending_data(
-    #     methodology="OECD",
-    #     flows=["gross_disbursements"],
-    #     source="OECD_CRS",
-    # )
-    #
-    # climate.convert_to_shares(
-    #     rolling_years=1,
-    #     groupby=["year", "provider", "recipient", "indicator", "flow_type"],
-    #     shareby=["year", "provider", "flow_type"],
-    # )
-
-    climate.load_multilateral_imputations_data(
-        spending_methodology="ONE",
-        source="OECD_CRDF_CRS_ALLOCABLE",
-        rolling_years_spending=2,
-        flows=["gross_disbursements"],
-        groupby=[
-            "year",
-            "oecd_provider_code",
-            "provider",
-            "indicator",
-            "flow_type",
-            "currency",
-            "prices",
-        ],
-        shareby=[
-            "year",
-            "oecd_provider_code",
-            "provider",
-            "flow_type",
-            "currency",
-            "prices",
-        ],
-    )
-
-    climate_df = climate.get_data()
```

### Comparing `climate_finance-1.0.1/climate_finance/core/deflators.py` & `climate_finance-1.1.0/climate_finance/core/deflators.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/core/dtypes.py` & `climate_finance-1.1.0/climate_finance/core/dtypes.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/core/enums.py` & `climate_finance-1.1.0/climate_finance/core/enums.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/core/loaders.py` & `climate_finance-1.1.0/climate_finance/core/loaders.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/core/tools.py` & `climate_finance-1.1.0/climate_finance/core/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import pandas as pd
+from bblocks import convert_id
 from oda_data.clean_data.schema import OdaSchema
+from thefuzz import process
 
 from climate_finance.common.schema import ClimateSchema, CRS_MAPPING
+from climate_finance.config import ClimateDataPath, logger
 from climate_finance.oecd.cleaning_tools.tools import (
     convert_flows_millions_to_units,
     clean_multisystem_indicators,
     channel_codes_to_names,
 )
 
 
@@ -429,7 +432,94 @@
     """
 
     # Convert all non-numeric columns
     for col in data.select_dtypes(exclude=[float, int, bool]):
         data[col] = data[col].astype(str).replace(missing, pd.NA, regex=True)
 
     return data
+
+
+def get_oecd_classification() -> dict:
+    """Read the OECD CRS classification and return it as a dictionary."""
+
+    df = pd.read_csv(ClimateDataPath.scripts / "core" / "oecd_classification.csv")
+
+    types = {}
+
+    for dt in df["type"].unique():
+        types[dt] = df.loc[df["type"] == dt].set_index("code")["name"].to_dict()
+
+    return types
+
+
+def get_available_providers(include_private: bool = False) -> dict:
+    """return a list of available providers"""
+
+    providers = get_oecd_classification()
+
+    available = (
+        providers["DAC member"]
+        | providers["Non-DAC member"]
+        | providers["Multilateral donor"]
+    )
+
+    if include_private:
+        available |= providers["Private donor"]
+
+    return available
+
+
+def fuzzy_match_provider(providers: list[str], options: dict) -> list:
+    results = []
+    providers_list = list(options)
+
+    for user_input in providers:
+        # Finding the best match for the user_input in the list of countries
+        best_match = process.extractOne(user_input, providers_list)
+        # best_match is a tuple like ('Country Name', score)
+        if best_match:
+            if best_match[1] < 89:
+                logger.info(f"No match found for {user_input}")
+                continue
+            # Find the key in the dictionary corresponding to the matched country
+            match_key = options[best_match[0]]
+            results.append(match_key)
+
+    return results
+
+
+def match_providers(providers: str | list[str]) -> list[int]:
+    """"""
+    # Silence the country_converter logger
+    import logging
+
+    cc_loger = logging.getLogger("country_converter")
+    cc_loger.setLevel(logging.CRITICAL)
+
+    # Ensure user_inputs is always a list to simplify processing
+    if not isinstance(providers, list):
+        providers = [providers]
+
+    # Get the available providers
+    options = {v: k for k, v in get_available_providers(include_private=True).items()}
+
+    # Attempt to match the providers to the DAC codes
+    match = convert_id(
+        series=pd.Series(providers, index=providers),
+        from_type="ISO3" if all(len(item) == 3 for item in providers) else "regex",
+        to_type="DACcode",
+        not_found=pd.NA,
+    ).astype("int32[pyarrow]")
+
+    # if missing, try fuzzy matching
+    if match.isna().any():
+        # Get the missing providers
+        missing = match[match.isna()].index.tolist()
+        # Fuzzy match the missing providers
+        results = fuzzy_match_provider(providers=missing, options=options)
+    else:
+        results = []
+
+    # Combine the matches
+    all_matches = match[match.notna()].tolist() + results
+
+    return all_matches
```

### Comparing `climate_finance-1.0.1/climate_finance/core/validation.py` & `climate_finance-1.1.0/climate_finance/core/validation.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/bilateral/bilateral_methodologies.py` & `climate_finance-1.1.0/climate_finance/methodologies/bilateral/bilateral_methodologies.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/bilateral/tools.py` & `climate_finance-1.1.0/climate_finance/methodologies/bilateral/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/crs_tools.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/crs_tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/multilateral_spending_data.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/multilateral_spending_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/one_multilateral/imputations.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/one_multilateral/imputations.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/multilateral/tools.py` & `climate_finance-1.1.0/climate_finance/methodologies/multilateral/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/spending/crdf.py` & `climate_finance-1.1.0/climate_finance/methodologies/spending/crdf.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/spending/crdf_crs.py` & `climate_finance-1.1.0/climate_finance/methodologies/spending/crdf_crs.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/spending/crs.py` & `climate_finance-1.1.0/climate_finance/methodologies/spending/crs.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/methodologies/spending/tools.py` & `climate_finance-1.1.0/climate_finance/methodologies/spending/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/names.py` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/names.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_agency_names.feather` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/provider_agency_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/provider_names.feather` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/provider_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/recipient_names.feather` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/recipient_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/settings.py` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/settings.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/cleaning_tools/tools.py` & `climate_finance-1.1.0/climate_finance/oecd/cleaning_tools/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/crdf/provider_perspective.py` & `climate_finance-1.1.0/climate_finance/oecd/crdf/provider_perspective.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/crdf/recipient_perspective.py` & `climate_finance-1.1.0/climate_finance/oecd/crdf/recipient_perspective.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/crdf/tools.py` & `climate_finance-1.1.0/climate_finance/oecd/crdf/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/crs/add_crs_data.py` & `climate_finance-1.1.0/climate_finance/oecd/crs/add_crs_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/crs/get_data.py` & `climate_finance-1.1.0/climate_finance/oecd/crs/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/multisystem/crs_channel_mapping.csv` & `climate_finance-1.1.0/climate_finance/oecd/multisystem/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/oecd/multisystem/get_data.py` & `climate_finance-1.1.0/climate_finance/oecd/multisystem/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/README.md` & `climate_finance-1.1.0/climate_finance/unfccc/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/tools.py` & `climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json` & `climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/cleaning_tools/validation.py` & `climate_finance-1.1.0/climate_finance/unfccc/cleaning_tools/validation.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/download/download_data.py` & `climate_finance-1.1.0/climate_finance/unfccc/download/download_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/download/get_data.py` & `climate_finance-1.1.0/climate_finance/unfccc/download/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/download/pre_process.py` & `climate_finance-1.1.0/climate_finance/unfccc/download/pre_process.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/get_unfccc_data.py` & `climate_finance-1.1.0/climate_finance/unfccc/get_unfccc_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/manual/get_data.py` & `climate_finance-1.1.0/climate_finance/unfccc/manual/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/manual/pre_process.py` & `climate_finance-1.1.0/climate_finance/unfccc/manual/pre_process.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/climate_finance/unfccc/manual/read_files.py` & `climate_finance-1.1.0/climate_finance/unfccc/manual/read_files.py`

 * *Files identical despite different names*

### Comparing `climate_finance-1.0.1/pyproject.toml` & `climate_finance-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "climate-finance"
-version = "1.0.1"
+version = "1.1.0"
 description = "Climate Finance data"
 authors = ["Jorge Rivera, The ONE Campaign"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "climate_finance"}]
 
 [tool.poetry.dependencies]
```

### Comparing `climate_finance-1.0.1/PKG-INFO` & `climate_finance-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climate-finance
-Version: 1.0.1
+Version: 1.1.0
 Summary: Climate Finance data
 License: MIT
 Author: Jorge Rivera, The ONE Campaign
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

