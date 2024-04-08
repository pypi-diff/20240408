# Comparing `tmp/affixapi-1.1.51.tar.gz` & `tmp/affixapi-1.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.51.tar", last modified: Sun Apr  7 22:32:06 2024, max compression
+gzip compressed data, was "affixapi-1.1.52.tar", last modified: Mon Apr  8 01:45:28 2024, max compression
```

## Comparing `affixapi-1.1.51.tar` & `affixapi-1.1.52.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.743336 affixapi-1.1.51/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 22:32:03.000000 affixapi-1.1.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-07 22:32:06.743336 affixapi-1.1.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-04-07 22:32:03.000000 affixapi-1.1.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.743336 affixapi-1.1.51/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 22:32:06.000000 affixapi-1.1.51/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.719335 affixapi-1.1.51/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.719335 affixapi-1.1.51/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52498 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.723335 affixapi-1.1.51/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.731335 affixapi-1.1.51/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.731335 affixapi-1.1.51/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-07 22:32:03.000000 affixapi-1.1.51/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 22:32:06.743336 affixapi-1.1.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-07 22:32:03.000000 affixapi-1.1.51/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:32:06.743336 affixapi-1.1.51/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-07 22:32:03.000000 affixapi-1.1.51/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.512152 affixapi-1.1.52/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 01:45:25.000000 affixapi-1.1.52/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-08 01:45:28.512152 affixapi-1.1.52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-04-08 01:45:25.000000 affixapi-1.1.52/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.512152 affixapi-1.1.52/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-04-08 01:45:28.000000 affixapi-1.1.52/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-08 01:45:28.000000 affixapi-1.1.52/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:45:28.000000 affixapi-1.1.52/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 01:45:28.000000 affixapi-1.1.52/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 01:45:28.000000 affixapi-1.1.52/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.488152 affixapi-1.1.52/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.488152 affixapi-1.1.52/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52498 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.488152 affixapi-1.1.52/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.500152 affixapi-1.1.52/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.500152 affixapi-1.1.52/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-08 01:45:25.000000 affixapi-1.1.52/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 01:45:28.512152 affixapi-1.1.52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 01:45:25.000000 affixapi-1.1.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:45:28.512152 affixapi-1.1.52/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-08 01:45:25.000000 affixapi-1.1.52/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.51/LICENSE` & `affixapi-1.1.52/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/PKG-INFO` & `affixapi-1.1.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.51
+Version: 1.1.52
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `affixapi-1.1.51/README.md` & `affixapi-1.1.52/README.md`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.52/affixapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.51
+Version: 1.1.52
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `affixapi-1.1.51/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.52/affixapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/__init__.py` & `affixapi-1.1.52/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.52/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/api/core_api.py` & `affixapi-1.1.52/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/api/management_api.py` & `affixapi-1.1.52/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.52/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/api_client.py` & `affixapi-1.1.52/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/apis/__init__.py` & `affixapi-1.1.52/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/configuration.py` & `affixapi-1.1.52/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/exceptions.py` & `affixapi-1.1.52/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.52/openapi_client/model/address_no_non_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,19 +65,24 @@
             'DE': "DE",
             'DK': "DK",
             'EE': "EE",
             'ES': "ES",
             'FR': "FR",
             'GB': "GB",
             'HK': "HK",
+            'ID': "ID",
             'IE': "IE",
+            'IN': "IN",
             'IT': "IT",
             'JP': "JP",
+            'KR': "KR",
             'LT': "LT",
             'LV': "LV",
+            'MO': "MO",
+            'MY': "MY",
             'NL': "NL",
             'NO': "NO",
             'PH': "PH",
             'PL': "PL",
             'RO': "RO",
             'SE': "SE",
             'SG': "SG",
```

### Comparing `affixapi-1.1.51/openapi_client/model/address_response.py` & `affixapi-1.1.52/openapi_client/model/address_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,24 @@
             'DE': "DE",
             'DK': "DK",
             'EE': "EE",
             'ES': "ES",
             'FR': "FR",
             'GB': "GB",
             'HK': "HK",
+            'ID': "ID",
             'IE': "IE",
+            'IN': "IN",
             'IT': "IT",
+            'KR': "KR",
             'JP': "JP",
             'LT': "LT",
             'LV': "LV",
+            'MO': "MO",
+            'MY': "MY",
             'NL': "NL",
             'NO': "NO",
             'PH': "PH",
             'PL': "PL",
             'RO': "RO",
             'SE': "SE",
             'SG': "SG",
```

### Comparing `affixapi-1.1.51/openapi_client/model/client_request.py` & `affixapi-1.1.52/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/client_response.py` & `affixapi-1.1.52/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.52/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/company_response.py` & `affixapi-1.1.52/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/create_employee_request.py` & `affixapi-1.1.52/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.52/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.52/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.52/openapi_client/model/currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/currency_response.py` & `affixapi-1.1.52/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/disconnect_response.py` & `affixapi-1.1.52/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/employee_response.py` & `affixapi-1.1.52/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.52/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.52/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.52/openapi_client/model/employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/employment_response.py` & `affixapi-1.1.52/openapi_client/model/employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.52/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/group_response.py` & `affixapi-1.1.52/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.52/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.52/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.52/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/identity_response.py` & `affixapi-1.1.52/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/inline_response400.py` & `affixapi-1.1.52/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/inline_response401.py` & `affixapi-1.1.52/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/inline_response409.py` & `affixapi-1.1.52/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/introspect_response.py` & `affixapi-1.1.52/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.52/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/location_response.py` & `affixapi-1.1.52/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/message_response.py` & `affixapi-1.1.52/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/mode_request.py` & `affixapi-1.1.52/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/mode_response.py` & `affixapi-1.1.52/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payrun_response.py` & `affixapi-1.1.52/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.52/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payslip_response.py` & `affixapi-1.1.52/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.52/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.52/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.52/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.52/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.52/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/provider_request.py` & `affixapi-1.1.52/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/provider_response.py` & `affixapi-1.1.52/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/providers_response.py` & `affixapi-1.1.52/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/scopes_request.py` & `affixapi-1.1.52/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/scopes_response.py` & `affixapi-1.1.52/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.52/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.52/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.52/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.52/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/timesheet_response.py` & `affixapi-1.1.52/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.52/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/token_request.py` & `affixapi-1.1.52/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/token_response.py` & `affixapi-1.1.52/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/tokens_response.py` & `affixapi-1.1.52/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.52/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/model_utils.py` & `affixapi-1.1.52/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/models/__init__.py` & `affixapi-1.1.52/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/openapi_client/rest.py` & `affixapi-1.1.52/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/setup.py` & `affixapi-1.1.52/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.51"
+VERSION = "1.1.52"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.51/test/test_2023_03_01_api.py` & `affixapi-1.1.52/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_address_no_non_null_request.py` & `affixapi-1.1.52/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_address_response.py` & `affixapi-1.1.52/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_client_request.py` & `affixapi-1.1.52/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_client_response.py` & `affixapi-1.1.52/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_companies20230301_response.py` & `affixapi-1.1.52/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_company_response.py` & `affixapi-1.1.52/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_core_api.py` & `affixapi-1.1.52/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_create_employee_request.py` & `affixapi-1.1.52/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.52/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_create_employee_request_manager.py` & `affixapi-1.1.52/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_currency_not_null_request.py` & `affixapi-1.1.52/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_currency_response.py` & `affixapi-1.1.52/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_disconnect_response.py` & `affixapi-1.1.52/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_employee_response.py` & `affixapi-1.1.52/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_employee_response_manager.py` & `affixapi-1.1.52/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_employees20230301_response.py` & `affixapi-1.1.52/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.52/test/test_employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_employment_response.py` & `affixapi-1.1.52/test/test_employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_group_no_null_enum_request.py` & `affixapi-1.1.52/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_group_response.py` & `affixapi-1.1.52/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_groups20230301_response.py` & `affixapi-1.1.52/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.52/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_id_and_message_response.py` & `affixapi-1.1.52/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_identity_response.py` & `affixapi-1.1.52/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_inline_response400.py` & `affixapi-1.1.52/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_inline_response401.py` & `affixapi-1.1.52/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_inline_response409.py` & `affixapi-1.1.52/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_introspect_response.py` & `affixapi-1.1.52/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_location_no_non_null_request.py` & `affixapi-1.1.52/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_location_response.py` & `affixapi-1.1.52/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_management_api.py` & `affixapi-1.1.52/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_message_response.py` & `affixapi-1.1.52/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_mode_request.py` & `affixapi-1.1.52/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_mode_response.py` & `affixapi-1.1.52/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payrun_response.py` & `affixapi-1.1.52/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payruns20230301_response.py` & `affixapi-1.1.52/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payslip_response.py` & `affixapi-1.1.52/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payslip_response_contributions.py` & `affixapi-1.1.52/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payslip_response_deductions.py` & `affixapi-1.1.52/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payslip_response_earnings.py` & `affixapi-1.1.52/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payslip_response_taxes.py` & `affixapi-1.1.52/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_payslips20230301_response.py` & `affixapi-1.1.52/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_provider_request.py` & `affixapi-1.1.52/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_provider_response.py` & `affixapi-1.1.52/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_providers_response.py` & `affixapi-1.1.52/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_scopes_request.py` & `affixapi-1.1.52/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_scopes_response.py` & `affixapi-1.1.52/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_time_off_balance_response.py` & `affixapi-1.1.52/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.52/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.52/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_time_off_entry_response.py` & `affixapi-1.1.52/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_timesheet_response.py` & `affixapi-1.1.52/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_timesheets20230301_response.py` & `affixapi-1.1.52/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_token_request.py` & `affixapi-1.1.52/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_token_response.py` & `affixapi-1.1.52/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_tokens_response.py` & `affixapi-1.1.52/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_work_locations20230301_response.py` & `affixapi-1.1.52/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.51/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.52/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

