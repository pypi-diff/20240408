# Comparing `tmp/pandadoc-python-client-6.1.0.tar.gz` & `tmp/pandadoc-python-client-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandadoc-python-client-6.1.0.tar", last modified: Wed Mar  6 15:14:51 2024, max compression
+gzip compressed data, was "pandadoc-python-client-6.2.0.tar", last modified: Mon Apr  8 08:40:54 2024, max compression
```

## Comparing `pandadoc-python-client-6.1.0.tar` & `pandadoc-python-client-6.2.0.tar`

### file list

```diff
@@ -1,186 +1,198 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.530000 pandadoc-python-client-6.1.0/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2865 2024-03-06 15:14:51.530000 pandadoc-python-client-6.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12747 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.520000 pandadoc-python-client-6.1.0/pandadoc_client/
--rw-r--r--   0 root         (0) root         (0)      666 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.520000 pandadoc-python-client-6.1.0/pandadoc_client/api/
--rw-r--r--   0 root         (0) root         (0)      219 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13436 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/api_logs_api.py
--rw-r--r--   0 root         (0) root         (0)    24668 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/contacts_api.py
--rw-r--r--   0 root         (0) root         (0)    12307 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/content_library_items_api.py
--rw-r--r--   0 root         (0) root         (0)    26634 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/document_attachments_api.py
--rw-r--r--   0 root         (0) root         (0)    22885 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/document_recipients_api.py
--rw-r--r--   0 root         (0) root         (0)    95468 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/documents_api.py
--rw-r--r--   0 root         (0) root         (0)    33709 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/folders_api_api.py
--rw-r--r--   0 root         (0) root         (0)     7569 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/forms_api.py
--rw-r--r--   0 root         (0) root         (0)    14315 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/members_api.py
--rw-r--r--   0 root         (0) root         (0)     7169 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/o_auth_2_0_authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/quotes_api.py
--rw-r--r--   0 root         (0) root         (0)    21473 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/sections_api.py
--rw-r--r--   0 root         (0) root         (0)    17365 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/templates_api.py
--rw-r--r--   0 root         (0) root         (0)    12699 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/webhook_events_api.py
--rw-r--r--   0 root         (0) root         (0)    30255 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api/webhook_subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    37539 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.520000 pandadoc-python-client-6.1.0/pandadoc_client/apis/
--rw-r--r--   0 root         (0) root         (0)     1399 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17253 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4980 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.530000 pandadoc-python-client-6.1.0/pandadoc_client/model/
--rw-r--r--   0 root         (0) root         (0)      348 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14744 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/api_log_details_response.py
--rw-r--r--   0 root         (0) root         (0)    11261 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/api_log_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11758 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/api_log_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    13093 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/contact_create_request.py
--rw-r--r--   0 root         (0) root         (0)    13219 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/contact_details_response.py
--rw-r--r--   0 root         (0) root         (0)    11241 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/contact_list_response.py
--rw-r--r--   0 root         (0) root         (0)    13045 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/contact_update_request.py
--rw-r--r--   0 root         (0) root         (0)    11382 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11804 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    15564 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_response.py
--rw-r--r--   0 root         (0) root         (0)    11801 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_response_created_by.py
--rw-r--r--   0 root         (0) root         (0)    11971 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_attachment_response.py
--rw-r--r--   0 root         (0) root         (0)    11801 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_attachment_response_created_by.py
--rw-r--r--   0 root         (0) root         (0)    15800 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_pdf_request.py
--rw-r--r--   0 root         (0) root         (0)    19930 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request.py
--rw-r--r--   0 root         (0) root         (0)    12490 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_content_library_items.py
--rw-r--r--   0 root         (0) root         (0)    11869 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_content_placeholders.py
--rw-r--r--   0 root         (0) root         (0)    11240 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_images.py
--rw-r--r--   0 root         (0) root         (0)    11912 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_recipients.py
--rw-r--r--   0 root         (0) root         (0)    11245 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_tokens.py
--rw-r--r--   0 root         (0) root         (0)    11609 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_link_request.py
--rw-r--r--   0 root         (0) root         (0)    11167 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_link_response.py
--rw-r--r--   0 root         (0) root         (0)    20578 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request.py
--rw-r--r--   0 root         (0) root         (0)    12508 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_content_library_items.py
--rw-r--r--   0 root         (0) root         (0)    11761 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_content_placeholders.py
--rw-r--r--   0 root         (0) root         (0)    11209 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_images.py
--rw-r--r--   0 root         (0) root         (0)    11849 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_recipients.py
--rw-r--r--   0 root         (0) root         (0)    13093 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_response.py
--rw-r--r--   0 root         (0) root         (0)    11323 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_response_links.py
--rw-r--r--   0 root         (0) root         (0)    18020 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response.py
--rw-r--r--   0 root         (0) root         (0)    12015 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_created_by.py
--rw-r--r--   0 root         (0) root         (0)    11198 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_grand_total.py
--rw-r--r--   0 root         (0) root         (0)    11603 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_linked_objects.py
--rw-r--r--   0 root         (0) root         (0)    14055 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_recipients.py
--rw-r--r--   0 root         (0) root         (0)    11151 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_template.py
--rw-r--r--   0 root         (0) root         (0)    11280 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_list_response.py
--rw-r--r--   0 root         (0) root         (0)    12228 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    13611 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_ordering_fields_enum.py
--rw-r--r--   0 root         (0) root         (0)    11303 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_recipient_create_request.py
--rw-r--r--   0 root         (0) root         (0)    13653 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_recipient_edit_request.py
--rw-r--r--   0 root         (0) root         (0)    11006 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)    13687 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request.py
--rw-r--r--   0 root         (0) root         (0)    11517 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_forwarding_settings.py
--rw-r--r--   0 root         (0) root         (0)    11450 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers.py
--rw-r--r--   0 root         (0) root         (0)    12035 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers_group.py
--rw-r--r--   0 root         (0) root         (0)    11335 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers_group_assignees.py
--rw-r--r--   0 root         (0) root         (0)    11659 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers_steps.py
--rw-r--r--   0 root         (0) root         (0)    12565 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_response.py
--rw-r--r--   0 root         (0) root         (0)    12024 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_change_request.py
--rw-r--r--   0 root         (0) root         (0)    13131 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_enum.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_request_enum.py
--rw-r--r--   0 root         (0) root         (0)    12718 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_response.py
--rw-r--r--   0 root         (0) root         (0)    11640 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_transfer_all_ownership_request.py
--rw-r--r--   0 root         (0) root         (0)    11120 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_transfer_ownership_request.py
--rw-r--r--   0 root         (0) root         (0)    14861 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_update_request.py
--rw-r--r--   0 root         (0) root         (0)    11568 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/document_update_request_recipients.py
--rw-r--r--   0 root         (0) root         (0)    11548 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_create_request.py
--rw-r--r--   0 root         (0) root         (0)    11374 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_create_response.py
--rw-r--r--   0 root         (0) root         (0)    11351 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11811 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_rename_request.py
--rw-r--r--   0 root         (0) root         (0)    11374 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_rename_response.py
--rw-r--r--   0 root         (0) root         (0)    11466 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/form_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11757 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/form_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    11972 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/linked_object_create_request.py
--rw-r--r--   0 root         (0) root         (0)    11987 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/linked_object_create_response.py
--rw-r--r--   0 root         (0) root         (0)    11320 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/linked_object_list_response.py
--rw-r--r--   0 root         (0) root         (0)    14634 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/member_details_response.py
--rw-r--r--   0 root         (0) root         (0)    11231 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/member_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11834 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/o_auth2_access_token_response.py
--rw-r--r--   0 root         (0) root         (0)    11731 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_response.py
--rw-r--r--   0 root         (0) root         (0)    12314 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request.py
--rw-r--r--   0 root         (0) root         (0)    11468 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request_row_options.py
--rw-r--r--   0 root         (0) root         (0)    12095 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request_rows.py
--rw-r--r--   0 root         (0) root         (0)    12057 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request_sections.py
--rw-r--r--   0 root         (0) root         (0)    12681 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response.py
--rw-r--r--   0 root         (0) root         (0)    11223 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_discount.py
--rw-r--r--   0 root         (0) root         (0)    17066 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_items.py
--rw-r--r--   0 root         (0) root         (0)    11889 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_options.py
--rw-r--r--   0 root         (0) root         (0)    11677 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_summary.py
--rw-r--r--   0 root         (0) root         (0)    12991 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response.py
--rw-r--r--   0 root         (0) root         (0)    11156 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_action.py
--rw-r--r--   0 root         (0) root         (0)    11722 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_condition.py
--rw-r--r--   0 root         (0) root         (0)    11170 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_condition_comparison.py
--rw-r--r--   0 root         (0) root         (0)    11996 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_merge_rules.py
--rw-r--r--   0 root         (0) root         (0)    11260 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_options.py
--rw-r--r--   0 root         (0) root         (0)    11619 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_section_column.py
--rw-r--r--   0 root         (0) root         (0)    16204 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_section_item.py
--rw-r--r--   0 root         (0) root         (0)    14215 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_section_summary.py
--rw-r--r--   0 root         (0) root         (0)    13078 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_sections.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_settings.py
--rw-r--r--   0 root         (0) root         (0)    15278 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_summary.py
--rw-r--r--   0 root         (0) root         (0)    11227 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_summary_discounts.py
--rw-r--r--   0 root         (0) root         (0)    11230 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_summary_recurring_subtotal.py
--rw-r--r--   0 root         (0) root         (0)    11545 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_section_settings.py
--rw-r--r--   0 root         (0) root         (0)    12147 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request.py
--rw-r--r--   0 root         (0) root         (0)    11255 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_discounts.py
--rw-r--r--   0 root         (0) root         (0)    11877 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_options.py
--rw-r--r--   0 root         (0) root         (0)    12116 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_price_settings.py
--rw-r--r--   0 root         (0) root         (0)    11281 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_price_settings_tiers.py
--rw-r--r--   0 root         (0) root         (0)    11563 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_settings.py
--rw-r--r--   0 root         (0) root         (0)    11164 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_settings1.py
--rw-r--r--   0 root         (0) root         (0)    12555 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/recipient_verification_settings.py
--rw-r--r--   0 root         (0) root         (0)    11298 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/recipient_verification_settings_passcode_verification.py
--rw-r--r--   0 root         (0) root         (0)    11307 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/recipient_verification_settings_phone_verification.py
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/section_info_response.py
--rw-r--r--   0 root         (0) root         (0)    15880 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response.py
--rw-r--r--   0 root         (0) root         (0)    11428 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_content_placeholders.py
--rw-r--r--   0 root         (0) root         (0)    11403 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_images.py
--rw-r--r--   0 root         (0) root         (0)    11679 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_preassigned_person.py
--rw-r--r--   0 root         (0) root         (0)    12047 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_roles.py
--rw-r--r--   0 root         (0) root         (0)    11161 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_tokens.py
--rw-r--r--   0 root         (0) root         (0)    11280 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_list_response.py
--rw-r--r--   0 root         (0) root         (0)    12037 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/template_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    11540 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_create_request.py
--rw-r--r--   0 root         (0) root         (0)    11374 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_create_response.py
--rw-r--r--   0 root         (0) root         (0)    11351 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11811 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_rename_request.py
--rw-r--r--   0 root         (0) root         (0)    11374 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_rename_response.py
--rw-r--r--   0 root         (0) root         (0)    13062 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/update_integration_quote_section.py
--rw-r--r--   0 root         (0) root         (0)    18079 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/update_integration_quote_section_item.py
--rw-r--r--   0 root         (0) root         (0)    15023 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_by_pdf_request.py
--rw-r--r--   0 root         (0) root         (0)    17199 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_by_template_request.py
--rw-r--r--   0 root         (0) root         (0)    11331 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_list_response.py
--rw-r--r--   0 root         (0) root         (0)    11165 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_list_response_results.py
--rw-r--r--   0 root         (0) root         (0)    18035 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_request.py
--rw-r--r--   0 root         (0) root         (0)    12977 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_response.py
--rw-r--r--   0 root         (0) root         (0)    11949 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_status_enum.py
--rw-r--r--   0 root         (0) root         (0)    12516 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_status_response.py
--rw-r--r--   0 root         (0) root         (0)    14711 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_details_response.py
--rw-r--r--   0 root         (0) root         (0)    11790 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_error_enum.py
--rw-r--r--   0 root         (0) root         (0)    11590 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_http_status_code_group_enum.py
--rw-r--r--   0 root         (0) root         (0)    12864 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_item_response.py
--rw-r--r--   0 root         (0) root         (0)    11261 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_page_response.py
--rw-r--r--   0 root         (0) root         (0)    12480 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_trigger_enum.py
--rw-r--r--   0 root         (0) root         (0)    12307 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_create_request.py
--rw-r--r--   0 root         (0) root         (0)    13494 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_item_response.py
--rw-r--r--   0 root         (0) root         (0)    11331 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_list_response.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_patch_request.py
--rw-r--r--   0 root         (0) root         (0)    11745 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_payload_enum.py
--rw-r--r--   0 root         (0) root         (0)    11029 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_shared_key_response.py
--rw-r--r--   0 root         (0) root         (0)    11610 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_status_enum.py
--rw-r--r--   0 root         (0) root         (0)    12501 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_trigger_enum.py
--rw-r--r--   0 root         (0) root         (0)    81995 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.530000 pandadoc-python-client-6.1.0/pandadoc_client/models/
--rw-r--r--   0 root         (0) root         (0)    14065 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14105 2024-03-06 15:14:49.000000 pandadoc-python-client-6.1.0/pandadoc_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:14:51.530000 pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2865 2024-03-06 15:14:51.000000 pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9398 2024-03-06 15:14:51.000000 pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 15:14:51.000000 pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-06 15:14:51.000000 pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-06 15:14:51.000000 pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-06 15:14:51.530000 pandadoc-python-client-6.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1325 2024-03-06 15:14:50.000000 pandadoc-python-client-6.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.730001 pandadoc-python-client-6.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 08:40:52.000000 pandadoc-python-client-6.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2865 2024-04-08 08:40:54.730001 pandadoc-python-client-6.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13237 2024-04-08 08:40:52.000000 pandadoc-python-client-6.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.720001 pandadoc-python-client-6.2.0/pandadoc_client/
+-rw-r--r--   0 root         (0) root         (0)      666 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.720001 pandadoc-python-client-6.2.0/pandadoc_client/api/
+-rw-r--r--   0 root         (0) root         (0)      219 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13436 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/api_logs_api.py
+-rw-r--r--   0 root         (0) root         (0)    24668 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/contacts_api.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/content_library_items_api.py
+-rw-r--r--   0 root         (0) root         (0)    26634 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/document_attachments_api.py
+-rw-r--r--   0 root         (0) root         (0)    22895 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/document_recipients_api.py
+-rw-r--r--   0 root         (0) root         (0)    95468 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/documents_api.py
+-rw-r--r--   0 root         (0) root         (0)    33709 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/folders_api_api.py
+-rw-r--r--   0 root         (0) root         (0)     7569 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/forms_api.py
+-rw-r--r--   0 root         (0) root         (0)    14315 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/members_api.py
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/o_auth_2_0_authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/quotes_api.py
+-rw-r--r--   0 root         (0) root         (0)    22203 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/sections_api.py
+-rw-r--r--   0 root         (0) root         (0)    17365 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/templates_api.py
+-rw-r--r--   0 root         (0) root         (0)    17333 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/user_and_workspace_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    12699 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/webhook_events_api.py
+-rw-r--r--   0 root         (0) root         (0)    30255 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api/webhook_subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    37539 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.720001 pandadoc-python-client-6.2.0/pandadoc_client/apis/
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17253 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.730001 pandadoc-python-client-6.2.0/pandadoc_client/model/
+-rw-r--r--   0 root         (0) root         (0)      348 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11376 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/add_member_request.py
+-rw-r--r--   0 root         (0) root         (0)    12129 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/add_member_response.py
+-rw-r--r--   0 root         (0) root         (0)    14744 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/api_log_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    11261 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/api_log_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/api_log_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    13078 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/contact_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    13252 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/contact_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    11241 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/contact_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    13078 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/contact_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    11382 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11804 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    15564 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_response.py
+-rw-r--r--   0 root         (0) root         (0)    11801 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_response_created_by.py
+-rw-r--r--   0 root         (0) root         (0)    12256 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    11588 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/create_user_request_user.py
+-rw-r--r--   0 root         (0) root         (0)    11362 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/create_user_request_workspaces.py
+-rw-r--r--   0 root         (0) root         (0)    10960 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/create_user_response.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/create_workspace_request.py
+-rw-r--r--   0 root         (0) root         (0)    11128 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/create_workspace_response.py
+-rw-r--r--   0 root         (0) root         (0)    11971 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_attachment_response.py
+-rw-r--r--   0 root         (0) root         (0)    11801 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_attachment_response_created_by.py
+-rw-r--r--   0 root         (0) root         (0)    15800 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_pdf_request.py
+-rw-r--r--   0 root         (0) root         (0)    19930 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request.py
+-rw-r--r--   0 root         (0) root         (0)    12490 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_content_library_items.py
+-rw-r--r--   0 root         (0) root         (0)    11869 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_content_placeholders.py
+-rw-r--r--   0 root         (0) root         (0)    11240 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_images.py
+-rw-r--r--   0 root         (0) root         (0)    13007 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_recipients.py
+-rw-r--r--   0 root         (0) root         (0)    11245 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    11609 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_link_request.py
+-rw-r--r--   0 root         (0) root         (0)    11167 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_link_response.py
+-rw-r--r--   0 root         (0) root         (0)    20578 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    12508 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_content_library_items.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_content_placeholders.py
+-rw-r--r--   0 root         (0) root         (0)    11209 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_images.py
+-rw-r--r--   0 root         (0) root         (0)    12944 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_recipients.py
+-rw-r--r--   0 root         (0) root         (0)    13093 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_response.py
+-rw-r--r--   0 root         (0) root         (0)    11323 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_response_links.py
+-rw-r--r--   0 root         (0) root         (0)    18020 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    12015 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_created_by.py
+-rw-r--r--   0 root         (0) root         (0)    11198 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_grand_total.py
+-rw-r--r--   0 root         (0) root         (0)    11603 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_linked_objects.py
+-rw-r--r--   0 root         (0) root         (0)    15134 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_recipients.py
+-rw-r--r--   0 root         (0) root         (0)    11151 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_template.py
+-rw-r--r--   0 root         (0) root         (0)    11280 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    12228 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    13611 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_ordering_fields_enum.py
+-rw-r--r--   0 root         (0) root         (0)    11303 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_recipient_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    14516 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_recipient_edit_request.py
+-rw-r--r--   0 root         (0) root         (0)    11006 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)    13687 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request.py
+-rw-r--r--   0 root         (0) root         (0)    11517 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_forwarding_settings.py
+-rw-r--r--   0 root         (0) root         (0)    11450 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers.py
+-rw-r--r--   0 root         (0) root         (0)    12035 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers_group.py
+-rw-r--r--   0 root         (0) root         (0)    11335 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers_group_assignees.py
+-rw-r--r--   0 root         (0) root         (0)    11659 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers_steps.py
+-rw-r--r--   0 root         (0) root         (0)    12895 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_response.py
+-rw-r--r--   0 root         (0) root         (0)    13173 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_response_recipients.py
+-rw-r--r--   0 root         (0) root         (0)    12024 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_change_request.py
+-rw-r--r--   0 root         (0) root         (0)    13131 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_request_enum.py
+-rw-r--r--   0 root         (0) root         (0)    12718 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_response.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_transfer_all_ownership_request.py
+-rw-r--r--   0 root         (0) root         (0)    11120 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_transfer_ownership_request.py
+-rw-r--r--   0 root         (0) root         (0)    14861 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    12711 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/document_update_request_recipients.py
+-rw-r--r--   0 root         (0) root         (0)    11548 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    11374 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_create_response.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11811 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_rename_request.py
+-rw-r--r--   0 root         (0) root         (0)    11374 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_rename_response.py
+-rw-r--r--   0 root         (0) root         (0)    11466 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/form_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11757 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/form_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/linked_object_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    11987 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/linked_object_create_response.py
+-rw-r--r--   0 root         (0) root         (0)    11320 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/linked_object_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    14634 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/member_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    11231 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/member_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11834 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/o_auth2_access_token_response.py
+-rw-r--r--   0 root         (0) root         (0)    11731 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_response.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request.py
+-rw-r--r--   0 root         (0) root         (0)    11468 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request_row_options.py
+-rw-r--r--   0 root         (0) root         (0)    12095 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request_rows.py
+-rw-r--r--   0 root         (0) root         (0)    12057 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request_sections.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_discount.py
+-rw-r--r--   0 root         (0) root         (0)    17066 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_items.py
+-rw-r--r--   0 root         (0) root         (0)    11889 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_options.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_summary.py
+-rw-r--r--   0 root         (0) root         (0)    12991 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response.py
+-rw-r--r--   0 root         (0) root         (0)    11156 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_action.py
+-rw-r--r--   0 root         (0) root         (0)    11722 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_condition.py
+-rw-r--r--   0 root         (0) root         (0)    11170 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_condition_comparison.py
+-rw-r--r--   0 root         (0) root         (0)    11996 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_merge_rules.py
+-rw-r--r--   0 root         (0) root         (0)    11260 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_options.py
+-rw-r--r--   0 root         (0) root         (0)    11619 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_section_column.py
+-rw-r--r--   0 root         (0) root         (0)    16204 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_section_item.py
+-rw-r--r--   0 root         (0) root         (0)    14215 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_section_summary.py
+-rw-r--r--   0 root         (0) root         (0)    13078 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_sections.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_settings.py
+-rw-r--r--   0 root         (0) root         (0)    15278 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_summary.py
+-rw-r--r--   0 root         (0) root         (0)    11227 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_summary_discounts.py
+-rw-r--r--   0 root         (0) root         (0)    11230 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_summary_recurring_subtotal.py
+-rw-r--r--   0 root         (0) root         (0)    11545 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_section_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12147 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    11255 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_discounts.py
+-rw-r--r--   0 root         (0) root         (0)    11877 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_options.py
+-rw-r--r--   0 root         (0) root         (0)    12116 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_price_settings.py
+-rw-r--r--   0 root         (0) root         (0)    11281 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_price_settings_tiers.py
+-rw-r--r--   0 root         (0) root         (0)    11563 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_settings.py
+-rw-r--r--   0 root         (0) root         (0)    11164 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_settings1.py
+-rw-r--r--   0 root         (0) root         (0)    11232 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    12555 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_verification_settings.py
+-rw-r--r--   0 root         (0) root         (0)    11298 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_verification_settings_passcode_verification.py
+-rw-r--r--   0 root         (0) root         (0)    11307 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_verification_settings_phone_verification.py
+-rw-r--r--   0 root         (0) root         (0)    11376 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/ricipient_delivery_methods.py
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/section_info_response.py
+-rw-r--r--   0 root         (0) root         (0)    15880 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    11428 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_content_placeholders.py
+-rw-r--r--   0 root         (0) root         (0)    11403 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_images.py
+-rw-r--r--   0 root         (0) root         (0)    11712 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_preassigned_person.py
+-rw-r--r--   0 root         (0) root         (0)    12047 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_roles.py
+-rw-r--r--   0 root         (0) root         (0)    11161 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    11280 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    12037 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/template_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    11540 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    11374 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_create_response.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11811 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_rename_request.py
+-rw-r--r--   0 root         (0) root         (0)    11374 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_rename_response.py
+-rw-r--r--   0 root         (0) root         (0)    13062 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/update_integration_quote_section.py
+-rw-r--r--   0 root         (0) root         (0)    18079 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/update_integration_quote_section_item.py
+-rw-r--r--   0 root         (0) root         (0)    15023 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_by_pdf_request.py
+-rw-r--r--   0 root         (0) root         (0)    17199 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_by_template_request.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    11165 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_list_response_results.py
+-rw-r--r--   0 root         (0) root         (0)    18035 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_request.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_response.py
+-rw-r--r--   0 root         (0) root         (0)    11949 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)    12516 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_status_response.py
+-rw-r--r--   0 root         (0) root         (0)    14711 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    11790 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_error_enum.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_http_status_code_group_enum.py
+-rw-r--r--   0 root         (0) root         (0)    12864 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_item_response.py
+-rw-r--r--   0 root         (0) root         (0)    11261 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_page_response.py
+-rw-r--r--   0 root         (0) root         (0)    12480 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_trigger_enum.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    13494 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_item_response.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_patch_request.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_payload_enum.py
+-rw-r--r--   0 root         (0) root         (0)    11029 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_shared_key_response.py
+-rw-r--r--   0 root         (0) root         (0)    11610 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)    12501 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_trigger_enum.py
+-rw-r--r--   0 root         (0) root         (0)    81995 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.730001 pandadoc-python-client-6.2.0/pandadoc_client/models/
+-rw-r--r--   0 root         (0) root         (0)    14949 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14105 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/pandadoc_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:40:54.730001 pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2865 2024-04-08 08:40:54.000000 pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9997 2024-04-08 08:40:54.000000 pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 08:40:54.000000 pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-08 08:40:54.000000 pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-08 08:40:54.000000 pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 08:40:54.730001 pandadoc-python-client-6.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-08 08:40:53.000000 pandadoc-python-client-6.2.0/setup.py
```

### Comparing `pandadoc-python-client-6.1.0/LICENSE` & `pandadoc-python-client-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/PKG-INFO` & `pandadoc-python-client-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandadoc-python-client
-Version: 6.1.0
+Version: 6.2.0
 Summary: PandaDoc Public API
 Home-page: https://github.com/PandaDoc/pandadoc-api-python-client
 Author: PandaDoc
 Author-email: 
 License: MIT
 Keywords: OpenAPI,PandaDoc Public API
 Requires-Python: >=3.6
```

### Comparing `pandadoc-python-client-6.1.0/README.md` & `pandadoc-python-client-6.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 *DocumentAttachmentsApi* | [**create_document_attachment**](docs/DocumentAttachmentsApi.md#create_document_attachment) | **POST** /public/v1/documents/{id}/attachments | Document Attachment Create
 *DocumentAttachmentsApi* | [**delete_document_attachment**](docs/DocumentAttachmentsApi.md#delete_document_attachment) | **DELETE** /public/v1/documents/{id}/attachments/{attachment_id} | Document Attachment Delete
 *DocumentAttachmentsApi* | [**details_document_attachment**](docs/DocumentAttachmentsApi.md#details_document_attachment) | **GET** /public/v1/documents/{id}/attachments/{attachment_id} | Document Attachment Details
 *DocumentAttachmentsApi* | [**download_document_attachment**](docs/DocumentAttachmentsApi.md#download_document_attachment) | **GET** /public/v1/documents/{id}/attachments/{attachment_id}/download | Document Attachment Download
 *DocumentAttachmentsApi* | [**list_document_attachments**](docs/DocumentAttachmentsApi.md#list_document_attachments) | **GET** /public/v1/documents/{id}/attachments | Document Attachment List
 *DocumentRecipientsApi* | [**add_document_recipient**](docs/DocumentRecipientsApi.md#add_document_recipient) | **POST** /public/v1/documents/{id}/recipients | Add Document Recipient
 *DocumentRecipientsApi* | [**delete_document_recipient**](docs/DocumentRecipientsApi.md#delete_document_recipient) | **DELETE** /public/v1/documents/{id}/recipients/{recipient_id} | Delete Document Recipient
-*DocumentRecipientsApi* | [**edit_document_recipient**](docs/DocumentRecipientsApi.md#edit_document_recipient) | **PATCH** /public/v1/documents/{id}/recipients/{recipient_id} | Edit Document Recipient
+*DocumentRecipientsApi* | [**edit_document_recipient**](docs/DocumentRecipientsApi.md#edit_document_recipient) | **PATCH** /public/v1/documents/{id}/recipients/recipient/{recipient_id} | Edit Document Recipient
 *DocumentRecipientsApi* | [**reassign_document_recipient**](docs/DocumentRecipientsApi.md#reassign_document_recipient) | **POST** /public/v1/documents/{id}/recipients/{recipient_id}/reassign | Reassign Document Recipient
 *DocumentsApi* | [**change_document_status**](docs/DocumentsApi.md#change_document_status) | **PATCH** /public/v1/documents/{id}/status | Document status change
 *DocumentsApi* | [**create_document**](docs/DocumentsApi.md#create_document) | **POST** /public/v1/documents | Create document
 *DocumentsApi* | [**create_document_link**](docs/DocumentsApi.md#create_document_link) | **POST** /public/v1/documents/{id}/session | Create a Document Link
 *DocumentsApi* | [**create_linked_object**](docs/DocumentsApi.md#create_linked_object) | **POST** /public/v1/documents/{id}/linked-objects | Create Linked Object
 *DocumentsApi* | [**delete_document**](docs/DocumentsApi.md#delete_document) | **DELETE** /public/v1/documents/{id} | Delete document by id
 *DocumentsApi* | [**delete_linked_object**](docs/DocumentsApi.md#delete_linked_object) | **DELETE** /public/v1/documents/{id}/linked-objects/{linked_object_id} | Delete Linked Object
@@ -127,14 +127,17 @@
 *SectionsApi* | [**list_sections**](docs/SectionsApi.md#list_sections) | **GET** /public/v1/documents/{document_id}/sections | List sections
 *SectionsApi* | [**section_details**](docs/SectionsApi.md#section_details) | **GET** /public/v1/documents/{document_id}/sections/uploads/{upload_id} | Section details
 *SectionsApi* | [**section_info**](docs/SectionsApi.md#section_info) | **GET** /public/v1/documents/{document_id}/sections/{section_id} | Section Info
 *SectionsApi* | [**upload_section**](docs/SectionsApi.md#upload_section) | **POST** /public/v1/documents/{document_id}/sections/uploads | Upload section
 *TemplatesApi* | [**delete_template**](docs/TemplatesApi.md#delete_template) | **DELETE** /public/v1/templates/{id} | Delete Template
 *TemplatesApi* | [**details_template**](docs/TemplatesApi.md#details_template) | **GET** /public/v1/templates/{id}/details | Details Template
 *TemplatesApi* | [**list_templates**](docs/TemplatesApi.md#list_templates) | **GET** /public/v1/templates | List Templates
+*UserAndWorkspaceManagementApi* | [**add_member**](docs/UserAndWorkspaceManagementApi.md#add_member) | **POST** /public/v1/workspaces/{workspace_id}/members | Add member
+*UserAndWorkspaceManagementApi* | [**create_user**](docs/UserAndWorkspaceManagementApi.md#create_user) | **POST** /public/v1/users | Create User
+*UserAndWorkspaceManagementApi* | [**create_workspace**](docs/UserAndWorkspaceManagementApi.md#create_workspace) | **POST** /public/v1/workspaces | Create Workspace
 *WebhookEventsApi* | [**details_webhook_event**](docs/WebhookEventsApi.md#details_webhook_event) | **GET** /public/v1/webhook-events/{id} | Get webhook event by uuid
 *WebhookEventsApi* | [**list_webhook_event**](docs/WebhookEventsApi.md#list_webhook_event) | **GET** /public/v1/webhook-events | Get webhook event page
 *WebhookSubscriptionsApi* | [**create_webhook_subscription**](docs/WebhookSubscriptionsApi.md#create_webhook_subscription) | **POST** /public/v1/webhook-subscriptions | Create webhook subscription
 *WebhookSubscriptionsApi* | [**delete_webhook_subscription**](docs/WebhookSubscriptionsApi.md#delete_webhook_subscription) | **DELETE** /public/v1/webhook-subscriptions/{id} | Delete webhook subscription
 *WebhookSubscriptionsApi* | [**details_webhook_subscription**](docs/WebhookSubscriptionsApi.md#details_webhook_subscription) | **GET** /public/v1/webhook-subscriptions/{id} | Get webhook subscription by uuid
 *WebhookSubscriptionsApi* | [**list_webhook_subscriptions**](docs/WebhookSubscriptionsApi.md#list_webhook_subscriptions) | **GET** /public/v1/webhook-subscriptions | Get all webhook subscriptions
 *WebhookSubscriptionsApi* | [**update_webhook_subscription**](docs/WebhookSubscriptionsApi.md#update_webhook_subscription) | **PATCH** /public/v1/webhook-subscriptions/{id} | Update webhook subscription
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/__init__.py` & `pandadoc-python-client-6.2.0/pandadoc_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     PandaDoc Public API documentation  # noqa: E501
 
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "6.1.0"
+__version__ = "6.2.0"
 
 # import ApiClient
 from pandadoc_client.api_client import ApiClient
 
 # import Configuration
 from pandadoc_client.configuration import Configuration
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/api_logs_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/api_logs_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/contacts_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/contacts_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/content_library_items_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/content_library_items_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/document_attachments_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/document_attachments_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/document_recipients_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/document_recipients_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         self.edit_document_recipient_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'apiKey',
                     'oauth2'
                 ],
-                'endpoint_path': '/public/v1/documents/{id}/recipients/{recipient_id}',
+                'endpoint_path': '/public/v1/documents/{id}/recipients/recipient/{recipient_id}',
                 'operation_id': 'edit_document_recipient',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/documents_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/folders_api_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/folders_api_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/forms_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/forms_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/members_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/members_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/o_auth_2_0_authentication_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/o_auth_2_0_authentication_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/quotes_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/quotes_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/sections_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/sections_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -218,43 +218,54 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'document_id',
                     'upload_section_request',
+                    'merge_field_scope',
                 ],
                 'required': [
                     'document_id',
                     'upload_section_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'merge_field_scope',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('merge_field_scope',): {
+
+                        "DOCUMENT": "document",
+                        "UPLOAD": "upload"
+                    },
                 },
                 'openapi_types': {
                     'document_id':
                         (str,),
                     'upload_section_request':
                         (UploadSectionRequest,),
+                    'merge_field_scope':
+                        (str,),
                 },
                 'attribute_map': {
                     'document_id': 'document_id',
+                    'merge_field_scope': 'merge_field_scope',
                 },
                 'location_map': {
                     'document_id': 'path',
                     'upload_section_request': 'body',
+                    'merge_field_scope': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -521,14 +532,15 @@
         >>> result = thread.get()
 
         Args:
             document_id (str): Document ID
             upload_section_request (UploadSectionRequest): Use a PandaDoc template or an existing PDF to upload a section. See the creation request examples [by template](/schemas/UploadSectionByTemplateRequest) and [by pdf](/schemas/UploadSectionByPdfRequest) 
 
         Keyword Args:
+            merge_field_scope (str): Determines how the fields are mapped when creating a section.   * document: Default value. The fields of the entire document are updated.   * upload: Only the fields from the created section are updated. The merge field is appended with the upload ID. . [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/templates_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/webhook_events_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/webhook_events_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api/webhook_subscriptions_api.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api/webhook_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/api_client.py` & `pandadoc-python-client-6.2.0/pandadoc_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'pandadoc_python_client/6.1.0'
+        self.user_agent = 'pandadoc_python_client/6.2.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/apis/__init__.py` & `pandadoc-python-client-6.2.0/pandadoc_client/apis/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 from pandadoc_client.api.folders_api_api import FoldersAPIApi
 from pandadoc_client.api.forms_api import FormsApi
 from pandadoc_client.api.members_api import MembersApi
 from pandadoc_client.api.o_auth_2_0_authentication_api import OAuth20AuthenticationApi
 from pandadoc_client.api.quotes_api import QuotesApi
 from pandadoc_client.api.sections_api import SectionsApi
 from pandadoc_client.api.templates_api import TemplatesApi
+from pandadoc_client.api.user_and_workspace_management_api import UserAndWorkspaceManagementApi
 from pandadoc_client.api.webhook_events_api import WebhookEventsApi
 from pandadoc_client.api.webhook_subscriptions_api import WebhookSubscriptionsApi
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/configuration.py` & `pandadoc-python-client-6.2.0/pandadoc_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,16 +410,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.0.0\n"\
-               "SDK Package Version: 6.1.0".\
+               "Version of the API: 6.2.0\n"\
+               "SDK Package Version: 6.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/exceptions.py` & `pandadoc-python-client-6.2.0/pandadoc_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/api_log_details_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/api_log_details_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/api_log_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/api_log_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/api_log_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/api_log_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/contact_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/contact_update_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class ContactCreateRequest(ModelNormal):
+class ContactUpdateRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,15 +76,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
             'first_name': (str, none_type,),  # noqa: E501
             'last_name': (str, none_type,),  # noqa: E501
             'company': (str, none_type,),  # noqa: E501
             'job_title': (str, none_type,),  # noqa: E501
             'phone': (str, none_type,),  # noqa: E501
             'state': (str, none_type,),  # noqa: E501
             'street_address': (str, none_type,),  # noqa: E501
@@ -113,19 +113,16 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
-        """ContactCreateRequest - a model defined in OpenAPI
-
-        Args:
-            email (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ContactUpdateRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -150,14 +147,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            email (str, none_type): [optional]  # noqa: E501
             first_name (str, none_type): [optional]  # noqa: E501
             last_name (str, none_type): [optional]  # noqa: E501
             company (str, none_type): [optional]  # noqa: E501
             job_title (str, none_type): [optional]  # noqa: E501
             phone (str, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
             street_address (str, none_type): [optional]  # noqa: E501
@@ -186,15 +184,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -207,19 +204,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, email, *args, **kwargs):  # noqa: E501
-        """ContactCreateRequest - a model defined in OpenAPI
-
-        Args:
-            email (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ContactUpdateRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,14 +238,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            email (str, none_type): [optional]  # noqa: E501
             first_name (str, none_type): [optional]  # noqa: E501
             last_name (str, none_type): [optional]  # noqa: E501
             company (str, none_type): [optional]  # noqa: E501
             job_title (str, none_type): [optional]  # noqa: E501
             phone (str, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
             street_address (str, none_type): [optional]  # noqa: E501
@@ -278,15 +273,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/contact_details_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/contact_details_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
             'first_name': (str, none_type,),  # noqa: E501
             'last_name': (str, none_type,),  # noqa: E501
             'company': (str, none_type,),  # noqa: E501
             'job_title': (str, none_type,),  # noqa: E501
             'phone': (str, none_type,),  # noqa: E501
             'state': (str, none_type,),  # noqa: E501
             'street_address': (str, none_type,),  # noqa: E501
@@ -150,15 +150,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
             first_name (str, none_type): [optional]  # noqa: E501
             last_name (str, none_type): [optional]  # noqa: E501
             company (str, none_type): [optional]  # noqa: E501
             job_title (str, none_type): [optional]  # noqa: E501
             phone (str, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
             street_address (str, none_type): [optional]  # noqa: E501
@@ -242,15 +242,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
             first_name (str, none_type): [optional]  # noqa: E501
             last_name (str, none_type): [optional]  # noqa: E501
             company (str, none_type): [optional]  # noqa: E501
             job_title (str, none_type): [optional]  # noqa: E501
             phone (str, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
             street_address (str, none_type): [optional]  # noqa: E501
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/contact_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/contact_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/contact_update_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/contact_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class ContactUpdateRequest(ModelNormal):
+class ContactCreateRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,15 +76,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
             'first_name': (str, none_type,),  # noqa: E501
             'last_name': (str, none_type,),  # noqa: E501
             'company': (str, none_type,),  # noqa: E501
             'job_title': (str, none_type,),  # noqa: E501
             'phone': (str, none_type,),  # noqa: E501
             'state': (str, none_type,),  # noqa: E501
             'street_address': (str, none_type,),  # noqa: E501
@@ -114,15 +114,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ContactUpdateRequest - a model defined in OpenAPI
+        """ContactCreateRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -147,15 +147,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
             first_name (str, none_type): [optional]  # noqa: E501
             last_name (str, none_type): [optional]  # noqa: E501
             company (str, none_type): [optional]  # noqa: E501
             job_title (str, none_type): [optional]  # noqa: E501
             phone (str, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
             street_address (str, none_type): [optional]  # noqa: E501
@@ -205,15 +205,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ContactUpdateRequest - a model defined in OpenAPI
+        """ContactCreateRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,15 +238,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
             first_name (str, none_type): [optional]  # noqa: E501
             last_name (str, none_type): [optional]  # noqa: E501
             company (str, none_type): [optional]  # noqa: E501
             job_title (str, none_type): [optional]  # noqa: E501
             phone (str, none_type): [optional]  # noqa: E501
             state (str, none_type): [optional]  # noqa: E501
             street_address (str, none_type): [optional]  # noqa: E501
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/content_library_item_response_created_by.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/content_library_item_response_created_by.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_attachment_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_attachment_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_attachment_response_created_by.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_attachment_response_created_by.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_pdf_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_pdf_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_content_library_items.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_content_library_items.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_content_placeholders.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_content_placeholders.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_images.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_images.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_recipients.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from pandadoc_client.model.pricing_table_request_sections import PricingTableRequestSections
+    globals()['PricingTableRequestSections'] = PricingTableRequestSections
 
-class DocumentCreateByTemplateRequestRecipients(ModelNormal):
+
+class PricingTableRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -61,61 +65,61 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'email': (str,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
-            'role': (str,),  # noqa: E501
-            'signing_order': (int, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'data_merge': (bool,),  # noqa: E501
+            'options': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'sections': ([PricingTableRequestSections],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
-        'role': 'role',  # noqa: E501
-        'signing_order': 'signing_order',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'data_merge': 'data_merge',  # noqa: E501
+        'options': 'options',  # noqa: E501
+        'sections': 'sections',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
-        """DocumentCreateByTemplateRequestRecipients - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """PricingTableRequest - a model defined in OpenAPI
 
         Args:
-            email (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,18 +144,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            role (str): [optional]  # noqa: E501
-            signing_order (int, none_type): [optional]  # noqa: E501
+            data_merge (bool): When set to true all field names in data rows must be passed as external names defined in the template.. [optional]  # noqa: E501
+            options ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            sections ([PricingTableRequestSections]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +174,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +195,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, email, *args, **kwargs):  # noqa: E501
-        """DocumentCreateByTemplateRequestRecipients - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """PricingTableRequest - a model defined in OpenAPI
 
         Args:
-            email (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,18 +232,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            role (str): [optional]  # noqa: E501
-            signing_order (int, none_type): [optional]  # noqa: E501
+            data_merge (bool): When set to true all field names in data rows must be passed as external names defined in the template.. [optional]  # noqa: E501
+            options ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            sections ([PricingTableRequestSections]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,15 +260,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_by_template_request_tokens.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_by_template_request_tokens.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_link_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_link_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_link_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_link_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_content_library_items.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_content_library_items.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_content_placeholders.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_content_placeholders.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_images.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_request_images.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_request_recipients.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_images.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class DocumentCreateRequestRecipients(ModelNormal):
+class TemplateDetailsResponseImages(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,46 +76,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
-            'role': (str,),  # noqa: E501
-            'signing_order': (int,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'block_uuid': (str,),  # noqa: E501
+            'urls': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
-        'role': 'role',  # noqa: E501
-        'signing_order': 'signing_order',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'block_uuid': 'block_uuid',  # noqa: E501
+        'urls': 'urls',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
-        """DocumentCreateRequestRecipients - a model defined in OpenAPI
-
-        Args:
-            email (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TemplateDetailsResponseImages - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,18 +133,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            role (str): [optional]  # noqa: E501
-            signing_order (int): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            block_uuid (str): [optional]  # noqa: E501
+            urls ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +163,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +183,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, email, *args, **kwargs):  # noqa: E501
-        """DocumentCreateRequestRecipients - a model defined in OpenAPI
-
-        Args:
-            email (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TemplateDetailsResponseImages - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,18 +217,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            role (str): [optional]  # noqa: E501
-            signing_order (int): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            block_uuid (str): [optional]  # noqa: E501
+            urls ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,15 +245,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_create_response_links.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_create_response_links.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_created_by.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_created_by.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_grand_total.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_grand_total.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_linked_objects.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_linked_objects.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_recipients.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_recipient_edit_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from pandadoc_client.model.recipient_redirect import RecipientRedirect
     from pandadoc_client.model.recipient_verification_settings import RecipientVerificationSettings
+    from pandadoc_client.model.ricipient_delivery_methods import RicipientDeliveryMethods
+    globals()['RecipientRedirect'] = RecipientRedirect
     globals()['RecipientVerificationSettings'] = RecipientVerificationSettings
+    globals()['RicipientDeliveryMethods'] = RicipientDeliveryMethods
 
 
-class DocumentDetailsResponseRecipients(ModelNormal):
+class DocumentRecipientEditRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -82,59 +86,59 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'recipient_type': (str,),  # noqa: E501
-            'role': (str,),  # noqa: E501
-            'roles': ([str],),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
-            'signing_order': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'contact_id': (str,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'has_completed': (bool,),  # noqa: E501
-            'shared_link': (str,),  # noqa: E501
-            'signature_date': (str, none_type,),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
+            'phone': (str, none_type,),  # noqa: E501
+            'delivery_methods': (RicipientDeliveryMethods,),  # noqa: E501
+            'first_name': (str, none_type,),  # noqa: E501
+            'last_name': (str, none_type,),  # noqa: E501
+            'company': (str, none_type,),  # noqa: E501
+            'job_title': (str, none_type,),  # noqa: E501
+            'state': (str, none_type,),  # noqa: E501
+            'street_address': (str, none_type,),  # noqa: E501
+            'city': (str, none_type,),  # noqa: E501
+            'postal_code': (str, none_type,),  # noqa: E501
             'verification_settings': (RecipientVerificationSettings,),  # noqa: E501
+            'redirect': (RecipientRedirect,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'recipient_type': 'recipient_type',  # noqa: E501
-        'role': 'role',  # noqa: E501
-        'roles': 'roles',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
-        'signing_order': 'signing_order',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'contact_id': 'contact_id',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
         'email': 'email',  # noqa: E501
-        'has_completed': 'has_completed',  # noqa: E501
-        'shared_link': 'shared_link',  # noqa: E501
-        'signature_date': 'signature_date',  # noqa: E501
+        'phone': 'phone',  # noqa: E501
+        'delivery_methods': 'delivery_methods',  # noqa: E501
+        'first_name': 'first_name',  # noqa: E501
+        'last_name': 'last_name',  # noqa: E501
+        'company': 'company',  # noqa: E501
+        'job_title': 'job_title',  # noqa: E501
+        'state': 'state',  # noqa: E501
+        'street_address': 'street_address',  # noqa: E501
+        'city': 'city',  # noqa: E501
+        'postal_code': 'postal_code',  # noqa: E501
         'verification_settings': 'verification_settings',  # noqa: E501
+        'redirect': 'redirect',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DocumentDetailsResponseRecipients - a model defined in OpenAPI
+        """DocumentRecipientEditRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -159,27 +163,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            recipient_type (str): [optional]  # noqa: E501
-            role (str): [optional]  # noqa: E501
-            roles ([str]): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            signing_order (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            contact_id (str): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            has_completed (bool): [optional]  # noqa: E501
-            shared_link (str): [optional]  # noqa: E501
-            signature_date (str, none_type): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
+            phone (str, none_type): [optional]  # noqa: E501
+            delivery_methods (RicipientDeliveryMethods): [optional]  # noqa: E501
+            first_name (str, none_type): [optional]  # noqa: E501
+            last_name (str, none_type): [optional]  # noqa: E501
+            company (str, none_type): [optional]  # noqa: E501
+            job_title (str, none_type): [optional]  # noqa: E501
+            state (str, none_type): [optional]  # noqa: E501
+            street_address (str, none_type): [optional]  # noqa: E501
+            city (str, none_type): [optional]  # noqa: E501
+            postal_code (str, none_type): [optional]  # noqa: E501
             verification_settings (RecipientVerificationSettings): [optional]  # noqa: E501
+            redirect (RecipientRedirect): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,15 +224,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DocumentDetailsResponseRecipients - a model defined in OpenAPI
+        """DocumentRecipientEditRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,27 +257,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            recipient_type (str): [optional]  # noqa: E501
-            role (str): [optional]  # noqa: E501
-            roles ([str]): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            signing_order (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            contact_id (str): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            has_completed (bool): [optional]  # noqa: E501
-            shared_link (str): [optional]  # noqa: E501
-            signature_date (str, none_type): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
+            phone (str, none_type): [optional]  # noqa: E501
+            delivery_methods (RicipientDeliveryMethods): [optional]  # noqa: E501
+            first_name (str, none_type): [optional]  # noqa: E501
+            last_name (str, none_type): [optional]  # noqa: E501
+            company (str, none_type): [optional]  # noqa: E501
+            job_title (str, none_type): [optional]  # noqa: E501
+            state (str, none_type): [optional]  # noqa: E501
+            street_address (str, none_type): [optional]  # noqa: E501
+            city (str, none_type): [optional]  # noqa: E501
+            postal_code (str, none_type): [optional]  # noqa: E501
             verification_settings (RecipientVerificationSettings): [optional]  # noqa: E501
+            redirect (RecipientRedirect): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_details_response_template.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_details_response_template.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_ordering_fields_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_ordering_fields_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_recipient_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_recipient_create_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_recipient_edit_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,19 +25,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from pandadoc_client.model.recipient_verification_settings import RecipientVerificationSettings
-    globals()['RecipientVerificationSettings'] = RecipientVerificationSettings
+    from pandadoc_client.model.quote_response_summary_discounts import QuoteResponseSummaryDiscounts
+    from pandadoc_client.model.quote_response_summary_recurring_subtotal import QuoteResponseSummaryRecurringSubtotal
+    globals()['QuoteResponseSummaryDiscounts'] = QuoteResponseSummaryDiscounts
+    globals()['QuoteResponseSummaryRecurringSubtotal'] = QuoteResponseSummaryRecurringSubtotal
 
 
-class DocumentRecipientEditRequest(ModelNormal):
+class QuoteResponseSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -82,55 +84,61 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'email': (str,),  # noqa: E501
-            'first_name': (str, none_type,),  # noqa: E501
-            'last_name': (str, none_type,),  # noqa: E501
-            'company': (str, none_type,),  # noqa: E501
-            'job_title': (str, none_type,),  # noqa: E501
-            'phone': (str, none_type,),  # noqa: E501
-            'state': (str, none_type,),  # noqa: E501
-            'street_address': (str, none_type,),  # noqa: E501
-            'city': (str, none_type,),  # noqa: E501
-            'postal_code': (str, none_type,),  # noqa: E501
-            'verification_settings': (RecipientVerificationSettings,),  # noqa: E501
+            'total': (str,),  # noqa: E501
+            'subtotal': (str, none_type,),  # noqa: E501
+            'one_time_subtotal': (str, none_type,),  # noqa: E501
+            'recurring_subtotal': ([QuoteResponseSummaryRecurringSubtotal], none_type,),  # noqa: E501
+            'total_qty': (str, none_type,),  # noqa: E501
+            'discounts': ({str: (QuoteResponseSummaryDiscounts,)}, none_type,),  # noqa: E501
+            'taxes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'fees': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'custom_fields': ({str: (str,)}, none_type,),  # noqa: E501
+            'total_discount': (str, none_type,),  # noqa: E501
+            'total_tax': (str, none_type,),  # noqa: E501
+            'total_fee': (str, none_type,),  # noqa: E501
+            'total_savings': (str, none_type,),  # noqa: E501
+            'total_contract_value': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
-        'company': 'company',  # noqa: E501
-        'job_title': 'job_title',  # noqa: E501
-        'phone': 'phone',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'street_address': 'street_address',  # noqa: E501
-        'city': 'city',  # noqa: E501
-        'postal_code': 'postal_code',  # noqa: E501
-        'verification_settings': 'verification_settings',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'subtotal': 'subtotal',  # noqa: E501
+        'one_time_subtotal': 'one_time_subtotal',  # noqa: E501
+        'recurring_subtotal': 'recurring_subtotal',  # noqa: E501
+        'total_qty': 'total_qty',  # noqa: E501
+        'discounts': 'discounts',  # noqa: E501
+        'taxes': 'taxes',  # noqa: E501
+        'fees': 'fees',  # noqa: E501
+        'custom_fields': 'custom_fields',  # noqa: E501
+        'total_discount': 'total_discount',  # noqa: E501
+        'total_tax': 'total_tax',  # noqa: E501
+        'total_fee': 'total_fee',  # noqa: E501
+        'total_savings': 'total_savings',  # noqa: E501
+        'total_contract_value': 'total_contract_value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DocumentRecipientEditRequest - a model defined in OpenAPI
+        """QuoteResponseSummary - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,25 +163,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): [optional]  # noqa: E501
-            first_name (str, none_type): [optional]  # noqa: E501
-            last_name (str, none_type): [optional]  # noqa: E501
-            company (str, none_type): [optional]  # noqa: E501
-            job_title (str, none_type): [optional]  # noqa: E501
-            phone (str, none_type): [optional]  # noqa: E501
-            state (str, none_type): [optional]  # noqa: E501
-            street_address (str, none_type): [optional]  # noqa: E501
-            city (str, none_type): [optional]  # noqa: E501
-            postal_code (str, none_type): [optional]  # noqa: E501
-            verification_settings (RecipientVerificationSettings): [optional]  # noqa: E501
+            total (str): [optional]  # noqa: E501
+            subtotal (str, none_type): [optional]  # noqa: E501
+            one_time_subtotal (str, none_type): [optional]  # noqa: E501
+            recurring_subtotal ([QuoteResponseSummaryRecurringSubtotal], none_type): [optional]  # noqa: E501
+            total_qty (str, none_type): [optional]  # noqa: E501
+            discounts ({str: (QuoteResponseSummaryDiscounts,)}, none_type): [optional]  # noqa: E501
+            taxes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            fees ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            custom_fields ({str: (str,)}, none_type): [optional]  # noqa: E501
+            total_discount (str, none_type): [optional]  # noqa: E501
+            total_tax (str, none_type): [optional]  # noqa: E501
+            total_fee (str, none_type): [optional]  # noqa: E501
+            total_savings (str, none_type): [optional]  # noqa: E501
+            total_contract_value (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +225,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DocumentRecipientEditRequest - a model defined in OpenAPI
+        """QuoteResponseSummary - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -247,25 +258,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): [optional]  # noqa: E501
-            first_name (str, none_type): [optional]  # noqa: E501
-            last_name (str, none_type): [optional]  # noqa: E501
-            company (str, none_type): [optional]  # noqa: E501
-            job_title (str, none_type): [optional]  # noqa: E501
-            phone (str, none_type): [optional]  # noqa: E501
-            state (str, none_type): [optional]  # noqa: E501
-            street_address (str, none_type): [optional]  # noqa: E501
-            city (str, none_type): [optional]  # noqa: E501
-            postal_code (str, none_type): [optional]  # noqa: E501
-            verification_settings (RecipientVerificationSettings): [optional]  # noqa: E501
+            total (str): [optional]  # noqa: E501
+            subtotal (str, none_type): [optional]  # noqa: E501
+            one_time_subtotal (str, none_type): [optional]  # noqa: E501
+            recurring_subtotal ([QuoteResponseSummaryRecurringSubtotal], none_type): [optional]  # noqa: E501
+            total_qty (str, none_type): [optional]  # noqa: E501
+            discounts ({str: (QuoteResponseSummaryDiscounts,)}, none_type): [optional]  # noqa: E501
+            taxes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            fees ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            custom_fields ({str: (str,)}, none_type): [optional]  # noqa: E501
+            total_discount (str, none_type): [optional]  # noqa: E501
+            total_tax (str, none_type): [optional]  # noqa: E501
+            total_fee (str, none_type): [optional]  # noqa: E501
+            total_savings (str, none_type): [optional]  # noqa: E501
+            total_contract_value (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_recipient_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_recipient_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_forwarding_settings.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_forwarding_settings.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers_group.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers_group.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers_group_assignees.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers_group_assignees.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_request_selected_approvers_steps.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_send_request_selected_approvers_steps.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_send_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class DocumentSendResponse(ModelNormal):
+class DocumentStatusResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -80,47 +80,47 @@
                 and the value is attribute type.
         """
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'date_created': (str,),  # noqa: E501
-            'date_modified': (str,),  # noqa: E501
-            'expiration_date': (str,),  # noqa: E501
-            'version': (str,),  # noqa: E501
+            'date_modified': (str, none_type,),  # noqa: E501
+            'date_completed': (str, none_type,),  # noqa: E501
+            'expiration_date': (str, none_type,),  # noqa: E501
+            'version': (str, none_type,),  # noqa: E501
             'uuid': (str,),  # noqa: E501
-            'shared_link': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'status': 'status',  # noqa: E501
         'date_created': 'date_created',  # noqa: E501
         'date_modified': 'date_modified',  # noqa: E501
+        'date_completed': 'date_completed',  # noqa: E501
         'expiration_date': 'expiration_date',  # noqa: E501
         'version': 'version',  # noqa: E501
         'uuid': 'uuid',  # noqa: E501
-        'shared_link': 'shared_link',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DocumentSendResponse - a model defined in OpenAPI
+        """DocumentStatusResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,19 +149,19 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
             status (str): [optional]  # noqa: E501
             date_created (str): [optional]  # noqa: E501
-            date_modified (str): [optional]  # noqa: E501
-            expiration_date (str): [optional]  # noqa: E501
-            version (str): [optional]  # noqa: E501
+            date_modified (str, none_type): [optional]  # noqa: E501
+            date_completed (str, none_type): [optional]  # noqa: E501
+            expiration_date (str, none_type): [optional]  # noqa: E501
+            version (str, none_type): [optional]  # noqa: E501
             uuid (str): [optional]  # noqa: E501
-            shared_link (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -202,15 +202,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DocumentSendResponse - a model defined in OpenAPI
+        """DocumentStatusResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,19 +239,19 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
             status (str): [optional]  # noqa: E501
             date_created (str): [optional]  # noqa: E501
-            date_modified (str): [optional]  # noqa: E501
-            expiration_date (str): [optional]  # noqa: E501
-            version (str): [optional]  # noqa: E501
+            date_modified (str, none_type): [optional]  # noqa: E501
+            date_completed (str, none_type): [optional]  # noqa: E501
+            expiration_date (str, none_type): [optional]  # noqa: E501
+            version (str, none_type): [optional]  # noqa: E501
             uuid (str): [optional]  # noqa: E501
-            shared_link (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_change_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_change_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_request_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_status_request_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_status_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class DocumentStatusResponse(ModelNormal):
+class PricingTableResponseSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,64 +63,54 @@
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'date_created': (str,),  # noqa: E501
-            'date_modified': (str, none_type,),  # noqa: E501
-            'date_completed': (str, none_type,),  # noqa: E501
-            'expiration_date': (str, none_type,),  # noqa: E501
-            'version': (str, none_type,),  # noqa: E501
-            'uuid': (str,),  # noqa: E501
+            'subtotal': (str, none_type,),  # noqa: E501
+            'total': (str, none_type,),  # noqa: E501
+            'discount': (str, none_type,),  # noqa: E501
+            'tax': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'date_created': 'date_created',  # noqa: E501
-        'date_modified': 'date_modified',  # noqa: E501
-        'date_completed': 'date_completed',  # noqa: E501
-        'expiration_date': 'expiration_date',  # noqa: E501
-        'version': 'version',  # noqa: E501
-        'uuid': 'uuid',  # noqa: E501
+        'subtotal': 'subtotal',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'discount': 'discount',  # noqa: E501
+        'tax': 'tax',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DocumentStatusResponse - a model defined in OpenAPI
+        """PricingTableResponseSummary - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,23 +135,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            status (str): [optional]  # noqa: E501
-            date_created (str): [optional]  # noqa: E501
-            date_modified (str, none_type): [optional]  # noqa: E501
-            date_completed (str, none_type): [optional]  # noqa: E501
-            expiration_date (str, none_type): [optional]  # noqa: E501
-            version (str, none_type): [optional]  # noqa: E501
-            uuid (str): [optional]  # noqa: E501
+            subtotal (str, none_type): [optional]  # noqa: E501
+            total (str, none_type): [optional]  # noqa: E501
+            discount (str, none_type): [optional]  # noqa: E501
+            tax (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -202,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DocumentStatusResponse - a model defined in OpenAPI
+        """PricingTableResponseSummary - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,23 +220,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            status (str): [optional]  # noqa: E501
-            date_created (str): [optional]  # noqa: E501
-            date_modified (str, none_type): [optional]  # noqa: E501
-            date_completed (str, none_type): [optional]  # noqa: E501
-            expiration_date (str, none_type): [optional]  # noqa: E501
-            version (str, none_type): [optional]  # noqa: E501
-            uuid (str): [optional]  # noqa: E501
+            subtotal (str, none_type): [optional]  # noqa: E501
+            total (str, none_type): [optional]  # noqa: E501
+            discount (str, none_type): [optional]  # noqa: E501
+            tax (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_transfer_all_ownership_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_transfer_all_ownership_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_transfer_ownership_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_transfer_ownership_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_update_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_update_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/document_update_request_recipients.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_rename_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class DocumentUpdateRequestRecipients(ModelNormal):
+class TemplatesFolderRenameResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,41 +76,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
+            'uuid': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'date_created': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
+        'uuid': 'uuid',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'date_created': 'date_created',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DocumentUpdateRequestRecipients - a model defined in OpenAPI
+        """TemplatesFolderRenameResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,18 +133,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
+            uuid (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            date_created (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DocumentUpdateRequestRecipients - a model defined in OpenAPI
+        """TemplatesFolderRenameResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,18 +217,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
+            uuid (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            date_created (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_create_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_create_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_create_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_rename_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_rename_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/documents_folder_rename_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/documents_folder_rename_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/form_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/form_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/form_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/form_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/linked_object_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/linked_object_create_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/linked_object_create_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/linked_object_create_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/linked_object_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/linked_object_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/member_details_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/member_details_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/member_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/member_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/o_auth2_access_token_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/o_auth2_access_token_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request_rows.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from pandadoc_client.model.pricing_table_request_sections import PricingTableRequestSections
-    globals()['PricingTableRequestSections'] = PricingTableRequestSections
+    from pandadoc_client.model.pricing_table_request_row_options import PricingTableRequestRowOptions
+    globals()['PricingTableRequestRowOptions'] = PricingTableRequestRowOptions
 
 
-class PricingTableRequest(ModelNormal):
+class PricingTableRequestRows(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -82,44 +82,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'data_merge': (bool,),  # noqa: E501
-            'options': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'sections': ([PricingTableRequestSections],),  # noqa: E501
+            'options': (PricingTableRequestRowOptions,),  # noqa: E501
+            'data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'data_merge': 'data_merge',  # noqa: E501
         'options': 'options',  # noqa: E501
-        'sections': 'sections',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'custom_fields': 'custom_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """PricingTableRequest - a model defined in OpenAPI
-
-        Args:
-            name (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """PricingTableRequestRows - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +139,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data_merge (bool): When set to true all field names in data rows must be passed as external names defined in the template.. [optional]  # noqa: E501
-            options ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            sections ([PricingTableRequestSections]): [optional]  # noqa: E501
+            options (PricingTableRequestRowOptions): [optional]  # noqa: E501
+            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,15 +169,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -195,19 +189,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """PricingTableRequest - a model defined in OpenAPI
-
-        Args:
-            name (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """PricingTableRequestRows - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,17 +223,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data_merge (bool): When set to true all field names in data rows must be passed as external names defined in the template.. [optional]  # noqa: E501
-            options ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            sections ([PricingTableRequestSections]): [optional]  # noqa: E501
+            options (PricingTableRequestRowOptions): [optional]  # noqa: E501
+            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -260,15 +251,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request_row_options.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request_row_options.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request_rows.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_create_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,20 +24,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from pandadoc_client.model.pricing_table_request_row_options import PricingTableRequestRowOptions
-    globals()['PricingTableRequestRowOptions'] = PricingTableRequestRowOptions
 
-
-class PricingTableRequestRows(ModelNormal):
+class TemplatesFolderCreateResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -65,56 +61,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'options': (PricingTableRequestRowOptions,),  # noqa: E501
-            'data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'uuid': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'date_created': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'options': 'options',  # noqa: E501
-        'data': 'data',  # noqa: E501
-        'custom_fields': 'custom_fields',  # noqa: E501
+        'uuid': 'uuid',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'date_created': 'date_created',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PricingTableRequestRows - a model defined in OpenAPI
+        """TemplatesFolderCreateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,17 +133,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            options (PricingTableRequestRowOptions): [optional]  # noqa: E501
-            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            uuid (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            date_created (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PricingTableRequestRows - a model defined in OpenAPI
+        """TemplatesFolderCreateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,17 +217,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            options (PricingTableRequestRowOptions): [optional]  # noqa: E501
-            data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            uuid (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            date_created (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_request_sections.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_request_sections.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_discount.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_discount.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_items.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_items.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_options.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/pricing_table_response_options.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/pricing_table_response_summary.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_section_column.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class PricingTableResponseSummary(ModelNormal):
+class QuoteResponseSectionColumn(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,54 +63,54 @@
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = True
+    _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'subtotal': (str, none_type,),  # noqa: E501
-            'total': (str, none_type,),  # noqa: E501
-            'discount': (str, none_type,),  # noqa: E501
-            'tax': (str, none_type,),  # noqa: E501
+            'header': (str, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'merge_name': (str, none_type,),  # noqa: E501
+            'hidden': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'subtotal': 'subtotal',  # noqa: E501
-        'total': 'total',  # noqa: E501
-        'discount': 'discount',  # noqa: E501
-        'tax': 'tax',  # noqa: E501
+        'header': 'header',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'merge_name': 'merge_name',  # noqa: E501
+        'hidden': 'hidden',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PricingTableResponseSummary - a model defined in OpenAPI
+        """QuoteResponseSectionColumn - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,18 +135,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            subtotal (str, none_type): [optional]  # noqa: E501
-            total (str, none_type): [optional]  # noqa: E501
-            discount (str, none_type): [optional]  # noqa: E501
-            tax (str, none_type): [optional]  # noqa: E501
+            header (str, none_type): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            merge_name (str, none_type): [optional]  # noqa: E501
+            hidden (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PricingTableResponseSummary - a model defined in OpenAPI
+        """QuoteResponseSectionColumn - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,18 +220,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            subtotal (str, none_type): [optional]  # noqa: E501
-            total (str, none_type): [optional]  # noqa: E501
-            discount (str, none_type): [optional]  # noqa: E501
-            tax (str, none_type): [optional]  # noqa: E501
+            header (str, none_type): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            merge_name (str, none_type): [optional]  # noqa: E501
+            hidden (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_action.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_action.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_condition.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_condition.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_condition_comparison.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_condition_comparison.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_merge_rules.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_merge_rules.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_options.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_options.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_section_column.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_summary_discounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class QuoteResponseSectionColumn(ModelNormal):
+class QuoteResponseSummaryDiscounts(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,41 +76,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'header': (str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'merge_name': (str, none_type,),  # noqa: E501
-            'hidden': (str,),  # noqa: E501
+            'type': (str, none_type,),  # noqa: E501
+            'value': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'header': 'header',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'merge_name': 'merge_name',  # noqa: E501
-        'hidden': 'hidden',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """QuoteResponseSectionColumn - a model defined in OpenAPI
+        """QuoteResponseSummaryDiscounts - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,18 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            header (str, none_type): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            merge_name (str, none_type): [optional]  # noqa: E501
-            hidden (str): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
+            value (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """QuoteResponseSectionColumn - a model defined in OpenAPI
+        """QuoteResponseSummaryDiscounts - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,18 +214,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            header (str, none_type): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            merge_name (str, none_type): [optional]  # noqa: E501
-            hidden (str): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
+            value (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_section_item.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_section_item.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_section_summary.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_section_summary.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_sections.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_sections.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_settings.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_settings.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_summary.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_details_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,21 +25,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from pandadoc_client.model.quote_response_summary_discounts import QuoteResponseSummaryDiscounts
-    from pandadoc_client.model.quote_response_summary_recurring_subtotal import QuoteResponseSummaryRecurringSubtotal
-    globals()['QuoteResponseSummaryDiscounts'] = QuoteResponseSummaryDiscounts
-    globals()['QuoteResponseSummaryRecurringSubtotal'] = QuoteResponseSummaryRecurringSubtotal
+    from pandadoc_client.model.webhook_event_error_enum import WebhookEventErrorEnum
+    from pandadoc_client.model.webhook_event_trigger_enum import WebhookEventTriggerEnum
+    globals()['WebhookEventErrorEnum'] = WebhookEventErrorEnum
+    globals()['WebhookEventTriggerEnum'] = WebhookEventTriggerEnum
 
 
-class QuoteResponseSummary(ModelNormal):
+class WebhookEventDetailsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,61 +84,57 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'total': (str,),  # noqa: E501
-            'subtotal': (str, none_type,),  # noqa: E501
-            'one_time_subtotal': (str, none_type,),  # noqa: E501
-            'recurring_subtotal': ([QuoteResponseSummaryRecurringSubtotal], none_type,),  # noqa: E501
-            'total_qty': (str, none_type,),  # noqa: E501
-            'discounts': ({str: (QuoteResponseSummaryDiscounts,)}, none_type,),  # noqa: E501
-            'taxes': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'fees': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'custom_fields': ({str: (str,)}, none_type,),  # noqa: E501
-            'total_discount': (str, none_type,),  # noqa: E501
-            'total_tax': (str, none_type,),  # noqa: E501
-            'total_fee': (str, none_type,),  # noqa: E501
-            'total_savings': (str, none_type,),  # noqa: E501
-            'total_contract_value': (str, none_type,),  # noqa: E501
+            'uuid': (str, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'type': (WebhookEventTriggerEnum,),  # noqa: E501
+            'http_status_code': (int, none_type,),  # noqa: E501
+            'error': (WebhookEventErrorEnum,),  # noqa: E501
+            'delivery_time': (datetime,),  # noqa: E501
+            'url': (str,),  # noqa: E501
+            'signature': (str,),  # noqa: E501
+            'request_body': (str,),  # noqa: E501
+            'response_body': (str, none_type,),  # noqa: E501
+            'response_headers': (str, none_type,),  # noqa: E501
+            'event_time': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'total': 'total',  # noqa: E501
-        'subtotal': 'subtotal',  # noqa: E501
-        'one_time_subtotal': 'one_time_subtotal',  # noqa: E501
-        'recurring_subtotal': 'recurring_subtotal',  # noqa: E501
-        'total_qty': 'total_qty',  # noqa: E501
-        'discounts': 'discounts',  # noqa: E501
-        'taxes': 'taxes',  # noqa: E501
-        'fees': 'fees',  # noqa: E501
-        'custom_fields': 'custom_fields',  # noqa: E501
-        'total_discount': 'total_discount',  # noqa: E501
-        'total_tax': 'total_tax',  # noqa: E501
-        'total_fee': 'total_fee',  # noqa: E501
-        'total_savings': 'total_savings',  # noqa: E501
-        'total_contract_value': 'total_contract_value',  # noqa: E501
+        'uuid': 'uuid',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'http_status_code': 'http_status_code',  # noqa: E501
+        'error': 'error',  # noqa: E501
+        'delivery_time': 'delivery_time',  # noqa: E501
+        'url': 'url',  # noqa: E501
+        'signature': 'signature',  # noqa: E501
+        'request_body': 'request_body',  # noqa: E501
+        'response_body': 'response_body',  # noqa: E501
+        'response_headers': 'response_headers',  # noqa: E501
+        'event_time': 'event_time',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """QuoteResponseSummary - a model defined in OpenAPI
+        """WebhookEventDetailsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -163,28 +159,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (str): [optional]  # noqa: E501
-            subtotal (str, none_type): [optional]  # noqa: E501
-            one_time_subtotal (str, none_type): [optional]  # noqa: E501
-            recurring_subtotal ([QuoteResponseSummaryRecurringSubtotal], none_type): [optional]  # noqa: E501
-            total_qty (str, none_type): [optional]  # noqa: E501
-            discounts ({str: (QuoteResponseSummaryDiscounts,)}, none_type): [optional]  # noqa: E501
-            taxes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            fees ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            custom_fields ({str: (str,)}, none_type): [optional]  # noqa: E501
-            total_discount (str, none_type): [optional]  # noqa: E501
-            total_tax (str, none_type): [optional]  # noqa: E501
-            total_fee (str, none_type): [optional]  # noqa: E501
-            total_savings (str, none_type): [optional]  # noqa: E501
-            total_contract_value (str, none_type): [optional]  # noqa: E501
+            uuid (str, none_type): Unique webhook subscription event identifier. [optional]  # noqa: E501
+            name (str): Webhook subscription name. [optional]  # noqa: E501
+            type (WebhookEventTriggerEnum): [optional]  # noqa: E501
+            http_status_code (int, none_type): Webhook subscription event response http status code. [optional]  # noqa: E501
+            error (WebhookEventErrorEnum): [optional]  # noqa: E501
+            delivery_time (datetime): Webhook subscription event delivery time. [optional]  # noqa: E501
+            url (str): Webhook subscription event destination url. [optional]  # noqa: E501
+            signature (str): Webhook subscription event digital signature. [optional]  # noqa: E501
+            request_body (str): Webhook subscription event request body. [optional]  # noqa: E501
+            response_body (str, none_type): Webhook subscription response body. [optional]  # noqa: E501
+            response_headers (str, none_type): Webhook subscription response headers. [optional]  # noqa: E501
+            event_time (datetime): Webhook subscription event trigger time. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -225,15 +219,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """QuoteResponseSummary - a model defined in OpenAPI
+        """WebhookEventDetailsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,28 +252,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (str): [optional]  # noqa: E501
-            subtotal (str, none_type): [optional]  # noqa: E501
-            one_time_subtotal (str, none_type): [optional]  # noqa: E501
-            recurring_subtotal ([QuoteResponseSummaryRecurringSubtotal], none_type): [optional]  # noqa: E501
-            total_qty (str, none_type): [optional]  # noqa: E501
-            discounts ({str: (QuoteResponseSummaryDiscounts,)}, none_type): [optional]  # noqa: E501
-            taxes ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            fees ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            custom_fields ({str: (str,)}, none_type): [optional]  # noqa: E501
-            total_discount (str, none_type): [optional]  # noqa: E501
-            total_tax (str, none_type): [optional]  # noqa: E501
-            total_fee (str, none_type): [optional]  # noqa: E501
-            total_savings (str, none_type): [optional]  # noqa: E501
-            total_contract_value (str, none_type): [optional]  # noqa: E501
+            uuid (str, none_type): Unique webhook subscription event identifier. [optional]  # noqa: E501
+            name (str): Webhook subscription name. [optional]  # noqa: E501
+            type (WebhookEventTriggerEnum): [optional]  # noqa: E501
+            http_status_code (int, none_type): Webhook subscription event response http status code. [optional]  # noqa: E501
+            error (WebhookEventErrorEnum): [optional]  # noqa: E501
+            delivery_time (datetime): Webhook subscription event delivery time. [optional]  # noqa: E501
+            url (str): Webhook subscription event destination url. [optional]  # noqa: E501
+            signature (str): Webhook subscription event digital signature. [optional]  # noqa: E501
+            request_body (str): Webhook subscription event request body. [optional]  # noqa: E501
+            response_body (str, none_type): Webhook subscription response body. [optional]  # noqa: E501
+            response_headers (str, none_type): Webhook subscription response headers. [optional]  # noqa: E501
+            event_time (datetime): Webhook subscription event trigger time. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_summary_discounts.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_discounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class QuoteResponseSummaryDiscounts(ModelNormal):
+class QuoteUpdateRequestDiscounts(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,14 +50,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'PERCENT': "percent",
+            'FLAT': "flat",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -76,16 +80,16 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'type': (str, none_type,),  # noqa: E501
-            'value': (str, none_type,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'value': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -98,15 +102,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """QuoteResponseSummaryDiscounts - a model defined in OpenAPI
+        """QuoteUpdateRequestDiscounts - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,16 +135,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str, none_type): [optional]  # noqa: E501
-            value (str, none_type): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            value (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """QuoteResponseSummaryDiscounts - a model defined in OpenAPI
+        """QuoteUpdateRequestDiscounts - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,16 +218,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str, none_type): [optional]  # noqa: E501
-            value (str, none_type): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            value (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_response_summary_recurring_subtotal.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_response_summary_recurring_subtotal.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_section_settings.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_section_settings.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_discounts.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class QuoteUpdateRequestDiscounts(ModelNormal):
+class TemplateDetailsResponseTokens(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,18 +50,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'PERCENT': "percent",
-            'FLAT': "flat",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -80,37 +76,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'type': (str,),  # noqa: E501
-            'value': (float,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
+        'name': 'name',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """QuoteUpdateRequestDiscounts - a model defined in OpenAPI
+        """TemplateDetailsResponseTokens - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,16 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            value (float): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """QuoteUpdateRequestDiscounts - a model defined in OpenAPI
+        """TemplateDetailsResponseTokens - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,16 +214,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            value (float): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_options.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_options.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_price_settings.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_price_settings.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_price_settings_tiers.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_price_settings_tiers.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_settings.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_settings.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/quote_update_request_settings1.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/quote_update_request_settings1.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/recipient_verification_settings.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_verification_settings.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/recipient_verification_settings_passcode_verification.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_verification_settings_passcode_verification.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/recipient_verification_settings_phone_verification.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/recipient_verification_settings_phone_verification.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/section_info_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/section_info_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_content_placeholders.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_content_placeholders.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_images.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/create_user_request_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class TemplateDetailsResponseImages(ModelNormal):
+class CreateUserRequestUser(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,39 +76,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str, none_type,),  # noqa: E501
-            'block_uuid': (str,),  # noqa: E501
-            'urls': ([str],),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'first_name': (str,),  # noqa: E501
+            'last_name': (str,),  # noqa: E501
+            'phone_number': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'block_uuid': 'block_uuid',  # noqa: E501
-        'urls': 'urls',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'first_name': 'first_name',  # noqa: E501
+        'last_name': 'last_name',  # noqa: E501
+        'phone_number': 'phone_number',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TemplateDetailsResponseImages - a model defined in OpenAPI
+        """CreateUserRequestUser - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,17 +135,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): [optional]  # noqa: E501
-            block_uuid (str): [optional]  # noqa: E501
-            urls ([str]): [optional]  # noqa: E501
+            email (str): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            phone_number (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TemplateDetailsResponseImages - a model defined in OpenAPI
+        """CreateUserRequestUser - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,17 +220,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): [optional]  # noqa: E501
-            block_uuid (str): [optional]  # noqa: E501
-            urls ([str]): [optional]  # noqa: E501
+            email (str): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            phone_number (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_preassigned_person.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_preassigned_person.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'placeholder_name': (str,),  # noqa: E501
             'placeholder_source': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -135,15 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
             type (str): [optional]  # noqa: E501
             placeholder_name (str): [optional]  # noqa: E501
             placeholder_source (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -220,15 +220,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
             type (str): [optional]  # noqa: E501
             placeholder_name (str): [optional]  # noqa: E501
             placeholder_source (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_roles.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_details_response_roles.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_details_response_tokens.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_list_response_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class TemplateDetailsResponseTokens(ModelNormal):
+class UploadSectionListResponseResults(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,37 +76,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'uuid': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'uuid': 'uuid',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TemplateDetailsResponseTokens - a model defined in OpenAPI
+        """UploadSectionListResponseResults - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,16 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            uuid (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TemplateDetailsResponseTokens - a model defined in OpenAPI
+        """UploadSectionListResponseResults - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,16 +214,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            uuid (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/template_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/template_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_create_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_create_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/create_workspace_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class TemplatesFolderCreateResponse(ModelNormal):
+class CreateWorkspaceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,39 +76,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'uuid': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'date_created': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'uuid': 'uuid',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'date_created': 'date_created',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TemplatesFolderCreateResponse - a model defined in OpenAPI
+        """CreateWorkspaceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,17 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
-            date_created (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TemplatesFolderCreateResponse - a model defined in OpenAPI
+        """CreateWorkspaceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,17 +214,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
-            date_created (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_list_response_results.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_rename_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/templates_folder_rename_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/templates_folder_rename_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/create_user_request_workspaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class TemplatesFolderRenameResponse(ModelNormal):
+class CreateUserRequestWorkspaces(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,14 +50,20 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('role',): {
+            'ADMIN': "Admin",
+            'MANAGER': "Manager",
+            'MEMBER': "Member",
+            'COLLABORATOR': "Collaborator",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -76,39 +82,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'uuid': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'date_created': (str,),  # noqa: E501
+            'workspace_id': (str,),  # noqa: E501
+            'role': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'uuid': 'uuid',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'date_created': 'date_created',  # noqa: E501
+        'workspace_id': 'workspace_id',  # noqa: E501
+        'role': 'role',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TemplatesFolderRenameResponse - a model defined in OpenAPI
+        """CreateUserRequestWorkspaces - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,17 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            date_created (str): [optional]  # noqa: E501
+            workspace_id (str): [optional]  # noqa: E501
+            role (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TemplatesFolderRenameResponse - a model defined in OpenAPI
+        """CreateUserRequestWorkspaces - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,17 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            date_created (str): [optional]  # noqa: E501
+            workspace_id (str): [optional]  # noqa: E501
+            role (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/update_integration_quote_section.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/update_integration_quote_section.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/update_integration_quote_section_item.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/update_integration_quote_section_item.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_by_pdf_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_by_pdf_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_by_template_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_by_template_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_list_response_results.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/ricipient_delivery_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 
-class UploadSectionListResponseResults(ModelNormal):
+class RicipientDeliveryMethods(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +63,50 @@
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'uuid': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'email': (bool,),  # noqa: E501
+            'sms': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'uuid': 'uuid',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'sms': 'sms',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UploadSectionListResponseResults - a model defined in OpenAPI
+        """RicipientDeliveryMethods - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,16 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
+            email (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
+            sms (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UploadSectionListResponseResults - a model defined in OpenAPI
+        """RicipientDeliveryMethods - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,16 +214,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
+            email (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
+            sms (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_status_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_status_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/upload_section_status_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/upload_section_status_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_details_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_item_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,21 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from pandadoc_client.model.webhook_event_error_enum import WebhookEventErrorEnum
-    from pandadoc_client.model.webhook_event_trigger_enum import WebhookEventTriggerEnum
-    globals()['WebhookEventErrorEnum'] = WebhookEventErrorEnum
-    globals()['WebhookEventTriggerEnum'] = WebhookEventTriggerEnum
+    from pandadoc_client.model.webhook_subscription_payload_enum import WebhookSubscriptionPayloadEnum
+    from pandadoc_client.model.webhook_subscription_status_enum import WebhookSubscriptionStatusEnum
+    from pandadoc_client.model.webhook_subscription_trigger_enum import WebhookSubscriptionTriggerEnum
+    globals()['WebhookSubscriptionPayloadEnum'] = WebhookSubscriptionPayloadEnum
+    globals()['WebhookSubscriptionStatusEnum'] = WebhookSubscriptionStatusEnum
+    globals()['WebhookSubscriptionTriggerEnum'] = WebhookSubscriptionTriggerEnum
 
 
-class WebhookEventDetailsResponse(ModelNormal):
+class WebhookSubscriptionItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,55 +88,49 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'uuid': (str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'type': (WebhookEventTriggerEnum,),  # noqa: E501
-            'http_status_code': (int, none_type,),  # noqa: E501
-            'error': (WebhookEventErrorEnum,),  # noqa: E501
-            'delivery_time': (datetime,),  # noqa: E501
             'url': (str,),  # noqa: E501
-            'signature': (str,),  # noqa: E501
-            'request_body': (str,),  # noqa: E501
-            'response_body': (str, none_type,),  # noqa: E501
-            'response_headers': (str, none_type,),  # noqa: E501
-            'event_time': (datetime,),  # noqa: E501
+            'active': (bool,),  # noqa: E501
+            'payload': ([WebhookSubscriptionPayloadEnum], none_type,),  # noqa: E501
+            'triggers': ([WebhookSubscriptionTriggerEnum], none_type,),  # noqa: E501
+            'workspace_id': (str,),  # noqa: E501
+            'shared_key': (str,),  # noqa: E501
+            'status': (WebhookSubscriptionStatusEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'uuid': 'uuid',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'http_status_code': 'http_status_code',  # noqa: E501
-        'error': 'error',  # noqa: E501
-        'delivery_time': 'delivery_time',  # noqa: E501
         'url': 'url',  # noqa: E501
-        'signature': 'signature',  # noqa: E501
-        'request_body': 'request_body',  # noqa: E501
-        'response_body': 'response_body',  # noqa: E501
-        'response_headers': 'response_headers',  # noqa: E501
-        'event_time': 'event_time',  # noqa: E501
+        'active': 'active',  # noqa: E501
+        'payload': 'payload',  # noqa: E501
+        'triggers': 'triggers',  # noqa: E501
+        'workspace_id': 'workspace_id',  # noqa: E501
+        'shared_key': 'shared_key',  # noqa: E501
+        'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookEventDetailsResponse - a model defined in OpenAPI
+        """WebhookSubscriptionItemResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -159,26 +155,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str, none_type): Unique webhook subscription event identifier. [optional]  # noqa: E501
-            name (str): Webhook subscription name. [optional]  # noqa: E501
-            type (WebhookEventTriggerEnum): [optional]  # noqa: E501
-            http_status_code (int, none_type): Webhook subscription event response http status code. [optional]  # noqa: E501
-            error (WebhookEventErrorEnum): [optional]  # noqa: E501
-            delivery_time (datetime): Webhook subscription event delivery time. [optional]  # noqa: E501
-            url (str): Webhook subscription event destination url. [optional]  # noqa: E501
-            signature (str): Webhook subscription event digital signature. [optional]  # noqa: E501
-            request_body (str): Webhook subscription event request body. [optional]  # noqa: E501
-            response_body (str, none_type): Webhook subscription response body. [optional]  # noqa: E501
-            response_headers (str, none_type): Webhook subscription response headers. [optional]  # noqa: E501
-            event_time (datetime): Webhook subscription event trigger time. [optional]  # noqa: E501
+            uuid (str, none_type): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            active (bool): [optional]  # noqa: E501
+            payload ([WebhookSubscriptionPayloadEnum], none_type): [optional]  # noqa: E501
+            triggers ([WebhookSubscriptionTriggerEnum], none_type): [optional]  # noqa: E501
+            workspace_id (str): [optional]  # noqa: E501
+            shared_key (str): [optional]  # noqa: E501
+            status (WebhookSubscriptionStatusEnum): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,15 +212,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookEventDetailsResponse - a model defined in OpenAPI
+        """WebhookSubscriptionItemResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,26 +245,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str, none_type): Unique webhook subscription event identifier. [optional]  # noqa: E501
-            name (str): Webhook subscription name. [optional]  # noqa: E501
-            type (WebhookEventTriggerEnum): [optional]  # noqa: E501
-            http_status_code (int, none_type): Webhook subscription event response http status code. [optional]  # noqa: E501
-            error (WebhookEventErrorEnum): [optional]  # noqa: E501
-            delivery_time (datetime): Webhook subscription event delivery time. [optional]  # noqa: E501
-            url (str): Webhook subscription event destination url. [optional]  # noqa: E501
-            signature (str): Webhook subscription event digital signature. [optional]  # noqa: E501
-            request_body (str): Webhook subscription event request body. [optional]  # noqa: E501
-            response_body (str, none_type): Webhook subscription response body. [optional]  # noqa: E501
-            response_headers (str, none_type): Webhook subscription response headers. [optional]  # noqa: E501
-            event_time (datetime): Webhook subscription event trigger time. [optional]  # noqa: E501
+            uuid (str, none_type): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
+            active (bool): [optional]  # noqa: E501
+            payload ([WebhookSubscriptionPayloadEnum], none_type): [optional]  # noqa: E501
+            triggers ([WebhookSubscriptionTriggerEnum], none_type): [optional]  # noqa: E501
+            workspace_id (str): [optional]  # noqa: E501
+            shared_key (str): [optional]  # noqa: E501
+            status (WebhookSubscriptionStatusEnum): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_error_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_error_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_http_status_code_group_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_http_status_code_group_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_item_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_item_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_page_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_page_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_event_trigger_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_event_trigger_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_create_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_create_request.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_item_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_patch_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,20 @@
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from pandadoc_client.model.webhook_subscription_payload_enum import WebhookSubscriptionPayloadEnum
-    from pandadoc_client.model.webhook_subscription_status_enum import WebhookSubscriptionStatusEnum
     from pandadoc_client.model.webhook_subscription_trigger_enum import WebhookSubscriptionTriggerEnum
     globals()['WebhookSubscriptionPayloadEnum'] = WebhookSubscriptionPayloadEnum
-    globals()['WebhookSubscriptionStatusEnum'] = WebhookSubscriptionStatusEnum
     globals()['WebhookSubscriptionTriggerEnum'] = WebhookSubscriptionTriggerEnum
 
 
-class WebhookSubscriptionItemResponse(ModelNormal):
+class WebhookSubscriptionPatchRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,51 +84,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'uuid': (str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'url': (str,),  # noqa: E501
             'active': (bool,),  # noqa: E501
             'payload': ([WebhookSubscriptionPayloadEnum], none_type,),  # noqa: E501
             'triggers': ([WebhookSubscriptionTriggerEnum], none_type,),  # noqa: E501
-            'workspace_id': (str,),  # noqa: E501
-            'shared_key': (str,),  # noqa: E501
-            'status': (WebhookSubscriptionStatusEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'uuid': 'uuid',  # noqa: E501
         'name': 'name',  # noqa: E501
         'url': 'url',  # noqa: E501
         'active': 'active',  # noqa: E501
         'payload': 'payload',  # noqa: E501
         'triggers': 'triggers',  # noqa: E501
-        'workspace_id': 'workspace_id',  # noqa: E501
-        'shared_key': 'shared_key',  # noqa: E501
-        'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookSubscriptionItemResponse - a model defined in OpenAPI
+        """WebhookSubscriptionPatchRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,23 +145,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str, none_type): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
             url (str): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
+            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
             payload ([WebhookSubscriptionPayloadEnum], none_type): [optional]  # noqa: E501
             triggers ([WebhookSubscriptionTriggerEnum], none_type): [optional]  # noqa: E501
-            workspace_id (str): [optional]  # noqa: E501
-            shared_key (str): [optional]  # noqa: E501
-            status (WebhookSubscriptionStatusEnum): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -212,15 +198,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookSubscriptionItemResponse - a model defined in OpenAPI
+        """WebhookSubscriptionPatchRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,23 +231,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uuid (str, none_type): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
             url (str): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
+            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
             payload ([WebhookSubscriptionPayloadEnum], none_type): [optional]  # noqa: E501
             triggers ([WebhookSubscriptionTriggerEnum], none_type): [optional]  # noqa: E501
-            workspace_id (str): [optional]  # noqa: E501
-            shared_key (str): [optional]  # noqa: E501
-            status (WebhookSubscriptionStatusEnum): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_list_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_list_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_patch_request.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/document_update_request_recipients.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,21 +25,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pandadoc_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from pandadoc_client.model.webhook_subscription_payload_enum import WebhookSubscriptionPayloadEnum
-    from pandadoc_client.model.webhook_subscription_trigger_enum import WebhookSubscriptionTriggerEnum
-    globals()['WebhookSubscriptionPayloadEnum'] = WebhookSubscriptionPayloadEnum
-    globals()['WebhookSubscriptionTriggerEnum'] = WebhookSubscriptionTriggerEnum
+    from pandadoc_client.model.recipient_redirect import RecipientRedirect
+    from pandadoc_client.model.ricipient_delivery_methods import RicipientDeliveryMethods
+    globals()['RecipientRedirect'] = RecipientRedirect
+    globals()['RicipientDeliveryMethods'] = RicipientDeliveryMethods
 
 
-class WebhookSubscriptionPatchRequest(ModelNormal):
+class DocumentUpdateRequestRecipients(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,43 +84,47 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'active': (bool,),  # noqa: E501
-            'payload': ([WebhookSubscriptionPayloadEnum], none_type,),  # noqa: E501
-            'triggers': ([WebhookSubscriptionTriggerEnum], none_type,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
+            'phone': (str, none_type,),  # noqa: E501
+            'first_name': (str,),  # noqa: E501
+            'last_name': (str,),  # noqa: E501
+            'delivery_methods': (RicipientDeliveryMethods,),  # noqa: E501
+            'redirect': (RecipientRedirect,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'active': 'active',  # noqa: E501
-        'payload': 'payload',  # noqa: E501
-        'triggers': 'triggers',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'phone': 'phone',  # noqa: E501
+        'first_name': 'first_name',  # noqa: E501
+        'last_name': 'last_name',  # noqa: E501
+        'delivery_methods': 'delivery_methods',  # noqa: E501
+        'redirect': 'redirect',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookSubscriptionPatchRequest - a model defined in OpenAPI
+        """DocumentUpdateRequestRecipients - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,19 +149,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
-            payload ([WebhookSubscriptionPayloadEnum], none_type): [optional]  # noqa: E501
-            triggers ([WebhookSubscriptionTriggerEnum], none_type): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
+            phone (str, none_type): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            delivery_methods (RicipientDeliveryMethods): [optional]  # noqa: E501
+            redirect (RecipientRedirect): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +204,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookSubscriptionPatchRequest - a model defined in OpenAPI
+        """DocumentUpdateRequestRecipients - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,19 +237,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
-            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
-            payload ([WebhookSubscriptionPayloadEnum], none_type): [optional]  # noqa: E501
-            triggers ([WebhookSubscriptionTriggerEnum], none_type): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            email (str, none_type): [optional]  # noqa: E501
+            phone (str, none_type): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            delivery_methods (RicipientDeliveryMethods): [optional]  # noqa: E501
+            redirect (RecipientRedirect): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_payload_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_payload_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_shared_key_response.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_shared_key_response.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_status_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_status_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model/webhook_subscription_trigger_enum.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model/webhook_subscription_trigger_enum.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/model_utils.py` & `pandadoc-python-client-6.2.0/pandadoc_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/models/__init__.py` & `pandadoc-python-client-6.2.0/pandadoc_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,30 @@
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from pandadoc_client.model.api_log_details_response import APILogDetailsResponse
 from pandadoc_client.model.api_log_list_response import APILogListResponse
 from pandadoc_client.model.api_log_list_response_results import APILogListResponseResults
+from pandadoc_client.model.add_member_request import AddMemberRequest
+from pandadoc_client.model.add_member_response import AddMemberResponse
 from pandadoc_client.model.contact_create_request import ContactCreateRequest
 from pandadoc_client.model.contact_details_response import ContactDetailsResponse
 from pandadoc_client.model.contact_list_response import ContactListResponse
 from pandadoc_client.model.contact_update_request import ContactUpdateRequest
 from pandadoc_client.model.content_library_item_list_response import ContentLibraryItemListResponse
 from pandadoc_client.model.content_library_item_list_response_results import ContentLibraryItemListResponseResults
 from pandadoc_client.model.content_library_item_response import ContentLibraryItemResponse
 from pandadoc_client.model.content_library_item_response_created_by import ContentLibraryItemResponseCreatedBy
+from pandadoc_client.model.create_user_request import CreateUserRequest
+from pandadoc_client.model.create_user_request_user import CreateUserRequestUser
+from pandadoc_client.model.create_user_request_workspaces import CreateUserRequestWorkspaces
+from pandadoc_client.model.create_user_response import CreateUserResponse
+from pandadoc_client.model.create_workspace_request import CreateWorkspaceRequest
+from pandadoc_client.model.create_workspace_response import CreateWorkspaceResponse
 from pandadoc_client.model.document_attachment_response import DocumentAttachmentResponse
 from pandadoc_client.model.document_attachment_response_created_by import DocumentAttachmentResponseCreatedBy
 from pandadoc_client.model.document_create_by_pdf_request import DocumentCreateByPdfRequest
 from pandadoc_client.model.document_create_by_template_request import DocumentCreateByTemplateRequest
 from pandadoc_client.model.document_create_by_template_request_content_library_items import DocumentCreateByTemplateRequestContentLibraryItems
 from pandadoc_client.model.document_create_by_template_request_content_placeholders import DocumentCreateByTemplateRequestContentPlaceholders
 from pandadoc_client.model.document_create_by_template_request_images import DocumentCreateByTemplateRequestImages
@@ -53,14 +61,15 @@
 from pandadoc_client.model.document_send_request import DocumentSendRequest
 from pandadoc_client.model.document_send_request_forwarding_settings import DocumentSendRequestForwardingSettings
 from pandadoc_client.model.document_send_request_selected_approvers import DocumentSendRequestSelectedApprovers
 from pandadoc_client.model.document_send_request_selected_approvers_group import DocumentSendRequestSelectedApproversGroup
 from pandadoc_client.model.document_send_request_selected_approvers_group_assignees import DocumentSendRequestSelectedApproversGroupAssignees
 from pandadoc_client.model.document_send_request_selected_approvers_steps import DocumentSendRequestSelectedApproversSteps
 from pandadoc_client.model.document_send_response import DocumentSendResponse
+from pandadoc_client.model.document_send_response_recipients import DocumentSendResponseRecipients
 from pandadoc_client.model.document_status_change_request import DocumentStatusChangeRequest
 from pandadoc_client.model.document_status_enum import DocumentStatusEnum
 from pandadoc_client.model.document_status_request_enum import DocumentStatusRequestEnum
 from pandadoc_client.model.document_status_response import DocumentStatusResponse
 from pandadoc_client.model.document_transfer_all_ownership_request import DocumentTransferAllOwnershipRequest
 from pandadoc_client.model.document_transfer_ownership_request import DocumentTransferOwnershipRequest
 from pandadoc_client.model.document_update_request import DocumentUpdateRequest
@@ -107,17 +116,19 @@
 from pandadoc_client.model.quote_update_request import QuoteUpdateRequest
 from pandadoc_client.model.quote_update_request_discounts import QuoteUpdateRequestDiscounts
 from pandadoc_client.model.quote_update_request_options import QuoteUpdateRequestOptions
 from pandadoc_client.model.quote_update_request_price_settings import QuoteUpdateRequestPriceSettings
 from pandadoc_client.model.quote_update_request_price_settings_tiers import QuoteUpdateRequestPriceSettingsTiers
 from pandadoc_client.model.quote_update_request_settings import QuoteUpdateRequestSettings
 from pandadoc_client.model.quote_update_request_settings1 import QuoteUpdateRequestSettings1
+from pandadoc_client.model.recipient_redirect import RecipientRedirect
 from pandadoc_client.model.recipient_verification_settings import RecipientVerificationSettings
 from pandadoc_client.model.recipient_verification_settings_passcode_verification import RecipientVerificationSettingsPasscodeVerification
 from pandadoc_client.model.recipient_verification_settings_phone_verification import RecipientVerificationSettingsPhoneVerification
+from pandadoc_client.model.ricipient_delivery_methods import RicipientDeliveryMethods
 from pandadoc_client.model.section_info_response import SectionInfoResponse
 from pandadoc_client.model.template_details_response import TemplateDetailsResponse
 from pandadoc_client.model.template_details_response_content_placeholders import TemplateDetailsResponseContentPlaceholders
 from pandadoc_client.model.template_details_response_images import TemplateDetailsResponseImages
 from pandadoc_client.model.template_details_response_preassigned_person import TemplateDetailsResponsePreassignedPerson
 from pandadoc_client.model.template_details_response_roles import TemplateDetailsResponseRoles
 from pandadoc_client.model.template_details_response_tokens import TemplateDetailsResponseTokens
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_client/rest.py` & `pandadoc-python-client-6.2.0/pandadoc_client/rest.py`

 * *Files identical despite different names*

### Comparing `pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/PKG-INFO` & `pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandadoc-python-client
-Version: 6.1.0
+Version: 6.2.0
 Summary: PandaDoc Public API
 Home-page: https://github.com/PandaDoc/pandadoc-api-python-client
 Author: PandaDoc
 Author-email: 
 License: MIT
 Keywords: OpenAPI,PandaDoc Public API
 Requires-Python: >=3.6
```

### Comparing `pandadoc-python-client-6.1.0/pandadoc_python_client.egg-info/SOURCES.txt` & `pandadoc-python-client-6.2.0/pandadoc_python_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,38 @@
 pandadoc_client/api/folders_api_api.py
 pandadoc_client/api/forms_api.py
 pandadoc_client/api/members_api.py
 pandadoc_client/api/o_auth_2_0_authentication_api.py
 pandadoc_client/api/quotes_api.py
 pandadoc_client/api/sections_api.py
 pandadoc_client/api/templates_api.py
+pandadoc_client/api/user_and_workspace_management_api.py
 pandadoc_client/api/webhook_events_api.py
 pandadoc_client/api/webhook_subscriptions_api.py
 pandadoc_client/apis/__init__.py
 pandadoc_client/model/__init__.py
+pandadoc_client/model/add_member_request.py
+pandadoc_client/model/add_member_response.py
 pandadoc_client/model/api_log_details_response.py
 pandadoc_client/model/api_log_list_response.py
 pandadoc_client/model/api_log_list_response_results.py
 pandadoc_client/model/contact_create_request.py
 pandadoc_client/model/contact_details_response.py
 pandadoc_client/model/contact_list_response.py
 pandadoc_client/model/contact_update_request.py
 pandadoc_client/model/content_library_item_list_response.py
 pandadoc_client/model/content_library_item_list_response_results.py
 pandadoc_client/model/content_library_item_response.py
 pandadoc_client/model/content_library_item_response_created_by.py
+pandadoc_client/model/create_user_request.py
+pandadoc_client/model/create_user_request_user.py
+pandadoc_client/model/create_user_request_workspaces.py
+pandadoc_client/model/create_user_response.py
+pandadoc_client/model/create_workspace_request.py
+pandadoc_client/model/create_workspace_response.py
 pandadoc_client/model/document_attachment_response.py
 pandadoc_client/model/document_attachment_response_created_by.py
 pandadoc_client/model/document_create_by_pdf_request.py
 pandadoc_client/model/document_create_by_template_request.py
 pandadoc_client/model/document_create_by_template_request_content_library_items.py
 pandadoc_client/model/document_create_by_template_request_content_placeholders.py
 pandadoc_client/model/document_create_by_template_request_images.py
@@ -69,14 +78,15 @@
 pandadoc_client/model/document_send_request.py
 pandadoc_client/model/document_send_request_forwarding_settings.py
 pandadoc_client/model/document_send_request_selected_approvers.py
 pandadoc_client/model/document_send_request_selected_approvers_group.py
 pandadoc_client/model/document_send_request_selected_approvers_group_assignees.py
 pandadoc_client/model/document_send_request_selected_approvers_steps.py
 pandadoc_client/model/document_send_response.py
+pandadoc_client/model/document_send_response_recipients.py
 pandadoc_client/model/document_status_change_request.py
 pandadoc_client/model/document_status_enum.py
 pandadoc_client/model/document_status_request_enum.py
 pandadoc_client/model/document_status_response.py
 pandadoc_client/model/document_transfer_all_ownership_request.py
 pandadoc_client/model/document_transfer_ownership_request.py
 pandadoc_client/model/document_update_request.py
@@ -123,17 +133,19 @@
 pandadoc_client/model/quote_update_request.py
 pandadoc_client/model/quote_update_request_discounts.py
 pandadoc_client/model/quote_update_request_options.py
 pandadoc_client/model/quote_update_request_price_settings.py
 pandadoc_client/model/quote_update_request_price_settings_tiers.py
 pandadoc_client/model/quote_update_request_settings.py
 pandadoc_client/model/quote_update_request_settings1.py
+pandadoc_client/model/recipient_redirect.py
 pandadoc_client/model/recipient_verification_settings.py
 pandadoc_client/model/recipient_verification_settings_passcode_verification.py
 pandadoc_client/model/recipient_verification_settings_phone_verification.py
+pandadoc_client/model/ricipient_delivery_methods.py
 pandadoc_client/model/section_info_response.py
 pandadoc_client/model/template_details_response.py
 pandadoc_client/model/template_details_response_content_placeholders.py
 pandadoc_client/model/template_details_response_images.py
 pandadoc_client/model/template_details_response_preassigned_person.py
 pandadoc_client/model/template_details_response_roles.py
 pandadoc_client/model/template_details_response_tokens.py
```

### Comparing `pandadoc-python-client-6.1.0/setup.py` & `pandadoc-python-client-6.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 description = ""
 from_index = full_description.find("### Documentation for API Endpoints")
 to_index = full_description.find("## License")
 if from_index and to_index:
     description = full_description[0:from_index] + full_description[to_index::]
 
 NAME = "pandadoc-python-client"
-VERSION = "6.1.0"
+VERSION = "6.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

