# Comparing `tmp/sky_api_client-3.3.1.tar.gz` & `tmp/sky_api_client-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sky_api_client-3.3.1.tar", last modified: Mon Feb  5 12:52:49 2024, max compression
+gzip compressed data, was "dist/sky_api_client-3.3.2.tar", last modified: Mon Apr  8 08:14:57 2024, max compression
```

## Comparing `sky_api_client-3.3.1.tar` & `sky_api_client-3.3.2.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/
--rw-r--r--   0 root         (0) root         (0)     4142 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2418 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client/
--rw-rw-rw-   0 root         (0) root         (0)     2888 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/address.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/base.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/code_table.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_address.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_code.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_education.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_email_address.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_online_presence.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_phone.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_relationship.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/constituent_solicit_code.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/custom_field_categories.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/education.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/email_addresses.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_fee.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_participant.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_participant_donation.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_participant_fee.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_participant_fee_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_participant_levels.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/event_participation_levels.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/fundraising_appeal.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/fundraising_campaign.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/fundraising_fund.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/fundraising_package.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gender.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift_aid.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift_batch.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift_batch_gift.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift_custom_field_values.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/gift_subtype.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/list.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/online_presence.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/phone.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/relationship.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/solicit_code.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/suffix.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/table_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/title.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/entity/webhook_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-05 12:52:29.000000 sky_api_client-3.3.1/sky_api_client/exceptions/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4142 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2283 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-05 12:52:49.000000 sky_api_client-3.3.1/sky_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/
+-rw-r--r--   0 root         (0) root         (0)     4141 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2418 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/sky_api_client/
+-rw-rw-rw-   0 root         (0) root         (0)     2888 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/sky_api_client/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/sky_api_client/common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/common/tasks/asyncio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/sky_api_client/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/address.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/code_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_education.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_email_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_online_presence.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_phone.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_relationship.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/constituent_solicit_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/custom_field_categories.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/education.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/email_addresses.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_fee.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_participant.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_participant_donation.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_participant_fee.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_participant_fee_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_participant_levels.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/event_participation_levels.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/fundraising_appeal.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/fundraising_campaign.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/fundraising_fund.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/fundraising_package.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gender.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift_aid.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift_batch.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift_batch_gift.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift_custom_field_values.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/gift_subtype.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/list.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/online_presence.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/phone.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/relationship.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/solicit_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/suffix.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/table_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/title.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/entity/webhook_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/sky_api_client/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-08 08:14:36.000000 sky_api_client-3.3.2/sky_api_client/exceptions/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:14:57.000000 sky_api_client-3.3.2/sky_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4141 2024-04-08 08:14:56.000000 sky_api_client-3.3.2/sky_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-04-08 08:14:56.000000 sky_api_client-3.3.2/sky_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 08:14:56.000000 sky_api_client-3.3.2/sky_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-08 08:14:56.000000 sky_api_client-3.3.2/sky_api_client.egg-info/top_level.txt
```

### Comparing `sky_api_client-3.3.1/PKG-INFO` & `sky_api_client-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sky_api_client
-Version: 3.3.1
+Version: 3.3.2
 Summary: Python client for RENXT APIs
 Home-page: https://bitbucket.org/kalyanvarma/skyapi
-Author: Uddesh Jain
-Author-email: uddesh@almabase.com
+Author: Rajeev K L
+Author-email: rajeev@almabase.com
 License: UNKNOWN
 Description: # Sky Api Client
         
         Python client for RENXT APIs.
         
         Developed by Uddesh at [Almabase](https://almabase.com)
```

### Comparing `sky_api_client-3.3.1/README.md` & `sky_api_client-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/setup.py` & `sky_api_client-3.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='sky_api_client',
-    version='3.3.1',
-    author='Uddesh Jain',
-    author_email='uddesh@almabase.com',
+    version='3.3.2',
+    author='Rajeev K L',
+    author_email='rajeev@almabase.com',
     description='Python client for RENXT APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/kalyanvarma/skyapi',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

### Comparing `sky_api_client-3.3.1/sky_api_client/__init__.py` & `sky_api_client-3.3.2/sky_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client/client.py` & `sky_api_client-3.3.2/sky_api_client/client.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client/entity/base.py` & `sky_api_client-3.3.2/sky_api_client/entity/base.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client/entity/constituent_code.py` & `sky_api_client-3.3.2/sky_api_client/entity/constituent_code.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client/entity/online_presence.py` & `sky_api_client-3.3.2/sky_api_client/entity/online_presence.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client/entity/solicit_code.py` & `sky_api_client-3.3.2/sky_api_client/entity/solicit_code.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client/entity/table_entry.py` & `sky_api_client-3.3.2/sky_api_client/entity/table_entry.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.3.1/sky_api_client.egg-info/PKG-INFO` & `sky_api_client-3.3.2/sky_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sky-api-client
-Version: 3.3.1
+Version: 3.3.2
 Summary: Python client for RENXT APIs
 Home-page: https://bitbucket.org/kalyanvarma/skyapi
-Author: Uddesh Jain
-Author-email: uddesh@almabase.com
+Author: Rajeev K L
+Author-email: rajeev@almabase.com
 License: UNKNOWN
 Description: # Sky Api Client
         
         Python client for RENXT APIs.
         
         Developed by Uddesh at [Almabase](https://almabase.com)
```

### Comparing `sky_api_client-3.3.1/sky_api_client.egg-info/SOURCES.txt` & `sky_api_client-3.3.2/sky_api_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 setup.py
 sky_api_client/__init__.py
 sky_api_client/client.py
 sky_api_client.egg-info/PKG-INFO
 sky_api_client.egg-info/SOURCES.txt
 sky_api_client.egg-info/dependency_links.txt
 sky_api_client.egg-info/top_level.txt
+sky_api_client/common/__init__.py
+sky_api_client/common/tasks/__init__.py
+sky_api_client/common/tasks/asyncio.py
 sky_api_client/entity/__init__.py
 sky_api_client/entity/address.py
 sky_api_client/entity/base.py
 sky_api_client/entity/code_table.py
 sky_api_client/entity/constituent.py
 sky_api_client/entity/constituent_address.py
 sky_api_client/entity/constituent_code.py
```

