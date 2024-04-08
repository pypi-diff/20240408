# Comparing `tmp/Firefly_III_API_Client-2.0.12.0.tar.gz` & `tmp/Firefly_III_API_Client-2.0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Firefly III API Client-2.0.12.0.tar", last modified: Mon Apr  8 21:14:20 2024, max compression
+gzip compressed data, was "Firefly III API Client-2.0.5.0.tar", last modified: Sun Aug  6 11:19:01 2023, max compression
```

## Comparing `Firefly_III_API_Client-2.0.12.0.tar` & `Firefly_III_API_Client-2.0.5.0.tar`

### file list

```diff
@@ -1,498 +1,1685 @@
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:14:20.517942 Firefly III API Client-2.0.12.0/
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:14:20.517942 Firefly III API Client-2.0.12.0/Firefly_III_API_Client.egg-info/
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      522 2024-04-08 21:14:20.000000 Firefly III API Client-2.0.12.0/Firefly_III_API_Client.egg-info/PKG-INFO
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    18643 2024-04-08 21:14:20.000000 Firefly III API Client-2.0.12.0/Firefly_III_API_Client.egg-info/SOURCES.txt
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)        1 2024-04-08 21:14:20.000000 Firefly III API Client-2.0.12.0/Firefly_III_API_Client.egg-info/dependency_links.txt
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)       76 2024-04-08 21:14:20.000000 Firefly III API Client-2.0.12.0/Firefly_III_API_Client.egg-info/requires.txt
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)       19 2024-04-08 21:14:20.000000 Firefly III API Client-2.0.12.0/Firefly_III_API_Client.egg-info/top_level.txt
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      522 2024-04-08 21:14:20.517942 Firefly III API Client-2.0.12.0/PKG-INFO
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    45436 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/README.md
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:14:20.481941 Firefly III API Client-2.0.12.0/firefly_iii_client/
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17751 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/__init__.py
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:14:20.485941 Firefly III API Client-2.0.12.0/firefly_iii_client/api/
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1636 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/__init__.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    37832 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/about_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   110771 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/accounts_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    88807 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/attachments_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   201559 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/autocomplete_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    28315 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/available_budgets_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   108241 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/bills_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   194806 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/budgets_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    94867 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/categories_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14286 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/charts_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    38425 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/configuration_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   208870 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/currencies_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   146127 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/data_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   369210 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/insight_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   143760 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/links_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    76558 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/object_groups_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    89322 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/piggy_banks_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    52649 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/preferences_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    80906 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/recurrences_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   115536 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/rule_groups_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    95899 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/rules_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    29813 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/search_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15482 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/summary_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    96341 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/tags_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   130899 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/transactions_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    61882 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/users_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)   165213 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api/webhooks_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    25808 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api_client.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      652 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/api_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15039 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/configuration.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5962 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/exceptions.py
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:14:20.497941 Firefly III API Client-2.0.12.0/firefly_iii_client/models/
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15580 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/__init__.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12540 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3202 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2933 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      918 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_role_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      819 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_search_field_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2725 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10532 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1366 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_type_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1164 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     9957 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      897 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachable_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4497 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachment.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3226 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachment_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3305 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachment_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2749 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachment_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3227 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachment_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2888 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/attachment_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      885 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/auto_budget_period.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      822 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/auto_budget_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3942 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_account.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2778 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_bill.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2618 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_budget.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2628 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_category.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2880 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_currency.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2927 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_currency_code.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2797 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_object_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4411 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_piggy.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4501 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_piggy_balance.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2842 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_recurrence.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2806 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_rule.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2838 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_rule_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2737 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_tag.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3062 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_transaction.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3112 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_transaction_id.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2795 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/autocomplete_transaction_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5373 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/available_budget.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3267 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/available_budget_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2998 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/available_budget_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2790 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/available_budget_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2619 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bad_request_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4528 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/basic_summary_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     9437 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3178 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3301 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_paid_dates_inner.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2909 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      859 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_repeat_frequency.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2701 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5274 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5353 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/bill_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6572 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3194 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5273 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_limit.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3235 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_limit_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2966 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_limit_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2758 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_limit_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3897 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_limit_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2925 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2717 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3126 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_spent.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5452 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5385 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/budget_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4373 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3210 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3139 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category_earned.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2941 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2733 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3134 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category_spent.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2761 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/category_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2616 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/chart_data_point.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4781 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/chart_data_set.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1925 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/config_value_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1032 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/config_value_update_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3093 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/configuration.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2756 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/configuration_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2790 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/configuration_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      829 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/credit_card_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3630 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/cron_result.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4318 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/cron_result_row.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3536 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/currency.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3550 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/currency_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2941 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/currency_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2733 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/currency_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3348 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/currency_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3532 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/currency_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1272 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/data_destroy_object.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      723 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/export_file_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3749 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/insight_group_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3495 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/insight_total_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4827 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/insight_transfer_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      930 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/interest_period_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2647 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/internal_exception_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      896 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/liability_direction_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      840 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/liability_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2783 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/link_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3551 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/link_type_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3290 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/link_type_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2734 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/link_type_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2673 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/link_type_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2782 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/meta.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2901 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/meta_pagination.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2611 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/not_found_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2992 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3235 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_group_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2966 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_group_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2758 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_group_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2648 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_group_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2855 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_link.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2551 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/object_link0.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3195 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/page_link.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8645 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3559 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4249 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_event.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3600 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_event_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3339 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_event_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3298 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2742 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5218 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5654 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/piggy_bank_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6831 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/polymorphic_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3223 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/preference.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3566 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/preference_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2957 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/preference_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2749 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/preference_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2769 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/preference_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6870 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3566 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3305 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4811 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_repetition.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3746 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_repetition_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      933 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_repetition_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3791 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_repetition_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2749 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5968 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11410 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_transaction.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6223 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_transaction_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      814 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_transaction_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5885 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_transaction_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5917 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5687 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4174 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_action.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1594 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_action_keyword.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3660 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_action_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3561 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_action_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3518 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3456 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3559 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_group_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3298 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_group_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2742 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_group_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3013 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_group_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3034 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_group_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3257 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2701 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5275 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4038 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_trigger.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2138 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_trigger_keyword.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3453 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_trigger_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      866 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_trigger_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3443 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_trigger_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5120 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/rule_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1066 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/short_account_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2753 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/system_info.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2885 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/system_info_data.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3510 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/tag_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5022 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/tag_model.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4670 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/tag_model_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4698 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/tag_model_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3270 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/tag_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2693 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/tag_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4040 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3574 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4006 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_link.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3607 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_link_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3346 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_link_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2790 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_link_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3634 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_link_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3784 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_link_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3313 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2757 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    26683 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_split.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19591 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_split_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21544 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_split_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4218 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1102 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_type_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      886 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4003 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/transaction_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2639 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/unauthenticated_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3878 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/user.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3518 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/user_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      825 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/user_blocked_code_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3257 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/user_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      790 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/user_role_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2701 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/user_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2989 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/validation_error_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3435 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/validation_error_response_errors.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4157 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3542 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4253 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_attempt.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3259 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_attempt_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2990 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_attempt_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2782 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_attempt_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      740 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_delivery.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3873 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_message.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3259 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_message_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2990 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_message_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2782 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_message_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3281 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      830 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2725 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3324 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      853 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_trigger.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3816 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/py.typed
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     9226 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/firefly_iii_client/rest.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)       69 2024-04-08 21:14:20.517942 Firefly III API Client-2.0.12.0/setup.cfg
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1314 2024-04-08 21:13:56.000000 Firefly III API Client-2.0.12.0/setup.py
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-04-08 21:14:20.517942 Firefly III API Client-2.0.12.0/test/
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1033 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_about_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2725 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6178 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4662 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      741 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_role_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      777 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_search_field_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5118 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2430 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      727 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_type_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      741 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2332 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_account_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1857 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_accounts_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      705 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachable_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2050 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachment.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4962 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachment_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3656 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachment_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4014 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachment_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1677 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachment_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1488 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachment_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1673 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_attachments_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      720 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_auto_budget_period.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      706 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_auto_budget_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2154 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_account.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4058 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1529 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_bill.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1518 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_budget.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1544 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_category.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1742 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_currency.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1803 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_currency_code.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1681 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_object_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1798 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_piggy.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1902 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_piggy_balance.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1625 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_recurrence.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1538 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_rule.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1615 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_rule_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1616 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_tag.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1716 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_transaction.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1761 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_transaction_id.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1703 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_autocomplete_transaction_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2650 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_available_budget.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5711 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_available_budget_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4257 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_available_budget_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4699 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_available_budget_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      994 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_available_budgets_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1491 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bad_request_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1791 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_basic_summary_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2831 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6118 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1546 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_paid_dates_inner.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4614 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      741 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_repeat_frequency.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5058 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2086 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1923 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bill_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1778 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_bills_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2123 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4742 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2042 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_limit.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4151 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_limit_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2905 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_limit_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3235 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_limit_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1839 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_limit_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3422 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3778 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1500 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_spent.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1711 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1723 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budget_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2769 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_budgets_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1683 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_categories_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2227 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4960 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1536 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category_earned.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3616 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3988 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1527 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category_spent.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1456 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_category_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1378 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_chart_data_point.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1872 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_chart_data_set.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      813 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_charts_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      727 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_config_value_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      770 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_config_value_update_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1567 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_configuration.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1160 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_configuration_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1830 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_configuration_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1466 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_configuration_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      763 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_credit_card_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2109 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_cron_result.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1493 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_cron_result_row.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3225 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currencies_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1706 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currency.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4450 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currency_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2330 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currency_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2606 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currency_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1650 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currency_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1554 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_currency_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2594 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_data_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      727 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_data_destroy_object.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      720 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_export_file_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4803 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_insight_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1605 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_insight_group_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1539 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_insight_total_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1779 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_insight_transfer_entry.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      762 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_interest_period_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1576 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_internal_exception_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      790 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_liability_direction_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      755 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_liability_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1580 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_link_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4759 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_link_type_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2619 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_link_type_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2907 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_link_type_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1483 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_link_type_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2375 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_links_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1494 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_meta.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1500 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_meta_pagination.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1472 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_not_found_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1566 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3171 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_group_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2069 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_group_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2327 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_group_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1496 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_group_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1634 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_groups_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1526 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_link.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1376 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_object_link0.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1661 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_page_link.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2367 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6827 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1752 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_event.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5498 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_event_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3252 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_event_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4395 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4831 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1946 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1910 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_bank_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1712 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_piggy_banks_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1407 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_polymorphic_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1561 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_preference.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4118 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_preference_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2054 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_preference_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2306 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_preference_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1428 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_preference_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1236 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_preferences_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4349 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11924 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8882 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1898 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_repetition.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1660 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_repetition_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      776 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_repetition_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1609 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_repetition_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     9624 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4412 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2900 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_transaction.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2272 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_transaction_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      783 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_transaction_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2449 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_transaction_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3118 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrence_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1630 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_recurrences_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3882 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1703 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_action.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      727 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_action_keyword.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1622 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_action_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1552 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_action_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8050 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1616 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_group.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5061 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_group_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2885 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_group_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3193 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_group_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1561 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_group_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1527 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_group_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1884 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_groups_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5464 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5966 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3195 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1691 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_trigger.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      734 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_trigger_keyword.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1610 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_trigger_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      713 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_trigger_type.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1552 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_trigger_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2323 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rule_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1575 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_rules_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      907 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_search_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      777 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_short_account_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      782 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_summary_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1601 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_system_info.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1540 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_system_info_data.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5184 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tag_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1684 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tag_model.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1629 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tag_model_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1606 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tag_model_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3002 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tag_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3300 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tag_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1558 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_tags_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8687 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13644 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1781 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_link.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5281 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_link_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3065 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_link_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3405 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_link_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1726 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_link_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1631 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_link_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10438 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11264 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4501 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_split.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3718 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_split_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3865 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_split_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6880 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      755 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_type_filter.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      769 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_type_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4542 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transaction_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2457 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_transactions_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1554 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_unauthenticated_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1552 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_user.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4968 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_user_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      770 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_user_blocked_code_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2814 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_user_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      720 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_user_role_property.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3100 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_user_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1264 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_users_api.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2482 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_validation_error_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2254 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_validation_error_response_errors.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1956 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5452 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1625 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_attempt.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3475 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_attempt_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2329 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_attempt_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2615 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_attempt_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      712 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_delivery.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1666 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_message.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3583 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_message_array.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2421 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_message_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2715 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_message_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3238 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_read.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      712 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_response.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3560 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_single.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1848 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_store.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      705 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_trigger.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1666 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhook_update.py
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2746 2024-04-08 21:07:21.000000 Firefly III API Client-2.0.12.0/test/test_webhooks_api.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.675772 Firefly III API Client-2.0.5.0/Firefly_III_API_Client.egg-info/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      368 2023-08-06 11:19:01.000000 Firefly III API Client-2.0.5.0/Firefly_III_API_Client.egg-info/PKG-INFO
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    71260 2023-08-06 11:19:01.000000 Firefly III API Client-2.0.5.0/Firefly_III_API_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        1 2023-08-06 11:19:01.000000 Firefly III API Client-2.0.5.0/Firefly_III_API_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      118 2023-08-06 11:19:01.000000 Firefly III API Client-2.0.5.0/Firefly_III_API_Client.egg-info/requires.txt
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)       24 2023-08-06 11:19:01.000000 Firefly III API Client-2.0.5.0/Firefly_III_API_Client.egg-info/top_level.txt
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      368 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/PKG-INFO
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    57260 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/README.md
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.675772 Firefly III API Client-2.0.5.0/firefly_iii_client/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      805 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    58538 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/api_client.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.675772 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      214 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    32209 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/path_to_api.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.691772 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      245 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      104 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_about.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      113 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_about_user.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      191 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_accounts.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      286 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_accounts_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      138 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_accounts_id_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_accounts_id_piggy_banks.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_accounts_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      200 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      298 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_attachments_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      138 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_attachments_id_download.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_attachments_id_upload.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      135 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_accounts.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      129 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_bills.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      133 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_budgets.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      139 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_categories.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      139 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_currencies.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      157 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_currencies_with_code.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      144 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_object_groups.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_piggy_banks.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      164 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_piggy_banks_with_balance.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_recurring.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_rule_groups.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      129 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_rules.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      127 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_tags.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      152 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_transaction_types.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      143 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      157 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_autocomplete_transactions_with_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      127 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_available_budgets.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_available_budgets_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      182 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_bills.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      274 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_bills_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_bills_id_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      120 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_bills_id_rules.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_bills_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      119 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budget_limits.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      188 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      282 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets_id_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      216 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets_id_limits.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets_id_limits_limit_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      167 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets_id_limits_limit_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      138 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_budgets_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      197 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_categories.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      294 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_categories_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      142 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_categories_id_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      144 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_categories_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_chart_account_overview.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      120 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_configuration.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      217 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_configuration_name.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      120 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_cron_cli_token.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      197 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      302 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_accounts.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      157 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_available_budgets.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_bills.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      149 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_budget_limits.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      141 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_default.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      141 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_disable.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      139 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_enable.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      146 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_recurrences.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_rules.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      148 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_code_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      129 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_currencies_default.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      139 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_bulk_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      126 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_destroy.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_accounts.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      126 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_bills.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      130 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_budgets.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_categories.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_piggy_banks.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_recurring.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      126 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_rules.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      124 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_tags.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_export_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      122 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_data_purge.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_asset.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_bill.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      138 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_expense.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_no_bill.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      141 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_no_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      145 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_no_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      135 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_no_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      130 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_expense_total.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_asset.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      138 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      143 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_no_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      133 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_no_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_revenue.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      128 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_income_total.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_transfer_asset.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      142 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_transfer_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      147 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_transfer_no_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_transfer_no_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_transfer_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      136 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_insight_transfer_total.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      196 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_link_types.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      293 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_link_types_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      143 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_link_types_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      119 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_object_groups.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      305 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_object_groups_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      135 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_object_groups_id_bills.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      146 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_object_groups_id_piggy_banks.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      199 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_piggy_banks.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      297 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_piggy_banks_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      143 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_piggy_banks_id_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      133 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_piggy_banks_id_events.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      200 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_preferences.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      211 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_preferences_name.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      200 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_recurrences.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      298 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_recurrences_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      146 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_recurrences_id_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      199 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rule_groups.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      297 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rule_groups_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      131 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rule_groups_id_rules.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      129 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rule_groups_id_test.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      138 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rule_groups_id_trigger.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      182 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rules.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      274 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rules_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      118 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rules_id_test.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      127 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_rules_id_trigger.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      123 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_search_accounts.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      131 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_search_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      119 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_summary_basic.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      179 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_tags.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      274 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_tags_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_tags_tag_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      134 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_tags_tag_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      240 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transaction_journals_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      149 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transaction_journals_id_links.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      217 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transaction_links.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transaction_links_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      203 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transactions.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      302 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transactions_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      146 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transactions_id_attachments.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      156 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_transactions_id_piggy_bank_events.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      182 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_users.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      274 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_users_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      191 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      286 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      132 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks_id_messages.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      262 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks_id_messages_message_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      169 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks_id_messages_message_id_attempts.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      319 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks_id_messages_message_id_attempts_attempt_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      131 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/paths/v1_webhooks_id_submit.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4118 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tag_to_api.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.691772 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      999 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      671 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/about_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1226 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/accounts_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1127 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/attachments_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2133 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/autocomplete_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      654 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/available_budgets_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1135 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/bills_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1877 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/budgets_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1137 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/categories_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      549 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/charts_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      749 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/configuration_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2178 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/currencies_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/data_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3169 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/insight_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1563 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/links_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1083 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/object_groups_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/piggy_banks_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      813 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/preferences_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1043 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/recurrences_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1199 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/rule_groups_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      980 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/rules_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      631 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/search_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      525 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/summary_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1024 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/tags_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1552 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/transactions_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      814 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/users_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1785 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/webhooks_api.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16046 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/configuration.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4534 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/exceptions.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/model/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      352 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    29685 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3876 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3479 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2107 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_role_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1407 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_search_field_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2524 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    23825 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3656 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_type_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2638 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_type_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    22652 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/account_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1691 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachable_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     9241 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachment.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3903 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachment_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4073 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachment_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2554 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachment_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5524 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachment_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4144 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/attachment_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2106 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/auto_budget_period.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1761 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/auto_budget_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7334 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_account.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1486 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_account_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3396 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_bill.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1459 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_bill_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2893 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1477 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_budget_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2897 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1495 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_category_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4536 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_currency.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1495 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_currency_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4544 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_currency_code.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1532 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_currency_code_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3395 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_object_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1523 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_object_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8718 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_piggy.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1468 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_piggy_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8784 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_piggy_balance.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1532 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_piggy_balance_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3471 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_recurrence.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1513 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_recurrence_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3459 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_rule.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1459 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_rule_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3469 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_rule_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1505 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_rule_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1450 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_tag_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4178 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1522 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4182 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1541 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction_id_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3387 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1559 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction_type_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10293 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/available_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3949 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/available_budget_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3560 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/available_budget_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2605 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/available_budget_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4617 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/available_budget_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/available_budget_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2983 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bad_request.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1449 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/basic_summary.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7747 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/basic_summary_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    26569 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3849 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3449 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1536 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill_repeat_frequency.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2494 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12003 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11986 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/bill_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12980 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3867 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10668 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_limit.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3913 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_limit_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3520 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_limit_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2565 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_limit_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6367 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_limit_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3469 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2514 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4922 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_spent.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10418 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10420 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/budget_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7667 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3885 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4928 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_earned.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3489 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2534 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4926 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_spent.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3627 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3629 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/category_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2395 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/chart_data_point.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8563 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/chart_data_set.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1408 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/chart_line.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4450 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/config_value_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1624 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/config_value_update_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3763 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/configuration.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1431 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/configuration_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2551 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/configuration_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2612 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/configuration_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/credit_card_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3913 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/cron_result.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6974 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/cron_result_row.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6225 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/currency.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4433 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/currency_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3489 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/currency_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2534 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/currency_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5091 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/currency_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5498 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/currency_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3258 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/data_destroy_object.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      975 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/export_file_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1449 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/insight_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5253 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/insight_group_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1449 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/insight_total.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/insight_total_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1476 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/insight_transfer.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7208 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/insight_transfer_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2045 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/interest_period.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2997 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/internal_exception.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1727 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/liability_direction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1761 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/liability_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3994 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/link_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4434 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/link_type_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4054 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/link_type_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2535 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/link_type_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3471 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/link_type_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3431 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/link_type_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7464 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/meta.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2979 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/not_found.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4106 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/object_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3913 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/object_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3520 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/object_group_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2565 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/object_group_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2974 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/object_group_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5528 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/object_link.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3367 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/page_link.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21371 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4443 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7511 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_event.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4489 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_event_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4115 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_event_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4064 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2545 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11730 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12859 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/piggy_bank_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3016 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/polymorphic_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4202 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/preference.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4451 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/preference_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3509 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/preference_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2554 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/preference_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/preference_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14893 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4451 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4073 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7758 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_repetition.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4196 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_repetition_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_repetition_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4176 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_repetition_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2554 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12610 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    28884 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_transaction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14384 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_transaction_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1278 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_transaction_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13358 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_transaction_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11842 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/recurrence_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11119 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6994 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_action.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4183 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_action_keyword.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5407 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_action_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5397 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_action_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4397 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5881 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4443 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4064 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_group_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2545 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_group_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4747 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_group_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4713 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_group_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4013 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2494 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10057 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6308 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_trigger.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6244 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_trigger_keyword.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4721 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_trigger_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1279 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_trigger_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4710 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_trigger_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     9383 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/rule_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2140 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/short_account_type_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1307 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/string_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      624 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/string_array_item.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7255 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/system_info.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4388 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/tag_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10035 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/tag_model.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8901 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/tag_model_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8873 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/tag_model_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4044 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/tag_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2484 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/tag_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6437 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4460 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6640 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_link.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4497 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_link_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4124 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_link_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2605 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_link_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5506 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_link_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5424 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_link_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4083 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2564 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    72775 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_split.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    52291 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_split_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    59374 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_split_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6758 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2618 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_type_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1572 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_type_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5982 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/transaction_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2993 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/unauthenticated.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5484 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/user.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4397 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/user_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1596 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/user_blocked_code_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4013 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/user_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1633 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/user_role_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2494 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/user_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21423 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/validation_error.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6960 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4424 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     7482 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_attempt.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3940 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_attempt_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3550 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_attempt_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_attempt_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1043 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_delivery.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     6312 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_message.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3940 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_message_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     3550 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_message_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_message_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     4043 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1333 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_response.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2524 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1417 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_trigger.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     5855 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/model/webhook_update.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/models/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17181 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/models/__init__.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     8701 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/__init__.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_about/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      311 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_about/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11976 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_about/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_about_user/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_about_user/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12119 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_about_user/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      317 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14822 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      323 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13713 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16152 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21685 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16334 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      346 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16353 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_piggy_banks/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      349 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17539 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_accounts_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      323 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14264 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19397 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      329 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13740 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14052 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21760 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id_download/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id_download/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14047 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id_download/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.715772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id_upload/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id_upload/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19517 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_attachments_id_upload/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15761 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_accounts/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      337 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14518 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_bills/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14548 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_budgets/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_categories/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_categories/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_categories/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_currencies/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_currencies/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_currencies/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_currencies_with_code/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      365 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_currencies_with_code/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14718 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_currencies_with_code/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_object_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      352 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_object_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14635 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_object_groups/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      348 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14549 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_piggy_banks/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_piggy_banks_with_balance/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      372 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_piggy_banks_with_balance/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14696 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_piggy_banks_with_balance/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_recurring/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_recurring/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14597 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_recurring/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_rule_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      348 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_rule_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14605 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_rule_groups/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      337 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14518 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_rules/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      335 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14492 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_tags/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transaction_types/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      360 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transaction_types/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14697 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transaction_types/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      351 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14635 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transactions_with_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      365 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transactions_with_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14742 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_autocomplete_transactions_with_id/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_available_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      334 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_available_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14896 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_available_budgets/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_available_budgets_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      340 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_available_budgets_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14139 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_available_budgets_id/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      311 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14712 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19246 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.719772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      317 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13667 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16378 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21610 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      329 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14078 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_rules/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16944 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_bills_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budget_limits/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      326 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budget_limits/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budget_limits/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      315 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14742 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19296 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13691 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16408 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21660 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16335 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      335 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16613 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21785 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      353 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14047 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14379 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    22050 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      379 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17052 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_limits_limit_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17512 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_budgets_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14235 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19313 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      327 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13715 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16438 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21710 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      351 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      353 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17255 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_categories_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.723772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_chart_account_overview/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_chart_account_overview/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14638 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_chart_account_overview/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      327 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12424 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration_name/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      337 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration_name/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14223 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration_name/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21831 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_configuration_name/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_cron_cli_token/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      329 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_cron_cli_token/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16365 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_cron_cli_token/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14235 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19346 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      331 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13729 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14036 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21824 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      349 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16933 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_accounts/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_available_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      366 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_available_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16464 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_available_budgets/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16287 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_bills/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_budget_limits/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      359 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_budget_limits/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16941 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_budget_limits/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_default/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_default/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14095 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_default/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_disable/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_disable/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14381 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_disable/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_enable/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_enable/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14078 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_enable/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_recurrences/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      355 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_recurrences/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16388 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_recurrences/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16287 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_rules/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      357 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17274 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_code_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_default/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      337 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_default/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12116 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_currencies_default/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_bulk_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_bulk_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    12168 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_bulk_transactions/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_destroy/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      325 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_destroy/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13993 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_destroy/delete.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14267 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_accounts/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.727772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      335 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14227 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_bills/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      339 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14274 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_budgets/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_categories/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_categories/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14290 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_categories/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      346 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14255 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_piggy_banks/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_recurring/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_recurring/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14292 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_recurring/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      335 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14247 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_rules/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      333 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14219 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_tags/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      349 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15163 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_export_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_purge/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_purge/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11143 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_data_purge/delete.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_asset/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_asset/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15465 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_asset/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_bill/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_bill/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16300 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_bill/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_budget/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_budget/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16340 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_budget/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      349 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16388 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_category/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_expense/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_expense/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15489 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_expense/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_bill/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      346 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_bill/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15474 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_bill/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_budget/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      350 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_budget/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15498 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_budget/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      354 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15522 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_category/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      344 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15462 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_no_tag/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      339 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16280 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_tag/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_total/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_total/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15445 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_expense_total/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_asset/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_asset/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15452 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_asset/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      347 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16375 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_category/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_no_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      352 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_no_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15509 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_no_category/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_no_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      342 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_no_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15449 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_no_tag/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.731772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_revenue/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_revenue/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15476 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_revenue/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      337 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16267 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_tag/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_total/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_total/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15432 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_income_total/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_asset/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_asset/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15426 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_asset/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      351 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16400 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_category/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_no_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      356 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_no_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15534 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_no_category/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_no_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      346 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_no_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15473 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_no_tag/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16292 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_tag/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_total/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      345 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_total/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15457 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_insight_transfer_total/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      320 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14250 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19333 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      326 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13736 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14034 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21729 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      352 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17214 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_link_types_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      326 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14301 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      332 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13762 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14079 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21804 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      344 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16320 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id_bills/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      355 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16412 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_object_groups_id_piggy_banks/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      322 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14261 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19390 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      328 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13738 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14049 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21754 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      352 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16366 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.735772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id_events/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      342 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id_events/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16342 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_piggy_banks_id_events/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      323 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14270 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19378 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences_name/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      333 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences_name/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14069 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences_name/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21764 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_preferences_name/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      323 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14275 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19407 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      329 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13750 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14063 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21771 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      355 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17298 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_recurrences_id_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      322 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14261 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19391 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      328 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13738 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14049 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21754 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      340 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16236 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_rules/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_test/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      338 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_test/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    18377 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_test/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_trigger/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      344 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_trigger/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17020 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rule_groups_id_trigger/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      311 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14174 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19246 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      317 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13668 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13962 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21610 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id_test/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      327 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id_test/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17342 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id_test/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id_trigger/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      333 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id_trigger/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16949 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_rules_id_trigger/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.739772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_search_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      331 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_search_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15253 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_search_accounts/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_search_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      339 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_search_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14601 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_search_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_summary_basic/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      327 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_summary_basic/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14911 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_summary_basic/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      309 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14159 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19254 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      317 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13663 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16111 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21625 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16297 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    17207 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_tags_tag_transactions/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      346 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13846 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14260 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id_links/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      358 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id_links/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16350 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_journals_id_links/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      334 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14351 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19550 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      340 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13829 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14127 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21916 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transaction_links_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      325 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    15178 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19421 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      331 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13751 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14067 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21865 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      355 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16378 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id_attachments/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id_piggy_bank_events/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      365 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id_piggy_bank_events/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16343 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_transactions_id_piggy_bank_events/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      311 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14174 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19213 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      317 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13667 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13962 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21593 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_users_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      317 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14219 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    19321 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks/post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.743772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      323 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    13703 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14007 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id/get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    21685 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id/put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.747772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      341 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14144 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.747772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      363 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14114 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14523 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.747772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      381 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    16721 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.747772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts_attempt_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      403 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts_attempt_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14517 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts_attempt_id/delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    14948 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_messages_message_id_attempts_attempt_id/get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.747772 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_submit/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      337 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_submit/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11147 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/paths/v1_webhooks_id_submit/post.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    10691 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/rest.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    97678 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/firefly_iii_client/schemas.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)       69 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/setup.cfg
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1212 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/setup.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.667771 Firefly III API Client-2.0.5.0/test/
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_models/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      565 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_role_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      636 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_search_field_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_type_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_type_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_account_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachable_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      577 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachment.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachment_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachment_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachment_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachment_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_attachment_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_auto_budget_period.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_auto_budget_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      614 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_account.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      635 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_account_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_bill.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_bill_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      610 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      631 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_budget_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      618 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      639 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_category_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      618 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_currency.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      639 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_currency_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      635 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_currency_code.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      656 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_currency_code_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      631 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_object_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      652 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_object_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      606 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_piggy.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      627 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_piggy_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      635 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_piggy_balance.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      656 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_piggy_balance_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      626 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_recurrence.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      647 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_recurrence_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_rule.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_rule_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_rule_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      644 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_rule_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_tag.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_tag_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      630 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      651 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      639 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction_id.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      660 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction_id_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      647 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      668 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction_type_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_available_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_available_budget_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_available_budget_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_available_budget_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_available_budget_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_available_budget_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bad_request.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_basic_summary.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_basic_summary_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      553 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill_repeat_frequency.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_bill_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      561 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_limit.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_limit_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_limit_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_limit_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_limit_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_spent.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_budget_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      569 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_earned.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_spent.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_category_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_chart_data_point.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      587 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_chart_data_set.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_chart_line.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_config_value_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      632 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_config_value_update_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      589 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_configuration.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      610 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_configuration_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      614 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_configuration_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      614 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_configuration_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_credit_card_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_cron_result.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      591 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_cron_result_row.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      569 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_currency.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_currency_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_currency_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_currency_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_currency_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_currency_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_data_destroy_object.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_export_file_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_insight_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_insight_group_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_insight_total.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_insight_total_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_insight_transfer.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_insight_transfer_entry.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_interest_period.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      606 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_internal_exception.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      610 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_liability_direction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_liability_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_link_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      591 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_link_type_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      587 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_link_type_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_link_type_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      591 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_link_type_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_link_type_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      553 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_meta.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_not_found.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_object_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_object_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_object_group_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_object_group_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_object_group_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_object_link.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_page_link.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_event.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      616 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_event_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      612 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_event_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      591 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      614 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_polymorphic_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      577 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_preference.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_preference_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_preference_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_preference_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_preference_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      577 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      618 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_repetition.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      639 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_repetition_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      635 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_repetition_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      643 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_repetition_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      622 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_transaction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      643 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_transaction_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      639 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_transaction_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      647 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_transaction_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_recurrence_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      553 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_action.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_action_keyword.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_action_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_action_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_group.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_group_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      591 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_group_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_group_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_group_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_group_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      611 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger_keyword.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger_type.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      607 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_rule_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      636 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_short_account_type_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_string_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      599 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_string_array_item.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_system_info.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_tag_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_tag_model.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      591 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_tag_model_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      595 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_tag_model_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      566 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_tag_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_tag_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      581 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_link.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_link_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_link_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_link_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_link_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_link_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      606 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_split.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_split_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      627 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_split_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      602 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      623 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_type_filter.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      631 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_type_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      606 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_transaction_update.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      597 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_unauthenticated.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      553 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_user.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      574 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_user_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      632 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_user_blocked_code_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      570 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_user_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      603 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_user_role_property.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      578 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_user_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_validation_error.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      565 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_attempt.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_attempt_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      611 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_attempt_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_attempt_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_delivery.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_message.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      615 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_message_array.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      611 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_message_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      619 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_message_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      582 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_read.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      598 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_response.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_single.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      586 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_store.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      594 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_trigger.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      590 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_models/test_webhook_update.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1995 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/__init__.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_about/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_about/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      823 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_about/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_about_user/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_about_user/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      845 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_about_user/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      821 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      829 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      867 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      829 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      838 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      866 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      886 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_piggy_banks/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      892 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_accounts_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.763772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      833 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      842 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      870 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      843 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      850 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id_download/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id_download/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id_download/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id_upload/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id_upload/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      883 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_attachments_id_upload/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      913 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_accounts/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      901 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_bills/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      909 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_budgets/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_categories/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_categories/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      921 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_categories/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      921 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies_with_code/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies_with_code/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1008 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies_with_code/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_object_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_object_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      931 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_object_groups/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      923 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_piggy_banks/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_piggy_banks_with_balance/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_piggy_banks_with_balance/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      996 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_piggy_banks_with_balance/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_recurring/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_recurring/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      930 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_recurring/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_rule_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_rule_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      923 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_rule_groups/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      901 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_rules/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      897 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_tags/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transaction_types/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transaction_types/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      949 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transaction_types/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      941 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions_with_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions_with_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     1039 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions_with_id/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_available_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_available_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      862 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_available_budgets/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_available_budgets_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_available_budgets_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      865 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_available_budgets_id/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      809 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      817 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.767772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      845 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      819 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      826 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      877 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      857 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_rules/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      886 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budget_limits/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budget_limits/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      849 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budget_limits/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      817 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      825 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      853 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      827 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      834 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      875 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      854 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      856 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      901 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      882 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      929 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_limits_limit_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      829 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      836 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      864 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      838 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      845 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      872 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      889 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_categories_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_chart_account_overview/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_chart_account_overview/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      896 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_chart_account_overview/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.771772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      864 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration_name/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration_name/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      882 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration_name/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      861 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_configuration_name/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_cron_cli_token/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_cron_cli_token/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      834 2023-08-06 11:18:04.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_cron_cli_token/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      829 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      836 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      870 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      844 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      851 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      884 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_accounts/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_available_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_available_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      918 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_available_budgets/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      872 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_bills/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_budget_limits/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_budget_limits/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      901 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_budget_limits/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_default/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_default/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      878 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_default/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_disable/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_disable/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      866 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_disable/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_enable/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_enable/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      869 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_enable/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_recurrences/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_recurrences/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      907 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_recurrences/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      872 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_rules/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      900 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_default/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_default/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      863 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_default/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_bulk_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_bulk_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      980 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_bulk_transactions/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_destroy/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_destroy/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      872 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_destroy/test_delete.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      871 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_accounts/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      855 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_bills/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_budgets/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_budgets/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      886 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_budgets/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.775772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_categories/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_categories/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      878 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_categories/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      877 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_piggy_banks/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_recurring/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_recurring/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      888 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_recurring/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      875 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_rules/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      855 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_tags/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      887 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_export_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_purge/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_purge/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      864 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_data_purge/test_delete.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_asset/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_asset/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      886 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_asset/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_bill/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_bill/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      874 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_bill/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_budget/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_budget/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      882 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_budget/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      890 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_category/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_expense/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_expense/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      894 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_expense/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_bill/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_bill/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      878 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_bill/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_budget/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_budget/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      886 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_budget/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      894 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_category/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      874 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_no_tag/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      870 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_tag/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_total/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_total/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      866 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_total/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_asset/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_asset/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      881 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_asset/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      885 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_category/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_no_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_no_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      889 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_no_category/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_no_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_no_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      869 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_no_tag/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_revenue/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_revenue/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      889 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_revenue/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      865 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_tag/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.779772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_total/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_total/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      861 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_income_total/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_asset/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_asset/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      884 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_asset/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      894 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_category/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_no_category/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_no_category/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      898 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_no_category/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_no_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_no_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      877 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_no_tag/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      874 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_tag/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_total/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_total/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      870 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_transfer_total/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      831 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      836 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      837 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      844 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      894 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_link_types_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      838 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      875 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      849 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      856 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id_bills/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id_bills/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      877 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id_bills/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      904 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_object_groups_id_piggy_banks/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      831 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      839 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      867 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      841 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      848 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id_events/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id_events/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      875 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_piggy_banks_id_events/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      839 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      856 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.783772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences_name/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences_name/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      852 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences_name/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      846 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_preferences_name/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      844 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      852 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      880 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      854 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      861 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      913 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_recurrences_id_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      831 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      840 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      867 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      841 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      848 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      863 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_rules/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_test/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_test/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      910 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_test/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_trigger/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_trigger/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      904 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rule_groups_id_trigger/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      809 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      817 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      846 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      819 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      826 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_test/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_test/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      888 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_test/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_trigger/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_trigger/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      882 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_trigger/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_search_accounts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_search_accounts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      841 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_search_accounts/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_search_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_search_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      857 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_search_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_summary_basic/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_summary_basic/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      853 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_summary_basic/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.787772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      805 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      813 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      845 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      818 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      825 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      857 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      874 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_tags_tag_transactions/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      903 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      943 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id_links/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id_links/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      937 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_journals_id_links/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      855 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      910 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      853 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      884 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transaction_links_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      849 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      845 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      873 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      847 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      934 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id_attachments/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id_attachments/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      878 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id_attachments/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id_piggy_bank_events/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id_piggy_bank_events/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      898 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_transactions_id_piggy_bank_events/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      809 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      817 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      845 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      819 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      843 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      821 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      829 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks/test_post.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      857 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      831 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id/test_get.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      838 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id/test_put.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.791772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      876 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      919 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      900 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      945 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts_attempt_id/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts_attempt_id/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      973 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts_attempt_id/test_delete.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      976 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_messages_message_id_attempts_attempt_id/test_get.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:19:01.795772 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_submit/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        0 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_submit/__init__.py
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      883 2023-08-06 11:18:05.000000 Firefly III API Client-2.0.5.0/test/test_paths/test_v1_webhooks_id_submit/test_post.py
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/__init__.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,270 +1,247 @@
 # coding: utf-8
 
 # flake8: noqa
 
-"""
-    Firefly III API Client
-
-    This is the Python client for Firefly III API
-
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-__version__ = "2.0.12.0"
-
-# import apis into sdk package
-from firefly_iii_client.api.about_api import AboutApi
-from firefly_iii_client.api.accounts_api import AccountsApi
-from firefly_iii_client.api.attachments_api import AttachmentsApi
-from firefly_iii_client.api.autocomplete_api import AutocompleteApi
-from firefly_iii_client.api.available_budgets_api import AvailableBudgetsApi
-from firefly_iii_client.api.bills_api import BillsApi
-from firefly_iii_client.api.budgets_api import BudgetsApi
-from firefly_iii_client.api.categories_api import CategoriesApi
-from firefly_iii_client.api.charts_api import ChartsApi
-from firefly_iii_client.api.configuration_api import ConfigurationApi
-from firefly_iii_client.api.currencies_api import CurrenciesApi
-from firefly_iii_client.api.data_api import DataApi
-from firefly_iii_client.api.insight_api import InsightApi
-from firefly_iii_client.api.links_api import LinksApi
-from firefly_iii_client.api.object_groups_api import ObjectGroupsApi
-from firefly_iii_client.api.piggy_banks_api import PiggyBanksApi
-from firefly_iii_client.api.preferences_api import PreferencesApi
-from firefly_iii_client.api.recurrences_api import RecurrencesApi
-from firefly_iii_client.api.rule_groups_api import RuleGroupsApi
-from firefly_iii_client.api.rules_api import RulesApi
-from firefly_iii_client.api.search_api import SearchApi
-from firefly_iii_client.api.summary_api import SummaryApi
-from firefly_iii_client.api.tags_api import TagsApi
-from firefly_iii_client.api.transactions_api import TransactionsApi
-from firefly_iii_client.api.users_api import UsersApi
-from firefly_iii_client.api.webhooks_api import WebhooksApi
-
-# import ApiClient
-from firefly_iii_client.api_response import ApiResponse
-from firefly_iii_client.api_client import ApiClient
-from firefly_iii_client.configuration import Configuration
-from firefly_iii_client.exceptions import OpenApiException
-from firefly_iii_client.exceptions import ApiTypeError
-from firefly_iii_client.exceptions import ApiValueError
-from firefly_iii_client.exceptions import ApiKeyError
-from firefly_iii_client.exceptions import ApiAttributeError
-from firefly_iii_client.exceptions import ApiException
-
-# import models into sdk package
-from firefly_iii_client.models.account import Account
-from firefly_iii_client.models.account_array import AccountArray
-from firefly_iii_client.models.account_read import AccountRead
-from firefly_iii_client.models.account_role_property import AccountRoleProperty
-from firefly_iii_client.models.account_search_field_filter import AccountSearchFieldFilter
-from firefly_iii_client.models.account_single import AccountSingle
-from firefly_iii_client.models.account_store import AccountStore
-from firefly_iii_client.models.account_type_filter import AccountTypeFilter
-from firefly_iii_client.models.account_type_property import AccountTypeProperty
-from firefly_iii_client.models.account_update import AccountUpdate
-from firefly_iii_client.models.attachable_type import AttachableType
-from firefly_iii_client.models.attachment import Attachment
-from firefly_iii_client.models.attachment_array import AttachmentArray
-from firefly_iii_client.models.attachment_read import AttachmentRead
-from firefly_iii_client.models.attachment_single import AttachmentSingle
-from firefly_iii_client.models.attachment_store import AttachmentStore
-from firefly_iii_client.models.attachment_update import AttachmentUpdate
-from firefly_iii_client.models.auto_budget_period import AutoBudgetPeriod
-from firefly_iii_client.models.auto_budget_type import AutoBudgetType
-from firefly_iii_client.models.autocomplete_account import AutocompleteAccount
-from firefly_iii_client.models.autocomplete_bill import AutocompleteBill
-from firefly_iii_client.models.autocomplete_budget import AutocompleteBudget
-from firefly_iii_client.models.autocomplete_category import AutocompleteCategory
-from firefly_iii_client.models.autocomplete_currency import AutocompleteCurrency
-from firefly_iii_client.models.autocomplete_currency_code import AutocompleteCurrencyCode
-from firefly_iii_client.models.autocomplete_object_group import AutocompleteObjectGroup
-from firefly_iii_client.models.autocomplete_piggy import AutocompletePiggy
-from firefly_iii_client.models.autocomplete_piggy_balance import AutocompletePiggyBalance
-from firefly_iii_client.models.autocomplete_recurrence import AutocompleteRecurrence
-from firefly_iii_client.models.autocomplete_rule import AutocompleteRule
-from firefly_iii_client.models.autocomplete_rule_group import AutocompleteRuleGroup
-from firefly_iii_client.models.autocomplete_tag import AutocompleteTag
-from firefly_iii_client.models.autocomplete_transaction import AutocompleteTransaction
-from firefly_iii_client.models.autocomplete_transaction_id import AutocompleteTransactionID
-from firefly_iii_client.models.autocomplete_transaction_type import AutocompleteTransactionType
-from firefly_iii_client.models.available_budget import AvailableBudget
-from firefly_iii_client.models.available_budget_array import AvailableBudgetArray
-from firefly_iii_client.models.available_budget_read import AvailableBudgetRead
-from firefly_iii_client.models.available_budget_single import AvailableBudgetSingle
-from firefly_iii_client.models.bad_request_response import BadRequestResponse
-from firefly_iii_client.models.basic_summary_entry import BasicSummaryEntry
-from firefly_iii_client.models.bill import Bill
-from firefly_iii_client.models.bill_array import BillArray
-from firefly_iii_client.models.bill_paid_dates_inner import BillPaidDatesInner
-from firefly_iii_client.models.bill_read import BillRead
-from firefly_iii_client.models.bill_repeat_frequency import BillRepeatFrequency
-from firefly_iii_client.models.bill_single import BillSingle
-from firefly_iii_client.models.bill_store import BillStore
-from firefly_iii_client.models.bill_update import BillUpdate
-from firefly_iii_client.models.budget import Budget
-from firefly_iii_client.models.budget_array import BudgetArray
-from firefly_iii_client.models.budget_limit import BudgetLimit
-from firefly_iii_client.models.budget_limit_array import BudgetLimitArray
-from firefly_iii_client.models.budget_limit_read import BudgetLimitRead
-from firefly_iii_client.models.budget_limit_single import BudgetLimitSingle
-from firefly_iii_client.models.budget_limit_store import BudgetLimitStore
-from firefly_iii_client.models.budget_read import BudgetRead
-from firefly_iii_client.models.budget_single import BudgetSingle
-from firefly_iii_client.models.budget_spent import BudgetSpent
-from firefly_iii_client.models.budget_store import BudgetStore
-from firefly_iii_client.models.budget_update import BudgetUpdate
-from firefly_iii_client.models.category import Category
-from firefly_iii_client.models.category_array import CategoryArray
-from firefly_iii_client.models.category_earned import CategoryEarned
-from firefly_iii_client.models.category_read import CategoryRead
-from firefly_iii_client.models.category_single import CategorySingle
-from firefly_iii_client.models.category_spent import CategorySpent
-from firefly_iii_client.models.category_update import CategoryUpdate
-from firefly_iii_client.models.chart_data_point import ChartDataPoint
-from firefly_iii_client.models.chart_data_set import ChartDataSet
-from firefly_iii_client.models.config_value_filter import ConfigValueFilter
-from firefly_iii_client.models.config_value_update_filter import ConfigValueUpdateFilter
-from firefly_iii_client.models.configuration import Configuration
-from firefly_iii_client.models.configuration_single import ConfigurationSingle
-from firefly_iii_client.models.configuration_update import ConfigurationUpdate
-from firefly_iii_client.models.credit_card_type_property import CreditCardTypeProperty
-from firefly_iii_client.models.cron_result import CronResult
-from firefly_iii_client.models.cron_result_row import CronResultRow
-from firefly_iii_client.models.currency import Currency
-from firefly_iii_client.models.currency_array import CurrencyArray
-from firefly_iii_client.models.currency_read import CurrencyRead
-from firefly_iii_client.models.currency_single import CurrencySingle
-from firefly_iii_client.models.currency_store import CurrencyStore
-from firefly_iii_client.models.currency_update import CurrencyUpdate
-from firefly_iii_client.models.data_destroy_object import DataDestroyObject
-from firefly_iii_client.models.export_file_filter import ExportFileFilter
-from firefly_iii_client.models.insight_group_entry import InsightGroupEntry
-from firefly_iii_client.models.insight_total_entry import InsightTotalEntry
-from firefly_iii_client.models.insight_transfer_entry import InsightTransferEntry
-from firefly_iii_client.models.interest_period_property import InterestPeriodProperty
-from firefly_iii_client.models.internal_exception_response import InternalExceptionResponse
-from firefly_iii_client.models.liability_direction_property import LiabilityDirectionProperty
-from firefly_iii_client.models.liability_type_property import LiabilityTypeProperty
-from firefly_iii_client.models.link_type import LinkType
-from firefly_iii_client.models.link_type_array import LinkTypeArray
-from firefly_iii_client.models.link_type_read import LinkTypeRead
-from firefly_iii_client.models.link_type_single import LinkTypeSingle
-from firefly_iii_client.models.link_type_update import LinkTypeUpdate
-from firefly_iii_client.models.meta import Meta
-from firefly_iii_client.models.meta_pagination import MetaPagination
-from firefly_iii_client.models.not_found_response import NotFoundResponse
-from firefly_iii_client.models.object_group import ObjectGroup
-from firefly_iii_client.models.object_group_array import ObjectGroupArray
-from firefly_iii_client.models.object_group_read import ObjectGroupRead
-from firefly_iii_client.models.object_group_single import ObjectGroupSingle
-from firefly_iii_client.models.object_group_update import ObjectGroupUpdate
-from firefly_iii_client.models.object_link import ObjectLink
-from firefly_iii_client.models.object_link0 import ObjectLink0
-from firefly_iii_client.models.page_link import PageLink
-from firefly_iii_client.models.piggy_bank import PiggyBank
-from firefly_iii_client.models.piggy_bank_array import PiggyBankArray
-from firefly_iii_client.models.piggy_bank_event import PiggyBankEvent
-from firefly_iii_client.models.piggy_bank_event_array import PiggyBankEventArray
-from firefly_iii_client.models.piggy_bank_event_read import PiggyBankEventRead
-from firefly_iii_client.models.piggy_bank_read import PiggyBankRead
-from firefly_iii_client.models.piggy_bank_single import PiggyBankSingle
-from firefly_iii_client.models.piggy_bank_store import PiggyBankStore
-from firefly_iii_client.models.piggy_bank_update import PiggyBankUpdate
-from firefly_iii_client.models.polymorphic_property import PolymorphicProperty
-from firefly_iii_client.models.preference import Preference
-from firefly_iii_client.models.preference_array import PreferenceArray
-from firefly_iii_client.models.preference_read import PreferenceRead
-from firefly_iii_client.models.preference_single import PreferenceSingle
-from firefly_iii_client.models.preference_update import PreferenceUpdate
-from firefly_iii_client.models.recurrence import Recurrence
-from firefly_iii_client.models.recurrence_array import RecurrenceArray
-from firefly_iii_client.models.recurrence_read import RecurrenceRead
-from firefly_iii_client.models.recurrence_repetition import RecurrenceRepetition
-from firefly_iii_client.models.recurrence_repetition_store import RecurrenceRepetitionStore
-from firefly_iii_client.models.recurrence_repetition_type import RecurrenceRepetitionType
-from firefly_iii_client.models.recurrence_repetition_update import RecurrenceRepetitionUpdate
-from firefly_iii_client.models.recurrence_single import RecurrenceSingle
-from firefly_iii_client.models.recurrence_store import RecurrenceStore
-from firefly_iii_client.models.recurrence_transaction import RecurrenceTransaction
-from firefly_iii_client.models.recurrence_transaction_store import RecurrenceTransactionStore
-from firefly_iii_client.models.recurrence_transaction_type import RecurrenceTransactionType
-from firefly_iii_client.models.recurrence_transaction_update import RecurrenceTransactionUpdate
-from firefly_iii_client.models.recurrence_update import RecurrenceUpdate
-from firefly_iii_client.models.rule import Rule
-from firefly_iii_client.models.rule_action import RuleAction
-from firefly_iii_client.models.rule_action_keyword import RuleActionKeyword
-from firefly_iii_client.models.rule_action_store import RuleActionStore
-from firefly_iii_client.models.rule_action_update import RuleActionUpdate
-from firefly_iii_client.models.rule_array import RuleArray
-from firefly_iii_client.models.rule_group import RuleGroup
-from firefly_iii_client.models.rule_group_array import RuleGroupArray
-from firefly_iii_client.models.rule_group_read import RuleGroupRead
-from firefly_iii_client.models.rule_group_single import RuleGroupSingle
-from firefly_iii_client.models.rule_group_store import RuleGroupStore
-from firefly_iii_client.models.rule_group_update import RuleGroupUpdate
-from firefly_iii_client.models.rule_read import RuleRead
-from firefly_iii_client.models.rule_single import RuleSingle
-from firefly_iii_client.models.rule_store import RuleStore
-from firefly_iii_client.models.rule_trigger import RuleTrigger
-from firefly_iii_client.models.rule_trigger_keyword import RuleTriggerKeyword
-from firefly_iii_client.models.rule_trigger_store import RuleTriggerStore
-from firefly_iii_client.models.rule_trigger_type import RuleTriggerType
-from firefly_iii_client.models.rule_trigger_update import RuleTriggerUpdate
-from firefly_iii_client.models.rule_update import RuleUpdate
-from firefly_iii_client.models.short_account_type_property import ShortAccountTypeProperty
-from firefly_iii_client.models.system_info import SystemInfo
-from firefly_iii_client.models.system_info_data import SystemInfoData
-from firefly_iii_client.models.tag_array import TagArray
-from firefly_iii_client.models.tag_model import TagModel
-from firefly_iii_client.models.tag_model_store import TagModelStore
-from firefly_iii_client.models.tag_model_update import TagModelUpdate
-from firefly_iii_client.models.tag_read import TagRead
-from firefly_iii_client.models.tag_single import TagSingle
-from firefly_iii_client.models.transaction import Transaction
-from firefly_iii_client.models.transaction_array import TransactionArray
-from firefly_iii_client.models.transaction_link import TransactionLink
-from firefly_iii_client.models.transaction_link_array import TransactionLinkArray
-from firefly_iii_client.models.transaction_link_read import TransactionLinkRead
-from firefly_iii_client.models.transaction_link_single import TransactionLinkSingle
-from firefly_iii_client.models.transaction_link_store import TransactionLinkStore
-from firefly_iii_client.models.transaction_link_update import TransactionLinkUpdate
-from firefly_iii_client.models.transaction_read import TransactionRead
-from firefly_iii_client.models.transaction_single import TransactionSingle
-from firefly_iii_client.models.transaction_split import TransactionSplit
-from firefly_iii_client.models.transaction_split_store import TransactionSplitStore
-from firefly_iii_client.models.transaction_split_update import TransactionSplitUpdate
-from firefly_iii_client.models.transaction_store import TransactionStore
-from firefly_iii_client.models.transaction_type_filter import TransactionTypeFilter
-from firefly_iii_client.models.transaction_type_property import TransactionTypeProperty
-from firefly_iii_client.models.transaction_update import TransactionUpdate
-from firefly_iii_client.models.unauthenticated_response import UnauthenticatedResponse
-from firefly_iii_client.models.user import User
-from firefly_iii_client.models.user_array import UserArray
-from firefly_iii_client.models.user_blocked_code_property import UserBlockedCodeProperty
-from firefly_iii_client.models.user_read import UserRead
-from firefly_iii_client.models.user_role_property import UserRoleProperty
-from firefly_iii_client.models.user_single import UserSingle
-from firefly_iii_client.models.validation_error_response import ValidationErrorResponse
-from firefly_iii_client.models.validation_error_response_errors import ValidationErrorResponseErrors
-from firefly_iii_client.models.webhook import Webhook
-from firefly_iii_client.models.webhook_array import WebhookArray
-from firefly_iii_client.models.webhook_attempt import WebhookAttempt
-from firefly_iii_client.models.webhook_attempt_array import WebhookAttemptArray
-from firefly_iii_client.models.webhook_attempt_read import WebhookAttemptRead
-from firefly_iii_client.models.webhook_attempt_single import WebhookAttemptSingle
-from firefly_iii_client.models.webhook_delivery import WebhookDelivery
-from firefly_iii_client.models.webhook_message import WebhookMessage
-from firefly_iii_client.models.webhook_message_array import WebhookMessageArray
-from firefly_iii_client.models.webhook_message_read import WebhookMessageRead
-from firefly_iii_client.models.webhook_message_single import WebhookMessageSingle
-from firefly_iii_client.models.webhook_read import WebhookRead
-from firefly_iii_client.models.webhook_response import WebhookResponse
-from firefly_iii_client.models.webhook_single import WebhookSingle
-from firefly_iii_client.models.webhook_store import WebhookStore
-from firefly_iii_client.models.webhook_trigger import WebhookTrigger
-from firefly_iii_client.models.webhook_update import WebhookUpdate
+# import all models into this package
+# if you have many models here with many references from one model to another this may
+# raise a RecursionError
+# to avoid this, import only the models that you directly need like:
+# from firefly_iii_client.model.pet import Pet
+# or import this package, but before doing it, use:
+# import sys
+# sys.setrecursionlimit(n)
+
+from firefly_iii_client.model.account import Account
+from firefly_iii_client.model.account_array import AccountArray
+from firefly_iii_client.model.account_read import AccountRead
+from firefly_iii_client.model.account_role_property import AccountRoleProperty
+from firefly_iii_client.model.account_search_field_filter import AccountSearchFieldFilter
+from firefly_iii_client.model.account_single import AccountSingle
+from firefly_iii_client.model.account_store import AccountStore
+from firefly_iii_client.model.account_type_filter import AccountTypeFilter
+from firefly_iii_client.model.account_type_property import AccountTypeProperty
+from firefly_iii_client.model.account_update import AccountUpdate
+from firefly_iii_client.model.attachable_type import AttachableType
+from firefly_iii_client.model.attachment import Attachment
+from firefly_iii_client.model.attachment_array import AttachmentArray
+from firefly_iii_client.model.attachment_read import AttachmentRead
+from firefly_iii_client.model.attachment_single import AttachmentSingle
+from firefly_iii_client.model.attachment_store import AttachmentStore
+from firefly_iii_client.model.attachment_update import AttachmentUpdate
+from firefly_iii_client.model.auto_budget_period import AutoBudgetPeriod
+from firefly_iii_client.model.auto_budget_type import AutoBudgetType
+from firefly_iii_client.model.autocomplete_account import AutocompleteAccount
+from firefly_iii_client.model.autocomplete_account_array import AutocompleteAccountArray
+from firefly_iii_client.model.autocomplete_bill import AutocompleteBill
+from firefly_iii_client.model.autocomplete_bill_array import AutocompleteBillArray
+from firefly_iii_client.model.autocomplete_budget import AutocompleteBudget
+from firefly_iii_client.model.autocomplete_budget_array import AutocompleteBudgetArray
+from firefly_iii_client.model.autocomplete_category import AutocompleteCategory
+from firefly_iii_client.model.autocomplete_category_array import AutocompleteCategoryArray
+from firefly_iii_client.model.autocomplete_currency import AutocompleteCurrency
+from firefly_iii_client.model.autocomplete_currency_array import AutocompleteCurrencyArray
+from firefly_iii_client.model.autocomplete_currency_code import AutocompleteCurrencyCode
+from firefly_iii_client.model.autocomplete_currency_code_array import AutocompleteCurrencyCodeArray
+from firefly_iii_client.model.autocomplete_object_group import AutocompleteObjectGroup
+from firefly_iii_client.model.autocomplete_object_group_array import AutocompleteObjectGroupArray
+from firefly_iii_client.model.autocomplete_piggy import AutocompletePiggy
+from firefly_iii_client.model.autocomplete_piggy_array import AutocompletePiggyArray
+from firefly_iii_client.model.autocomplete_piggy_balance import AutocompletePiggyBalance
+from firefly_iii_client.model.autocomplete_piggy_balance_array import AutocompletePiggyBalanceArray
+from firefly_iii_client.model.autocomplete_recurrence import AutocompleteRecurrence
+from firefly_iii_client.model.autocomplete_recurrence_array import AutocompleteRecurrenceArray
+from firefly_iii_client.model.autocomplete_rule import AutocompleteRule
+from firefly_iii_client.model.autocomplete_rule_array import AutocompleteRuleArray
+from firefly_iii_client.model.autocomplete_rule_group import AutocompleteRuleGroup
+from firefly_iii_client.model.autocomplete_rule_group_array import AutocompleteRuleGroupArray
+from firefly_iii_client.model.autocomplete_tag import AutocompleteTag
+from firefly_iii_client.model.autocomplete_tag_array import AutocompleteTagArray
+from firefly_iii_client.model.autocomplete_transaction import AutocompleteTransaction
+from firefly_iii_client.model.autocomplete_transaction_array import AutocompleteTransactionArray
+from firefly_iii_client.model.autocomplete_transaction_id import AutocompleteTransactionID
+from firefly_iii_client.model.autocomplete_transaction_id_array import AutocompleteTransactionIDArray
+from firefly_iii_client.model.autocomplete_transaction_type import AutocompleteTransactionType
+from firefly_iii_client.model.autocomplete_transaction_type_array import AutocompleteTransactionTypeArray
+from firefly_iii_client.model.available_budget import AvailableBudget
+from firefly_iii_client.model.available_budget_array import AvailableBudgetArray
+from firefly_iii_client.model.available_budget_read import AvailableBudgetRead
+from firefly_iii_client.model.available_budget_single import AvailableBudgetSingle
+from firefly_iii_client.model.available_budget_store import AvailableBudgetStore
+from firefly_iii_client.model.available_budget_update import AvailableBudgetUpdate
+from firefly_iii_client.model.bad_request import BadRequest
+from firefly_iii_client.model.basic_summary import BasicSummary
+from firefly_iii_client.model.basic_summary_entry import BasicSummaryEntry
+from firefly_iii_client.model.bill import Bill
+from firefly_iii_client.model.bill_array import BillArray
+from firefly_iii_client.model.bill_read import BillRead
+from firefly_iii_client.model.bill_repeat_frequency import BillRepeatFrequency
+from firefly_iii_client.model.bill_single import BillSingle
+from firefly_iii_client.model.bill_store import BillStore
+from firefly_iii_client.model.bill_update import BillUpdate
+from firefly_iii_client.model.budget import Budget
+from firefly_iii_client.model.budget_array import BudgetArray
+from firefly_iii_client.model.budget_limit import BudgetLimit
+from firefly_iii_client.model.budget_limit_array import BudgetLimitArray
+from firefly_iii_client.model.budget_limit_read import BudgetLimitRead
+from firefly_iii_client.model.budget_limit_single import BudgetLimitSingle
+from firefly_iii_client.model.budget_limit_store import BudgetLimitStore
+from firefly_iii_client.model.budget_read import BudgetRead
+from firefly_iii_client.model.budget_single import BudgetSingle
+from firefly_iii_client.model.budget_spent import BudgetSpent
+from firefly_iii_client.model.budget_store import BudgetStore
+from firefly_iii_client.model.budget_update import BudgetUpdate
+from firefly_iii_client.model.category import Category
+from firefly_iii_client.model.category_array import CategoryArray
+from firefly_iii_client.model.category_earned import CategoryEarned
+from firefly_iii_client.model.category_read import CategoryRead
+from firefly_iii_client.model.category_single import CategorySingle
+from firefly_iii_client.model.category_spent import CategorySpent
+from firefly_iii_client.model.category_store import CategoryStore
+from firefly_iii_client.model.category_update import CategoryUpdate
+from firefly_iii_client.model.chart_data_point import ChartDataPoint
+from firefly_iii_client.model.chart_data_set import ChartDataSet
+from firefly_iii_client.model.chart_line import ChartLine
+from firefly_iii_client.model.config_value_filter import ConfigValueFilter
+from firefly_iii_client.model.config_value_update_filter import ConfigValueUpdateFilter
+from firefly_iii_client.model.configuration import Configuration
+from firefly_iii_client.model.configuration_array import ConfigurationArray
+from firefly_iii_client.model.configuration_single import ConfigurationSingle
+from firefly_iii_client.model.configuration_update import ConfigurationUpdate
+from firefly_iii_client.model.credit_card_type import CreditCardType
+from firefly_iii_client.model.cron_result import CronResult
+from firefly_iii_client.model.cron_result_row import CronResultRow
+from firefly_iii_client.model.currency import Currency
+from firefly_iii_client.model.currency_array import CurrencyArray
+from firefly_iii_client.model.currency_read import CurrencyRead
+from firefly_iii_client.model.currency_single import CurrencySingle
+from firefly_iii_client.model.currency_store import CurrencyStore
+from firefly_iii_client.model.currency_update import CurrencyUpdate
+from firefly_iii_client.model.data_destroy_object import DataDestroyObject
+from firefly_iii_client.model.export_file_filter import ExportFileFilter
+from firefly_iii_client.model.insight_group import InsightGroup
+from firefly_iii_client.model.insight_group_entry import InsightGroupEntry
+from firefly_iii_client.model.insight_total import InsightTotal
+from firefly_iii_client.model.insight_total_entry import InsightTotalEntry
+from firefly_iii_client.model.insight_transfer import InsightTransfer
+from firefly_iii_client.model.insight_transfer_entry import InsightTransferEntry
+from firefly_iii_client.model.interest_period import InterestPeriod
+from firefly_iii_client.model.internal_exception import InternalException
+from firefly_iii_client.model.liability_direction import LiabilityDirection
+from firefly_iii_client.model.liability_type import LiabilityType
+from firefly_iii_client.model.link_type import LinkType
+from firefly_iii_client.model.link_type_array import LinkTypeArray
+from firefly_iii_client.model.link_type_read import LinkTypeRead
+from firefly_iii_client.model.link_type_single import LinkTypeSingle
+from firefly_iii_client.model.link_type_store import LinkTypeStore
+from firefly_iii_client.model.link_type_update import LinkTypeUpdate
+from firefly_iii_client.model.meta import Meta
+from firefly_iii_client.model.not_found import NotFound
+from firefly_iii_client.model.object_group import ObjectGroup
+from firefly_iii_client.model.object_group_array import ObjectGroupArray
+from firefly_iii_client.model.object_group_read import ObjectGroupRead
+from firefly_iii_client.model.object_group_single import ObjectGroupSingle
+from firefly_iii_client.model.object_group_update import ObjectGroupUpdate
+from firefly_iii_client.model.object_link import ObjectLink
+from firefly_iii_client.model.page_link import PageLink
+from firefly_iii_client.model.piggy_bank import PiggyBank
+from firefly_iii_client.model.piggy_bank_array import PiggyBankArray
+from firefly_iii_client.model.piggy_bank_event import PiggyBankEvent
+from firefly_iii_client.model.piggy_bank_event_array import PiggyBankEventArray
+from firefly_iii_client.model.piggy_bank_event_read import PiggyBankEventRead
+from firefly_iii_client.model.piggy_bank_read import PiggyBankRead
+from firefly_iii_client.model.piggy_bank_single import PiggyBankSingle
+from firefly_iii_client.model.piggy_bank_store import PiggyBankStore
+from firefly_iii_client.model.piggy_bank_update import PiggyBankUpdate
+from firefly_iii_client.model.polymorphic_property import PolymorphicProperty
+from firefly_iii_client.model.preference import Preference
+from firefly_iii_client.model.preference_array import PreferenceArray
+from firefly_iii_client.model.preference_read import PreferenceRead
+from firefly_iii_client.model.preference_single import PreferenceSingle
+from firefly_iii_client.model.preference_update import PreferenceUpdate
+from firefly_iii_client.model.recurrence import Recurrence
+from firefly_iii_client.model.recurrence_array import RecurrenceArray
+from firefly_iii_client.model.recurrence_read import RecurrenceRead
+from firefly_iii_client.model.recurrence_repetition import RecurrenceRepetition
+from firefly_iii_client.model.recurrence_repetition_store import RecurrenceRepetitionStore
+from firefly_iii_client.model.recurrence_repetition_type import RecurrenceRepetitionType
+from firefly_iii_client.model.recurrence_repetition_update import RecurrenceRepetitionUpdate
+from firefly_iii_client.model.recurrence_single import RecurrenceSingle
+from firefly_iii_client.model.recurrence_store import RecurrenceStore
+from firefly_iii_client.model.recurrence_transaction import RecurrenceTransaction
+from firefly_iii_client.model.recurrence_transaction_store import RecurrenceTransactionStore
+from firefly_iii_client.model.recurrence_transaction_type import RecurrenceTransactionType
+from firefly_iii_client.model.recurrence_transaction_update import RecurrenceTransactionUpdate
+from firefly_iii_client.model.recurrence_update import RecurrenceUpdate
+from firefly_iii_client.model.rule import Rule
+from firefly_iii_client.model.rule_action import RuleAction
+from firefly_iii_client.model.rule_action_keyword import RuleActionKeyword
+from firefly_iii_client.model.rule_action_store import RuleActionStore
+from firefly_iii_client.model.rule_action_update import RuleActionUpdate
+from firefly_iii_client.model.rule_array import RuleArray
+from firefly_iii_client.model.rule_group import RuleGroup
+from firefly_iii_client.model.rule_group_array import RuleGroupArray
+from firefly_iii_client.model.rule_group_read import RuleGroupRead
+from firefly_iii_client.model.rule_group_single import RuleGroupSingle
+from firefly_iii_client.model.rule_group_store import RuleGroupStore
+from firefly_iii_client.model.rule_group_update import RuleGroupUpdate
+from firefly_iii_client.model.rule_read import RuleRead
+from firefly_iii_client.model.rule_single import RuleSingle
+from firefly_iii_client.model.rule_store import RuleStore
+from firefly_iii_client.model.rule_trigger import RuleTrigger
+from firefly_iii_client.model.rule_trigger_keyword import RuleTriggerKeyword
+from firefly_iii_client.model.rule_trigger_store import RuleTriggerStore
+from firefly_iii_client.model.rule_trigger_type import RuleTriggerType
+from firefly_iii_client.model.rule_trigger_update import RuleTriggerUpdate
+from firefly_iii_client.model.rule_update import RuleUpdate
+from firefly_iii_client.model.short_account_type_property import ShortAccountTypeProperty
+from firefly_iii_client.model.string_array import StringArray
+from firefly_iii_client.model.string_array_item import StringArrayItem
+from firefly_iii_client.model.system_info import SystemInfo
+from firefly_iii_client.model.tag_array import TagArray
+from firefly_iii_client.model.tag_model import TagModel
+from firefly_iii_client.model.tag_model_store import TagModelStore
+from firefly_iii_client.model.tag_model_update import TagModelUpdate
+from firefly_iii_client.model.tag_read import TagRead
+from firefly_iii_client.model.tag_single import TagSingle
+from firefly_iii_client.model.transaction import Transaction
+from firefly_iii_client.model.transaction_array import TransactionArray
+from firefly_iii_client.model.transaction_link import TransactionLink
+from firefly_iii_client.model.transaction_link_array import TransactionLinkArray
+from firefly_iii_client.model.transaction_link_read import TransactionLinkRead
+from firefly_iii_client.model.transaction_link_single import TransactionLinkSingle
+from firefly_iii_client.model.transaction_link_store import TransactionLinkStore
+from firefly_iii_client.model.transaction_link_update import TransactionLinkUpdate
+from firefly_iii_client.model.transaction_read import TransactionRead
+from firefly_iii_client.model.transaction_single import TransactionSingle
+from firefly_iii_client.model.transaction_split import TransactionSplit
+from firefly_iii_client.model.transaction_split_store import TransactionSplitStore
+from firefly_iii_client.model.transaction_split_update import TransactionSplitUpdate
+from firefly_iii_client.model.transaction_store import TransactionStore
+from firefly_iii_client.model.transaction_type_filter import TransactionTypeFilter
+from firefly_iii_client.model.transaction_type_property import TransactionTypeProperty
+from firefly_iii_client.model.transaction_update import TransactionUpdate
+from firefly_iii_client.model.unauthenticated import Unauthenticated
+from firefly_iii_client.model.user import User
+from firefly_iii_client.model.user_array import UserArray
+from firefly_iii_client.model.user_blocked_code_property import UserBlockedCodeProperty
+from firefly_iii_client.model.user_read import UserRead
+from firefly_iii_client.model.user_role_property import UserRoleProperty
+from firefly_iii_client.model.user_single import UserSingle
+from firefly_iii_client.model.validation_error import ValidationError
+from firefly_iii_client.model.webhook import Webhook
+from firefly_iii_client.model.webhook_array import WebhookArray
+from firefly_iii_client.model.webhook_attempt import WebhookAttempt
+from firefly_iii_client.model.webhook_attempt_array import WebhookAttemptArray
+from firefly_iii_client.model.webhook_attempt_read import WebhookAttemptRead
+from firefly_iii_client.model.webhook_attempt_single import WebhookAttemptSingle
+from firefly_iii_client.model.webhook_delivery import WebhookDelivery
+from firefly_iii_client.model.webhook_message import WebhookMessage
+from firefly_iii_client.model.webhook_message_array import WebhookMessageArray
+from firefly_iii_client.model.webhook_message_read import WebhookMessageRead
+from firefly_iii_client.model.webhook_message_single import WebhookMessageSingle
+from firefly_iii_client.model.webhook_read import WebhookRead
+from firefly_iii_client.model.webhook_response import WebhookResponse
+from firefly_iii_client.model.webhook_single import WebhookSingle
+from firefly_iii_client.model.webhook_store import WebhookStore
+from firefly_iii_client.model.webhook_trigger import WebhookTrigger
+from firefly_iii_client.model.webhook_update import WebhookUpdate
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/configuration.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,102 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import copy
 import logging
-from logging import FileHandler
 import multiprocessing
 import sys
-from typing import Optional
 import urllib3
 
-import http.client as httplib
+from http import client as http_client
+from firefly_iii_client.exceptions import ApiValueError
+
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems'
+    'minLength', 'pattern', 'maxItems', 'minItems',
+    'uniqueItems', 'maxProperties', 'minProperties',
 }
 
-class Configuration:
-    """This class contains various settings of the API client.
+class Configuration(object):
+    """NOTE: This class is auto generated by OpenAPI Generator
 
-    :param host: Base url.
+    Ref: https://openapi-generator.tech
+    Do not edit the class manually.
+
+    :param host: Base url
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication.
-    :param password: Password for HTTP basic authentication.
-    :param access_token: Access token.
+    :param username: Username for HTTP basic authentication
+    :param password: Password for HTTP basic authentication
+    :param discard_unknown_keys: Boolean value indicating whether to discard
+      unknown properties. A server may send a response that includes additional
+      properties that are not known by the client in the following scenarios:
+      1. The OpenAPI document is incomplete, i.e. it does not match the server
+         implementation.
+      2. The client was generated using an older version of the OpenAPI document
+         and the server has been upgraded since then.
+      If a schema in the OpenAPI document defines the additionalProperties attribute,
+      then all undeclared properties received by the server are injected into the
+      additional properties map. In that case, there are undeclared properties, and
+      nothing to discard.
+    :param disabled_client_side_validations (string): Comma-separated list of
+      JSON schema validation keywords to disable JSON schema structural validation
+      rules. The following keywords may be specified: multipleOf, maximum,
+      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+      maxItems, minItems.
+      By default, the validation is performed for data generated locally by the client
+      and data received from the server, independent of any validation performed by
+      the server side. If the input data does not satisfy the JSON schema validation
+      rules specified in the OpenAPI document, an exception is raised.
+      If disabled_client_side_validations is set, structural validation is
+      disabled. This can be useful to troubleshoot data validation problem, such as
+      when the OpenAPI document validation rules do not match the actual API data
+      received by the server.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum
-      values before.
-    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format.
+      The validation of enums is performed for variables with defined enum values before.
 
     :Example:
     """
 
     _default = None
 
-    def __init__(self, host=None,
-                 api_key=None, api_key_prefix=None,
-                 username=None, password=None,
-                 access_token=None,
-                 server_index=None, server_variables=None,
-                 server_operation_index=None, server_operation_variables=None,
-                 ssl_ca_cert=None,
-                 ) -> None:
+    def __init__(
+        self,
+        host=None,
+        discard_unknown_keys=False,
+        disabled_client_side_validations="",
+        server_index=None,
+        server_variables=None,
+        server_operation_index=None,
+        server_operation_variables=None,
+        access_token=None,
+    ):
         """Constructor
         """
         self._base_path = "https://demo.firefly-iii.org/api" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -82,63 +106,45 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.api_key = {}
-        if api_key:
-            self.api_key = api_key
-        """dict to store API key(s)
-        """
-        self.api_key_prefix = {}
-        if api_key_prefix:
-            self.api_key_prefix = api_key_prefix
-        """dict to store API prefix (e.g. Bearer)
-        """
-        self.refresh_api_key_hook = None
-        """function hook to refresh API key if expired
-        """
-        self.username = username
-        """Username for HTTP basic authentication
-        """
-        self.password = password
-        """Password for HTTP basic authentication
-        """
-        self.access_token = access_token
-        """Access token
+        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = None
+        """access token for OAuth/Bearer
         """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("firefly_iii_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
-        self.logger_file_handler: Optional[FileHandler] = None
+        self.logger_file_handler = None
         """Log file handler
         """
         self.logger_file = None
         """Debug file location
         """
         self.debug = False
         """Debug switch
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = ssl_ca_cert
+        self.ssl_ca_cert = None
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -155,40 +161,31 @@
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
-        self.proxy: Optional[str] = None
+        self.proxy = None
         """Proxy URL
         """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
+        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
-        """Options to pass down to the underlying urllib3 socket
-        """
-
-        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
-        """datetime format
-        """
-
-        self.date_format = "%Y-%m-%d"
-        """date format
-        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -198,49 +195,46 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError(
+                        "Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = default
+        cls._default = copy.deepcopy(default)
 
     @classmethod
     def get_default_copy(cls):
-        """Deprecated. Please use `get_default` instead.
-
-        Deprecated. Please use `get_default` instead.
-
-        :return: The configuration object.
-        """
-        return cls.get_default()
-
-    @classmethod
-    def get_default(cls):
-        """Return the default configuration.
+        """Return new instance of configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration.
+        configuration passed by the set_default method.
 
         :return: The configuration object.
         """
-        if cls._default is None:
-            cls._default = Configuration()
-        return cls._default
+        if cls._default is not None:
+            return copy.deepcopy(cls._default)
+        return Configuration()
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -286,23 +280,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -381,16 +375,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.12\n"\
-               "SDK Package Version: 2.0.12.0".\
+               "Version of the API: 2.0.5\n"\
+               "SDK Package Version: 2.0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/exceptions.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+import dataclasses
+import typing
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from urllib3._collections import HTTPHeaderDict
 
-from typing import Any, Optional
-from typing_extensions import Self
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
     def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None) -> None:
+                 key_type=None):
         """ Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
@@ -45,15 +45,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiTypeError, self).__init__(full_msg)
 
 
 class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None) -> None:
+    def __init__(self, msg, path_to_item=None):
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list) the path to the exception in the
                 received_data dict. None if unset
@@ -63,15 +63,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
 class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None) -> None:
+    def __init__(self, msg, path_to_item=None):
         """
         Raised when an attribute reference or assignment fails.
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -82,15 +82,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiAttributeError, self).__init__(full_msg)
 
 
 class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None) -> None:
+    def __init__(self, msg, path_to_item=None):
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (None/list) the path to the exception in the
                 received_data dict
@@ -98,101 +98,49 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-class ApiException(OpenApiException):
+T = typing.TypeVar("T")
+
 
-    def __init__(
-        self, 
-        status=None, 
-        reason=None, 
-        http_resp=None,
-        *,
-        body: Optional[str] = None,
-        data: Optional[Any] = None,
-    ) -> None:
-        self.status = status
-        self.reason = reason
-        self.body = body
-        self.data = data
-        self.headers = None
-
-        if http_resp:
-            if self.status is None:
-                self.status = http_resp.status
-            if self.reason is None:
-                self.reason = http_resp.reason
-            if self.body is None:
-                try:
-                    self.body = http_resp.data.decode('utf-8')
-                except Exception:
-                    pass
-            self.headers = http_resp.getheaders()
-
-    @classmethod
-    def from_response(
-        cls, 
-        *, 
-        http_resp, 
-        body: Optional[str], 
-        data: Optional[Any],
-    ) -> Self:
-        if http_resp.status == 400:
-            raise BadRequestException(http_resp=http_resp, body=body, data=data)
-
-        if http_resp.status == 401:
-            raise UnauthorizedException(http_resp=http_resp, body=body, data=data)
-
-        if http_resp.status == 403:
-            raise ForbiddenException(http_resp=http_resp, body=body, data=data)
-
-        if http_resp.status == 404:
-            raise NotFoundException(http_resp=http_resp, body=body, data=data)
-
-        if 500 <= http_resp.status <= 599:
-            raise ServiceException(http_resp=http_resp, body=body, data=data)
-        raise ApiException(http_resp=http_resp, body=body, data=data)
+@dataclasses.dataclass
+class ApiException(OpenApiException, typing.Generic[T]):
+    status: int
+    reason: str
+    api_response: typing.Optional[T] = None
+
+    @property
+    def body(self) -> typing.Union[str, bytes, None]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.data
+
+    @property
+    def headers(self) -> typing.Optional[HTTPHeaderDict]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.getheaders()
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
                 self.headers)
 
-        if self.data or self.body:
-            error_message += "HTTP response body: {0}\n".format(self.data or self.body)
+        if self.body:
+            error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
-class BadRequestException(ApiException):
-    pass
-
-
-class NotFoundException(ApiException):
-    pass
-
-
-class UnauthorizedException(ApiException):
-    pass
-
-
-class ForbiddenException(ApiException):
-    pass
-
-
-class ServiceException(ApiException):
-    pass
-
-
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/account_search_field_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_insight_transfer_entry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import firefly_iii_client
+from firefly_iii_client.model.insight_transfer_entry import InsightTransferEntry
+from firefly_iii_client import configuration
 
 
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
-
-
-class AccountSearchFieldFilter(str, Enum):
-    """
-    AccountSearchFieldFilter
-    """
-
-    """
-    allowed enum values
-    """
-    ALL = 'all'
-    IBAN = 'iban'
-    NAME = 'name'
-    NUMBER = 'number'
-    ID = 'id'
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AccountSearchFieldFilter from a JSON string"""
-        return cls(json.loads(json_str))
+class TestInsightTransferEntry(unittest.TestCase):
+    """InsightTransferEntry unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/auto_budget_type.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_autocomplete_transaction_type_array.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import firefly_iii_client
+from firefly_iii_client.model.autocomplete_transaction_type_array import AutocompleteTransactionTypeArray
+from firefly_iii_client import configuration
 
 
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
-
-
-class AutoBudgetType(str, Enum):
-    """
-    The type of auto-budget that Firefly III must create.
-    """
-
-    """
-    allowed enum values
-    """
-    RESET = 'reset'
-    ROLLOVER = 'rollover'
-    NONE = 'none'
-    NULL = 'null'
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AutoBudgetType from a JSON string"""
-        return cls(json.loads(json_str))
+class TestAutocompleteTransactionTypeArray(unittest.TestCase):
+    """AutocompleteTransactionTypeArray unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/config_value_update_filter.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_currencies_with_code/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
 
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import unittest
+from unittest.mock import patch
 
+import urllib3
 
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
+import firefly_iii_client
+from firefly_iii_client.paths.v1_autocomplete_currencies_with_code import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class ConfigValueUpdateFilter(str, Enum):
-    """
-    ConfigValueUpdateFilter
-    """
 
+class TestV1AutocompleteCurrenciesWithCode(ApiTestMixin, unittest.TestCase):
     """
-    allowed enum values
+    V1AutocompleteCurrenciesWithCode unit test stubs
+        Returns all currencies of the user returned in a basic auto-complete array. This endpoint is DEPRECATED and I suggest you DO NOT use it.  # noqa: E501
     """
-    CONFIGURATION_DOT_IS_DEMO_SITE = 'configuration.is_demo_site'
-    CONFIGURATION_DOT_PERMISSION_UPDATE_CHECK = 'configuration.permission_update_check'
-    CONFIGURATION_DOT_LAST_UPDATE_CHECK = 'configuration.last_update_check'
-    CONFIGURATION_DOT_SINGLE_USER_MODE = 'configuration.single_user_mode'
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ConfigValueUpdateFilter from a JSON string"""
-        return cls(json.loads(json_str))
+    _configuration = configuration.Configuration()
+
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    response_status = 200
+
+
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/credit_card_type_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_not_found.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
+    Generated by: https://openapi-generator.tech
+"""
 
+import unittest
 
-class CreditCardTypeProperty(str, Enum):
-    """
-    Mandatory when the account_role is ccAsset. Can only be monthlyFull or null.
-    """
+import firefly_iii_client
+from firefly_iii_client.model.not_found import NotFound
+from firefly_iii_client import configuration
 
-    """
-    allowed enum values
-    """
-    MONTHLYFULL = 'monthlyFull'
-    NULL = 'null'
 
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CreditCardTypeProperty from a JSON string"""
-        return cls(json.loads(json_str))
+class TestNotFound(unittest.TestCase):
+    """NotFound unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/export_file_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_piggy_bank_update.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
+    Generated by: https://openapi-generator.tech
+"""
 
+import unittest
 
-class ExportFileFilter(str, Enum):
-    """
-    ExportFileFilter
-    """
+import firefly_iii_client
+from firefly_iii_client.model.piggy_bank_update import PiggyBankUpdate
+from firefly_iii_client import configuration
 
-    """
-    allowed enum values
-    """
-    CSV = 'csv'
 
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ExportFileFilter from a JSON string"""
-        return cls(json.loads(json_str))
+class TestPiggyBankUpdate(unittest.TestCase):
+    """PiggyBankUpdate unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/liability_type_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_attachment_single.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import firefly_iii_client
+from firefly_iii_client.model.attachment_single import AttachmentSingle
+from firefly_iii_client import configuration
 
 
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
-
-
-class LiabilityTypeProperty(str, Enum):
-    """
-    Mandatory when type is liability. Specifies the exact type.
-    """
-
-    """
-    allowed enum values
-    """
-    LOAN = 'loan'
-    DEBT = 'debt'
-    MORTGAGE = 'mortgage'
-    NULL = 'null'
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of LiabilityTypeProperty from a JSON string"""
-        return cls(json.loads(json_str))
+class TestAttachmentSingle(unittest.TestCase):
+    """AttachmentSingle unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/recurrence_array.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/model/configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,117 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
 
+import frozendict  # noqa: F401
+
+from firefly_iii_client import schemas  # noqa: F401
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
 
-from pydantic import BaseModel, ConfigDict
-from typing import Any, ClassVar, Dict, List
-from firefly_iii_client.models.meta import Meta
-from firefly_iii_client.models.page_link import PageLink
-from firefly_iii_client.models.recurrence_read import RecurrenceRead
-from typing import Optional, Set
-from typing_extensions import Self
+class Configuration(
+    schemas.DictSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
 
-class RecurrenceArray(BaseModel):
+    Do not edit the class manually.
     """
-    RecurrenceArray
-    """ # noqa: E501
-    data: List[RecurrenceRead]
-    links: PageLink
-    meta: Meta
-    __properties: ClassVar[List[str]] = ["data", "links", "meta"]
-
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecurrenceArray from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
-
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
-        # override the default output from pydantic by calling `to_dict()` of links
-        if self.links:
-            _dict['links'] = self.links.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of meta
-        if self.meta:
-            _dict['meta'] = self.meta.to_dict()
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecurrenceArray from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "data": [RecurrenceRead.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
-            "links": PageLink.from_dict(obj["links"]) if obj.get("links") is not None else None,
-            "meta": Meta.from_dict(obj["meta"]) if obj.get("meta") is not None else None
-        })
-        return _obj
 
 
+    class MetaOapg:
+        required = {
+            "editable",
+            "title",
+            "value",
+        }
+        
+        class properties:
+            editable = schemas.BoolSchema
+        
+            @staticmethod
+            def title() -> typing.Type['ConfigValueFilter']:
+                return ConfigValueFilter
+        
+            @staticmethod
+            def value() -> typing.Type['PolymorphicProperty']:
+                return PolymorphicProperty
+            __annotations__ = {
+                "editable": editable,
+                "title": title,
+                "value": value,
+            }
+    
+    editable: MetaOapg.properties.editable
+    title: 'ConfigValueFilter'
+    value: 'PolymorphicProperty'
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["editable"]) -> MetaOapg.properties.editable: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["title"]) -> 'ConfigValueFilter': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["value"]) -> 'PolymorphicProperty': ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["editable", "title", "value", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["editable"]) -> MetaOapg.properties.editable: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["title"]) -> 'ConfigValueFilter': ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["value"]) -> 'PolymorphicProperty': ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["editable", "title", "value", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        editable: typing.Union[MetaOapg.properties.editable, bool, ],
+        title: 'ConfigValueFilter',
+        value: 'PolymorphicProperty',
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'Configuration':
+        return super().__new__(
+            cls,
+            *_args,
+            editable=editable,
+            title=title,
+            value=value,
+            _configuration=_configuration,
+            **kwargs,
+        )
+
+from firefly_iii_client.model.config_value_filter import ConfigValueFilter
+from firefly_iii_client.model.polymorphic_property import PolymorphicProperty
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/user_blocked_code_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_user_role_property.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
+    Generated by: https://openapi-generator.tech
+"""
 
+import unittest
 
-class UserBlockedCodeProperty(str, Enum):
-    """
-    If you say the user must be blocked, this will be the reason code.
-    """
+import firefly_iii_client
+from firefly_iii_client.model.user_role_property import UserRoleProperty
+from firefly_iii_client import configuration
 
-    """
-    allowed enum values
-    """
-    EMAIL_CHANGED = 'email_changed'
-    NULL = 'null'
 
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserBlockedCodeProperty from a JSON string"""
-        return cls(json.loads(json_str))
+class TestUserRoleProperty(unittest.TestCase):
+    """UserRoleProperty unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_delivery.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
+    Generated by: https://openapi-generator.tech
+"""
 
+import unittest
 
-class WebhookDelivery(str, Enum):
-    """
-    Format of the delivered response.
-    """
+import firefly_iii_client
+from firefly_iii_client.model.user import User
+from firefly_iii_client import configuration
 
-    """
-    allowed enum values
-    """
-    JSON = 'JSON'
 
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of WebhookDelivery from a JSON string"""
-        return cls(json.loads(json_str))
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/models/webhook_trigger.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_webhook_trigger.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import firefly_iii_client
+from firefly_iii_client.model.webhook_trigger import WebhookTrigger
+from firefly_iii_client import configuration
 
 
-from __future__ import annotations
-import json
-from enum import Enum
-from typing_extensions import Self
-
-
-class WebhookTrigger(str, Enum):
-    """
-    The trigger for the webhook.
-    """
-
-    """
-    allowed enum values
-    """
-    STORE_TRANSACTION = 'STORE_TRANSACTION'
-    UPDATE_TRANSACTION = 'UPDATE_TRANSACTION'
-    DESTROY_TRANSACTION = 'DESTROY_TRANSACTION'
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of WebhookTrigger from a JSON string"""
-        return cls(json.loads(json_str))
+class TestWebhookTrigger(unittest.TestCase):
+    """WebhookTrigger unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/firefly_iii_client/rest.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/rest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,256 +1,258 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
-import io
-import json
-import re
+import logging
 import ssl
+from urllib.parse import urlencode
+import typing
 
+import certifi
 import urllib3
+from urllib3._collections import HTTPHeaderDict
 
 from firefly_iii_client.exceptions import ApiException, ApiValueError
 
-SUPPORTED_SOCKS_PROXIES = {"socks5", "socks5h", "socks4", "socks4a"}
-RESTResponseType = urllib3.HTTPResponse
-
-
-def is_socks_proxy_url(url):
-    if url is None:
-        return False
-    split_section = url.split("://")
-    if len(split_section) < 2:
-        return False
-    else:
-        return split_section[0].lower() in SUPPORTED_SOCKS_PROXIES
-
-
-class RESTResponse(io.IOBase):
-
-    def __init__(self, resp) -> None:
-        self.response = resp
-        self.status = resp.status
-        self.reason = resp.reason
-        self.data = None
-
-    def read(self):
-        if self.data is None:
-            self.data = self.response.data
-        return self.data
-
-    def getheaders(self):
-        """Returns a dictionary of the response headers."""
-        return self.response.headers
 
-    def getheader(self, name, default=None):
-        """Returns a given response header."""
-        return self.response.headers.get(name, default)
+logger = logging.getLogger(__name__)
 
 
-class RESTClientObject:
+class RESTClientObject(object):
 
-    def __init__(self, configuration) -> None:
+    def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
+        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
         # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
-        pool_args = {
-            "cert_reqs": cert_reqs,
-            "ca_certs": configuration.ssl_ca_cert,
-            "cert_file": configuration.cert_file,
-            "key_file": configuration.key_file,
-        }
+        # ca_certs
+        if configuration.ssl_ca_cert:
+            ca_certs = configuration.ssl_ca_cert
+        else:
+            # if not set certificate file, use Mozilla's root certificates.
+            ca_certs = certifi.where()
+
+        addition_pool_args = {}
         if configuration.assert_hostname is not None:
-            pool_args['assert_hostname'] = (
-                configuration.assert_hostname
-            )
+            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
-            pool_args['retries'] = configuration.retries
+            addition_pool_args['retries'] = configuration.retries
 
         if configuration.tls_server_name:
-            pool_args['server_hostname'] = configuration.tls_server_name
-
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
 
         if configuration.socket_options is not None:
-            pool_args['socket_options'] = configuration.socket_options
+            addition_pool_args['socket_options'] = configuration.socket_options
 
-        if configuration.connection_pool_maxsize is not None:
-            pool_args['maxsize'] = configuration.connection_pool_maxsize
+        if maxsize is None:
+            if configuration.connection_pool_maxsize is not None:
+                maxsize = configuration.connection_pool_maxsize
+            else:
+                maxsize = 4
 
         # https pool manager
-        self.pool_manager: urllib3.PoolManager
-
         if configuration.proxy:
-            if is_socks_proxy_url(configuration.proxy):
-                from urllib3.contrib.socks import SOCKSProxyManager
-                pool_args["proxy_url"] = configuration.proxy
-                pool_args["headers"] = configuration.proxy_headers
-                self.pool_manager = SOCKSProxyManager(**pool_args)
-            else:
-                pool_args["proxy_url"] = configuration.proxy
-                pool_args["proxy_headers"] = configuration.proxy_headers
-                self.pool_manager = urllib3.ProxyManager(**pool_args)
+            self.pool_manager = urllib3.ProxyManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=ca_certs,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                proxy_url=configuration.proxy,
+                proxy_headers=configuration.proxy_headers,
+                **addition_pool_args
+            )
         else:
-            self.pool_manager = urllib3.PoolManager(**pool_args)
+            self.pool_manager = urllib3.PoolManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=ca_certs,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                **addition_pool_args
+            )
 
     def request(
         self,
-        method,
-        url,
-        headers=None,
-        body=None,
-        post_params=None,
-        _request_timeout=None
-    ):
+        method: str,
+        url: str,
+        headers: typing.Optional[HTTPHeaderDict] = None,
+        fields: typing.Optional[typing.Tuple[typing.Tuple[str, typing.Any], ...]] = None,
+        body: typing.Optional[typing.Union[str, bytes]] = None,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> urllib3.HTTPResponse:
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param headers: http request headers
-        :param body: request json body, for `application/json`
-        :param post_params: request post parameters,
-                            `application/x-www-form-urlencoded`
-                            and `multipart/form-data`
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
+        :param body: request body, for other types
+        :param fields: request parameters for
+                                `application/x-www-form-urlencoded`
+                                or `multipart/form-data`
+        :param stream: if True, the urllib3.HTTPResponse object will
+                                be returned without reading/decoding response
+                                data. Default is False.
+        :param timeout: timeout setting for this request. If one
+                                number provided, it will be total request
+                                timeout. It can also be a pair (tuple) of
+                                (connection, read) timeouts.
         """
         method = method.upper()
-        assert method in [
-            'GET',
-            'HEAD',
-            'DELETE',
-            'POST',
-            'PUT',
-            'PATCH',
-            'OPTIONS'
-        ]
+        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
+                          'PATCH', 'OPTIONS']
 
-        if post_params and body:
+        if fields and body:
             raise ApiValueError(
-                "body parameter cannot be used with post_params parameter."
+                "body parameter cannot be used with fields parameter."
             )
 
-        post_params = post_params or {}
+        fields = fields or {}
         headers = headers or {}
 
-        timeout = None
-        if _request_timeout:
-            if isinstance(_request_timeout, (int, float)):
-                timeout = urllib3.Timeout(total=_request_timeout)
-            elif (
-                    isinstance(_request_timeout, tuple)
-                    and len(_request_timeout) == 2
-                ):
-                timeout = urllib3.Timeout(
-                    connect=_request_timeout[0],
-                    read=_request_timeout[1]
-                )
+        if timeout:
+            if isinstance(timeout, (int, float)):  # noqa: E501,F821
+                timeout = urllib3.Timeout(total=timeout)
+            elif (isinstance(timeout, tuple) and
+                  len(timeout) == 2):
+                timeout = urllib3.Timeout(connect=timeout[0], read=timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-
-                # no content type provided or payload is json
-                content_type = headers.get('Content-Type')
-                if (
-                    not content_type
-                    or re.search('json', content_type, re.IGNORECASE)
-                ):
-                    request_body = None
-                    if body is not None:
-                        request_body = json.dumps(body)
+                if 'Content-Type' not in headers and body is None:
                     r = self.pool_manager.request(
                         method,
                         url,
-                        body=request_body,
+                        preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
-                        preload_content=False
+                        headers=headers
                     )
-                elif content_type == 'application/x-www-form-urlencoded':
+                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
                     r = self.pool_manager.request(
-                        method,
-                        url,
-                        fields=post_params,
+                        method, url,
+                        body=body,
+                        fields=fields,
                         encode_multipart=False,
+                        preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
-                        preload_content=False
-                    )
-                elif content_type == 'multipart/form-data':
+                        headers=headers)
+                elif headers['Content-Type'] == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
                     r = self.pool_manager.request(
-                        method,
-                        url,
-                        fields=post_params,
+                        method, url,
+                        fields=fields,
                         encode_multipart=True,
+                        preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
-                        preload_content=False
-                    )
+                        headers=headers)
                 # Pass a `string` parameter directly in the body to support
-                # other content types than JSON when `body` argument is
-                # provided in serialized form.
+                # other content types than Json when `body` argument is
+                # provided in serialized form
                 elif isinstance(body, str) or isinstance(body, bytes):
+                    request_body = body
                     r = self.pool_manager.request(
-                        method,
-                        url,
-                        body=body,
-                        timeout=timeout,
-                        headers=headers,
-                        preload_content=False
-                    )
-                elif headers['Content-Type'] == 'text/plain' and isinstance(body, bool):
-                    request_body = "true" if body else "false"
-                    r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         body=request_body,
-                        preload_content=False,
+                        preload_content=not stream,
                         timeout=timeout,
                         headers=headers)
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
-                r = self.pool_manager.request(
-                    method,
-                    url,
-                    fields={},
-                    timeout=timeout,
-                    headers=headers,
-                    preload_content=False
-                )
+                r = self.pool_manager.request(method, url,
+                                              preload_content=not stream,
+                                              timeout=timeout,
+                                              headers=headers)
         except urllib3.exceptions.SSLError as e:
-            msg = "\n".join([type(e).__name__, str(e)])
+            msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
-        return RESTResponse(r)
+        if not stream:
+            # log response body
+            logger.debug("response body: %s", r.data)
+
+        return r
+
+    def GET(self, url, headers=None, stream=False,
+            timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("GET", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            fields=fields)
+
+    def HEAD(self, url, headers=None, stream=False,
+             timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("HEAD", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            fields=fields)
+
+    def OPTIONS(self, url, headers=None,
+                body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("OPTIONS", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def DELETE(self, url, headers=None, body=None,
+               stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("DELETE", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def POST(self, url, headers=None,
+             body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("POST", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def PUT(self, url, headers=None,
+            body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("PUT", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def PATCH(self, url, headers=None,
+              body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("PATCH", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_about_api.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_bill/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
-
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
 
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
+from unittest.mock import patch
 
-from firefly_iii_client.api.about_api import AboutApi
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_insight_expense_bill import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-class TestAboutApi(unittest.TestCase):
-    """AboutApi unit test stubs"""
+from .. import ApiTestMixin
 
-    def setUp(self) -> None:
-        self.api = AboutApi()
 
-    def tearDown(self) -> None:
-        pass
+class TestV1InsightExpenseBill(ApiTestMixin, unittest.TestCase):
+    """
+    V1InsightExpenseBill unit test stubs
+        Insight into expenses, grouped by bill.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
-    def test_get_about(self) -> None:
-        """Test case for get_about
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
-        System information end point.
-        """
+    def tearDown(self):
         pass
 
-    def test_get_cron(self) -> None:
-        """Test case for get_cron
+    response_status = 200
 
-        Cron job endpoint
-        """
-        pass
-
-    def test_get_current_user(self) -> None:
-        """Test case for get_current_user
 
-        Currently authenticated user endpoint.
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_account_role_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_transaction_type_property.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.account_role_property import AccountRoleProperty
-
-class TestAccountRoleProperty(unittest.TestCase):
-    """AccountRoleProperty unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.transaction_type_property import TransactionTypeProperty
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestTransactionTypeProperty(unittest.TestCase):
+    """TransactionTypeProperty unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testAccountRoleProperty(self):
-        """Test AccountRoleProperty"""
-        # inst = AccountRoleProperty()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_account_search_field_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_account_search_field_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.account_search_field_filter import AccountSearchFieldFilter
+import firefly_iii_client
+from firefly_iii_client.model.account_search_field_filter import AccountSearchFieldFilter
+from firefly_iii_client import configuration
+
 
 class TestAccountSearchFieldFilter(unittest.TestCase):
     """AccountSearchFieldFilter unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testAccountSearchFieldFilter(self):
-        """Test AccountSearchFieldFilter"""
-        # inst = AccountSearchFieldFilter()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_account_type_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_rule_group.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.account_type_filter import AccountTypeFilter
-
-class TestAccountTypeFilter(unittest.TestCase):
-    """AccountTypeFilter unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.rule_group import RuleGroup
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestRuleGroup(unittest.TestCase):
+    """RuleGroup unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testAccountTypeFilter(self):
-        """Test AccountTypeFilter"""
-        # inst = AccountTypeFilter()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_account_type_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_short_account_type_property.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.account_type_property import AccountTypeProperty
-
-class TestAccountTypeProperty(unittest.TestCase):
-    """AccountTypeProperty unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.short_account_type_property import ShortAccountTypeProperty
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestShortAccountTypeProperty(unittest.TestCase):
+    """ShortAccountTypeProperty unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testAccountTypeProperty(self):
-        """Test AccountTypeProperty"""
-        # inst = AccountTypeProperty()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_attachable_type.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_bill_array.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.attachable_type import AttachableType
-
-class TestAttachableType(unittest.TestCase):
-    """AttachableType unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.bill_array import BillArray
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestBillArray(unittest.TestCase):
+    """BillArray unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testAttachableType(self):
-        """Test AttachableType"""
-        # inst = AttachableType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_auto_budget_period.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_budget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.auto_budget_period import AutoBudgetPeriod
-
-class TestAutoBudgetPeriod(unittest.TestCase):
-    """AutoBudgetPeriod unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.budget import Budget
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestBudget(unittest.TestCase):
+    """Budget unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testAutoBudgetPeriod(self):
-        """Test AutoBudgetPeriod"""
-        # inst = AutoBudgetPeriod()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_auto_budget_type.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_budget_array.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.auto_budget_type import AutoBudgetType
-
-class TestAutoBudgetType(unittest.TestCase):
-    """AutoBudgetType unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.budget_array import BudgetArray
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestBudgetArray(unittest.TestCase):
+    """BudgetArray unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testAutoBudgetType(self):
-        """Test AutoBudgetType"""
-        # inst = AutoBudgetType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_autocomplete_transaction_id.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/model/autocomplete_transaction_array.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
+    Generated by: https://openapi-generator.tech
+"""
 
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from firefly_iii_client import schemas  # noqa: F401
+
+
+class AutocompleteTransactionArray(
+    schemas.ListSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
 
-import unittest
+    Do not edit the class manually.
+    """
 
-from firefly_iii_client.models.autocomplete_transaction_id import AutocompleteTransactionID
 
-class TestAutocompleteTransactionID(unittest.TestCase):
-    """AutocompleteTransactionID unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional) -> AutocompleteTransactionID:
-        """Test AutocompleteTransactionID
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `AutocompleteTransactionID`
-        """
-        model = AutocompleteTransactionID()
-        if include_optional:
-            return AutocompleteTransactionID(
-                description = '#12: Transaction',
-                id = '2',
-                name = '#12: Transaction',
-                transaction_group_id = '2'
-            )
-        else:
-            return AutocompleteTransactionID(
-                description = '#12: Transaction',
-                id = '2',
-                name = '#12: Transaction',
+    class MetaOapg:
+        
+        @staticmethod
+        def items() -> typing.Type['AutocompleteTransaction']:
+            return AutocompleteTransaction
+
+    def __new__(
+        cls,
+        _arg: typing.Union[typing.Tuple['AutocompleteTransaction'], typing.List['AutocompleteTransaction']],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> 'AutocompleteTransactionArray':
+        return super().__new__(
+            cls,
+            _arg,
+            _configuration=_configuration,
         )
-        """
 
-    def testAutocompleteTransactionID(self):
-        """Test AutocompleteTransactionID"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    def __getitem__(self, i: int) -> 'AutocompleteTransaction':
+        return super().__getitem__(i)
 
-if __name__ == '__main__':
-    unittest.main()
+from firefly_iii_client.model.autocomplete_transaction import AutocompleteTransaction
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_bill_repeat_frequency.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.bill_repeat_frequency import BillRepeatFrequency
-
-class TestBillRepeatFrequency(unittest.TestCase):
-    """BillRepeatFrequency unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.rule_trigger import RuleTrigger
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestRuleTrigger(unittest.TestCase):
+    """RuleTrigger unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testBillRepeatFrequency(self):
-        """Test BillRepeatFrequency"""
-        # inst = BillRepeatFrequency()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_charts_api.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_chart_data_point.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.api.charts_api import ChartsApi
-
-
-class TestChartsApi(unittest.TestCase):
-    """ChartsApi unit test stubs"""
-
-    def setUp(self) -> None:
-        self.api = ChartsApi()
-
-    def tearDown(self) -> None:
-        pass
+import firefly_iii_client
+from firefly_iii_client.model.chart_data_point import ChartDataPoint
+from firefly_iii_client import configuration
 
-    def test_get_chart_account_overview(self) -> None:
-        """Test case for get_chart_account_overview
 
-        Dashboard chart with asset account balance information.
-        """
-        pass
+class TestChartDataPoint(unittest.TestCase):
+    """ChartDataPoint unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_config_value_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_account_type_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.config_value_filter import ConfigValueFilter
-
-class TestConfigValueFilter(unittest.TestCase):
-    """ConfigValueFilter unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.account_type_filter import AccountTypeFilter
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestAccountTypeFilter(unittest.TestCase):
+    """AccountTypeFilter unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testConfigValueFilter(self):
-        """Test ConfigValueFilter"""
-        # inst = ConfigValueFilter()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_config_value_update_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_config_value_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.config_value_update_filter import ConfigValueUpdateFilter
-
-class TestConfigValueUpdateFilter(unittest.TestCase):
-    """ConfigValueUpdateFilter unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.config_value_filter import ConfigValueFilter
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestConfigValueFilter(unittest.TestCase):
+    """ConfigValueFilter unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testConfigValueUpdateFilter(self):
-        """Test ConfigValueUpdateFilter"""
-        # inst = ConfigValueUpdateFilter()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_configuration.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/model/config_value_update_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
-import unittest
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from firefly_iii_client import schemas  # noqa: F401
+
+
+class ConfigValueUpdateFilter(
+    schemas.EnumBase,
+    schemas.StrSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
 
-from firefly_iii_client.models.configuration import Configuration
+    Do not edit the class manually.
+    """
 
-class TestConfiguration(unittest.TestCase):
-    """Configuration unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional) -> Configuration:
-        """Test Configuration
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `Configuration`
-        """
-        model = Configuration()
-        if include_optional:
-            return Configuration(
-                editable = True,
-                title = 'configuration.is_demo_site',
-                value = None
-            )
-        else:
-            return Configuration(
-                editable = True,
-                title = 'configuration.is_demo_site',
-                value = None,
-        )
-        """
-
-    def testConfiguration(self):
-        """Test Configuration"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
-    unittest.main()
+    class MetaOapg:
+        enum_value_to_name = {
+            "configuration.is_demo_site": "IS_DEMO_SITE",
+            "configuration.permission_update_check": "PERMISSION_UPDATE_CHECK",
+            "configuration.last_update_check": "LAST_UPDATE_CHECK",
+            "configuration.single_user_mode": "SINGLE_USER_MODE",
+        }
+    
+    @schemas.classproperty
+    def IS_DEMO_SITE(cls):
+        return cls("configuration.is_demo_site")
+    
+    @schemas.classproperty
+    def PERMISSION_UPDATE_CHECK(cls):
+        return cls("configuration.permission_update_check")
+    
+    @schemas.classproperty
+    def LAST_UPDATE_CHECK(cls):
+        return cls("configuration.last_update_check")
+    
+    @schemas.classproperty
+    def SINGLE_USER_MODE(cls):
+        return cls("configuration.single_user_mode")
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_configuration_api.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_insight_expense_total/test_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
-
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
 
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
+from unittest.mock import patch
 
-from firefly_iii_client.api.configuration_api import ConfigurationApi
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_insight_expense_total import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-class TestConfigurationApi(unittest.TestCase):
-    """ConfigurationApi unit test stubs"""
+from .. import ApiTestMixin
 
-    def setUp(self) -> None:
-        self.api = ConfigurationApi()
 
-    def tearDown(self) -> None:
-        pass
+class TestV1InsightExpenseTotal(ApiTestMixin, unittest.TestCase):
+    """
+    V1InsightExpenseTotal unit test stubs
+        Insight into total expenses.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
-    def test_get_configuration(self) -> None:
-        """Test case for get_configuration
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
-        Get Firefly III system configuration values.
-        """
+    def tearDown(self):
         pass
 
-    def test_get_single_configuration(self) -> None:
-        """Test case for get_single_configuration
+    response_status = 200
 
-        Get a single Firefly III system configuration value
-        """
-        pass
-
-    def test_set_configuration(self) -> None:
-        """Test case for set_configuration
 
-        Update configuration value
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_configuration_single.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_currencies_code_transactions/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
 
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
+from unittest.mock import patch
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_currencies_code_transactions import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-import unittest
+from .. import ApiTestMixin
 
-from firefly_iii_client.models.configuration_single import ConfigurationSingle
 
-class TestConfigurationSingle(unittest.TestCase):
-    """ConfigurationSingle unit test stubs"""
+class TestV1CurrenciesCodeTransactions(ApiTestMixin, unittest.TestCase):
+    """
+    V1CurrenciesCodeTransactions unit test stubs
+        List all transactions with this currency.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ConfigurationSingle:
-        """Test ConfigurationSingle
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `ConfigurationSingle`
-        """
-        model = ConfigurationSingle()
-        if include_optional:
-            return ConfigurationSingle(
-                data = firefly_iii_client.models.configuration.Configuration(
-                    editable = True, 
-                    title = 'configuration.is_demo_site', 
-                    value = null, )
-            )
-        else:
-            return ConfigurationSingle(
-                data = firefly_iii_client.models.configuration.Configuration(
-                    editable = True, 
-                    title = 'configuration.is_demo_site', 
-                    value = null, ),
-        )
-        """
-
-    def testConfigurationSingle(self):
-        """Test ConfigurationSingle"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_credit_card_type_property.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_users/test_get.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
 
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
+from unittest.mock import patch
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_users import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-import unittest
+from .. import ApiTestMixin
 
-from firefly_iii_client.models.credit_card_type_property import CreditCardTypeProperty
 
-class TestCreditCardTypeProperty(unittest.TestCase):
-    """CreditCardTypeProperty unit test stubs"""
+class TestV1Users(ApiTestMixin, unittest.TestCase):
+    """
+    V1Users unit test stubs
+        List all users.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testCreditCardTypeProperty(self):
-        """Test CreditCardTypeProperty"""
-        # inst = CreditCardTypeProperty()
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_data_destroy_object.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_data_destroy_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.data_destroy_object import DataDestroyObject
+import firefly_iii_client
+from firefly_iii_client.model.data_destroy_object import DataDestroyObject
+from firefly_iii_client import configuration
+
 
 class TestDataDestroyObject(unittest.TestCase):
     """DataDestroyObject unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testDataDestroyObject(self):
-        """Test DataDestroyObject"""
-        # inst = DataDestroyObject()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_export_file_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.export_file_filter import ExportFileFilter
-
-class TestExportFileFilter(unittest.TestCase):
-    """ExportFileFilter unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.meta import Meta
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestMeta(unittest.TestCase):
+    """Meta unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testExportFileFilter(self):
-        """Test ExportFileFilter"""
-        # inst = ExportFileFilter()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_liability_direction_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_rule_trigger_keyword.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.liability_direction_property import LiabilityDirectionProperty
-
-class TestLiabilityDirectionProperty(unittest.TestCase):
-    """LiabilityDirectionProperty unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.rule_trigger_keyword import RuleTriggerKeyword
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestRuleTriggerKeyword(unittest.TestCase):
+    """RuleTriggerKeyword unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testLiabilityDirectionProperty(self):
-        """Test LiabilityDirectionProperty"""
-        # inst = LiabilityDirectionProperty()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_liability_type_property.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_user_read.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.liability_type_property import LiabilityTypeProperty
-
-class TestLiabilityTypeProperty(unittest.TestCase):
-    """LiabilityTypeProperty unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.user_read import UserRead
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestUserRead(unittest.TestCase):
+    """UserRead unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testLiabilityTypeProperty(self):
-        """Test LiabilityTypeProperty"""
-        # inst = LiabilityTypeProperty()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_recurrence_repetition_type.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_budgets/test_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
 
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
+from unittest.mock import patch
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_budgets import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-import unittest
+from .. import ApiTestMixin
 
-from firefly_iii_client.models.recurrence_repetition_type import RecurrenceRepetitionType
 
-class TestRecurrenceRepetitionType(unittest.TestCase):
-    """RecurrenceRepetitionType unit test stubs"""
+class TestV1Budgets(ApiTestMixin, unittest.TestCase):
+    """
+    V1Budgets unit test stubs
+        List all budgets.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testRecurrenceRepetitionType(self):
-        """Test RecurrenceRepetitionType"""
-        # inst = RecurrenceRepetitionType()
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_recurrence_transaction_type.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_autocomplete_transactions_with_id/test_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
 
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
+from unittest.mock import patch
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_autocomplete_transactions_with_id import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-import unittest
+from .. import ApiTestMixin
 
-from firefly_iii_client.models.recurrence_transaction_type import RecurrenceTransactionType
 
-class TestRecurrenceTransactionType(unittest.TestCase):
-    """RecurrenceTransactionType unit test stubs"""
+class TestV1AutocompleteTransactionsWithId(ApiTestMixin, unittest.TestCase):
+    """
+    V1AutocompleteTransactionsWithId unit test stubs
+        Returns all transactions, complemented with their ID, of the user returned in a basic auto-complete array. This endpoint is DEPRECATED and I suggest you DO NOT use it.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testRecurrenceTransactionType(self):
-        """Test RecurrenceTransactionType"""
-        # inst = RecurrenceTransactionType()
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_rule_action_keyword.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_bill_single.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.rule_action_keyword import RuleActionKeyword
-
-class TestRuleActionKeyword(unittest.TestCase):
-    """RuleActionKeyword unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.bill_single import BillSingle
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestBillSingle(unittest.TestCase):
+    """BillSingle unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testRuleActionKeyword(self):
-        """Test RuleActionKeyword"""
-        # inst = RuleActionKeyword()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_rule_trigger_keyword.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_bills/test_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
 
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+    Generated by: https://openapi-generator.tech
+"""
+
+import unittest
+from unittest.mock import patch
 
-    Do not edit the class manually.
-"""  # noqa: E501
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_bills import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-import unittest
+from .. import ApiTestMixin
 
-from firefly_iii_client.models.rule_trigger_keyword import RuleTriggerKeyword
 
-class TestRuleTriggerKeyword(unittest.TestCase):
-    """RuleTriggerKeyword unit test stubs"""
+class TestV1Bills(ApiTestMixin, unittest.TestCase):
+    """
+    V1Bills unit test stubs
+        List all bills.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testRuleTriggerKeyword(self):
-        """Test RuleTriggerKeyword"""
-        # inst = RuleTriggerKeyword()
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_rule_trigger_type.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_rule_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.rule_trigger_type import RuleTriggerType
-
-class TestRuleTriggerType(unittest.TestCase):
-    """RuleTriggerType unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.rule_update import RuleUpdate
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestRuleUpdate(unittest.TestCase):
+    """RuleUpdate unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testRuleTriggerType(self):
-        """Test RuleTriggerType"""
-        # inst = RuleTriggerType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_search_api.py` & `Firefly III API Client-2.0.5.0/test/test_paths/test_v1_rules_id_test/test_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 # coding: utf-8
 
 """
-    Firefly III API Client
 
-    This is the Python client for Firefly III API
-
-    The version of the OpenAPI document: 2.0.12
-    Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
 
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
+from unittest.mock import patch
 
-from firefly_iii_client.api.search_api import SearchApi
+import urllib3
 
+import firefly_iii_client
+from firefly_iii_client.paths.v1_rules_id_test import get  # noqa: E501
+from firefly_iii_client import configuration, schemas, api_client
 
-class TestSearchApi(unittest.TestCase):
-    """SearchApi unit test stubs"""
+from .. import ApiTestMixin
 
-    def setUp(self) -> None:
-        self.api = SearchApi()
 
-    def tearDown(self) -> None:
-        pass
+class TestV1RulesIdTest(ApiTestMixin, unittest.TestCase):
+    """
+    V1RulesIdTest unit test stubs
+        Test which transactions would be hit by the rule. No changes will be made.  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
-    def test_search_accounts(self) -> None:
-        """Test case for search_accounts
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
-        Search for accounts
-        """
+    def tearDown(self):
         pass
 
-    def test_search_transactions(self) -> None:
-        """Test case for search_transactions
+    response_status = 200
+
 
-        Search for transactions
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_short_account_type_property.py` & `Firefly III API Client-2.0.5.0/firefly_iii_client/apis/tags/summary_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-import unittest
-
-from firefly_iii_client.models.short_account_type_property import ShortAccountTypeProperty
-
-class TestShortAccountTypeProperty(unittest.TestCase):
-    """ShortAccountTypeProperty unit test stubs"""
+    Generated by: https://openapi-generator.tech
+"""
 
-    def setUp(self):
-        pass
+from firefly_iii_client.paths.v1_summary_basic.get import GetBasicSummary
 
-    def tearDown(self):
-        pass
 
-    def testShortAccountTypeProperty(self):
-        """Test ShortAccountTypeProperty"""
-        # inst = ShortAccountTypeProperty()
+class SummaryApi(
+    GetBasicSummary,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-if __name__ == '__main__':
-    unittest.main()
+    Do not edit the class manually.
+    """
+    pass
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_summary_api.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_basic_summary_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.api.summary_api import SummaryApi
-
-
-class TestSummaryApi(unittest.TestCase):
-    """SummaryApi unit test stubs"""
-
-    def setUp(self) -> None:
-        self.api = SummaryApi()
-
-    def tearDown(self) -> None:
-        pass
+import firefly_iii_client
+from firefly_iii_client.model.basic_summary_entry import BasicSummaryEntry
+from firefly_iii_client import configuration
 
-    def test_get_basic_summary(self) -> None:
-        """Test case for get_basic_summary
 
-        Returns basic sums of the users data.
-        """
-        pass
+class TestBasicSummaryEntry(unittest.TestCase):
+    """BasicSummaryEntry unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_transaction_type_filter.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_transaction_type_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.transaction_type_filter import TransactionTypeFilter
+import firefly_iii_client
+from firefly_iii_client.model.transaction_type_filter import TransactionTypeFilter
+from firefly_iii_client import configuration
+
 
 class TestTransactionTypeFilter(unittest.TestCase):
     """TransactionTypeFilter unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testTransactionTypeFilter(self):
-        """Test TransactionTypeFilter"""
-        # inst = TransactionTypeFilter()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_webhook_delivery.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_webhook_delivery.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.webhook_delivery import WebhookDelivery
+import firefly_iii_client
+from firefly_iii_client.model.webhook_delivery import WebhookDelivery
+from firefly_iii_client import configuration
+
 
 class TestWebhookDelivery(unittest.TestCase):
     """WebhookDelivery unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testWebhookDelivery(self):
-        """Test WebhookDelivery"""
-        # inst = WebhookDelivery()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_webhook_response.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_webhook_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.webhook_response import WebhookResponse
+import firefly_iii_client
+from firefly_iii_client.model.webhook_response import WebhookResponse
+from firefly_iii_client import configuration
+
 
 class TestWebhookResponse(unittest.TestCase):
     """WebhookResponse unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testWebhookResponse(self):
-        """Test WebhookResponse"""
-        # inst = WebhookResponse()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Firefly III API Client-2.0.12.0/test/test_webhook_trigger.py` & `Firefly III API Client-2.0.5.0/test/test_models/test_tag_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 """
     Firefly III API Client
 
-    This is the Python client for Firefly III API
+    This is the Python client for Firefly III API  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.12
+    The version of the OpenAPI document: 2.0.5
     Contact: james@firefly-iii.org
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
+    Generated by: https://openapi-generator.tech
+"""
 
 import unittest
 
-from firefly_iii_client.models.webhook_trigger import WebhookTrigger
-
-class TestWebhookTrigger(unittest.TestCase):
-    """WebhookTrigger unit test stubs"""
+import firefly_iii_client
+from firefly_iii_client.model.tag_model import TagModel
+from firefly_iii_client import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+class TestTagModel(unittest.TestCase):
+    """TagModel unit test stubs"""
+    _configuration = configuration.Configuration()
 
-    def testWebhookTrigger(self):
-        """Test WebhookTrigger"""
-        # inst = WebhookTrigger()
 
 if __name__ == '__main__':
     unittest.main()
```

