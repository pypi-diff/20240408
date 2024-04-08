# Comparing `tmp/affixapi-1.1.50.tar.gz` & `tmp/affixapi-1.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.50.tar", last modified: Sun Apr  7 15:43:29 2024, max compression
+gzip compressed data, was "affixapi-1.1.51.tar", last modified: Sun Apr  7 22:32:06 2024, max compression
```

## Comparing `affixapi-1.1.50.tar` & `affixapi-1.1.51.tar`

### file list

```diff
@@ -1,144 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.287886 affixapi-1.1.50/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 15:43:26.000000 affixapi-1.1.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21363 2024-04-07 15:43:29.287886 affixapi-1.1.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-04-07 15:43:26.000000 affixapi-1.1.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.287886 affixapi-1.1.50/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21363 2024-04-07 15:43:29.000000 affixapi-1.1.50/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-07 15:43:29.000000 affixapi-1.1.50/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:43:29.000000 affixapi-1.1.50/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-07 15:43:29.000000 affixapi-1.1.50/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 15:43:29.000000 affixapi-1.1.50/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.267886 affixapi-1.1.50/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.267886 affixapi-1.1.50/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52498 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.267886 affixapi-1.1.50/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.279886 affixapi-1.1.50/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.279886 affixapi-1.1.50/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-07 15:43:26.000000 affixapi-1.1.50/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 15:43:29.287886 affixapi-1.1.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-07 15:43:26.000000 affixapi-1.1.50/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:43:29.287886 affixapi-1.1.50/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-07 15:43:26.000000 affixapi-1.1.50/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.743336 affixapi-1.1.51/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 22:32:03.000000 affixapi-1.1.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-07 22:32:06.743336 affixapi-1.1.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-04-07 22:32:03.000000 affixapi-1.1.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.743336 affixapi-1.1.51/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.719335 affixapi-1.1.51/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.719335 affixapi-1.1.51/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52498 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.723335 affixapi-1.1.51/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.731335 affixapi-1.1.51/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.731335 affixapi-1.1.51/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 22:32:06.743336 affixapi-1.1.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-07 22:32:03.000000 affixapi-1.1.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.743336 affixapi-1.1.51/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.50/LICENSE` & `affixapi-1.1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/PKG-INFO` & `affixapi-1.1.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.50
+Version: 1.1.51
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -359,14 +359,15 @@
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
+ - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
```

### Comparing `affixapi-1.1.50/README.md` & `affixapi-1.1.51/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,15 @@
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
+ - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
```

### Comparing `affixapi-1.1.50/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.51/affixapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.50
+Version: 1.1.51
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -359,14 +359,15 @@
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
+ - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
```

### Comparing `affixapi-1.1.50/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.51/affixapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 openapi_client/model/create_employee_request.py
 openapi_client/model/create_employee_request_bank_account.py
 openapi_client/model/create_employee_request_manager.py
 openapi_client/model/currency_not_null_request.py
 openapi_client/model/currency_response.py
 openapi_client/model/disconnect_response.py
 openapi_client/model/employee_response.py
+openapi_client/model/employee_response_manager.py
 openapi_client/model/employees20230301_response.py
 openapi_client/model/employment_no_null_enum_request.py
 openapi_client/model/employment_response.py
 openapi_client/model/group_no_null_enum_request.py
 openapi_client/model/group_response.py
 openapi_client/model/groups20230301_response.py
 openapi_client/model/groups_no_null_enum_request.py
@@ -86,14 +87,15 @@
 test/test_create_employee_request.py
 test/test_create_employee_request_bank_account.py
 test/test_create_employee_request_manager.py
 test/test_currency_not_null_request.py
 test/test_currency_response.py
 test/test_disconnect_response.py
 test/test_employee_response.py
+test/test_employee_response_manager.py
 test/test_employees20230301_response.py
 test/test_employment_no_null_enum_request.py
 test/test_employment_response.py
 test/test_group_no_null_enum_request.py
 test/test_group_response.py
 test/test_groups20230301_response.py
 test/test_groups_no_null_enum_request.py
```

### Comparing `affixapi-1.1.50/openapi_client/__init__.py` & `affixapi-1.1.51/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.51/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/api/core_api.py` & `affixapi-1.1.51/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/api/management_api.py` & `affixapi-1.1.51/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.51/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/api_client.py` & `affixapi-1.1.51/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/apis/__init__.py` & `affixapi-1.1.51/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/configuration.py` & `affixapi-1.1.51/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/exceptions.py` & `affixapi-1.1.51/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.51/openapi_client/model/address_no_non_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,36 +52,41 @@
           as additional properties values.
     """
 
     allowed_values = {
         ('country',): {
             'None': None,
             'AT': "AT",
+            'AU': "AU",
             'BE': "BE",
             'CA': "CA",
             'CH': "CH",
+            'CN': "CN",
             'CZ': "CZ",
             'DE': "DE",
             'DK': "DK",
             'EE': "EE",
             'ES': "ES",
             'FR': "FR",
             'GB': "GB",
+            'HK': "HK",
             'IE': "IE",
             'IT': "IT",
             'JP': "JP",
             'LT': "LT",
             'LV': "LV",
             'NL': "NL",
             'NO': "NO",
+            'PH': "PH",
             'PL': "PL",
             'RO': "RO",
             'SE': "SE",
             'SG': "SG",
             'SK': "SK",
+            'TW': "TW",
             'US': "US",
         },
     }
 
     validations = {
     }
```

### Comparing `affixapi-1.1.50/openapi_client/model/address_response.py` & `affixapi-1.1.51/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/client_request.py` & `affixapi-1.1.51/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/client_response.py` & `affixapi-1.1.51/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.51/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/company_response.py` & `affixapi-1.1.51/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/create_employee_request.py` & `affixapi-1.1.51/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.51/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.51/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.51/openapi_client/model/currency_not_null_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,26 +46,27 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
+            'None': None,
             'USD': "usd",
             'GBP': "gbp",
             'EUR': "eur",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `affixapi-1.1.50/openapi_client/model/currency_response.py` & `affixapi-1.1.51/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/disconnect_response.py` & `affixapi-1.1.51/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/employee_response.py` & `affixapi-1.1.51/openapi_client/model/employee_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
     from openapi_client.model.address_response import AddressResponse
     from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
-    from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
+    from openapi_client.model.employee_response_manager import EmployeeResponseManager
     from openapi_client.model.employment_response import EmploymentResponse
     from openapi_client.model.groups20230301_response import Groups20230301Response
     from openapi_client.model.location_response import LocationResponse
     globals()['AddressResponse'] = AddressResponse
     globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
-    globals()['CreateEmployeeRequestManager'] = CreateEmployeeRequestManager
+    globals()['EmployeeResponseManager'] = EmployeeResponseManager
     globals()['EmploymentResponse'] = EmploymentResponse
     globals()['Groups20230301Response'] = Groups20230301Response
     globals()['LocationResponse'] = LocationResponse
 
 
 class EmployeeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
@@ -149,15 +149,15 @@
             'employment_type': (str, none_type,),  # noqa: E501
             'start_date': (date, none_type,),  # noqa: E501
             'remote_created_at': (date, none_type,),  # noqa: E501
             'termination_date': (date, none_type,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'home_location': (AddressResponse,),  # noqa: E501
             'work_location': (LocationResponse,),  # noqa: E501
-            'manager': (CreateEmployeeRequestManager,),  # noqa: E501
+            'manager': (EmployeeResponseManager,),  # noqa: E501
             'bank_account': (CreateEmployeeRequestBankAccount,),  # noqa: E501
             'employments': ([EmploymentResponse], none_type,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'groups': (Groups20230301Response,),  # noqa: E501
         }
 
     @cached_property
@@ -233,15 +233,15 @@
             employment_type (str, none_type):
             start_date (date, none_type):
             remote_created_at (date, none_type):
             termination_date (date, none_type):
             avatar (str, none_type):
             home_location (AddressResponse):
             work_location (LocationResponse):
-            manager (CreateEmployeeRequestManager):
+            manager (EmployeeResponseManager):
             bank_account (CreateEmployeeRequestBankAccount):
             employments ([EmploymentResponse], none_type):
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type):
             groups (Groups20230301Response):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `affixapi-1.1.50/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.51/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.51/openapi_client/model/employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/employment_response.py` & `affixapi-1.1.51/openapi_client/model/employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.51/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/group_response.py` & `affixapi-1.1.51/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.51/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.51/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.51/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/identity_response.py` & `affixapi-1.1.51/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/inline_response400.py` & `affixapi-1.1.51/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/inline_response401.py` & `affixapi-1.1.51/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/inline_response409.py` & `affixapi-1.1.51/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/introspect_response.py` & `affixapi-1.1.51/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.51/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/location_response.py` & `affixapi-1.1.51/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/message_response.py` & `affixapi-1.1.51/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/mode_request.py` & `affixapi-1.1.51/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/mode_response.py` & `affixapi-1.1.51/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payrun_response.py` & `affixapi-1.1.51/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.51/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payslip_response.py` & `affixapi-1.1.51/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.51/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.51/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.51/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.51/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.51/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/provider_request.py` & `affixapi-1.1.51/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/provider_response.py` & `affixapi-1.1.51/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/providers_response.py` & `affixapi-1.1.51/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/scopes_request.py` & `affixapi-1.1.51/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/scopes_response.py` & `affixapi-1.1.51/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.51/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.51/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.51/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.51/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/timesheet_response.py` & `affixapi-1.1.51/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.51/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/token_request.py` & `affixapi-1.1.51/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/token_response.py` & `affixapi-1.1.51/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/tokens_response.py` & `affixapi-1.1.51/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.51/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/model_utils.py` & `affixapi-1.1.51/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/openapi_client/models/__init__.py` & `affixapi-1.1.51/openapi_client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
 from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
 from openapi_client.model.currency_response import CurrencyResponse
 from openapi_client.model.disconnect_response import DisconnectResponse
 from openapi_client.model.employee_response import EmployeeResponse
+from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
 from openapi_client.model.employment_response import EmploymentResponse
 from openapi_client.model.group_no_null_enum_request import GroupNoNullEnumRequest
 from openapi_client.model.group_response import GroupResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
```

### Comparing `affixapi-1.1.50/openapi_client/rest.py` & `affixapi-1.1.51/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/setup.py` & `affixapi-1.1.51/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.50"
+VERSION = "1.1.51"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.50/test/test_2023_03_01_api.py` & `affixapi-1.1.51/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_address_no_non_null_request.py` & `affixapi-1.1.51/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_address_response.py` & `affixapi-1.1.51/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_client_request.py` & `affixapi-1.1.51/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_client_response.py` & `affixapi-1.1.51/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_companies20230301_response.py` & `affixapi-1.1.51/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_company_response.py` & `affixapi-1.1.51/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_core_api.py` & `affixapi-1.1.51/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_create_employee_request.py` & `affixapi-1.1.51/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.51/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_create_employee_request_manager.py` & `affixapi-1.1.51/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_currency_not_null_request.py` & `affixapi-1.1.51/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_currency_response.py` & `affixapi-1.1.51/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_disconnect_response.py` & `affixapi-1.1.51/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_employee_response.py` & `affixapi-1.1.51/test/test_employee_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 import sys
 import unittest
 
 import openapi_client
 from openapi_client.model.address_response import AddressResponse
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
-from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
+from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employment_response import EmploymentResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.location_response import LocationResponse
 globals()['AddressResponse'] = AddressResponse
 globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
-globals()['CreateEmployeeRequestManager'] = CreateEmployeeRequestManager
+globals()['EmployeeResponseManager'] = EmployeeResponseManager
 globals()['EmploymentResponse'] = EmploymentResponse
 globals()['Groups20230301Response'] = Groups20230301Response
 globals()['LocationResponse'] = LocationResponse
 from openapi_client.model.employee_response import EmployeeResponse
 
 
 class TestEmployeeResponse(unittest.TestCase):
```

### Comparing `affixapi-1.1.50/test/test_employees20230301_response.py` & `affixapi-1.1.51/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.51/test/test_employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_employment_response.py` & `affixapi-1.1.51/test/test_employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_group_no_null_enum_request.py` & `affixapi-1.1.51/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_group_response.py` & `affixapi-1.1.51/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_groups20230301_response.py` & `affixapi-1.1.51/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.51/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_id_and_message_response.py` & `affixapi-1.1.51/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_identity_response.py` & `affixapi-1.1.51/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_inline_response400.py` & `affixapi-1.1.51/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_inline_response401.py` & `affixapi-1.1.51/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_inline_response409.py` & `affixapi-1.1.51/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_introspect_response.py` & `affixapi-1.1.51/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_location_no_non_null_request.py` & `affixapi-1.1.51/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_location_response.py` & `affixapi-1.1.51/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_management_api.py` & `affixapi-1.1.51/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_message_response.py` & `affixapi-1.1.51/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_mode_request.py` & `affixapi-1.1.51/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_mode_response.py` & `affixapi-1.1.51/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payrun_response.py` & `affixapi-1.1.51/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payruns20230301_response.py` & `affixapi-1.1.51/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payslip_response.py` & `affixapi-1.1.51/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payslip_response_contributions.py` & `affixapi-1.1.51/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payslip_response_deductions.py` & `affixapi-1.1.51/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payslip_response_earnings.py` & `affixapi-1.1.51/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payslip_response_taxes.py` & `affixapi-1.1.51/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_payslips20230301_response.py` & `affixapi-1.1.51/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_provider_request.py` & `affixapi-1.1.51/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_provider_response.py` & `affixapi-1.1.51/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_providers_response.py` & `affixapi-1.1.51/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_scopes_request.py` & `affixapi-1.1.51/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_scopes_response.py` & `affixapi-1.1.51/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_time_off_balance_response.py` & `affixapi-1.1.51/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.51/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.51/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_time_off_entry_response.py` & `affixapi-1.1.51/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_timesheet_response.py` & `affixapi-1.1.51/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_timesheets20230301_response.py` & `affixapi-1.1.51/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_token_request.py` & `affixapi-1.1.51/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_token_response.py` & `affixapi-1.1.51/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_tokens_response.py` & `affixapi-1.1.51/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_work_locations20230301_response.py` & `affixapi-1.1.51/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.50/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.51/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

