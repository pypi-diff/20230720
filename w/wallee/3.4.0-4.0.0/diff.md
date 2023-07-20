# Comparing `tmp/wallee-3.4.0.tar.gz` & `tmp/wallee-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallee-3.4.0.tar", last modified: Wed Feb 15 10:58:02 2023, max compression
+gzip compressed data, was "wallee-4.0.0.tar", last modified: Thu Jul 20 14:43:36 2023, max compression
```

## Comparing `wallee-3.4.0.tar` & `wallee-4.0.0.tar`

### file list

```diff
@@ -1,568 +1,564 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 10:58:02.594859 wallee-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11338 2023-02-15 10:57:41.000000 wallee-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4444 2023-02-15 10:58:02.594859 wallee-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-02-15 10:57:41.000000 wallee-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-15 10:58:02.594859 wallee-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-02-15 10:57:41.000000 wallee-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 10:58:02.466840 wallee-3.4.0/wallee/
--rw-r--r--   0 runner    (1001) docker     (122)    42205 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 10:58:02.486843 wallee-3.4.0/wallee/api/
--rw-r--r--   0 runner    (1001) docker     (122)     8185 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22346 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/account_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    23793 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/analytics_query_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    22652 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/application_user_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12601 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/bank_account_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12657 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12720 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/card_processing_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12629 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/charge_attempt_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12748 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/charge_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12832 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/charge_flow_level_payment_link_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    16951 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/charge_flow_level_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    30984 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/charge_flow_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/condition_type_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/country_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/country_state_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12720 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/currency_bank_account_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3335 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/currency_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    29526 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/customer_address_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    33455 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/customer_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25176 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/customer_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    52466 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/debt_collection_case_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12816 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/debt_collector_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6998 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/debt_collector_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21638 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/delivery_indication_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12671 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/document_template_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/document_template_type_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12895 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/external_transfer_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    26237 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/human_user_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    18576 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/installment_payment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    13112 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/installment_payment_slice_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/installment_plan_calculation_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    13192 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/installment_plan_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    13281 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/installment_plan_slice_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12895 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/internal_transfer_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    22981 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/invoice_reconciliation_record_invoice_link_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25146 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/invoice_reconciliation_record_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    22187 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/invoice_reimbursement_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/label_description_group_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7049 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/label_description_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/language_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/legal_organization_form_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/manual_task_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     5194 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/mertic_usage_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12858 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_connector_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_connector_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25403 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_link_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_method_brand_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12816 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_method_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_method_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12858 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_processor_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_processor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    29426 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_terminal_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12382 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_terminal_till_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17314 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_terminal_transaction_summary_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    41578 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/payment_web_app_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6971 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/permission_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12748 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/refund_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    28762 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/refund_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12867 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/refund_recovery_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    34753 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/refund_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17023 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_recurring_order_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17321 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_subscriber_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21910 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_subscription_product_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    31258 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_subscription_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21495 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_subscription_suspension_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12818 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_subscription_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12699 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/shopify_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    22284 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/space_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7002 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/static_value_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25350 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscriber_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25675 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_affiliate_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    20897 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_charge_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    16949 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_ledger_entry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25632 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_metric_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17150 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_metric_usage_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12762 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_period_bill_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    26033 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_component_group_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25862 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_component_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25736 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_fee_tier_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25653 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_metered_fee_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25622 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_period_fee_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17086 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_retirement_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21585 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25591 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_setup_fee_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17234 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_version_retirement_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    26347 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_product_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    52338 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21307 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_suspension_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12681 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/subscription_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    42780 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/token_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17069 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/token_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    28970 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    31171 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_completion_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_iframe_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    29101 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_invoice_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    40552 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_invoice_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_lightbox_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    17291 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_line_item_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_mobile_sdk_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4484 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_payment_page_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    80350 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_terminal_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21279 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/transaction_void_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    13178 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/user_account_role_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12719 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/user_space_role_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/web_app_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25551 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/webhook_listener_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25396 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api/webhook_url_service_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25534 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     8517 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 10:58:02.594859 wallee-3.4.0/wallee/models/
--rw-r--r--   0 runner    (1001) docker     (122)    27196 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4510 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_account_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_application_user_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     7396 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_customer_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_customer_address_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_customer_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     8982 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_debt_collection_case_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_human_user_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_payment_link_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_refund_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)    16919 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_shopify_subscription_product_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     9707 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_space_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    11397 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_subscriber_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_subscription_affiliate_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_subscription_metric_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     8738 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_subscription_product_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     8747 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_token_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_transaction_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2506 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_transaction_invoice_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)    20184 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_transaction_pending.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_webhook_listener_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     4495 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/abstract_webhook_url_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14922 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/account_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/account_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/account_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/account_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    17834 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/address.py
--rw-r--r--   0 runner    (1001) docker     (122)    18278 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/address_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     9337 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/analytics_query.py
--rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/analytics_query_execution.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/analytics_query_execution_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/analytics_query_result_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     8401 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/analytics_schema_column.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/analytics_schema_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/application_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/application_user_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2470 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/application_user_create_with_mac_key.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/application_user_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/authenticated_card_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12532 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/authenticated_card_data_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7917 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_account_environment.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_account_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_account_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    15797 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_transaction_flow_direction.py
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_transaction_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/bank_transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/card_authentication_response.py
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/card_authentication_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/card_cryptogram.py
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/card_cryptogram_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/card_cryptogram_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/cardholder_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     7170 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/cardholder_authentication_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge.py
--rw-r--r--   0 runner    (1001) docker     (122)    21469 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_attempt.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_attempt_environment.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_attempt_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     8390 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     8320 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_flow.py
--rw-r--r--   0 runner    (1001) docker     (122)     9394 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_flow_level.py
--rw-r--r--   0 runner    (1001) docker     (122)    10355 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_flow_level_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_flow_level_configuration_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_flow_level_payment_link.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_flow_level_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/charge_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4921 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/client_error.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/client_error_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/completion_line_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/completion_line_item_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7163 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/condition_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     6649 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/connector_invocation.py
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/connector_invocation_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/creation_entity_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/criteria_operator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/currency_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     9754 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     7214 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_address.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_address_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_address_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_address_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     8420 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_comment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    18996 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_postal_address.py
--rw-r--r--   0 runner    (1001) docker     (122)    19440 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customer_postal_address_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/customers_presence.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/data_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/database_translated_string.py
--rw-r--r--   0 runner    (1001) docker     (122)     2353 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/database_translated_string_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/database_translated_string_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/database_translated_string_item_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_case.py
--rw-r--r--   0 runner    (1001) docker     (122)     5190 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_case_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    10485 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_case_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_case_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_case_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_case_update.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_environment.py
--rw-r--r--   0 runner    (1001) docker     (122)    10048 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_receipt.py
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collection_receipt_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collector.py
--rw-r--r--   0 runner    (1001) docker     (122)     7321 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collector_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     3830 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collector_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    11916 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/debt_collector_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    10848 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/delivery_indication.py
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/delivery_indication_decision_reason.py
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/delivery_indication_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     9844 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/document_template.py
--rw-r--r--   0 runner    (1001) docker     (122)     4756 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/document_template_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/document_template_type_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/entity_export_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     6248 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/entity_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/entity_query_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/entity_query_filter_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/entity_query_order_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/entity_query_order_by_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (122)     7592 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/external_transfer_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/failure_category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4887 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/failure_reason.py
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/feature_category.py
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (122)    11567 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/human_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/human_user_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3456 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/human_user_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     5683 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_calculated_plan.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_calculated_slice.py
--rw-r--r--   0 runner    (1001) docker     (122)     8613 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_payment.py
--rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_payment_slice.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_payment_slice_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_payment_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    17656 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_plan_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    10827 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/installment_plan_slice_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     5929 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/internal_transfer_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)    25217 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reconciliation_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reconciliation_record_invoice_link.py
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reconciliation_record_rejection_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reconciliation_record_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reconciliation_record_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    17743 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reimbursement.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reimbursement_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/invoice_reimbursement_with_refund_reference.py
--rw-r--r--   0 runner    (1001) docker     (122)     4736 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     6616 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/label_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/label_descriptor_category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/label_descriptor_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/label_descriptor_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     5060 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/legal_organization_form.py
--rw-r--r--   0 runner    (1001) docker     (122)    18658 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item_attribute.py
--rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item_attribute_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     4382 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item_reduction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item_reduction_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/line_item_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3440 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/localized_string.py
--rw-r--r--   0 runner    (1001) docker     (122)     8757 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/manual_task.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/manual_task_action.py
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/manual_task_action_style.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/manual_task_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4271 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/manual_task_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/metric_usage.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/one_click_payment_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_adjustment_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_charge_attempt_target_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     7658 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_charge_attempt_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     7987 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_completion_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     8125 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_completion_configuration_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_completion_target_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5881 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_completion_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    14889 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_connector.py
--rw-r--r--   0 runner    (1001) docker     (122)    12593 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_connector_creation_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_connector_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    16126 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7576 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_processor_creation_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_processor_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5112 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_refund_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     5202 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_refund_configuration_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_refund_target_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5681 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_refund_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_void_target_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_app_void_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_connector.py
--rw-r--r--   0 runner    (1001) docker     (122)    16324 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_connector_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_connector_feature.py
--rw-r--r--   0 runner    (1001) docker     (122)    12577 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_contract.py
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_contract_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4342 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_information_hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_information_hash_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_initiation_advice_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      288 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_initiation_advice_file_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    20033 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_link_active.py
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_link_address_handling_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_link_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_link_protection_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)    15538 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_link_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     6842 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_method_brand.py
--rw-r--r--   0 runner    (1001) docker     (122)    18023 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_method_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_primary_risk_taker.py
--rw-r--r--   0 runner    (1001) docker     (122)     7208 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_processor_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    11541 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)    12395 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_address.py
--rw-r--r--   0 runner    (1001) docker     (122)     7555 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_configuration_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    14186 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_configuration_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_configuration_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     7778 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_dcc_transaction_sum.py
--rw-r--r--   0 runner    (1001) docker     (122)     7852 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_location.py
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_location_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    10642 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_location_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_location_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3830 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_receipt_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    10388 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_transaction_sum.py
--rw-r--r--   0 runner    (1001) docker     (122)     9759 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     4708 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_transaction_summary_fetch_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/payment_terminal_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     8505 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/persistable_currency_amount.py
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/persistable_currency_amount_update.py
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_fee_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     8591 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_metered_fee.py
--rw-r--r--   0 runner    (1001) docker     (122)     7624 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_metered_fee_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_metered_tier_fee.py
--rw-r--r--   0 runner    (1001) docker     (122)     6283 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_metered_tier_fee_update.py
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_metered_tier_pricing.py
--rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_period_fee.py
--rw-r--r--   0 runner    (1001) docker     (122)     9155 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_period_fee_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    10445 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_setup_fee.py
--rw-r--r--   0 runner    (1001) docker     (122)     9617 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/product_setup_fee_update.py
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/recurring_indicator.py
--rw-r--r--   0 runner    (1001) docker     (122)    24283 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund.py
--rw-r--r--   0 runner    (1001) docker     (122)     7428 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     8298 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_comment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     8523 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_recovery_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/refund_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4190 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rendered_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     5264 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rendered_terminal_receipt.py
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rendered_terminal_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     6775 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/resource_path.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/resource_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rest_address_format.py
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rest_address_format_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     6925 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rest_country.py
--rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rest_country_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rest_currency.py
--rw-r--r--   0 runner    (1001) docker     (122)     6797 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/rest_language.py
--rw-r--r--   0 runner    (1001) docker     (122)     7673 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/role.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/role_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5359 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/sales_channel.py
--rw-r--r--   0 runner    (1001) docker     (122)    10096 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/scope.py
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/server_error.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_additional_line_item_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    23991 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_integration_payment_app_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_integration_subscription_app_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    12494 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_recurring_order.py
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_recurring_order_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_recurring_order_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     9518 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscriber_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     4338 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscriber_creation.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscriber_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    15120 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_address.py
--rw-r--r--   0 runner    (1001) docker     (122)    19218 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_address_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_billing_interval_unit.py
--rw-r--r--   0 runner    (1001) docker     (122)    15014 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_creation_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    11797 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_model_billing_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_model_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_model_tax_line.py
--rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_product.py
--rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_product_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_product_pricing_option.py
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_product_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_product_update.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    11116 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_suspension.py
--rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_suspension_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_suspension_initiator.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_suspension_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_suspension_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4129 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_update_addresses_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     6215 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    24539 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5449 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_version_item.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_version_item_price_strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_subscription_weekday.py
--rw-r--r--   0 runner    (1001) docker     (122)     4695 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_tax_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8383 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/shopify_transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    18402 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space.py
--rw-r--r--   0 runner    (1001) docker     (122)    13381 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_address.py
--rw-r--r--   0 runner    (1001) docker     (122)    13759 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_address_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     6678 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_reference.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_reference_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/space_view.py
--rw-r--r--   0 runner    (1001) docker     (122)     4214 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/static_value.py
--rw-r--r--   0 runner    (1001) docker     (122)    15617 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscriber_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     3625 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscriber_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    12763 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscriber_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    16381 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)    10016 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_affiliate.py
--rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_affiliate_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_affiliate_deleted.py
--rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_affiliate_deleting.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_affiliate_inactive.py
--rw-r--r--   0 runner    (1001) docker     (122)     6531 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_affiliate_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     7470 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_change_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    18892 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_charge.py
--rw-r--r--   0 runner    (1001) docker     (122)     9268 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_charge_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_charge_processing_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_charge_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3031 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_component_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_component_reference_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6112 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_create_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_ledger_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_ledger_entry_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_ledger_entry_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     4399 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4783 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    11198 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric_usage_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_metric_usage_report_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3822 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_pending.py
--rw-r--r--   0 runner    (1001) docker     (122)    10613 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_period_bill.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_period_bill_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    13275 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_active.py
--rw-r--r--   0 runner    (1001) docker     (122)    15044 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     7650 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_component_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     7204 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_component_group_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     7834 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_component_reference.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_component_reference_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_component_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7432 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_retirement.py
--rw-r--r--   0 runner    (1001) docker     (122)     4401 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_retirement_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    20901 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13626 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_version_pending.py
--rw-r--r--   0 runner    (1001) docker     (122)     8003 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_version_retirement.py
--rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_version_retirement_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_product_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    13218 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_suspension.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_suspension_action.py
--rw-r--r--   0 runner    (1001) docker     (122)     5831 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_suspension_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_suspension_reason.py
--rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_suspension_running.py
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_suspension_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5688 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_update_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    17339 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/subscription_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tax_calculation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6892 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tax_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tax_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3642 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tenant_database.py
--rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/terminal_receipt_fetch_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/terminal_receipt_format.py
--rw-r--r--   0 runner    (1001) docker     (122)    13760 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/token_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/token_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    19146 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/token_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/token_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/token_version_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tokenization_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tokenized_card_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/tokenized_card_data_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    63423 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_aware_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_comment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (122)    24689 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_completion.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_completion_behavior.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_completion_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_completion_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_completion_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    10944 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_environment_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)     7596 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_group_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    17796 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_invoice.py
--rw-r--r--   0 runner    (1001) docker     (122)     9047 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_invoice_comment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_invoice_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_invoice_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7715 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_invoice_replacement.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_invoice_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    16354 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_line_item_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_line_item_version_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_line_item_version_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_pending.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_user_interface_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    13168 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_void.py
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_void_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/transaction_void_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/two_factor_authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     5530 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/user_account_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/user_space_role.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/user_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/wallet_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/web_app_confirmation_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/web_app_confirmation_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     6513 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_identity.py
--rw-r--r--   0 runner    (1001) docker     (122)    10739 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_listener_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3525 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_listener_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_listener_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     8381 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_url_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/models/webhook_url_update.py
--rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-02-15 10:57:41.000000 wallee-3.4.0/wallee/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 10:58:02.466840 wallee-3.4.0/wallee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4444 2023-02-15 10:58:02.000000 wallee-3.4.0/wallee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24015 2023-02-15 10:58:02.000000 wallee-3.4.0/wallee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-15 10:58:02.000000 wallee-3.4.0/wallee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-02-15 10:58:02.000000 wallee-3.4.0/wallee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-15 10:58:02.000000 wallee-3.4.0/wallee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:43:36.299796 wallee-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11338 2023-07-20 14:43:21.000000 wallee-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4444 2023-07-20 14:43:36.299796 wallee-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-07-20 14:43:21.000000 wallee-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 14:43:36.299796 wallee-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-07-20 14:43:21.000000 wallee-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:43:36.183794 wallee-4.0.0/wallee/
+-rw-r--r--   0 runner    (1001) docker     (122)    41849 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:43:36.207795 wallee-4.0.0/wallee/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     8185 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22346 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/account_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23793 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/analytics_query_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22652 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/application_user_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12601 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/bank_account_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12657 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12720 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/card_processing_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12629 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/charge_attempt_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12748 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/charge_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12832 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/charge_flow_level_payment_link_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16951 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/charge_flow_level_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30984 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/charge_flow_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/condition_type_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/country_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/country_state_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12720 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/currency_bank_account_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3335 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/currency_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29526 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/customer_address_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33455 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/customer_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25176 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/customer_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52466 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/debt_collection_case_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12816 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/debt_collector_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6998 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/debt_collector_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21638 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/delivery_indication_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12671 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/document_template_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/document_template_type_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12895 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/external_transfer_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26237 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/human_user_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18576 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/installment_payment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13112 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/installment_payment_slice_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/installment_plan_calculation_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13192 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/installment_plan_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13281 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/installment_plan_slice_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12895 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/internal_transfer_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22981 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/invoice_reconciliation_record_invoice_link_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25146 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/invoice_reconciliation_record_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22187 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/invoice_reimbursement_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/label_description_group_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7049 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/label_description_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/language_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/legal_organization_form_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/manual_task_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5194 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/mertic_usage_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12858 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_connector_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_connector_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25403 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_link_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_method_brand_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12816 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_method_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_method_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12858 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_processor_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_processor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29426 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_terminal_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12382 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_terminal_till_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17314 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_terminal_transaction_summary_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41578 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/payment_web_app_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6971 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/permission_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12748 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/refund_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28762 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/refund_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12867 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/refund_recovery_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34753 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/refund_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17023 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_recurring_order_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17321 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_subscriber_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21910 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_subscription_product_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31258 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_subscription_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21495 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_subscription_suspension_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12818 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_subscription_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12699 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/shopify_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22284 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/space_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7002 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/static_value_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25350 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscriber_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25675 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_affiliate_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20897 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_charge_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16949 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_ledger_entry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25632 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_metric_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17150 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_metric_usage_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12762 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_period_bill_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26033 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_component_group_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25862 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_component_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25736 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_fee_tier_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25653 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_metered_fee_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25622 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_period_fee_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17086 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_retirement_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21585 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25591 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_setup_fee_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17234 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_version_retirement_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26347 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_product_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52338 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21307 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_suspension_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12681 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/subscription_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42780 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/token_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17069 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/token_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28970 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31171 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_completion_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_iframe_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29101 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_invoice_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40552 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_invoice_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_lightbox_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17291 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_line_item_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_mobile_sdk_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4484 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_payment_page_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80350 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_terminal_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21279 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/transaction_void_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13178 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/user_account_role_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12719 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/user_space_role_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/web_app_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25551 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/webhook_listener_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25396 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api/webhook_url_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25534 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8517 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:43:36.299796 wallee-4.0.0/wallee/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    26892 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4372 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_account_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_application_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_customer_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3287 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_customer_address_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_customer_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8982 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_debt_collection_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_human_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_payment_link_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_refund_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16919 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_shopify_subscription_product_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9041 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_space_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11391 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_subscriber_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4911 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_subscription_affiliate_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_subscription_metric_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8738 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_subscription_product_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8747 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2515 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_transaction_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_transaction_invoice_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20178 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_transaction_pending.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5060 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_webhook_listener_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4087 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/abstract_webhook_url_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14712 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/account_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/account_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/account_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19096 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19676 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/address_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9337 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/analytics_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12454 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/analytics_query_execution.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/analytics_query_execution_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/analytics_query_result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8401 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/analytics_schema_column.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/analytics_schema_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/application_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/application_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/application_user_create_with_mac_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/application_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/authenticated_card_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12532 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/authenticated_card_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7917 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_account_environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_account_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4326 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15797 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_transaction_flow_direction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_transaction_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/bank_transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/card_authentication_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/card_authentication_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/card_cryptogram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/card_cryptogram_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/card_cryptogram_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/cardholder_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7170 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/cardholder_authentication_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21469 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_attempt_environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_attempt_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8390 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8320 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_flow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9394 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_flow_level.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10355 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_flow_level_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_flow_level_configuration_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_flow_level_payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_flow_level_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/charge_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4921 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/client_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/client_error_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/completion_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/completion_line_item_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7163 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6649 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/connector_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/connector_invocation_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/creation_entity_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/criteria_operator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/currency_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10100 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7550 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_address.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_address_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_address_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8846 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_comment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20258 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20702 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customer_postal_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/customers_presence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/data_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_case.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5190 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10485 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_case_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4592 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_case_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_case_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10048 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collection_receipt_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7321 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collector_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3726 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collector_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11916 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/debt_collector_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10848 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/delivery_indication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/delivery_indication_decision_reason.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/delivery_indication_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9844 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/document_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4756 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/document_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/document_template_type_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/entity_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6248 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/entity_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/entity_query_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/entity_query_filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/entity_query_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/entity_query_order_by_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7592 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/external_transfer_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/failure_category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4783 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/failure_reason.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7624 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/feature_category.py
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11579 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/human_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/human_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3456 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/human_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5683 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_calculated_plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_calculated_slice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8613 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_payment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_payment_slice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_payment_slice_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_payment_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17626 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_plan_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10797 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/installment_plan_slice_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5929 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/internal_transfer_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25217 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reconciliation_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reconciliation_record_invoice_link.py
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reconciliation_record_rejection_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reconciliation_record_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3801 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reconciliation_record_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17743 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reimbursement.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reimbursement_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/invoice_reimbursement_with_refund_reference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4736 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/label_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/label_descriptor_category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/label_descriptor_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/label_descriptor_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5586 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/legal_organization_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18658 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item_attribute_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4382 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item_reduction_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/line_item_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/localized_string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8177 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/manual_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/manual_task_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/manual_task_action_style.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/manual_task_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4245 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/manual_task_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/metric_usage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/one_click_payment_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_adjustment_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_charge_attempt_target_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7658 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_charge_attempt_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7987 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_completion_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8125 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_completion_configuration_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_completion_target_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5881 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_completion_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14889 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_connector.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12593 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_connector_creation_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_connector_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16126 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7576 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_processor_creation_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_processor_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5112 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_refund_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5202 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_refund_configuration_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_refund_target_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5681 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_refund_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_void_target_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_app_void_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11445 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_connector.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16324 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_connector_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_connector_feature.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12577 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_contract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_contract_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_information_hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_information_hash_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_initiation_advice_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_initiation_advice_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20033 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_link_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_link_address_handling_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_link_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_link_protection_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15538 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_link_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6738 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5729 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_method_brand.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17963 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_method_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_primary_risk_taker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7104 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_processor_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12362 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13283 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_address.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7555 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_configuration_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14186 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_configuration_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_configuration_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7778 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_dcc_transaction_sum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7852 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_location_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10642 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_location_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_location_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3726 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_receipt_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10388 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_transaction_sum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9759 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4708 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_transaction_summary_fetch_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/payment_terminal_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9149 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/persistable_currency_amount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/persistable_currency_amount_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_fee_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8531 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_metered_fee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7528 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_metered_fee_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_metered_tier_fee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6283 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_metered_tier_fee_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_metered_tier_pricing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9919 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_period_fee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9011 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_period_fee_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10385 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_setup_fee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9521 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/product_setup_fee_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/recurring_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24283 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7428 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8644 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_comment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8523 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_recovery_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/refund_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4190 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rendered_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5264 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rendered_terminal_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rendered_terminal_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6775 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/resource_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/resource_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5042 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rest_address_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rest_address_format_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6297 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rest_country.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4783 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rest_country_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rest_currency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7056 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/rest_language.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7371 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/role_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/sales_channel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/scope.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/server_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_additional_line_item_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23991 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_integration_payment_app_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_integration_subscription_app_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12494 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_recurring_order.py
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_recurring_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_recurring_order_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9518 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscriber_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4338 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscriber_creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscriber_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15120 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_address.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20480 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_billing_interval_unit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15014 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_creation_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11797 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_model_billing_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_model_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_model_tax_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_product.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_product_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_product_pricing_option.py
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_product_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_product_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11116 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_suspension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_suspension_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_suspension_initiator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_suspension_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_suspension_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4129 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_update_addresses_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6215 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24539 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5449 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_version_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_version_item_price_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_subscription_weekday.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4695 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_tax_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8383 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/shopify_transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17704 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14295 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_address.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14673 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6678 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_reference.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_reference_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/space_view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4110 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/static_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15611 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscriber_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3625 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscriber_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12757 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscriber_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16381 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10010 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_affiliate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_affiliate_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_affiliate_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_affiliate_deleting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_affiliate_inactive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_affiliate_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7470 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_change_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18892 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_charge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9268 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_charge_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_charge_processing_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_charge_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3031 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_component_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_component_reference_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6112 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_ledger_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_ledger_entry_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_ledger_entry_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4295 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11198 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric_usage_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_metric_usage_report_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3822 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_pending.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10613 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_period_bill.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_period_bill_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13275 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14984 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7620 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_component_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7156 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_component_group_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7834 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_component_reference.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_component_reference_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14570 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_component_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7432 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_retirement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4401 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_retirement_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20871 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13578 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_version_pending.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8003 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_version_retirement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_version_retirement_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_product_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13218 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_suspension.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_suspension_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5831 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_suspension_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_suspension_reason.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_suspension_running.py
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_suspension_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5688 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17339 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/subscription_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tax_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6892 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tax_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tax_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tenant_database.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/terminal_receipt_fetch_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/terminal_receipt_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13760 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/token_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/token_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19146 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/token_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/token_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/token_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tokenization_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tokenized_card_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/tokenized_card_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63417 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_aware_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8949 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_comment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24689 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_completion_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_completion_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_completion_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_completion_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10944 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_environment_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7596 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_group_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17796 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9393 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_invoice_comment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_invoice_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_invoice_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7715 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_invoice_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_invoice_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16354 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_line_item_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_line_item_version_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_line_item_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_pending.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_user_interface_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13168 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_void.py
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_void_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/transaction_void_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5137 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/two_factor_authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/user_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/user_space_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/wallet_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/web_app_confirmation_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/web_app_confirmation_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_identity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10015 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_listener_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_listener_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_listener_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8011 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_url_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/models/webhook_url_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-07-20 14:43:21.000000 wallee-4.0.0/wallee/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:43:36.183794 wallee-4.0.0/wallee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4444 2023-07-20 14:43:36.000000 wallee-4.0.0/wallee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23815 2023-07-20 14:43:36.000000 wallee-4.0.0/wallee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:43:36.000000 wallee-4.0.0/wallee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-20 14:43:36.000000 wallee-4.0.0/wallee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-20 14:43:36.000000 wallee-4.0.0/wallee.egg-info/top_level.txt
```

### Comparing `wallee-3.4.0/LICENSE` & `wallee-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/PKG-INFO` & `wallee-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallee
-Version: 3.4.0
+Version: 4.0.0
 Summary: SDK that allows you to access wallee
 Author: Wallee AG
 License: Apache-2.0
 Keywords: wallee,Payment,Payment Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wallee-3.4.0/README.md` & `wallee-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/setup.py` & `wallee-4.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 NAME = "wallee"
-VERSION = "3.4.0"
+VERSION = "4.0.0"
 
 REQUIRES = [
     "certifi>=2017.4.17",
     "python-dateutil>=2.1",
     "six>=1.10",
     "urllib3>=1.23"
 ]
```

### Comparing `wallee-3.4.0/wallee/__init__.py` & `wallee-4.0.0/wallee/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,18 +185,14 @@
 from wallee.models.customer_address import CustomerAddress
 from wallee.models.customer_address_type import CustomerAddressType
 from wallee.models.customer_comment import CustomerComment
 from wallee.models.customer_postal_address import CustomerPostalAddress
 from wallee.models.customer_postal_address_create import CustomerPostalAddressCreate
 from wallee.models.customers_presence import CustomersPresence
 from wallee.models.data_collection_type import DataCollectionType
-from wallee.models.database_translated_string import DatabaseTranslatedString
-from wallee.models.database_translated_string_create import DatabaseTranslatedStringCreate
-from wallee.models.database_translated_string_item import DatabaseTranslatedStringItem
-from wallee.models.database_translated_string_item_create import DatabaseTranslatedStringItemCreate
 from wallee.models.debt_collection_case import DebtCollectionCase
 from wallee.models.debt_collection_case_document import DebtCollectionCaseDocument
 from wallee.models.debt_collection_case_source import DebtCollectionCaseSource
 from wallee.models.debt_collection_case_state import DebtCollectionCaseState
 from wallee.models.debt_collection_environment import DebtCollectionEnvironment
 from wallee.models.debt_collection_receipt import DebtCollectionReceipt
 from wallee.models.debt_collection_receipt_source import DebtCollectionReceiptSource
```

### Comparing `wallee-3.4.0/wallee/api/__init__.py` & `wallee-4.0.0/wallee/api/__init__.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/account_service_api.py` & `wallee-4.0.0/wallee/api/account_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/analytics_query_service_api.py` & `wallee-4.0.0/wallee/api/analytics_query_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/application_user_service_api.py` & `wallee-4.0.0/wallee/api/application_user_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/bank_account_service_api.py` & `wallee-4.0.0/wallee/api/bank_account_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/bank_transaction_service_api.py` & `wallee-4.0.0/wallee/api/bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/card_processing_service_api.py` & `wallee-4.0.0/wallee/api/card_processing_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/charge_attempt_service_api.py` & `wallee-4.0.0/wallee/api/charge_attempt_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/charge_bank_transaction_service_api.py` & `wallee-4.0.0/wallee/api/charge_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/charge_flow_level_payment_link_service_api.py` & `wallee-4.0.0/wallee/api/charge_flow_level_payment_link_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/charge_flow_level_service_api.py` & `wallee-4.0.0/wallee/api/charge_flow_level_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/charge_flow_service_api.py` & `wallee-4.0.0/wallee/api/charge_flow_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/condition_type_service_api.py` & `wallee-4.0.0/wallee/api/condition_type_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/country_service_api.py` & `wallee-4.0.0/wallee/api/country_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/country_state_service_api.py` & `wallee-4.0.0/wallee/api/country_state_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/currency_bank_account_service_api.py` & `wallee-4.0.0/wallee/api/currency_bank_account_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/currency_service_api.py` & `wallee-4.0.0/wallee/api/currency_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/customer_address_service_api.py` & `wallee-4.0.0/wallee/api/customer_address_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/customer_comment_service_api.py` & `wallee-4.0.0/wallee/api/customer_comment_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/customer_service_api.py` & `wallee-4.0.0/wallee/api/customer_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/debt_collection_case_service_api.py` & `wallee-4.0.0/wallee/api/debt_collection_case_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/debt_collector_configuration_service_api.py` & `wallee-4.0.0/wallee/api/debt_collector_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/debt_collector_service_api.py` & `wallee-4.0.0/wallee/api/debt_collector_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/delivery_indication_service_api.py` & `wallee-4.0.0/wallee/api/delivery_indication_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/document_template_service_api.py` & `wallee-4.0.0/wallee/api/document_template_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/document_template_type_service_api.py` & `wallee-4.0.0/wallee/api/document_template_type_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/external_transfer_bank_transaction_service_api.py` & `wallee-4.0.0/wallee/api/external_transfer_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/human_user_service_api.py` & `wallee-4.0.0/wallee/api/human_user_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/installment_payment_service_api.py` & `wallee-4.0.0/wallee/api/installment_payment_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/installment_payment_slice_service_api.py` & `wallee-4.0.0/wallee/api/installment_payment_slice_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/installment_plan_calculation_service_api.py` & `wallee-4.0.0/wallee/api/installment_plan_calculation_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/installment_plan_configuration_service_api.py` & `wallee-4.0.0/wallee/api/installment_plan_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/installment_plan_slice_configuration_service_api.py` & `wallee-4.0.0/wallee/api/installment_plan_slice_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/internal_transfer_bank_transaction_service_api.py` & `wallee-4.0.0/wallee/api/internal_transfer_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/invoice_reconciliation_record_invoice_link_service_api.py` & `wallee-4.0.0/wallee/api/invoice_reconciliation_record_invoice_link_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/invoice_reconciliation_record_service_api.py` & `wallee-4.0.0/wallee/api/invoice_reconciliation_record_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/invoice_reimbursement_service_api.py` & `wallee-4.0.0/wallee/api/invoice_reimbursement_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/label_description_group_service_api.py` & `wallee-4.0.0/wallee/api/label_description_group_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/label_description_service_api.py` & `wallee-4.0.0/wallee/api/label_description_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/language_service_api.py` & `wallee-4.0.0/wallee/api/language_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/legal_organization_form_service_api.py` & `wallee-4.0.0/wallee/api/legal_organization_form_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/manual_task_service_api.py` & `wallee-4.0.0/wallee/api/manual_task_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/mertic_usage_service_api.py` & `wallee-4.0.0/wallee/api/mertic_usage_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_connector_configuration_service_api.py` & `wallee-4.0.0/wallee/api/payment_connector_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_connector_service_api.py` & `wallee-4.0.0/wallee/api/payment_connector_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_link_service_api.py` & `wallee-4.0.0/wallee/api/payment_link_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_method_brand_service_api.py` & `wallee-4.0.0/wallee/api/payment_method_brand_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_method_configuration_service_api.py` & `wallee-4.0.0/wallee/api/payment_method_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_method_service_api.py` & `wallee-4.0.0/wallee/api/payment_method_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_processor_configuration_service_api.py` & `wallee-4.0.0/wallee/api/payment_processor_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_processor_service_api.py` & `wallee-4.0.0/wallee/api/payment_processor_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_terminal_service_api.py` & `wallee-4.0.0/wallee/api/payment_terminal_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_terminal_till_service_api.py` & `wallee-4.0.0/wallee/api/payment_terminal_till_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_terminal_transaction_summary_service_api.py` & `wallee-4.0.0/wallee/api/payment_terminal_transaction_summary_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/payment_web_app_service_api.py` & `wallee-4.0.0/wallee/api/payment_web_app_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/permission_service_api.py` & `wallee-4.0.0/wallee/api/permission_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/refund_bank_transaction_service_api.py` & `wallee-4.0.0/wallee/api/refund_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/refund_comment_service_api.py` & `wallee-4.0.0/wallee/api/refund_comment_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/refund_recovery_bank_transaction_service_api.py` & `wallee-4.0.0/wallee/api/refund_recovery_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/refund_service_api.py` & `wallee-4.0.0/wallee/api/refund_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_recurring_order_service_api.py` & `wallee-4.0.0/wallee/api/shopify_recurring_order_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_subscriber_service_api.py` & `wallee-4.0.0/wallee/api/shopify_subscriber_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_subscription_product_service_api.py` & `wallee-4.0.0/wallee/api/shopify_subscription_product_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_subscription_service_api.py` & `wallee-4.0.0/wallee/api/shopify_subscription_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_subscription_suspension_service_api.py` & `wallee-4.0.0/wallee/api/shopify_subscription_suspension_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_subscription_version_service_api.py` & `wallee-4.0.0/wallee/api/shopify_subscription_version_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/shopify_transaction_service_api.py` & `wallee-4.0.0/wallee/api/shopify_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/space_service_api.py` & `wallee-4.0.0/wallee/api/space_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/static_value_service_api.py` & `wallee-4.0.0/wallee/api/static_value_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscriber_service_api.py` & `wallee-4.0.0/wallee/api/subscriber_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_affiliate_service_api.py` & `wallee-4.0.0/wallee/api/subscription_affiliate_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_charge_service_api.py` & `wallee-4.0.0/wallee/api/subscription_charge_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_ledger_entry_service_api.py` & `wallee-4.0.0/wallee/api/subscription_ledger_entry_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_metric_service_api.py` & `wallee-4.0.0/wallee/api/subscription_metric_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_metric_usage_service_api.py` & `wallee-4.0.0/wallee/api/subscription_metric_usage_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_period_bill_service_api.py` & `wallee-4.0.0/wallee/api/subscription_period_bill_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_component_group_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_component_group_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_component_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_component_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_fee_tier_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_fee_tier_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_metered_fee_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_metered_fee_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_period_fee_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_period_fee_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_retirement_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_retirement_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_setup_fee_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_setup_fee_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_version_retirement_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_version_retirement_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_product_version_service_api.py` & `wallee-4.0.0/wallee/api/subscription_product_version_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_service_api.py` & `wallee-4.0.0/wallee/api/subscription_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_suspension_service_api.py` & `wallee-4.0.0/wallee/api/subscription_suspension_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/subscription_version_service_api.py` & `wallee-4.0.0/wallee/api/subscription_version_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/token_service_api.py` & `wallee-4.0.0/wallee/api/token_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/token_version_service_api.py` & `wallee-4.0.0/wallee/api/token_version_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_comment_service_api.py` & `wallee-4.0.0/wallee/api/transaction_comment_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_completion_service_api.py` & `wallee-4.0.0/wallee/api/transaction_completion_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_iframe_service_api.py` & `wallee-4.0.0/wallee/api/transaction_iframe_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_invoice_comment_service_api.py` & `wallee-4.0.0/wallee/api/transaction_invoice_comment_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_invoice_service_api.py` & `wallee-4.0.0/wallee/api/transaction_invoice_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_lightbox_service_api.py` & `wallee-4.0.0/wallee/api/transaction_lightbox_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_line_item_version_service_api.py` & `wallee-4.0.0/wallee/api/transaction_line_item_version_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_mobile_sdk_service_api.py` & `wallee-4.0.0/wallee/api/transaction_mobile_sdk_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_payment_page_service_api.py` & `wallee-4.0.0/wallee/api/transaction_payment_page_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_service_api.py` & `wallee-4.0.0/wallee/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_terminal_service_api.py` & `wallee-4.0.0/wallee/api/transaction_terminal_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/transaction_void_service_api.py` & `wallee-4.0.0/wallee/api/transaction_void_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/user_account_role_service_api.py` & `wallee-4.0.0/wallee/api/user_account_role_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/user_space_role_service_api.py` & `wallee-4.0.0/wallee/api/user_space_role_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/web_app_service_api.py` & `wallee-4.0.0/wallee/api/web_app_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/webhook_listener_service_api.py` & `wallee-4.0.0/wallee/api/webhook_listener_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api/webhook_url_service_api.py` & `wallee-4.0.0/wallee/api/webhook_url_service_api.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/api_client.py` & `wallee-4.0.0/wallee/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     wallee
 
     Python SDK
 
-    OpenAPI spec version: 3.4.0
+    OpenAPI spec version: 4.0.0
     
 """
 
 from __future__ import absolute_import
 
 import time
 import hashlib
@@ -60,15 +60,15 @@
         for name, value in configuration.default_headers.items():
             self.default_headers[name] = value
 
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'wallee/3.4.0/python'
+        self.user_agent = 'wallee/4.0.0/python'
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
 
     @property
@@ -99,15 +99,15 @@
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
 
         # predefined default headers
         default_headers = {
-            'x-meta-sdk-version': '3.4.0',
+            'x-meta-sdk-version': '4.0.0',
             'x-meta-sdk-language': 'python',
             'x-meta-sdk-provider': 'wallee',
             'x-meta-sdk-language-version': platform.python_version()
         }
 
         header_params.update(self.default_headers)
         header_params.update(default_headers)
```

### Comparing `wallee-3.4.0/wallee/configuration.py` & `wallee-4.0.0/wallee/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 3.4.0\n"\
-               "SDK Package Version: 3.4.0".\
+               "Version of the API: 4.0.0\n"\
+               "SDK Package Version: 4.0.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `wallee-3.4.0/wallee/models/__init__.py` & `wallee-4.0.0/wallee/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,14 @@
 from .customer_address import CustomerAddress
 from .customer_address_type import CustomerAddressType
 from .customer_comment import CustomerComment
 from .customer_postal_address import CustomerPostalAddress
 from .customer_postal_address_create import CustomerPostalAddressCreate
 from .customers_presence import CustomersPresence
 from .data_collection_type import DataCollectionType
-from .database_translated_string import DatabaseTranslatedString
-from .database_translated_string_create import DatabaseTranslatedStringCreate
-from .database_translated_string_item import DatabaseTranslatedStringItem
-from .database_translated_string_item_create import DatabaseTranslatedStringItemCreate
 from .debt_collection_case import DebtCollectionCase
 from .debt_collection_case_document import DebtCollectionCaseDocument
 from .debt_collection_case_source import DebtCollectionCaseSource
 from .debt_collection_case_state import DebtCollectionCaseState
 from .debt_collection_environment import DebtCollectionEnvironment
 from .debt_collection_receipt import DebtCollectionReceipt
 from .debt_collection_receipt_source import DebtCollectionReceiptSource
```

### Comparing `wallee-3.4.0/wallee/models/abstract_account_update.py` & `wallee-4.0.0/wallee/models/abstract_account_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,26 +55,26 @@
 
         self._last_modified_date = last_modified_date
     
     @property
     def name(self):
         """Gets the name of this AbstractAccountUpdate.
 
-            The name of the account identifies the account within the administrative interface.
+            The name used to identify the account.
 
         :return: The name of this AbstractAccountUpdate.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this AbstractAccountUpdate.
 
-            The name of the account identifies the account within the administrative interface.
+            The name used to identify the account.
 
         :param name: The name of this AbstractAccountUpdate.
         :type: str
         """
         if name is not None and len(name) > 200:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `200`")
         if name is not None and len(name) < 3:
@@ -82,26 +82,26 @@
 
         self._name = name
     
     @property
     def subaccount_limit(self):
         """Gets the subaccount_limit of this AbstractAccountUpdate.
 
-            This property restricts the number of subaccounts which can be created within this account.
+            The number of sub-accounts that can be created within this account.
 
         :return: The subaccount_limit of this AbstractAccountUpdate.
         :rtype: int
         """
         return self._subaccount_limit
 
     @subaccount_limit.setter
     def subaccount_limit(self, subaccount_limit):
         """Sets the subaccount_limit of this AbstractAccountUpdate.
 
-            This property restricts the number of subaccounts which can be created within this account.
+            The number of sub-accounts that can be created within this account.
 
         :param subaccount_limit: The subaccount_limit of this AbstractAccountUpdate.
         :type: int
         """
 
         self._subaccount_limit = subaccount_limit
```

### Comparing `wallee-3.4.0/wallee/models/abstract_application_user_update.py` & `wallee-4.0.0/wallee/models/abstract_application_user_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,51 +32,51 @@
         
 
     
     @property
     def name(self):
         """Gets the name of this AbstractApplicationUserUpdate.
 
-            The user name is used to identify the application user in administrative interfaces.
+            The name used to identify the application user.
 
         :return: The name of this AbstractApplicationUserUpdate.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this AbstractApplicationUserUpdate.
 
-            The user name is used to identify the application user in administrative interfaces.
+            The name used to identify the application user.
 
         :param name: The name of this AbstractApplicationUserUpdate.
         :type: str
         """
         if name is not None and len(name) > 256:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `256`")
 
         self._name = name
     
     @property
     def request_limit(self):
         """Gets the request_limit of this AbstractApplicationUserUpdate.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted every 2 minutes.
 
         :return: The request_limit of this AbstractApplicationUserUpdate.
         :rtype: int
         """
         return self._request_limit
 
     @request_limit.setter
     def request_limit(self, request_limit):
         """Sets the request_limit of this AbstractApplicationUserUpdate.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted every 2 minutes.
 
         :param request_limit: The request_limit of this AbstractApplicationUserUpdate.
         :type: int
         """
 
         self._request_limit = request_limit
```

### Comparing `wallee-3.4.0/wallee/models/abstract_customer_active.py` & `wallee-4.0.0/wallee/models/abstract_customer_active.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,101 +44,101 @@
         
 
     
     @property
     def customer_id(self):
         """Gets the customer_id of this AbstractCustomerActive.
 
-            
+            The customer's ID in the merchant's system.
 
         :return: The customer_id of this AbstractCustomerActive.
         :rtype: str
         """
         return self._customer_id
 
     @customer_id.setter
     def customer_id(self, customer_id):
         """Sets the customer_id of this AbstractCustomerActive.
 
-            
+            The customer's ID in the merchant's system.
 
         :param customer_id: The customer_id of this AbstractCustomerActive.
         :type: str
         """
         if customer_id is not None and len(customer_id) > 100:
             raise ValueError("Invalid value for `customer_id`, length must be less than or equal to `100`")
 
         self._customer_id = customer_id
     
     @property
     def email_address(self):
         """Gets the email_address of this AbstractCustomerActive.
 
-            
+            The customer's email address.
 
         :return: The email_address of this AbstractCustomerActive.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this AbstractCustomerActive.
 
-            
+            The customer's email address.
 
         :param email_address: The email_address of this AbstractCustomerActive.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this AbstractCustomerActive.
 
-            
+            The customer's family or last name.
 
         :return: The family_name of this AbstractCustomerActive.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this AbstractCustomerActive.
 
-            
+            The customer's family or last name.
 
         :param family_name: The family_name of this AbstractCustomerActive.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
     def given_name(self):
         """Gets the given_name of this AbstractCustomerActive.
 
-            
+            The customer's given or first name.
 
         :return: The given_name of this AbstractCustomerActive.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this AbstractCustomerActive.
 
-            
+            The customer's given or first name.
 
         :param given_name: The given_name of this AbstractCustomerActive.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
@@ -167,49 +167,49 @@
 
         self._language = language
     
     @property
     def meta_data(self):
         """Gets the meta_data of this AbstractCustomerActive.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this AbstractCustomerActive.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this AbstractCustomerActive.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this AbstractCustomerActive.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
     
     @property
     def preferred_currency(self):
         """Gets the preferred_currency of this AbstractCustomerActive.
 
-            
+            The customer's preferred currency.
 
         :return: The preferred_currency of this AbstractCustomerActive.
         :rtype: str
         """
         return self._preferred_currency
 
     @preferred_currency.setter
     def preferred_currency(self, preferred_currency):
         """Sets the preferred_currency of this AbstractCustomerActive.
 
-            
+            The customer's preferred currency.
 
         :param preferred_currency: The preferred_currency of this AbstractCustomerActive.
         :type: str
         """
 
         self._preferred_currency = preferred_currency
```

### Comparing `wallee-3.4.0/wallee/models/abstract_customer_address_active.py` & `wallee-4.0.0/wallee/models/abstract_customer_address_active.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,49 +29,49 @@
         
 
     
     @property
     def address(self):
         """Gets the address of this AbstractCustomerAddressActive.
 
-            
+            The actual postal address.
 
         :return: The address of this AbstractCustomerAddressActive.
         :rtype: CustomerPostalAddressCreate
         """
         return self._address
 
     @address.setter
     def address(self, address):
         """Sets the address of this AbstractCustomerAddressActive.
 
-            
+            The actual postal address.
 
         :param address: The address of this AbstractCustomerAddressActive.
         :type: CustomerPostalAddressCreate
         """
 
         self._address = address
     
     @property
     def address_type(self):
         """Gets the address_type of this AbstractCustomerAddressActive.
 
-            
+            Whether the address is for billing or shipping or both.
 
         :return: The address_type of this AbstractCustomerAddressActive.
         :rtype: CustomerAddressType
         """
         return self._address_type
 
     @address_type.setter
     def address_type(self, address_type):
         """Sets the address_type of this AbstractCustomerAddressActive.
 
-            
+            Whether the address is for billing or shipping or both.
 
         :param address_type: The address_type of this AbstractCustomerAddressActive.
         :type: CustomerAddressType
         """
 
         self._address_type = address_type
```

### Comparing `wallee-3.4.0/wallee/models/abstract_customer_comment_active.py` & `wallee-4.0.0/wallee/models/abstract_refund_comment_active.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class AbstractCustomerCommentActive:
+class AbstractRefundCommentActive:
 
     swagger_types = {
     
         'content': 'str',
     }
 
     attribute_map = {
@@ -24,30 +24,30 @@
         
         self.content = kwargs.get('content', None)
         
 
     
     @property
     def content(self):
-        """Gets the content of this AbstractCustomerCommentActive.
+        """Gets the content of this AbstractRefundCommentActive.
 
-            
+            The comment's actual content.
 
-        :return: The content of this AbstractCustomerCommentActive.
+        :return: The content of this AbstractRefundCommentActive.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
-        """Sets the content of this AbstractCustomerCommentActive.
+        """Sets the content of this AbstractRefundCommentActive.
 
-            
+            The comment's actual content.
 
-        :param content: The content of this AbstractCustomerCommentActive.
+        :param content: The content of this AbstractRefundCommentActive.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
@@ -70,27 +70,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(AbstractCustomerCommentActive, dict):
+        if issubclass(AbstractRefundCommentActive, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, AbstractCustomerCommentActive):
+        if not isinstance(other, AbstractRefundCommentActive):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/abstract_debt_collection_case_update.py` & `wallee-4.0.0/wallee/models/abstract_debt_collection_case_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/abstract_human_user_update.py` & `wallee-4.0.0/wallee/models/abstract_human_user_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,124 +47,124 @@
         
 
     
     @property
     def email_address(self):
         """Gets the email_address of this AbstractHumanUserUpdate.
 
-            The email address of the user.
+            The user's email address.
 
         :return: The email_address of this AbstractHumanUserUpdate.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this AbstractHumanUserUpdate.
 
-            The email address of the user.
+            The user's email address.
 
         :param email_address: The email_address of this AbstractHumanUserUpdate.
         :type: str
         """
         if email_address is not None and len(email_address) > 128:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `128`")
 
         self._email_address = email_address
     
     @property
     def firstname(self):
         """Gets the firstname of this AbstractHumanUserUpdate.
 
-            The first name of the user.
+            The user's first name.
 
         :return: The firstname of this AbstractHumanUserUpdate.
         :rtype: str
         """
         return self._firstname
 
     @firstname.setter
     def firstname(self, firstname):
         """Sets the firstname of this AbstractHumanUserUpdate.
 
-            The first name of the user.
+            The user's first name.
 
         :param firstname: The firstname of this AbstractHumanUserUpdate.
         :type: str
         """
         if firstname is not None and len(firstname) > 100:
             raise ValueError("Invalid value for `firstname`, length must be less than or equal to `100`")
 
         self._firstname = firstname
     
     @property
     def language(self):
         """Gets the language of this AbstractHumanUserUpdate.
 
-            The preferred language of the user.
+            The user's preferred language.
 
         :return: The language of this AbstractHumanUserUpdate.
         :rtype: str
         """
         return self._language
 
     @language.setter
     def language(self, language):
         """Sets the language of this AbstractHumanUserUpdate.
 
-            The preferred language of the user.
+            The user's preferred language.
 
         :param language: The language of this AbstractHumanUserUpdate.
         :type: str
         """
 
         self._language = language
     
     @property
     def lastname(self):
         """Gets the lastname of this AbstractHumanUserUpdate.
 
-            The last name of the user.
+            The user's last name.
 
         :return: The lastname of this AbstractHumanUserUpdate.
         :rtype: str
         """
         return self._lastname
 
     @lastname.setter
     def lastname(self, lastname):
         """Sets the lastname of this AbstractHumanUserUpdate.
 
-            The last name of the user.
+            The user's last name.
 
         :param lastname: The lastname of this AbstractHumanUserUpdate.
         :type: str
         """
         if lastname is not None and len(lastname) > 100:
             raise ValueError("Invalid value for `lastname`, length must be less than or equal to `100`")
 
         self._lastname = lastname
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this AbstractHumanUserUpdate.
 
-            
+            The user's mobile phone number.
 
         :return: The mobile_phone_number of this AbstractHumanUserUpdate.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this AbstractHumanUserUpdate.
 
-            
+            The user's mobile phone number.
 
         :param mobile_phone_number: The mobile_phone_number of this AbstractHumanUserUpdate.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 30:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `30`")
 
@@ -193,49 +193,49 @@
 
         self._state = state
     
     @property
     def time_zone(self):
         """Gets the time_zone of this AbstractHumanUserUpdate.
 
-            The time zone which is applied for the user. If no timezone is specified the browser is used to determine an appropriate time zone.
+            The user's time zone. If none is specified, the one provided by the browser will be used.
 
         :return: The time_zone of this AbstractHumanUserUpdate.
         :rtype: str
         """
         return self._time_zone
 
     @time_zone.setter
     def time_zone(self, time_zone):
         """Sets the time_zone of this AbstractHumanUserUpdate.
 
-            The time zone which is applied for the user. If no timezone is specified the browser is used to determine an appropriate time zone.
+            The user's time zone. If none is specified, the one provided by the browser will be used.
 
         :param time_zone: The time_zone of this AbstractHumanUserUpdate.
         :type: str
         """
 
         self._time_zone = time_zone
     
     @property
     def two_factor_enabled(self):
         """Gets the two_factor_enabled of this AbstractHumanUserUpdate.
 
-            Defines whether two-factor authentication is enabled for this user.
+            Whether two-factor authentication is enabled for this user.
 
         :return: The two_factor_enabled of this AbstractHumanUserUpdate.
         :rtype: bool
         """
         return self._two_factor_enabled
 
     @two_factor_enabled.setter
     def two_factor_enabled(self, two_factor_enabled):
         """Sets the two_factor_enabled of this AbstractHumanUserUpdate.
 
-            Defines whether two-factor authentication is enabled for this user.
+            Whether two-factor authentication is enabled for this user.
 
         :param two_factor_enabled: The two_factor_enabled of this AbstractHumanUserUpdate.
         :type: bool
         """
 
         self._two_factor_enabled = two_factor_enabled
```

### Comparing `wallee-3.4.0/wallee/models/abstract_payment_link_update.py` & `wallee-4.0.0/wallee/models/abstract_payment_link_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/abstract_refund_comment_active.py` & `wallee-4.0.0/wallee/models/abstract_transaction_invoice_comment_active.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class AbstractRefundCommentActive:
+class AbstractTransactionInvoiceCommentActive:
 
     swagger_types = {
     
         'content': 'str',
     }
 
     attribute_map = {
@@ -24,30 +24,30 @@
         
         self.content = kwargs.get('content', None)
         
 
     
     @property
     def content(self):
-        """Gets the content of this AbstractRefundCommentActive.
+        """Gets the content of this AbstractTransactionInvoiceCommentActive.
 
-            
+            The comment's actual content.
 
-        :return: The content of this AbstractRefundCommentActive.
+        :return: The content of this AbstractTransactionInvoiceCommentActive.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
-        """Sets the content of this AbstractRefundCommentActive.
+        """Sets the content of this AbstractTransactionInvoiceCommentActive.
 
-            
+            The comment's actual content.
 
-        :param content: The content of this AbstractRefundCommentActive.
+        :param content: The content of this AbstractTransactionInvoiceCommentActive.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
@@ -70,27 +70,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(AbstractRefundCommentActive, dict):
+        if issubclass(AbstractTransactionInvoiceCommentActive, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, AbstractRefundCommentActive):
+        if not isinstance(other, AbstractTransactionInvoiceCommentActive):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/abstract_shopify_subscription_product_update.py` & `wallee-4.0.0/wallee/models/abstract_shopify_subscription_product_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/abstract_space_update.py` & `wallee-4.0.0/wallee/models/abstract_space_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,26 +70,26 @@
 
         self._last_modified_date = last_modified_date
     
     @property
     def name(self):
         """Gets the name of this AbstractSpaceUpdate.
 
-            The space name is used internally to identify the space in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the space.
 
         :return: The name of this AbstractSpaceUpdate.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this AbstractSpaceUpdate.
 
-            The space name is used internally to identify the space in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the space.
 
         :param name: The name of this AbstractSpaceUpdate.
         :type: str
         """
         if name is not None and len(name) > 200:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `200`")
         if name is not None and len(name) < 3:
@@ -97,72 +97,72 @@
 
         self._name = name
     
     @property
     def postal_address(self):
         """Gets the postal_address of this AbstractSpaceUpdate.
 
-            The address to use in communication with clients for example in email, documents etc.
+            The address that is used in communication with clients for example in emails, documents, etc.
 
         :return: The postal_address of this AbstractSpaceUpdate.
         :rtype: SpaceAddressCreate
         """
         return self._postal_address
 
     @postal_address.setter
     def postal_address(self, postal_address):
         """Sets the postal_address of this AbstractSpaceUpdate.
 
-            The address to use in communication with clients for example in email, documents etc.
+            The address that is used in communication with clients for example in emails, documents, etc.
 
         :param postal_address: The postal_address of this AbstractSpaceUpdate.
         :type: SpaceAddressCreate
         """
 
         self._postal_address = postal_address
     
     @property
     def primary_currency(self):
         """Gets the primary_currency of this AbstractSpaceUpdate.
 
-            This is the currency that is used to display aggregated amounts in the space.
+            The currency that is used to display aggregated amounts in the space.
 
         :return: The primary_currency of this AbstractSpaceUpdate.
         :rtype: str
         """
         return self._primary_currency
 
     @primary_currency.setter
     def primary_currency(self, primary_currency):
         """Sets the primary_currency of this AbstractSpaceUpdate.
 
-            This is the currency that is used to display aggregated amounts in the space.
+            The currency that is used to display aggregated amounts in the space.
 
         :param primary_currency: The primary_currency of this AbstractSpaceUpdate.
         :type: str
         """
 
         self._primary_currency = primary_currency
     
     @property
     def request_limit(self):
         """Gets the request_limit of this AbstractSpaceUpdate.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes for this space. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted within two minutes. This limit can only be changed with special privileges.
 
         :return: The request_limit of this AbstractSpaceUpdate.
         :rtype: int
         """
         return self._request_limit
 
     @request_limit.setter
     def request_limit(self, request_limit):
         """Sets the request_limit of this AbstractSpaceUpdate.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes for this space. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted within two minutes. This limit can only be changed with special privileges.
 
         :param request_limit: The request_limit of this AbstractSpaceUpdate.
         :type: int
         """
 
         self._request_limit = request_limit
     
@@ -189,49 +189,49 @@
 
         self._state = state
     
     @property
     def technical_contact_addresses(self):
         """Gets the technical_contact_addresses of this AbstractSpaceUpdate.
 
-            The email address provided as contact addresses will be informed about technical issues or errors triggered by the space.
+            The email address that will receive messages about technical issues and errors that occur in the space.
 
         :return: The technical_contact_addresses of this AbstractSpaceUpdate.
         :rtype: list[str]
         """
         return self._technical_contact_addresses
 
     @technical_contact_addresses.setter
     def technical_contact_addresses(self, technical_contact_addresses):
         """Sets the technical_contact_addresses of this AbstractSpaceUpdate.
 
-            The email address provided as contact addresses will be informed about technical issues or errors triggered by the space.
+            The email address that will receive messages about technical issues and errors that occur in the space.
 
         :param technical_contact_addresses: The technical_contact_addresses of this AbstractSpaceUpdate.
         :type: list[str]
         """
 
         self._technical_contact_addresses = technical_contact_addresses
     
     @property
     def time_zone(self):
         """Gets the time_zone of this AbstractSpaceUpdate.
 
-            The time zone assigned to the space determines the time offset for calculating dates within the space. This is typically used for background processed which needs to be triggered on a specific hour within the day. Changing the space time zone will not change the display of dates.
+            The time zone that is used to schedule and run background processes. This does not affect the formatting of dates in the user interface.
 
         :return: The time_zone of this AbstractSpaceUpdate.
         :rtype: str
         """
         return self._time_zone
 
     @time_zone.setter
     def time_zone(self, time_zone):
         """Sets the time_zone of this AbstractSpaceUpdate.
 
-            The time zone assigned to the space determines the time offset for calculating dates within the space. This is typically used for background processed which needs to be triggered on a specific hour within the day. Changing the space time zone will not change the display of dates.
+            The time zone that is used to schedule and run background processes. This does not affect the formatting of dates in the user interface.
 
         :param time_zone: The time_zone of this AbstractSpaceUpdate.
         :type: str
         """
 
         self._time_zone = time_zone
```

### Comparing `wallee-3.4.0/wallee/models/abstract_subscriber_update.py` & `wallee-4.0.0/wallee/models/abstract_subscriber_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,26 +192,26 @@
 
         self._language = language
     
     @property
     def meta_data(self):
         """Gets the meta_data of this AbstractSubscriberUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this AbstractSubscriberUpdate.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this AbstractSubscriberUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this AbstractSubscriberUpdate.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/abstract_subscription_affiliate_update.py` & `wallee-4.0.0/wallee/models/abstract_subscription_affiliate_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,26 +58,26 @@
 
         self._language = language
     
     @property
     def meta_data(self):
         """Gets the meta_data of this AbstractSubscriptionAffiliateUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this AbstractSubscriptionAffiliateUpdate.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this AbstractSubscriptionAffiliateUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this AbstractSubscriptionAffiliateUpdate.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/abstract_subscription_metric_update.py` & `wallee-4.0.0/wallee/models/abstract_subscription_metric_update.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 
 class AbstractSubscriptionMetricUpdate:
 
     swagger_types = {
     
-        'description': 'DatabaseTranslatedStringCreate',
-        'name': 'DatabaseTranslatedStringCreate',
+        'description': 'dict(str, str)',
+        'name': 'dict(str, str)',
     }
 
     attribute_map = {
         'description': 'description','name': 'name',
     }
 
     
@@ -32,49 +32,49 @@
     @property
     def description(self):
         """Gets the description of this AbstractSubscriptionMetricUpdate.
 
             
 
         :return: The description of this AbstractSubscriptionMetricUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this AbstractSubscriptionMetricUpdate.
 
             
 
         :param description: The description of this AbstractSubscriptionMetricUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def name(self):
         """Gets the name of this AbstractSubscriptionMetricUpdate.
 
             
 
         :return: The name of this AbstractSubscriptionMetricUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this AbstractSubscriptionMetricUpdate.
 
             
 
         :param name: The name of this AbstractSubscriptionMetricUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
 
     def to_dict(self):
         result = {}
```

### Comparing `wallee-3.4.0/wallee/models/abstract_subscription_product_active.py` & `wallee-4.0.0/wallee/models/abstract_subscription_product_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/abstract_token_update.py` & `wallee-4.0.0/wallee/models/abstract_token_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/abstract_transaction_comment_active.py` & `wallee-4.0.0/wallee/models/abstract_transaction_comment_active.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,26 +26,26 @@
         
 
     
     @property
     def content(self):
         """Gets the content of this AbstractTransactionCommentActive.
 
-            
+            The comment's actual content.
 
         :return: The content of this AbstractTransactionCommentActive.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
         """Sets the content of this AbstractTransactionCommentActive.
 
-            
+            The comment's actual content.
 
         :param content: The content of this AbstractTransactionCommentActive.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
```

### Comparing `wallee-3.4.0/wallee/models/abstract_transaction_invoice_comment_active.py` & `wallee-4.0.0/wallee/models/abstract_customer_comment_active.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class AbstractTransactionInvoiceCommentActive:
+class AbstractCustomerCommentActive:
 
     swagger_types = {
     
         'content': 'str',
     }
 
     attribute_map = {
@@ -24,30 +24,30 @@
         
         self.content = kwargs.get('content', None)
         
 
     
     @property
     def content(self):
-        """Gets the content of this AbstractTransactionInvoiceCommentActive.
+        """Gets the content of this AbstractCustomerCommentActive.
 
-            
+            The comment's actual content.
 
-        :return: The content of this AbstractTransactionInvoiceCommentActive.
+        :return: The content of this AbstractCustomerCommentActive.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
-        """Sets the content of this AbstractTransactionInvoiceCommentActive.
+        """Sets the content of this AbstractCustomerCommentActive.
 
-            
+            The comment's actual content.
 
-        :param content: The content of this AbstractTransactionInvoiceCommentActive.
+        :param content: The content of this AbstractCustomerCommentActive.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
@@ -70,27 +70,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(AbstractTransactionInvoiceCommentActive, dict):
+        if issubclass(AbstractCustomerCommentActive, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, AbstractTransactionInvoiceCommentActive):
+        if not isinstance(other, AbstractCustomerCommentActive):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/abstract_transaction_pending.py` & `wallee-4.0.0/wallee/models/abstract_transaction_pending.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,26 +366,26 @@
 
         self._merchant_reference = merchant_reference
     
     @property
     def meta_data(self):
         """Gets the meta_data of this AbstractTransactionPending.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this AbstractTransactionPending.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this AbstractTransactionPending.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this AbstractTransactionPending.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/abstract_webhook_listener_update.py` & `wallee-4.0.0/wallee/models/abstract_webhook_listener_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,74 +35,74 @@
         
 
     
     @property
     def entity_states(self):
         """Gets the entity_states of this AbstractWebhookListenerUpdate.
 
-            The target state identifies the state into which entities need to move into to trigger the webhook listener.
+            The entity's target states that are to be monitored.
 
         :return: The entity_states of this AbstractWebhookListenerUpdate.
         :rtype: list[str]
         """
         return self._entity_states
 
     @entity_states.setter
     def entity_states(self, entity_states):
         """Sets the entity_states of this AbstractWebhookListenerUpdate.
 
-            The target state identifies the state into which entities need to move into to trigger the webhook listener.
+            The entity's target states that are to be monitored.
 
         :param entity_states: The entity_states of this AbstractWebhookListenerUpdate.
         :type: list[str]
         """
 
         self._entity_states = entity_states
     
     @property
     def name(self):
         """Gets the name of this AbstractWebhookListenerUpdate.
 
-            The webhook listener name is used internally to identify the webhook listener in administrative interfaces.For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook listener.
 
         :return: The name of this AbstractWebhookListenerUpdate.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this AbstractWebhookListenerUpdate.
 
-            The webhook listener name is used internally to identify the webhook listener in administrative interfaces.For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook listener.
 
         :param name: The name of this AbstractWebhookListenerUpdate.
         :type: str
         """
         if name is not None and len(name) > 50:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")
 
         self._name = name
     
     @property
     def notify_every_change(self):
         """Gets the notify_every_change of this AbstractWebhookListenerUpdate.
 
-            Defines whether the webhook listener is to be informed about every change made to the entity in contrast to state transitions only.
+            Whether every update of the entity or only state changes are to be monitored.
 
         :return: The notify_every_change of this AbstractWebhookListenerUpdate.
         :rtype: bool
         """
         return self._notify_every_change
 
     @notify_every_change.setter
     def notify_every_change(self, notify_every_change):
         """Sets the notify_every_change of this AbstractWebhookListenerUpdate.
 
-            Defines whether the webhook listener is to be informed about every change made to the entity in contrast to state transitions only.
+            Whether every update of the entity or only state changes are to be monitored.
 
         :param notify_every_change: The notify_every_change of this AbstractWebhookListenerUpdate.
         :type: bool
         """
 
         self._notify_every_change = notify_every_change
```

### Comparing `wallee-3.4.0/wallee/models/abstract_webhook_url_update.py` & `wallee-4.0.0/wallee/models/abstract_webhook_url_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def name(self):
         """Gets the name of this AbstractWebhookUrlUpdate.
 
-            The URL name is used internally to identify the URL in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook URL.
 
         :return: The name of this AbstractWebhookUrlUpdate.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this AbstractWebhookUrlUpdate.
 
-            The URL name is used internally to identify the URL in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook URL.
 
         :param name: The name of this AbstractWebhookUrlUpdate.
         :type: str
         """
         if name is not None and len(name) > 50:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")
 
@@ -80,26 +80,26 @@
 
         self._state = state
     
     @property
     def url(self):
         """Gets the url of this AbstractWebhookUrlUpdate.
 
-            The URL to which the HTTP requests are sent to. An example URL could look like https://www.example.com/some/path?some-query-parameter=value.
+            The actual URL where notifications about entity changes are sent to.
 
         :return: The url of this AbstractWebhookUrlUpdate.
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """Sets the url of this AbstractWebhookUrlUpdate.
 
-            The URL to which the HTTP requests are sent to. An example URL could look like https://www.example.com/some/path?some-query-parameter=value.
+            The actual URL where notifications about entity changes are sent to.
 
         :param url: The url of this AbstractWebhookUrlUpdate.
         :type: str
         """
         if url is not None and len(url) > 500:
             raise ValueError("Invalid value for `url`, length must be less than or equal to `500`")
         if url is not None and len(url) < 9:
```

### Comparing `wallee-3.4.0/wallee/models/account.py` & `wallee-4.0.0/wallee/models/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,141 +74,141 @@
         
 
     
     @property
     def active(self):
         """Gets the active of this Account.
 
-            Active means that this account and all accounts in the hierarchy are active.
+            Whether this account and all its parent accounts are active.
 
         :return: The active of this Account.
         :rtype: bool
         """
         return self._active
 
     @active.setter
     def active(self, active):
         """Sets the active of this Account.
 
-            Active means that this account and all accounts in the hierarchy are active.
+            Whether this account and all its parent accounts are active.
 
         :param active: The active of this Account.
         :type: bool
         """
 
         self._active = active
     
     @property
     def active_or_restricted_active(self):
         """Gets the active_or_restricted_active of this Account.
 
-            This property is true when all accounts in the hierarchy are active or restricted active.
+            Whether this account and all its parent accounts are active or restricted active.
 
         :return: The active_or_restricted_active of this Account.
         :rtype: bool
         """
         return self._active_or_restricted_active
 
     @active_or_restricted_active.setter
     def active_or_restricted_active(self, active_or_restricted_active):
         """Sets the active_or_restricted_active of this Account.
 
-            This property is true when all accounts in the hierarchy are active or restricted active.
+            Whether this account and all its parent accounts are active or restricted active.
 
         :param active_or_restricted_active: The active_or_restricted_active of this Account.
         :type: bool
         """
 
         self._active_or_restricted_active = active_or_restricted_active
     
     @property
     def created_by(self):
         """Gets the created_by of this Account.
 
-            The ID of the user who created this entity.
+            The ID of the user the account was created by.
 
         :return: The created_by of this Account.
         :rtype: int
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this Account.
 
-            The ID of the user who created this entity.
+            The ID of the user the account was created by.
 
         :param created_by: The created_by of this Account.
         :type: int
         """
 
         self._created_by = created_by
     
     @property
     def created_on(self):
         """Gets the created_on of this Account.
 
-            The date and time when this entity was created.
+            The date and time when the account was created.
 
         :return: The created_on of this Account.
         :rtype: datetime
         """
         return self._created_on
 
     @created_on.setter
     def created_on(self, created_on):
         """Sets the created_on of this Account.
 
-            The date and time when this entity was created.
+            The date and time when the account was created.
 
         :param created_on: The created_on of this Account.
         :type: datetime
         """
 
         self._created_on = created_on
     
     @property
     def deleted_by(self):
         """Gets the deleted_by of this Account.
 
-            The ID of a user that deleted this entity.
+            The ID of a user the account was deleted by.
 
         :return: The deleted_by of this Account.
         :rtype: int
         """
         return self._deleted_by
 
     @deleted_by.setter
     def deleted_by(self, deleted_by):
         """Sets the deleted_by of this Account.
 
-            The ID of a user that deleted this entity.
+            The ID of a user the account was deleted by.
 
         :param deleted_by: The deleted_by of this Account.
         :type: int
         """
 
         self._deleted_by = deleted_by
     
     @property
     def deleted_on(self):
         """Gets the deleted_on of this Account.
 
-            The date and time when this entity was deleted.
+            The date and time when the account was deleted.
 
         :return: The deleted_on of this Account.
         :rtype: datetime
         """
         return self._deleted_on
 
     @deleted_on.setter
     def deleted_on(self, deleted_on):
         """Sets the deleted_on of this Account.
 
-            The date and time when this entity was deleted.
+            The date and time when the account was deleted.
 
         :param deleted_on: The deleted_on of this Account.
         :type: datetime
         """
 
         self._deleted_on = deleted_on
     
@@ -258,26 +258,26 @@
 
         self._last_modified_date = last_modified_date
     
     @property
     def name(self):
         """Gets the name of this Account.
 
-            The name of the account identifies the account within the administrative interface.
+            The name used to identify the account.
 
         :return: The name of this Account.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Account.
 
-            The name of the account identifies the account within the administrative interface.
+            The name used to identify the account.
 
         :param name: The name of this Account.
         :type: str
         """
         if name is not None and len(name) > 200:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `200`")
         if name is not None and len(name) < 3:
@@ -285,26 +285,26 @@
 
         self._name = name
     
     @property
     def parent_account(self):
         """Gets the parent_account of this Account.
 
-            The account which is responsible for administering the account.
+            The parent account responsible for administering this account.
 
         :return: The parent_account of this Account.
         :rtype: Account
         """
         return self._parent_account
 
     @parent_account.setter
     def parent_account(self, parent_account):
         """Sets the parent_account of this Account.
 
-            The account which is responsible for administering the account.
+            The parent account responsible for administering this account.
 
         :param parent_account: The parent_account of this Account.
         :type: Account
         """
 
         self._parent_account = parent_account
     
@@ -331,49 +331,49 @@
 
         self._planned_purge_date = planned_purge_date
     
     @property
     def restricted_active(self):
         """Gets the restricted_active of this Account.
 
-            Restricted active means that at least one account in the hierarchy is only restricted active, but all are either restricted active or active.
+            Whether this account and all its parent accounts are active or restricted active. There is at least one account that is restricted active.
 
         :return: The restricted_active of this Account.
         :rtype: bool
         """
         return self._restricted_active
 
     @restricted_active.setter
     def restricted_active(self, restricted_active):
         """Sets the restricted_active of this Account.
 
-            Restricted active means that at least one account in the hierarchy is only restricted active, but all are either restricted active or active.
+            Whether this account and all its parent accounts are active or restricted active. There is at least one account that is restricted active.
 
         :param restricted_active: The restricted_active of this Account.
         :type: bool
         """
 
         self._restricted_active = restricted_active
     
     @property
     def scope(self):
         """Gets the scope of this Account.
 
-            This is the scope to which the account belongs to.
+            The scope that the account belongs to.
 
         :return: The scope of this Account.
         :rtype: int
         """
         return self._scope
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this Account.
 
-            This is the scope to which the account belongs to.
+            The scope that the account belongs to.
 
         :param scope: The scope of this Account.
         :type: int
         """
 
         self._scope = scope
     
@@ -400,49 +400,49 @@
 
         self._state = state
     
     @property
     def subaccount_limit(self):
         """Gets the subaccount_limit of this Account.
 
-            This property restricts the number of subaccounts which can be created within this account.
+            The number of sub-accounts that can be created within this account.
 
         :return: The subaccount_limit of this Account.
         :rtype: int
         """
         return self._subaccount_limit
 
     @subaccount_limit.setter
     def subaccount_limit(self, subaccount_limit):
         """Sets the subaccount_limit of this Account.
 
-            This property restricts the number of subaccounts which can be created within this account.
+            The number of sub-accounts that can be created within this account.
 
         :param subaccount_limit: The subaccount_limit of this Account.
         :type: int
         """
 
         self._subaccount_limit = subaccount_limit
     
     @property
     def type(self):
         """Gets the type of this Account.
 
-            The account type defines which role and capabilities it has.
+            The account's type which defines its role and capabilities.
 
         :return: The type of this Account.
         :rtype: AccountType
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this Account.
 
-            The account type defines which role and capabilities it has.
+            The account's type which defines its role and capabilities.
 
         :param type: The type of this Account.
         :type: AccountType
         """
 
         self._type = type
```

### Comparing `wallee-3.4.0/wallee/models/account_create.py` & `wallee-4.0.0/wallee/models/space_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,62 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractAccountUpdate
+from . import AbstractSpaceUpdate
 
 
-class AccountCreate(AbstractAccountUpdate):
+class SpaceCreate(AbstractSpaceUpdate):
 
     swagger_types = {
     
-        'parent_account': 'int',
-        'scope': 'int',
+        'account': 'int',
     }
 
     attribute_map = {
-        'parent_account': 'parentAccount','scope': 'scope',
+        'account': 'account',
     }
 
     
-    _parent_account = None
-    _scope = None
+    _account = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.parent_account = kwargs.get('parent_account', None)
-        self.scope = kwargs.get('scope')
+        self.account = kwargs.get('account')
 
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def parent_account(self):
-        """Gets the parent_account of this AccountCreate.
+    def account(self):
+        """Gets the account of this SpaceCreate.
 
-            The account which is responsible for administering the account.
+            The account that the space belongs to.
 
-        :return: The parent_account of this AccountCreate.
+        :return: The account of this SpaceCreate.
         :rtype: int
         """
-        return self._parent_account
+        return self._account
 
-    @parent_account.setter
-    def parent_account(self, parent_account):
-        """Sets the parent_account of this AccountCreate.
+    @account.setter
+    def account(self, account):
+        """Sets the account of this SpaceCreate.
 
-            The account which is responsible for administering the account.
+            The account that the space belongs to.
 
-        :param parent_account: The parent_account of this AccountCreate.
+        :param account: The account of this SpaceCreate.
         :type: int
         """
+        if account is None:
+            raise ValueError("Invalid value for `account`, must not be `None`")
 
-        self._parent_account = parent_account
-    
-    @property
-    def scope(self):
-        """Gets the scope of this AccountCreate.
-
-            This is the scope to which the account belongs to.
-
-        :return: The scope of this AccountCreate.
-        :rtype: int
-        """
-        return self._scope
-
-    @scope.setter
-    def scope(self, scope):
-        """Sets the scope of this AccountCreate.
-
-            This is the scope to which the account belongs to.
-
-        :param scope: The scope of this AccountCreate.
-        :type: int
-        """
-        if scope is None:
-            raise ValueError("Invalid value for `scope`, must not be `None`")
-
-        self._scope = scope
+        self._account = account
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -99,27 +73,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(AccountCreate, dict):
+        if issubclass(SpaceCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, AccountCreate):
+        if not isinstance(other, SpaceCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/account_update.py` & `wallee-4.0.0/wallee/models/account_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/address.py` & `wallee-4.0.0/wallee/models/address_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class Address:
+class AddressCreate:
 
     swagger_types = {
     
         'city': 'str',
         'commercial_register_number': 'str',
         'country': 'str',
         'date_of_birth': 'date',
         'dependent_locality': 'str',
         'email_address': 'str',
         'family_name': 'str',
         'gender': 'Gender',
         'given_name': 'str',
-        'legal_organization_form': 'LegalOrganizationForm',
+        'legal_organization_form': 'int',
         'mobile_phone_number': 'str',
         'organization_name': 'str',
         'phone_number': 'str',
         'postal_state': 'str',
         'postcode': 'str',
         'sales_tax_number': 'str',
         'salutation': 'str',
@@ -81,495 +81,495 @@
         self.sorting_code = kwargs.get('sorting_code', None)
         self.street = kwargs.get('street', None)
         
 
     
     @property
     def city(self):
-        """Gets the city of this Address.
+        """Gets the city of this AddressCreate.
 
-            
+            The city, town or village.
 
-        :return: The city of this Address.
+        :return: The city of this AddressCreate.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
-        """Sets the city of this Address.
+        """Sets the city of this AddressCreate.
 
-            
+            The city, town or village.
 
-        :param city: The city of this Address.
+        :param city: The city of this AddressCreate.
         :type: str
         """
         if city is not None and len(city) > 100:
             raise ValueError("Invalid value for `city`, length must be less than or equal to `100`")
 
         self._city = city
     
     @property
     def commercial_register_number(self):
-        """Gets the commercial_register_number of this Address.
+        """Gets the commercial_register_number of this AddressCreate.
 
-            
+            The commercial registration number of the organization.
 
-        :return: The commercial_register_number of this Address.
+        :return: The commercial_register_number of this AddressCreate.
         :rtype: str
         """
         return self._commercial_register_number
 
     @commercial_register_number.setter
     def commercial_register_number(self, commercial_register_number):
-        """Sets the commercial_register_number of this Address.
+        """Sets the commercial_register_number of this AddressCreate.
 
-            
+            The commercial registration number of the organization.
 
-        :param commercial_register_number: The commercial_register_number of this Address.
+        :param commercial_register_number: The commercial_register_number of this AddressCreate.
         :type: str
         """
         if commercial_register_number is not None and len(commercial_register_number) > 100:
             raise ValueError("Invalid value for `commercial_register_number`, length must be less than or equal to `100`")
 
         self._commercial_register_number = commercial_register_number
     
     @property
     def country(self):
-        """Gets the country of this Address.
+        """Gets the country of this AddressCreate.
 
-            
+            The country is represented with a two-letter code (ISO 3166-1 alpha-2 standard) - for example, CH for Switzerland.
 
-        :return: The country of this Address.
+        :return: The country of this AddressCreate.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
-        """Sets the country of this Address.
+        """Sets the country of this AddressCreate.
 
-            
+            The country is represented with a two-letter code (ISO 3166-1 alpha-2 standard) - for example, CH for Switzerland.
 
-        :param country: The country of this Address.
+        :param country: The country of this AddressCreate.
         :type: str
         """
 
         self._country = country
     
     @property
     def date_of_birth(self):
-        """Gets the date_of_birth of this Address.
+        """Gets the date_of_birth of this AddressCreate.
 
-            
+            The date of birth.
 
-        :return: The date_of_birth of this Address.
+        :return: The date_of_birth of this AddressCreate.
         :rtype: date
         """
         return self._date_of_birth
 
     @date_of_birth.setter
     def date_of_birth(self, date_of_birth):
-        """Sets the date_of_birth of this Address.
+        """Sets the date_of_birth of this AddressCreate.
 
-            
+            The date of birth.
 
-        :param date_of_birth: The date_of_birth of this Address.
+        :param date_of_birth: The date_of_birth of this AddressCreate.
         :type: date
         """
 
         self._date_of_birth = date_of_birth
     
     @property
     def dependent_locality(self):
-        """Gets the dependent_locality of this Address.
+        """Gets the dependent_locality of this AddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
-        :return: The dependent_locality of this Address.
+        :return: The dependent_locality of this AddressCreate.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
-        """Sets the dependent_locality of this Address.
+        """Sets the dependent_locality of this AddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
-        :param dependent_locality: The dependent_locality of this Address.
+        :param dependent_locality: The dependent_locality of this AddressCreate.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
-        """Gets the email_address of this Address.
+        """Gets the email_address of this AddressCreate.
 
-            
+            The email address.
 
-        :return: The email_address of this Address.
+        :return: The email_address of this AddressCreate.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
-        """Sets the email_address of this Address.
+        """Sets the email_address of this AddressCreate.
 
-            
+            The email address.
 
-        :param email_address: The email_address of this Address.
+        :param email_address: The email_address of this AddressCreate.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
-        """Gets the family_name of this Address.
+        """Gets the family_name of this AddressCreate.
 
-            
+            The family or last name.
 
-        :return: The family_name of this Address.
+        :return: The family_name of this AddressCreate.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
-        """Sets the family_name of this Address.
+        """Sets the family_name of this AddressCreate.
 
-            
+            The family or last name.
 
-        :param family_name: The family_name of this Address.
+        :param family_name: The family_name of this AddressCreate.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
     def gender(self):
-        """Gets the gender of this Address.
+        """Gets the gender of this AddressCreate.
 
-            
+            The gender.
 
-        :return: The gender of this Address.
+        :return: The gender of this AddressCreate.
         :rtype: Gender
         """
         return self._gender
 
     @gender.setter
     def gender(self, gender):
-        """Sets the gender of this Address.
+        """Sets the gender of this AddressCreate.
 
-            
+            The gender.
 
-        :param gender: The gender of this Address.
+        :param gender: The gender of this AddressCreate.
         :type: Gender
         """
 
         self._gender = gender
     
     @property
     def given_name(self):
-        """Gets the given_name of this Address.
+        """Gets the given_name of this AddressCreate.
 
-            
+            The given or first name.
 
-        :return: The given_name of this Address.
+        :return: The given_name of this AddressCreate.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
-        """Sets the given_name of this Address.
+        """Sets the given_name of this AddressCreate.
 
-            
+            The given or first name.
 
-        :param given_name: The given_name of this Address.
+        :param given_name: The given_name of this AddressCreate.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
         self._given_name = given_name
     
     @property
     def legal_organization_form(self):
-        """Gets the legal_organization_form of this Address.
+        """Gets the legal_organization_form of this AddressCreate.
 
-            
+            The legal form of the organization.
 
-        :return: The legal_organization_form of this Address.
-        :rtype: LegalOrganizationForm
+        :return: The legal_organization_form of this AddressCreate.
+        :rtype: int
         """
         return self._legal_organization_form
 
     @legal_organization_form.setter
     def legal_organization_form(self, legal_organization_form):
-        """Sets the legal_organization_form of this Address.
+        """Sets the legal_organization_form of this AddressCreate.
 
-            
+            The legal form of the organization.
 
-        :param legal_organization_form: The legal_organization_form of this Address.
-        :type: LegalOrganizationForm
+        :param legal_organization_form: The legal_organization_form of this AddressCreate.
+        :type: int
         """
 
         self._legal_organization_form = legal_organization_form
     
     @property
     def mobile_phone_number(self):
-        """Gets the mobile_phone_number of this Address.
+        """Gets the mobile_phone_number of this AddressCreate.
 
-            
+            The phone number of a mobile phone.
 
-        :return: The mobile_phone_number of this Address.
+        :return: The mobile_phone_number of this AddressCreate.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
-        """Sets the mobile_phone_number of this Address.
+        """Sets the mobile_phone_number of this AddressCreate.
 
-            
+            The phone number of a mobile phone.
 
-        :param mobile_phone_number: The mobile_phone_number of this Address.
+        :param mobile_phone_number: The mobile_phone_number of this AddressCreate.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
-        """Gets the organization_name of this Address.
+        """Gets the organization_name of this AddressCreate.
 
-            
+            The organization's name.
 
-        :return: The organization_name of this Address.
+        :return: The organization_name of this AddressCreate.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
-        """Sets the organization_name of this Address.
+        """Sets the organization_name of this AddressCreate.
 
-            
+            The organization's name.
 
-        :param organization_name: The organization_name of this Address.
+        :param organization_name: The organization_name of this AddressCreate.
         :type: str
         """
         if organization_name is not None and len(organization_name) > 100:
             raise ValueError("Invalid value for `organization_name`, length must be less than or equal to `100`")
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
-        """Gets the phone_number of this Address.
+        """Gets the phone_number of this AddressCreate.
 
-            
+            The phone number.
 
-        :return: The phone_number of this Address.
+        :return: The phone_number of this AddressCreate.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
-        """Sets the phone_number of this Address.
+        """Sets the phone_number of this AddressCreate.
 
-            
+            The phone number.
 
-        :param phone_number: The phone_number of this Address.
+        :param phone_number: The phone_number of this AddressCreate.
         :type: str
         """
         if phone_number is not None and len(phone_number) > 100:
             raise ValueError("Invalid value for `phone_number`, length must be less than or equal to `100`")
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
-        """Gets the postal_state of this Address.
+        """Gets the postal_state of this AddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
-        :return: The postal_state of this Address.
+        :return: The postal_state of this AddressCreate.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
-        """Sets the postal_state of this Address.
+        """Sets the postal_state of this AddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
-        :param postal_state: The postal_state of this Address.
+        :param postal_state: The postal_state of this AddressCreate.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
-        """Gets the postcode of this Address.
+        """Gets the postcode of this AddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
-        :return: The postcode of this Address.
+        :return: The postcode of this AddressCreate.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
-        """Sets the postcode of this Address.
+        """Sets the postcode of this AddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
-        :param postcode: The postcode of this Address.
+        :param postcode: The postcode of this AddressCreate.
         :type: str
         """
         if postcode is not None and len(postcode) > 40:
             raise ValueError("Invalid value for `postcode`, length must be less than or equal to `40`")
 
         self._postcode = postcode
     
     @property
     def sales_tax_number(self):
-        """Gets the sales_tax_number of this Address.
+        """Gets the sales_tax_number of this AddressCreate.
 
-            
+            The sales tax number of the organization.
 
-        :return: The sales_tax_number of this Address.
+        :return: The sales_tax_number of this AddressCreate.
         :rtype: str
         """
         return self._sales_tax_number
 
     @sales_tax_number.setter
     def sales_tax_number(self, sales_tax_number):
-        """Sets the sales_tax_number of this Address.
+        """Sets the sales_tax_number of this AddressCreate.
 
-            
+            The sales tax number of the organization.
 
-        :param sales_tax_number: The sales_tax_number of this Address.
+        :param sales_tax_number: The sales_tax_number of this AddressCreate.
         :type: str
         """
         if sales_tax_number is not None and len(sales_tax_number) > 100:
             raise ValueError("Invalid value for `sales_tax_number`, length must be less than or equal to `100`")
 
         self._sales_tax_number = sales_tax_number
     
     @property
     def salutation(self):
-        """Gets the salutation of this Address.
+        """Gets the salutation of this AddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
-        :return: The salutation of this Address.
+        :return: The salutation of this AddressCreate.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
-        """Sets the salutation of this Address.
+        """Sets the salutation of this AddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
-        :param salutation: The salutation of this Address.
+        :param salutation: The salutation of this AddressCreate.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
     def social_security_number(self):
-        """Gets the social_security_number of this Address.
+        """Gets the social_security_number of this AddressCreate.
 
-            
+            The social security number.
 
-        :return: The social_security_number of this Address.
+        :return: The social_security_number of this AddressCreate.
         :rtype: str
         """
         return self._social_security_number
 
     @social_security_number.setter
     def social_security_number(self, social_security_number):
-        """Sets the social_security_number of this Address.
+        """Sets the social_security_number of this AddressCreate.
 
-            
+            The social security number.
 
-        :param social_security_number: The social_security_number of this Address.
+        :param social_security_number: The social_security_number of this AddressCreate.
         :type: str
         """
         if social_security_number is not None and len(social_security_number) > 100:
             raise ValueError("Invalid value for `social_security_number`, length must be less than or equal to `100`")
 
         self._social_security_number = social_security_number
     
     @property
     def sorting_code(self):
-        """Gets the sorting_code of this Address.
+        """Gets the sorting_code of this AddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
-        :return: The sorting_code of this Address.
+        :return: The sorting_code of this AddressCreate.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
-        """Sets the sorting_code of this Address.
+        """Sets the sorting_code of this AddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
-        :param sorting_code: The sorting_code of this Address.
+        :param sorting_code: The sorting_code of this AddressCreate.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
-        """Gets the street of this Address.
+        """Gets the street of this AddressCreate.
 
-            
+            The street or PO Box.
 
-        :return: The street of this Address.
+        :return: The street of this AddressCreate.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
-        """Sets the street of this Address.
+        """Sets the street of this AddressCreate.
 
-            
+            The street or PO Box.
 
-        :param street: The street of this Address.
+        :param street: The street of this AddressCreate.
         :type: str
         """
         if street is not None and len(street) > 300:
             raise ValueError("Invalid value for `street`, length must be less than or equal to `300`")
 
         self._street = street
     
@@ -592,27 +592,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(Address, dict):
+        if issubclass(AddressCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, Address):
+        if not isinstance(other, AddressCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/address_create.py` & `wallee-4.0.0/wallee/models/space_address_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,579 +1,437 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class AddressCreate:
+class SpaceAddressCreate:
 
     swagger_types = {
     
         'city': 'str',
-        'commercial_register_number': 'str',
         'country': 'str',
-        'date_of_birth': 'date',
         'dependent_locality': 'str',
         'email_address': 'str',
         'family_name': 'str',
-        'gender': 'Gender',
         'given_name': 'str',
-        'legal_organization_form': 'int',
         'mobile_phone_number': 'str',
         'organization_name': 'str',
         'phone_number': 'str',
         'postal_state': 'str',
         'postcode': 'str',
         'sales_tax_number': 'str',
         'salutation': 'str',
-        'social_security_number': 'str',
         'sorting_code': 'str',
         'street': 'str',
     }
 
     attribute_map = {
-        'city': 'city','commercial_register_number': 'commercialRegisterNumber','country': 'country','date_of_birth': 'dateOfBirth','dependent_locality': 'dependentLocality','email_address': 'emailAddress','family_name': 'familyName','gender': 'gender','given_name': 'givenName','legal_organization_form': 'legalOrganizationForm','mobile_phone_number': 'mobilePhoneNumber','organization_name': 'organizationName','phone_number': 'phoneNumber','postal_state': 'postalState','postcode': 'postcode','sales_tax_number': 'salesTaxNumber','salutation': 'salutation','social_security_number': 'socialSecurityNumber','sorting_code': 'sortingCode','street': 'street',
+        'city': 'city','country': 'country','dependent_locality': 'dependentLocality','email_address': 'emailAddress','family_name': 'familyName','given_name': 'givenName','mobile_phone_number': 'mobilePhoneNumber','organization_name': 'organizationName','phone_number': 'phoneNumber','postal_state': 'postalState','postcode': 'postcode','sales_tax_number': 'salesTaxNumber','salutation': 'salutation','sorting_code': 'sortingCode','street': 'street',
     }
 
     
     _city = None
-    _commercial_register_number = None
     _country = None
-    _date_of_birth = None
     _dependent_locality = None
     _email_address = None
     _family_name = None
-    _gender = None
     _given_name = None
-    _legal_organization_form = None
     _mobile_phone_number = None
     _organization_name = None
     _phone_number = None
     _postal_state = None
     _postcode = None
     _sales_tax_number = None
     _salutation = None
-    _social_security_number = None
     _sorting_code = None
     _street = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.city = kwargs.get('city', None)
-        self.commercial_register_number = kwargs.get('commercial_register_number', None)
         self.country = kwargs.get('country', None)
-        self.date_of_birth = kwargs.get('date_of_birth', None)
         self.dependent_locality = kwargs.get('dependent_locality', None)
         self.email_address = kwargs.get('email_address', None)
         self.family_name = kwargs.get('family_name', None)
-        self.gender = kwargs.get('gender', None)
         self.given_name = kwargs.get('given_name', None)
-        self.legal_organization_form = kwargs.get('legal_organization_form', None)
         self.mobile_phone_number = kwargs.get('mobile_phone_number', None)
         self.organization_name = kwargs.get('organization_name', None)
         self.phone_number = kwargs.get('phone_number', None)
         self.postal_state = kwargs.get('postal_state', None)
         self.postcode = kwargs.get('postcode', None)
         self.sales_tax_number = kwargs.get('sales_tax_number', None)
         self.salutation = kwargs.get('salutation', None)
-        self.social_security_number = kwargs.get('social_security_number', None)
         self.sorting_code = kwargs.get('sorting_code', None)
         self.street = kwargs.get('street', None)
         
 
     
     @property
     def city(self):
-        """Gets the city of this AddressCreate.
+        """Gets the city of this SpaceAddressCreate.
 
-            
+            The city, town or village.
 
-        :return: The city of this AddressCreate.
+        :return: The city of this SpaceAddressCreate.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
-        """Sets the city of this AddressCreate.
+        """Sets the city of this SpaceAddressCreate.
 
-            
+            The city, town or village.
 
-        :param city: The city of this AddressCreate.
+        :param city: The city of this SpaceAddressCreate.
         :type: str
         """
-        if city is not None and len(city) > 100:
-            raise ValueError("Invalid value for `city`, length must be less than or equal to `100`")
 
         self._city = city
     
     @property
-    def commercial_register_number(self):
-        """Gets the commercial_register_number of this AddressCreate.
-
-            
-
-        :return: The commercial_register_number of this AddressCreate.
-        :rtype: str
-        """
-        return self._commercial_register_number
-
-    @commercial_register_number.setter
-    def commercial_register_number(self, commercial_register_number):
-        """Sets the commercial_register_number of this AddressCreate.
-
-            
-
-        :param commercial_register_number: The commercial_register_number of this AddressCreate.
-        :type: str
-        """
-        if commercial_register_number is not None and len(commercial_register_number) > 100:
-            raise ValueError("Invalid value for `commercial_register_number`, length must be less than or equal to `100`")
-
-        self._commercial_register_number = commercial_register_number
-    
-    @property
     def country(self):
-        """Gets the country of this AddressCreate.
+        """Gets the country of this SpaceAddressCreate.
 
-            
+            The two-letter country code (ISO 3166 format).
 
-        :return: The country of this AddressCreate.
+        :return: The country of this SpaceAddressCreate.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
-        """Sets the country of this AddressCreate.
+        """Sets the country of this SpaceAddressCreate.
 
-            
+            The two-letter country code (ISO 3166 format).
 
-        :param country: The country of this AddressCreate.
+        :param country: The country of this SpaceAddressCreate.
         :type: str
         """
 
         self._country = country
     
     @property
-    def date_of_birth(self):
-        """Gets the date_of_birth of this AddressCreate.
-
-            
-
-        :return: The date_of_birth of this AddressCreate.
-        :rtype: date
-        """
-        return self._date_of_birth
-
-    @date_of_birth.setter
-    def date_of_birth(self, date_of_birth):
-        """Sets the date_of_birth of this AddressCreate.
-
-            
-
-        :param date_of_birth: The date_of_birth of this AddressCreate.
-        :type: date
-        """
-
-        self._date_of_birth = date_of_birth
-    
-    @property
     def dependent_locality(self):
-        """Gets the dependent_locality of this AddressCreate.
+        """Gets the dependent_locality of this SpaceAddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
-        :return: The dependent_locality of this AddressCreate.
+        :return: The dependent_locality of this SpaceAddressCreate.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
-        """Sets the dependent_locality of this AddressCreate.
+        """Sets the dependent_locality of this SpaceAddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
-        :param dependent_locality: The dependent_locality of this AddressCreate.
+        :param dependent_locality: The dependent_locality of this SpaceAddressCreate.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
-        """Gets the email_address of this AddressCreate.
+        """Gets the email_address of this SpaceAddressCreate.
 
-            
+            The email address used for communication with clients.
 
-        :return: The email_address of this AddressCreate.
+        :return: The email_address of this SpaceAddressCreate.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
-        """Sets the email_address of this AddressCreate.
+        """Sets the email_address of this SpaceAddressCreate.
 
-            
+            The email address used for communication with clients.
 
-        :param email_address: The email_address of this AddressCreate.
+        :param email_address: The email_address of this SpaceAddressCreate.
         :type: str
         """
-        if email_address is not None and len(email_address) > 254:
-            raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
-        """Gets the family_name of this AddressCreate.
+        """Gets the family_name of this SpaceAddressCreate.
 
-            
+            The family or last name.
 
-        :return: The family_name of this AddressCreate.
+        :return: The family_name of this SpaceAddressCreate.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
-        """Sets the family_name of this AddressCreate.
+        """Sets the family_name of this SpaceAddressCreate.
 
-            
+            The family or last name.
 
-        :param family_name: The family_name of this AddressCreate.
+        :param family_name: The family_name of this SpaceAddressCreate.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
-    def gender(self):
-        """Gets the gender of this AddressCreate.
-
-            
-
-        :return: The gender of this AddressCreate.
-        :rtype: Gender
-        """
-        return self._gender
-
-    @gender.setter
-    def gender(self, gender):
-        """Sets the gender of this AddressCreate.
-
-            
-
-        :param gender: The gender of this AddressCreate.
-        :type: Gender
-        """
-
-        self._gender = gender
-    
-    @property
     def given_name(self):
-        """Gets the given_name of this AddressCreate.
+        """Gets the given_name of this SpaceAddressCreate.
 
-            
+            The given or first name.
 
-        :return: The given_name of this AddressCreate.
+        :return: The given_name of this SpaceAddressCreate.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
-        """Sets the given_name of this AddressCreate.
+        """Sets the given_name of this SpaceAddressCreate.
 
-            
+            The given or first name.
 
-        :param given_name: The given_name of this AddressCreate.
+        :param given_name: The given_name of this SpaceAddressCreate.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
         self._given_name = given_name
     
     @property
-    def legal_organization_form(self):
-        """Gets the legal_organization_form of this AddressCreate.
-
-            
-
-        :return: The legal_organization_form of this AddressCreate.
-        :rtype: int
-        """
-        return self._legal_organization_form
-
-    @legal_organization_form.setter
-    def legal_organization_form(self, legal_organization_form):
-        """Sets the legal_organization_form of this AddressCreate.
-
-            
-
-        :param legal_organization_form: The legal_organization_form of this AddressCreate.
-        :type: int
-        """
-
-        self._legal_organization_form = legal_organization_form
-    
-    @property
     def mobile_phone_number(self):
-        """Gets the mobile_phone_number of this AddressCreate.
+        """Gets the mobile_phone_number of this SpaceAddressCreate.
 
-            
+            The phone number of a mobile phone.
 
-        :return: The mobile_phone_number of this AddressCreate.
+        :return: The mobile_phone_number of this SpaceAddressCreate.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
-        """Sets the mobile_phone_number of this AddressCreate.
+        """Sets the mobile_phone_number of this SpaceAddressCreate.
 
-            
+            The phone number of a mobile phone.
 
-        :param mobile_phone_number: The mobile_phone_number of this AddressCreate.
+        :param mobile_phone_number: The mobile_phone_number of this SpaceAddressCreate.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
-        """Gets the organization_name of this AddressCreate.
+        """Gets the organization_name of this SpaceAddressCreate.
 
-            
+            The organization's name.
 
-        :return: The organization_name of this AddressCreate.
+        :return: The organization_name of this SpaceAddressCreate.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
-        """Sets the organization_name of this AddressCreate.
+        """Sets the organization_name of this SpaceAddressCreate.
 
-            
+            The organization's name.
 
-        :param organization_name: The organization_name of this AddressCreate.
+        :param organization_name: The organization_name of this SpaceAddressCreate.
         :type: str
         """
         if organization_name is not None and len(organization_name) > 100:
             raise ValueError("Invalid value for `organization_name`, length must be less than or equal to `100`")
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
-        """Gets the phone_number of this AddressCreate.
+        """Gets the phone_number of this SpaceAddressCreate.
 
-            
+            The phone number.
 
-        :return: The phone_number of this AddressCreate.
+        :return: The phone_number of this SpaceAddressCreate.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
-        """Sets the phone_number of this AddressCreate.
+        """Sets the phone_number of this SpaceAddressCreate.
 
-            
+            The phone number.
 
-        :param phone_number: The phone_number of this AddressCreate.
+        :param phone_number: The phone_number of this SpaceAddressCreate.
         :type: str
         """
         if phone_number is not None and len(phone_number) > 100:
             raise ValueError("Invalid value for `phone_number`, length must be less than or equal to `100`")
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
-        """Gets the postal_state of this AddressCreate.
+        """Gets the postal_state of this SpaceAddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
-        :return: The postal_state of this AddressCreate.
+        :return: The postal_state of this SpaceAddressCreate.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
-        """Sets the postal_state of this AddressCreate.
+        """Sets the postal_state of this SpaceAddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
-        :param postal_state: The postal_state of this AddressCreate.
+        :param postal_state: The postal_state of this SpaceAddressCreate.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
-        """Gets the postcode of this AddressCreate.
+        """Gets the postcode of this SpaceAddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
-        :return: The postcode of this AddressCreate.
+        :return: The postcode of this SpaceAddressCreate.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
-        """Sets the postcode of this AddressCreate.
+        """Sets the postcode of this SpaceAddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
-        :param postcode: The postcode of this AddressCreate.
+        :param postcode: The postcode of this SpaceAddressCreate.
         :type: str
         """
-        if postcode is not None and len(postcode) > 40:
-            raise ValueError("Invalid value for `postcode`, length must be less than or equal to `40`")
 
         self._postcode = postcode
     
     @property
     def sales_tax_number(self):
-        """Gets the sales_tax_number of this AddressCreate.
+        """Gets the sales_tax_number of this SpaceAddressCreate.
 
-            
+            The sales tax number of the organization.
 
-        :return: The sales_tax_number of this AddressCreate.
+        :return: The sales_tax_number of this SpaceAddressCreate.
         :rtype: str
         """
         return self._sales_tax_number
 
     @sales_tax_number.setter
     def sales_tax_number(self, sales_tax_number):
-        """Sets the sales_tax_number of this AddressCreate.
+        """Sets the sales_tax_number of this SpaceAddressCreate.
 
-            
+            The sales tax number of the organization.
 
-        :param sales_tax_number: The sales_tax_number of this AddressCreate.
+        :param sales_tax_number: The sales_tax_number of this SpaceAddressCreate.
         :type: str
         """
         if sales_tax_number is not None and len(sales_tax_number) > 100:
             raise ValueError("Invalid value for `sales_tax_number`, length must be less than or equal to `100`")
 
         self._sales_tax_number = sales_tax_number
     
     @property
     def salutation(self):
-        """Gets the salutation of this AddressCreate.
+        """Gets the salutation of this SpaceAddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
-        :return: The salutation of this AddressCreate.
+        :return: The salutation of this SpaceAddressCreate.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
-        """Sets the salutation of this AddressCreate.
+        """Sets the salutation of this SpaceAddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
-        :param salutation: The salutation of this AddressCreate.
+        :param salutation: The salutation of this SpaceAddressCreate.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
-    def social_security_number(self):
-        """Gets the social_security_number of this AddressCreate.
-
-            
-
-        :return: The social_security_number of this AddressCreate.
-        :rtype: str
-        """
-        return self._social_security_number
-
-    @social_security_number.setter
-    def social_security_number(self, social_security_number):
-        """Sets the social_security_number of this AddressCreate.
-
-            
-
-        :param social_security_number: The social_security_number of this AddressCreate.
-        :type: str
-        """
-        if social_security_number is not None and len(social_security_number) > 100:
-            raise ValueError("Invalid value for `social_security_number`, length must be less than or equal to `100`")
-
-        self._social_security_number = social_security_number
-    
-    @property
     def sorting_code(self):
-        """Gets the sorting_code of this AddressCreate.
+        """Gets the sorting_code of this SpaceAddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
-        :return: The sorting_code of this AddressCreate.
+        :return: The sorting_code of this SpaceAddressCreate.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
-        """Sets the sorting_code of this AddressCreate.
+        """Sets the sorting_code of this SpaceAddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
-        :param sorting_code: The sorting_code of this AddressCreate.
+        :param sorting_code: The sorting_code of this SpaceAddressCreate.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
-        """Gets the street of this AddressCreate.
+        """Gets the street of this SpaceAddressCreate.
 
-            
+            The street or PO Box.
 
-        :return: The street of this AddressCreate.
+        :return: The street of this SpaceAddressCreate.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
-        """Sets the street of this AddressCreate.
+        """Sets the street of this SpaceAddressCreate.
 
-            
+            The street or PO Box.
 
-        :param street: The street of this AddressCreate.
+        :param street: The street of this SpaceAddressCreate.
         :type: str
         """
-        if street is not None and len(street) > 300:
-            raise ValueError("Invalid value for `street`, length must be less than or equal to `300`")
 
         self._street = street
     
 
     def to_dict(self):
         result = {}
 
@@ -592,27 +450,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(AddressCreate, dict):
+        if issubclass(SpaceAddressCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, AddressCreate):
+        if not isinstance(other, SpaceAddressCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/analytics_query.py` & `wallee-4.0.0/wallee/models/analytics_query.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/analytics_query_execution.py` & `wallee-4.0.0/wallee/models/analytics_query_execution.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 
 
 class AnalyticsQueryExecution:
 
     swagger_types = {
     
         'account': 'int',
+        'error_message': 'str',
         'external_id': 'str',
         'failure_reason': 'FailureReason',
         'id': 'int',
         'processing_end_time': 'datetime',
         'processing_start_time': 'datetime',
         'query_string': 'str',
         'scanned_data_in_gb': 'float',
         'scanned_data_limit': 'float',
         'spaces': 'list[int]',
         'state': 'AnalyticsQueryExecutionState',
     }
 
     attribute_map = {
-        'account': 'account','external_id': 'externalId','failure_reason': 'failureReason','id': 'id','processing_end_time': 'processingEndTime','processing_start_time': 'processingStartTime','query_string': 'queryString','scanned_data_in_gb': 'scannedDataInGb','scanned_data_limit': 'scannedDataLimit','spaces': 'spaces','state': 'state',
+        'account': 'account','error_message': 'errorMessage','external_id': 'externalId','failure_reason': 'failureReason','id': 'id','processing_end_time': 'processingEndTime','processing_start_time': 'processingStartTime','query_string': 'queryString','scanned_data_in_gb': 'scannedDataInGb','scanned_data_limit': 'scannedDataLimit','spaces': 'spaces','state': 'state',
     }
 
     
     _account = None
+    _error_message = None
     _external_id = None
     _failure_reason = None
     _id = None
     _processing_end_time = None
     _processing_start_time = None
     _query_string = None
     _scanned_data_in_gb = None
@@ -39,14 +41,15 @@
     _spaces = None
     _state = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.account = kwargs.get('account', None)
+        self.error_message = kwargs.get('error_message', None)
         self.external_id = kwargs.get('external_id', None)
         self.failure_reason = kwargs.get('failure_reason', None)
         self.id = kwargs.get('id', None)
         self.processing_end_time = kwargs.get('processing_end_time', None)
         self.processing_start_time = kwargs.get('processing_start_time', None)
         self.query_string = kwargs.get('query_string', None)
         self.scanned_data_in_gb = kwargs.get('scanned_data_in_gb', None)
@@ -76,14 +79,37 @@
         :param account: The account of this AnalyticsQueryExecution.
         :type: int
         """
 
         self._account = account
     
     @property
+    def error_message(self):
+        """Gets the error_message of this AnalyticsQueryExecution.
+
+            The error message if and only if the query has failed, otherwise null.
+
+        :return: The error_message of this AnalyticsQueryExecution.
+        :rtype: str
+        """
+        return self._error_message
+
+    @error_message.setter
+    def error_message(self, error_message):
+        """Sets the error_message of this AnalyticsQueryExecution.
+
+            The error message if and only if the query has failed, otherwise null.
+
+        :param error_message: The error_message of this AnalyticsQueryExecution.
+        :type: str
+        """
+
+        self._error_message = error_message
+    
+    @property
     def external_id(self):
         """Gets the external_id of this AnalyticsQueryExecution.
 
             The External ID of the query if one had been specified; otherwise null.
 
         :return: The external_id of this AnalyticsQueryExecution.
         :rtype: str
```

### Comparing `wallee-3.4.0/wallee/models/analytics_query_result_batch.py` & `wallee-4.0.0/wallee/models/analytics_query_result_batch.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/analytics_schema_column.py` & `wallee-4.0.0/wallee/models/analytics_schema_column.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/analytics_schema_table.py` & `wallee-4.0.0/wallee/models/analytics_schema_table.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/application_user.py` & `wallee-4.0.0/wallee/models/application_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class ApplicationUser(User):
 
     swagger_types = {
     
         'name': 'str',
-        'primary_account': 'Account',
+        'primary_account': 'int',
         'request_limit': 'int',
     }
 
     attribute_map = {
         'name': 'name','primary_account': 'primaryAccount','request_limit': 'requestLimit',
     }
 
@@ -34,74 +34,74 @@
         self.attribute_map.update(super().attribute_map)
 
     
     @property
     def name(self):
         """Gets the name of this ApplicationUser.
 
-            The user name is used to identify the application user in administrative interfaces.
+            The name used to identify the application user.
 
         :return: The name of this ApplicationUser.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ApplicationUser.
 
-            The user name is used to identify the application user in administrative interfaces.
+            The name used to identify the application user.
 
         :param name: The name of this ApplicationUser.
         :type: str
         """
         if name is not None and len(name) > 256:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `256`")
 
         self._name = name
     
     @property
     def primary_account(self):
         """Gets the primary_account of this ApplicationUser.
 
-            The account that this user is associated with. The account owner will be able to manage this user.
+            The primary account that the user belongs to.
 
         :return: The primary_account of this ApplicationUser.
-        :rtype: Account
+        :rtype: int
         """
         return self._primary_account
 
     @primary_account.setter
     def primary_account(self, primary_account):
         """Sets the primary_account of this ApplicationUser.
 
-            The account that this user is associated with. The account owner will be able to manage this user.
+            The primary account that the user belongs to.
 
         :param primary_account: The primary_account of this ApplicationUser.
-        :type: Account
+        :type: int
         """
 
         self._primary_account = primary_account
     
     @property
     def request_limit(self):
         """Gets the request_limit of this ApplicationUser.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted every 2 minutes.
 
         :return: The request_limit of this ApplicationUser.
         :rtype: int
         """
         return self._request_limit
 
     @request_limit.setter
     def request_limit(self, request_limit):
         """Sets the request_limit of this ApplicationUser.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted every 2 minutes.
 
         :param request_limit: The request_limit of this ApplicationUser.
         :type: int
         """
 
         self._request_limit = request_limit
```

### Comparing `wallee-3.4.0/wallee/models/application_user_create.py` & `wallee-4.0.0/wallee/models/application_user_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         self.attribute_map.update(super().attribute_map)
 
     
     @property
     def primary_account(self):
         """Gets the primary_account of this ApplicationUserCreate.
 
-            The account that this user is associated with. The account owner will be able to manage this user.
+            The primary account that the user belongs to.
 
         :return: The primary_account of this ApplicationUserCreate.
         :rtype: int
         """
         return self._primary_account
 
     @primary_account.setter
     def primary_account(self, primary_account):
         """Sets the primary_account of this ApplicationUserCreate.
 
-            The account that this user is associated with. The account owner will be able to manage this user.
+            The primary account that the user belongs to.
 
         :param primary_account: The primary_account of this ApplicationUserCreate.
         :type: int
         """
         if primary_account is None:
             raise ValueError("Invalid value for `primary_account`, must not be `None`")
```

### Comparing `wallee-3.4.0/wallee/models/application_user_create_with_mac_key.py` & `wallee-4.0.0/wallee/models/refund_comment_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import ApplicationUser
+from . import AbstractRefundCommentActive
 
 
-class ApplicationUserCreateWithMacKey(ApplicationUser):
+class RefundCommentCreate(AbstractRefundCommentActive):
 
     swagger_types = {
     
-        'mac_key': 'str',
+        'refund': 'int',
     }
 
     attribute_map = {
-        'mac_key': 'macKey',
+        'refund': 'refund',
     }
 
     
-    _mac_key = None
+    _refund = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.mac_key = kwargs.get('mac_key', None)
+        self.refund = kwargs.get('refund')
+
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def mac_key(self):
-        """Gets the mac_key of this ApplicationUserCreateWithMacKey.
+    def refund(self):
+        """Gets the refund of this RefundCommentCreate.
 
             
 
-        :return: The mac_key of this ApplicationUserCreateWithMacKey.
-        :rtype: str
+        :return: The refund of this RefundCommentCreate.
+        :rtype: int
         """
-        return self._mac_key
+        return self._refund
 
-    @mac_key.setter
-    def mac_key(self, mac_key):
-        """Sets the mac_key of this ApplicationUserCreateWithMacKey.
+    @refund.setter
+    def refund(self, refund):
+        """Sets the refund of this RefundCommentCreate.
 
             
 
-        :param mac_key: The mac_key of this ApplicationUserCreateWithMacKey.
-        :type: str
+        :param refund: The refund of this RefundCommentCreate.
+        :type: int
         """
+        if refund is None:
+            raise ValueError("Invalid value for `refund`, must not be `None`")
 
-        self._mac_key = mac_key
+        self._refund = refund
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -70,27 +73,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(ApplicationUserCreateWithMacKey, dict):
+        if issubclass(RefundCommentCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, ApplicationUserCreateWithMacKey):
+        if not isinstance(other, RefundCommentCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/application_user_update.py` & `wallee-4.0.0/wallee/models/application_user_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/authenticated_card_data.py` & `wallee-4.0.0/wallee/models/authenticated_card_data.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/authenticated_card_data_create.py` & `wallee-4.0.0/wallee/models/authenticated_card_data_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/bank_account.py` & `wallee-4.0.0/wallee/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/bank_account_type.py` & `wallee-4.0.0/wallee/models/bank_account_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this BankAccountType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this BankAccountType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this BankAccountType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this BankAccountType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._identifier_name = identifier_name
     
     @property
     def name(self):
         """Gets the name of this BankAccountType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this BankAccountType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this BankAccountType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this BankAccountType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/bank_transaction.py` & `wallee-4.0.0/wallee/models/bank_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/bank_transaction_source.py` & `wallee-4.0.0/wallee/models/bank_transaction_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this BankTransactionSource.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this BankTransactionSource.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this BankTransactionSource.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this BankTransactionSource.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this BankTransactionSource.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this BankTransactionSource.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this BankTransactionSource.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this BankTransactionSource.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/bank_transaction_type.py` & `wallee-4.0.0/wallee/models/bank_transaction_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this BankTransactionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this BankTransactionType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this BankTransactionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this BankTransactionType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this BankTransactionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this BankTransactionType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this BankTransactionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this BankTransactionType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/card_cryptogram.py` & `wallee-4.0.0/wallee/models/card_cryptogram.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/card_cryptogram_create.py` & `wallee-4.0.0/wallee/models/card_cryptogram_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/cardholder_authentication.py` & `wallee-4.0.0/wallee/models/cardholder_authentication.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/cardholder_authentication_create.py` & `wallee-4.0.0/wallee/models/cardholder_authentication_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge.py` & `wallee-4.0.0/wallee/models/charge.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge_attempt.py` & `wallee-4.0.0/wallee/models/charge_attempt.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge_bank_transaction.py` & `wallee-4.0.0/wallee/models/charge_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge_flow.py` & `wallee-4.0.0/wallee/models/charge_flow.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge_flow_level.py` & `wallee-4.0.0/wallee/models/charge_flow_level.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge_flow_level_configuration.py` & `wallee-4.0.0/wallee/models/charge_flow_level_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/charge_flow_level_configuration_type.py` & `wallee-4.0.0/wallee/models/charge_flow_level_configuration_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this ChargeFlowLevelConfigurationType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this ChargeFlowLevelConfigurationType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ChargeFlowLevelConfigurationType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this ChargeFlowLevelConfigurationType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._label = label
     
     @property
     def name(self):
         """Gets the name of this ChargeFlowLevelConfigurationType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this ChargeFlowLevelConfigurationType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ChargeFlowLevelConfigurationType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this ChargeFlowLevelConfigurationType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/charge_flow_level_payment_link.py` & `wallee-4.0.0/wallee/models/charge_flow_level_payment_link.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/client_error.py` & `wallee-4.0.0/wallee/models/client_error.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/completion_line_item.py` & `wallee-4.0.0/wallee/models/completion_line_item.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/completion_line_item_create.py` & `wallee-4.0.0/wallee/models/completion_line_item_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/condition.py` & `wallee-4.0.0/wallee/models/condition.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/condition_type.py` & `wallee-4.0.0/wallee/models/condition_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this ConditionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this ConditionType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ConditionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this ConditionType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this ConditionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this ConditionType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ConditionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this ConditionType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/connector_invocation.py` & `wallee-4.0.0/wallee/models/connector_invocation.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/criteria_operator.py` & `wallee-4.0.0/wallee/models/criteria_operator.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/currency_bank_account.py` & `wallee-4.0.0/wallee/models/currency_bank_account.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/customer.py` & `wallee-4.0.0/wallee/models/customer.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,101 +79,101 @@
 
         self._created_on = created_on
     
     @property
     def customer_id(self):
         """Gets the customer_id of this Customer.
 
-            
+            The customer's ID in the merchant's system.
 
         :return: The customer_id of this Customer.
         :rtype: str
         """
         return self._customer_id
 
     @customer_id.setter
     def customer_id(self, customer_id):
         """Sets the customer_id of this Customer.
 
-            
+            The customer's ID in the merchant's system.
 
         :param customer_id: The customer_id of this Customer.
         :type: str
         """
         if customer_id is not None and len(customer_id) > 100:
             raise ValueError("Invalid value for `customer_id`, length must be less than or equal to `100`")
 
         self._customer_id = customer_id
     
     @property
     def email_address(self):
         """Gets the email_address of this Customer.
 
-            
+            The customer's email address.
 
         :return: The email_address of this Customer.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this Customer.
 
-            
+            The customer's email address.
 
         :param email_address: The email_address of this Customer.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this Customer.
 
-            
+            The customer's family or last name.
 
         :return: The family_name of this Customer.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this Customer.
 
-            
+            The customer's family or last name.
 
         :param family_name: The family_name of this Customer.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
     def given_name(self):
         """Gets the given_name of this Customer.
 
-            
+            The customer's given or first name.
 
         :return: The given_name of this Customer.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this Customer.
 
-            
+            The customer's given or first name.
 
         :param given_name: The given_name of this Customer.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
@@ -248,49 +248,49 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def meta_data(self):
         """Gets the meta_data of this Customer.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this Customer.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this Customer.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this Customer.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
     
     @property
     def preferred_currency(self):
         """Gets the preferred_currency of this Customer.
 
-            
+            The customer's preferred currency.
 
         :return: The preferred_currency of this Customer.
         :rtype: str
         """
         return self._preferred_currency
 
     @preferred_currency.setter
     def preferred_currency(self, preferred_currency):
         """Sets the preferred_currency of this Customer.
 
-            
+            The customer's preferred currency.
 
         :param preferred_currency: The preferred_currency of this Customer.
         :type: str
         """
 
         self._preferred_currency = preferred_currency
```

### Comparing `wallee-3.4.0/wallee/models/customer_active.py` & `wallee-4.0.0/wallee/models/customer_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/customer_address.py` & `wallee-4.0.0/wallee/models/customer_address.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,49 +47,49 @@
         
 
     
     @property
     def address(self):
         """Gets the address of this CustomerAddress.
 
-            
+            The actual postal address.
 
         :return: The address of this CustomerAddress.
         :rtype: CustomerPostalAddress
         """
         return self._address
 
     @address.setter
     def address(self, address):
         """Sets the address of this CustomerAddress.
 
-            
+            The actual postal address.
 
         :param address: The address of this CustomerAddress.
         :type: CustomerPostalAddress
         """
 
         self._address = address
     
     @property
     def address_type(self):
         """Gets the address_type of this CustomerAddress.
 
-            
+            Whether the address is for billing or shipping or both.
 
         :return: The address_type of this CustomerAddress.
         :rtype: CustomerAddressType
         """
         return self._address_type
 
     @address_type.setter
     def address_type(self, address_type):
         """Sets the address_type of this CustomerAddress.
 
-            
+            Whether the address is for billing or shipping or both.
 
         :param address_type: The address_type of this CustomerAddress.
         :type: CustomerAddressType
         """
 
         self._address_type = address_type
     
@@ -116,49 +116,49 @@
 
         self._created_on = created_on
     
     @property
     def customer(self):
         """Gets the customer of this CustomerAddress.
 
-            
+            The customer that the object belongs to.
 
         :return: The customer of this CustomerAddress.
         :rtype: Customer
         """
         return self._customer
 
     @customer.setter
     def customer(self, customer):
         """Sets the customer of this CustomerAddress.
 
-            
+            The customer that the object belongs to.
 
         :param customer: The customer of this CustomerAddress.
         :type: Customer
         """
 
         self._customer = customer
     
     @property
     def default_address(self):
         """Gets the default_address of this CustomerAddress.
 
-            
+            Whether this is the customer's default address.
 
         :return: The default_address of this CustomerAddress.
         :rtype: bool
         """
         return self._default_address
 
     @default_address.setter
     def default_address(self, default_address):
         """Sets the default_address of this CustomerAddress.
 
-            
+            Whether this is the customer's default address.
 
         :param default_address: The default_address of this CustomerAddress.
         :type: bool
         """
 
         self._default_address = default_address
```

### Comparing `wallee-3.4.0/wallee/models/customer_address_active.py` & `wallee-4.0.0/wallee/models/customer_address_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/customer_address_create.py` & `wallee-4.0.0/wallee/models/customer_address_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         self.attribute_map.update(super().attribute_map)
 
     
     @property
     def customer(self):
         """Gets the customer of this CustomerAddressCreate.
 
-            
+            The customer that the object belongs to.
 
         :return: The customer of this CustomerAddressCreate.
         :rtype: int
         """
         return self._customer
 
     @customer.setter
     def customer(self, customer):
         """Sets the customer of this CustomerAddressCreate.
 
-            
+            The customer that the object belongs to.
 
         :param customer: The customer of this CustomerAddressCreate.
         :type: int
         """
         if customer is None:
             raise ValueError("Invalid value for `customer`, must not be `None`")
```

### Comparing `wallee-3.4.0/wallee/models/customer_comment.py` & `wallee-4.0.0/wallee/models/customer_comment.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,51 +53,51 @@
         
 
     
     @property
     def content(self):
         """Gets the content of this CustomerComment.
 
-            
+            The comment's actual content.
 
         :return: The content of this CustomerComment.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
         """Sets the content of this CustomerComment.
 
-            
+            The comment's actual content.
 
         :param content: The content of this CustomerComment.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
     @property
     def created_by(self):
         """Gets the created_by of this CustomerComment.
 
-            
+            The ID of the user the comment was created by.
 
         :return: The created_by of this CustomerComment.
         :rtype: int
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this CustomerComment.
 
-            
+            The ID of the user the comment was created by.
 
         :param created_by: The created_by of this CustomerComment.
         :type: int
         """
 
         self._created_by = created_by
     
@@ -124,72 +124,72 @@
 
         self._created_on = created_on
     
     @property
     def customer(self):
         """Gets the customer of this CustomerComment.
 
-            
+            The customer that the object belongs to.
 
         :return: The customer of this CustomerComment.
         :rtype: int
         """
         return self._customer
 
     @customer.setter
     def customer(self, customer):
         """Sets the customer of this CustomerComment.
 
-            
+            The customer that the object belongs to.
 
         :param customer: The customer of this CustomerComment.
         :type: int
         """
 
         self._customer = customer
     
     @property
     def edited_by(self):
         """Gets the edited_by of this CustomerComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :return: The edited_by of this CustomerComment.
         :rtype: int
         """
         return self._edited_by
 
     @edited_by.setter
     def edited_by(self, edited_by):
         """Sets the edited_by of this CustomerComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :param edited_by: The edited_by of this CustomerComment.
         :type: int
         """
 
         self._edited_by = edited_by
     
     @property
     def edited_on(self):
         """Gets the edited_on of this CustomerComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :return: The edited_on of this CustomerComment.
         :rtype: datetime
         """
         return self._edited_on
 
     @edited_on.setter
     def edited_on(self, edited_on):
         """Sets the edited_on of this CustomerComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :param edited_on: The edited_on of this CustomerComment.
         :type: datetime
         """
 
         self._edited_on = edited_on
     
@@ -239,26 +239,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def pinned(self):
         """Gets the pinned of this CustomerComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :return: The pinned of this CustomerComment.
         :rtype: bool
         """
         return self._pinned
 
     @pinned.setter
     def pinned(self, pinned):
         """Sets the pinned of this CustomerComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :param pinned: The pinned of this CustomerComment.
         :type: bool
         """
 
         self._pinned = pinned
```

### Comparing `wallee-3.4.0/wallee/models/customer_comment_active.py` & `wallee-4.0.0/wallee/models/customer_comment_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/customer_comment_create.py` & `wallee-4.0.0/wallee/models/customer_comment_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         self.attribute_map.update(super().attribute_map)
 
     
     @property
     def customer(self):
         """Gets the customer of this CustomerCommentCreate.
 
-            
+            The customer that the object belongs to.
 
         :return: The customer of this CustomerCommentCreate.
         :rtype: int
         """
         return self._customer
 
     @customer.setter
     def customer(self, customer):
         """Sets the customer of this CustomerCommentCreate.
 
-            
+            The customer that the object belongs to.
 
         :param customer: The customer of this CustomerCommentCreate.
         :type: int
         """
         if customer is None:
             raise ValueError("Invalid value for `customer`, must not be `None`")
```

### Comparing `wallee-3.4.0/wallee/models/customer_create.py` & `wallee-4.0.0/wallee/models/customer_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/customer_postal_address.py` & `wallee-4.0.0/wallee/models/customer_postal_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,491 +83,491 @@
         
 
     
     @property
     def city(self):
         """Gets the city of this CustomerPostalAddress.
 
-            
+            The city, town or village.
 
         :return: The city of this CustomerPostalAddress.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
         """Sets the city of this CustomerPostalAddress.
 
-            
+            The city, town or village.
 
         :param city: The city of this CustomerPostalAddress.
         :type: str
         """
         if city is not None and len(city) > 100:
             raise ValueError("Invalid value for `city`, length must be less than or equal to `100`")
 
         self._city = city
     
     @property
     def commercial_register_number(self):
         """Gets the commercial_register_number of this CustomerPostalAddress.
 
-            
+            The commercial registration number of the organization.
 
         :return: The commercial_register_number of this CustomerPostalAddress.
         :rtype: str
         """
         return self._commercial_register_number
 
     @commercial_register_number.setter
     def commercial_register_number(self, commercial_register_number):
         """Sets the commercial_register_number of this CustomerPostalAddress.
 
-            
+            The commercial registration number of the organization.
 
         :param commercial_register_number: The commercial_register_number of this CustomerPostalAddress.
         :type: str
         """
         if commercial_register_number is not None and len(commercial_register_number) > 100:
             raise ValueError("Invalid value for `commercial_register_number`, length must be less than or equal to `100`")
 
         self._commercial_register_number = commercial_register_number
     
     @property
     def country(self):
         """Gets the country of this CustomerPostalAddress.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :return: The country of this CustomerPostalAddress.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
         """Sets the country of this CustomerPostalAddress.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :param country: The country of this CustomerPostalAddress.
         :type: str
         """
 
         self._country = country
     
     @property
     def date_of_birth(self):
         """Gets the date_of_birth of this CustomerPostalAddress.
 
-            
+            The date of birth.
 
         :return: The date_of_birth of this CustomerPostalAddress.
         :rtype: date
         """
         return self._date_of_birth
 
     @date_of_birth.setter
     def date_of_birth(self, date_of_birth):
         """Sets the date_of_birth of this CustomerPostalAddress.
 
-            
+            The date of birth.
 
         :param date_of_birth: The date_of_birth of this CustomerPostalAddress.
         :type: date
         """
 
         self._date_of_birth = date_of_birth
     
     @property
     def dependent_locality(self):
         """Gets the dependent_locality of this CustomerPostalAddress.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :return: The dependent_locality of this CustomerPostalAddress.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
         """Sets the dependent_locality of this CustomerPostalAddress.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :param dependent_locality: The dependent_locality of this CustomerPostalAddress.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
         """Gets the email_address of this CustomerPostalAddress.
 
-            
+            The email address.
 
         :return: The email_address of this CustomerPostalAddress.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this CustomerPostalAddress.
 
-            
+            The email address.
 
         :param email_address: The email_address of this CustomerPostalAddress.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this CustomerPostalAddress.
 
-            
+            The family or last name.
 
         :return: The family_name of this CustomerPostalAddress.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this CustomerPostalAddress.
 
-            
+            The family or last name.
 
         :param family_name: The family_name of this CustomerPostalAddress.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
     def gender(self):
         """Gets the gender of this CustomerPostalAddress.
 
-            
+            The gender.
 
         :return: The gender of this CustomerPostalAddress.
         :rtype: Gender
         """
         return self._gender
 
     @gender.setter
     def gender(self, gender):
         """Sets the gender of this CustomerPostalAddress.
 
-            
+            The gender.
 
         :param gender: The gender of this CustomerPostalAddress.
         :type: Gender
         """
 
         self._gender = gender
     
     @property
     def given_name(self):
         """Gets the given_name of this CustomerPostalAddress.
 
-            
+            The given or first name.
 
         :return: The given_name of this CustomerPostalAddress.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this CustomerPostalAddress.
 
-            
+            The given or first name.
 
         :param given_name: The given_name of this CustomerPostalAddress.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
         self._given_name = given_name
     
     @property
     def legal_organization_form(self):
         """Gets the legal_organization_form of this CustomerPostalAddress.
 
-            
+            The legal form of the organization.
 
         :return: The legal_organization_form of this CustomerPostalAddress.
         :rtype: LegalOrganizationForm
         """
         return self._legal_organization_form
 
     @legal_organization_form.setter
     def legal_organization_form(self, legal_organization_form):
         """Sets the legal_organization_form of this CustomerPostalAddress.
 
-            
+            The legal form of the organization.
 
         :param legal_organization_form: The legal_organization_form of this CustomerPostalAddress.
         :type: LegalOrganizationForm
         """
 
         self._legal_organization_form = legal_organization_form
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this CustomerPostalAddress.
 
-            
+            The phone number of a mobile phone.
 
         :return: The mobile_phone_number of this CustomerPostalAddress.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this CustomerPostalAddress.
 
-            
+            The phone number of a mobile phone.
 
         :param mobile_phone_number: The mobile_phone_number of this CustomerPostalAddress.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
         """Gets the organization_name of this CustomerPostalAddress.
 
-            
+            The organization's name.
 
         :return: The organization_name of this CustomerPostalAddress.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
         """Sets the organization_name of this CustomerPostalAddress.
 
-            
+            The organization's name.
 
         :param organization_name: The organization_name of this CustomerPostalAddress.
         :type: str
         """
         if organization_name is not None and len(organization_name) > 100:
             raise ValueError("Invalid value for `organization_name`, length must be less than or equal to `100`")
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
         """Gets the phone_number of this CustomerPostalAddress.
 
-            
+            The phone number.
 
         :return: The phone_number of this CustomerPostalAddress.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
         """Sets the phone_number of this CustomerPostalAddress.
 
-            
+            The phone number.
 
         :param phone_number: The phone_number of this CustomerPostalAddress.
         :type: str
         """
         if phone_number is not None and len(phone_number) > 100:
             raise ValueError("Invalid value for `phone_number`, length must be less than or equal to `100`")
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
         """Gets the postal_state of this CustomerPostalAddress.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :return: The postal_state of this CustomerPostalAddress.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
         """Sets the postal_state of this CustomerPostalAddress.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :param postal_state: The postal_state of this CustomerPostalAddress.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
         """Gets the postcode of this CustomerPostalAddress.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :return: The postcode of this CustomerPostalAddress.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
         """Sets the postcode of this CustomerPostalAddress.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :param postcode: The postcode of this CustomerPostalAddress.
         :type: str
         """
         if postcode is not None and len(postcode) > 40:
             raise ValueError("Invalid value for `postcode`, length must be less than or equal to `40`")
 
         self._postcode = postcode
     
     @property
     def sales_tax_number(self):
         """Gets the sales_tax_number of this CustomerPostalAddress.
 
-            
+            The sales tax number of the organization.
 
         :return: The sales_tax_number of this CustomerPostalAddress.
         :rtype: str
         """
         return self._sales_tax_number
 
     @sales_tax_number.setter
     def sales_tax_number(self, sales_tax_number):
         """Sets the sales_tax_number of this CustomerPostalAddress.
 
-            
+            The sales tax number of the organization.
 
         :param sales_tax_number: The sales_tax_number of this CustomerPostalAddress.
         :type: str
         """
         if sales_tax_number is not None and len(sales_tax_number) > 100:
             raise ValueError("Invalid value for `sales_tax_number`, length must be less than or equal to `100`")
 
         self._sales_tax_number = sales_tax_number
     
     @property
     def salutation(self):
         """Gets the salutation of this CustomerPostalAddress.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :return: The salutation of this CustomerPostalAddress.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
         """Sets the salutation of this CustomerPostalAddress.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :param salutation: The salutation of this CustomerPostalAddress.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
     def social_security_number(self):
         """Gets the social_security_number of this CustomerPostalAddress.
 
-            
+            The social security number.
 
         :return: The social_security_number of this CustomerPostalAddress.
         :rtype: str
         """
         return self._social_security_number
 
     @social_security_number.setter
     def social_security_number(self, social_security_number):
         """Sets the social_security_number of this CustomerPostalAddress.
 
-            
+            The social security number.
 
         :param social_security_number: The social_security_number of this CustomerPostalAddress.
         :type: str
         """
         if social_security_number is not None and len(social_security_number) > 100:
             raise ValueError("Invalid value for `social_security_number`, length must be less than or equal to `100`")
 
         self._social_security_number = social_security_number
     
     @property
     def sorting_code(self):
         """Gets the sorting_code of this CustomerPostalAddress.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :return: The sorting_code of this CustomerPostalAddress.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
         """Sets the sorting_code of this CustomerPostalAddress.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :param sorting_code: The sorting_code of this CustomerPostalAddress.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
         """Gets the street of this CustomerPostalAddress.
 
-            
+            The street or PO Box.
 
         :return: The street of this CustomerPostalAddress.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
         """Sets the street of this CustomerPostalAddress.
 
-            
+            The street or PO Box.
 
         :param street: The street of this CustomerPostalAddress.
         :type: str
         """
         if street is not None and len(street) > 300:
             raise ValueError("Invalid value for `street`, length must be less than or equal to `300`")
```

### Comparing `wallee-3.4.0/wallee/models/customer_postal_address_create.py` & `wallee-4.0.0/wallee/models/customer_postal_address_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,491 +83,491 @@
         
 
     
     @property
     def city(self):
         """Gets the city of this CustomerPostalAddressCreate.
 
-            
+            The city, town or village.
 
         :return: The city of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
         """Sets the city of this CustomerPostalAddressCreate.
 
-            
+            The city, town or village.
 
         :param city: The city of this CustomerPostalAddressCreate.
         :type: str
         """
         if city is not None and len(city) > 100:
             raise ValueError("Invalid value for `city`, length must be less than or equal to `100`")
 
         self._city = city
     
     @property
     def commercial_register_number(self):
         """Gets the commercial_register_number of this CustomerPostalAddressCreate.
 
-            
+            The commercial registration number of the organization.
 
         :return: The commercial_register_number of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._commercial_register_number
 
     @commercial_register_number.setter
     def commercial_register_number(self, commercial_register_number):
         """Sets the commercial_register_number of this CustomerPostalAddressCreate.
 
-            
+            The commercial registration number of the organization.
 
         :param commercial_register_number: The commercial_register_number of this CustomerPostalAddressCreate.
         :type: str
         """
         if commercial_register_number is not None and len(commercial_register_number) > 100:
             raise ValueError("Invalid value for `commercial_register_number`, length must be less than or equal to `100`")
 
         self._commercial_register_number = commercial_register_number
     
     @property
     def country(self):
         """Gets the country of this CustomerPostalAddressCreate.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :return: The country of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
         """Sets the country of this CustomerPostalAddressCreate.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :param country: The country of this CustomerPostalAddressCreate.
         :type: str
         """
 
         self._country = country
     
     @property
     def date_of_birth(self):
         """Gets the date_of_birth of this CustomerPostalAddressCreate.
 
-            
+            The date of birth.
 
         :return: The date_of_birth of this CustomerPostalAddressCreate.
         :rtype: date
         """
         return self._date_of_birth
 
     @date_of_birth.setter
     def date_of_birth(self, date_of_birth):
         """Sets the date_of_birth of this CustomerPostalAddressCreate.
 
-            
+            The date of birth.
 
         :param date_of_birth: The date_of_birth of this CustomerPostalAddressCreate.
         :type: date
         """
 
         self._date_of_birth = date_of_birth
     
     @property
     def dependent_locality(self):
         """Gets the dependent_locality of this CustomerPostalAddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :return: The dependent_locality of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
         """Sets the dependent_locality of this CustomerPostalAddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :param dependent_locality: The dependent_locality of this CustomerPostalAddressCreate.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
         """Gets the email_address of this CustomerPostalAddressCreate.
 
-            
+            The email address.
 
         :return: The email_address of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this CustomerPostalAddressCreate.
 
-            
+            The email address.
 
         :param email_address: The email_address of this CustomerPostalAddressCreate.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this CustomerPostalAddressCreate.
 
-            
+            The family or last name.
 
         :return: The family_name of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this CustomerPostalAddressCreate.
 
-            
+            The family or last name.
 
         :param family_name: The family_name of this CustomerPostalAddressCreate.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
     def gender(self):
         """Gets the gender of this CustomerPostalAddressCreate.
 
-            
+            The gender.
 
         :return: The gender of this CustomerPostalAddressCreate.
         :rtype: Gender
         """
         return self._gender
 
     @gender.setter
     def gender(self, gender):
         """Sets the gender of this CustomerPostalAddressCreate.
 
-            
+            The gender.
 
         :param gender: The gender of this CustomerPostalAddressCreate.
         :type: Gender
         """
 
         self._gender = gender
     
     @property
     def given_name(self):
         """Gets the given_name of this CustomerPostalAddressCreate.
 
-            
+            The given or first name.
 
         :return: The given_name of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this CustomerPostalAddressCreate.
 
-            
+            The given or first name.
 
         :param given_name: The given_name of this CustomerPostalAddressCreate.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
         self._given_name = given_name
     
     @property
     def legal_organization_form(self):
         """Gets the legal_organization_form of this CustomerPostalAddressCreate.
 
-            
+            The legal form of the organization.
 
         :return: The legal_organization_form of this CustomerPostalAddressCreate.
         :rtype: int
         """
         return self._legal_organization_form
 
     @legal_organization_form.setter
     def legal_organization_form(self, legal_organization_form):
         """Sets the legal_organization_form of this CustomerPostalAddressCreate.
 
-            
+            The legal form of the organization.
 
         :param legal_organization_form: The legal_organization_form of this CustomerPostalAddressCreate.
         :type: int
         """
 
         self._legal_organization_form = legal_organization_form
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this CustomerPostalAddressCreate.
 
-            
+            The phone number of a mobile phone.
 
         :return: The mobile_phone_number of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this CustomerPostalAddressCreate.
 
-            
+            The phone number of a mobile phone.
 
         :param mobile_phone_number: The mobile_phone_number of this CustomerPostalAddressCreate.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
         """Gets the organization_name of this CustomerPostalAddressCreate.
 
-            
+            The organization's name.
 
         :return: The organization_name of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
         """Sets the organization_name of this CustomerPostalAddressCreate.
 
-            
+            The organization's name.
 
         :param organization_name: The organization_name of this CustomerPostalAddressCreate.
         :type: str
         """
         if organization_name is not None and len(organization_name) > 100:
             raise ValueError("Invalid value for `organization_name`, length must be less than or equal to `100`")
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
         """Gets the phone_number of this CustomerPostalAddressCreate.
 
-            
+            The phone number.
 
         :return: The phone_number of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
         """Sets the phone_number of this CustomerPostalAddressCreate.
 
-            
+            The phone number.
 
         :param phone_number: The phone_number of this CustomerPostalAddressCreate.
         :type: str
         """
         if phone_number is not None and len(phone_number) > 100:
             raise ValueError("Invalid value for `phone_number`, length must be less than or equal to `100`")
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
         """Gets the postal_state of this CustomerPostalAddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :return: The postal_state of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
         """Sets the postal_state of this CustomerPostalAddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :param postal_state: The postal_state of this CustomerPostalAddressCreate.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
         """Gets the postcode of this CustomerPostalAddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :return: The postcode of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
         """Sets the postcode of this CustomerPostalAddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :param postcode: The postcode of this CustomerPostalAddressCreate.
         :type: str
         """
         if postcode is not None and len(postcode) > 40:
             raise ValueError("Invalid value for `postcode`, length must be less than or equal to `40`")
 
         self._postcode = postcode
     
     @property
     def sales_tax_number(self):
         """Gets the sales_tax_number of this CustomerPostalAddressCreate.
 
-            
+            The sales tax number of the organization.
 
         :return: The sales_tax_number of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._sales_tax_number
 
     @sales_tax_number.setter
     def sales_tax_number(self, sales_tax_number):
         """Sets the sales_tax_number of this CustomerPostalAddressCreate.
 
-            
+            The sales tax number of the organization.
 
         :param sales_tax_number: The sales_tax_number of this CustomerPostalAddressCreate.
         :type: str
         """
         if sales_tax_number is not None and len(sales_tax_number) > 100:
             raise ValueError("Invalid value for `sales_tax_number`, length must be less than or equal to `100`")
 
         self._sales_tax_number = sales_tax_number
     
     @property
     def salutation(self):
         """Gets the salutation of this CustomerPostalAddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :return: The salutation of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
         """Sets the salutation of this CustomerPostalAddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :param salutation: The salutation of this CustomerPostalAddressCreate.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
     def social_security_number(self):
         """Gets the social_security_number of this CustomerPostalAddressCreate.
 
-            
+            The social security number.
 
         :return: The social_security_number of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._social_security_number
 
     @social_security_number.setter
     def social_security_number(self, social_security_number):
         """Sets the social_security_number of this CustomerPostalAddressCreate.
 
-            
+            The social security number.
 
         :param social_security_number: The social_security_number of this CustomerPostalAddressCreate.
         :type: str
         """
         if social_security_number is not None and len(social_security_number) > 100:
             raise ValueError("Invalid value for `social_security_number`, length must be less than or equal to `100`")
 
         self._social_security_number = social_security_number
     
     @property
     def sorting_code(self):
         """Gets the sorting_code of this CustomerPostalAddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :return: The sorting_code of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
         """Sets the sorting_code of this CustomerPostalAddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :param sorting_code: The sorting_code of this CustomerPostalAddressCreate.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
         """Gets the street of this CustomerPostalAddressCreate.
 
-            
+            The street or PO Box.
 
         :return: The street of this CustomerPostalAddressCreate.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
         """Sets the street of this CustomerPostalAddressCreate.
 
-            
+            The street or PO Box.
 
         :param street: The street of this CustomerPostalAddressCreate.
         :type: str
         """
         if street is not None and len(street) > 300:
             raise ValueError("Invalid value for `street`, length must be less than or equal to `300`")
```

### Comparing `wallee-3.4.0/wallee/models/database_translated_string.py` & `wallee-4.0.0/wallee/models/localized_string.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,83 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class DatabaseTranslatedString:
+class LocalizedString:
 
     swagger_types = {
     
-        'available_languages': 'list[str]',
-        'display_name': 'str',
-        'items': 'list[DatabaseTranslatedStringItem]',
+        'language': 'str',
+        'string': 'str',
     }
 
     attribute_map = {
-        'available_languages': 'availableLanguages','display_name': 'displayName','items': 'items',
+        'language': 'language','string': 'string',
     }
 
     
-    _available_languages = None
-    _display_name = None
-    _items = None
+    _language = None
+    _string = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.available_languages = kwargs.get('available_languages', None)
-        self.display_name = kwargs.get('display_name', None)
-        self.items = kwargs.get('items', None)
+        self.language = kwargs.get('language', None)
+        self.string = kwargs.get('string', None)
         
 
     
     @property
-    def available_languages(self):
-        """Gets the available_languages of this DatabaseTranslatedString.
+    def language(self):
+        """Gets the language of this LocalizedString.
 
-            
+            The term's language.
 
-        :return: The available_languages of this DatabaseTranslatedString.
-        :rtype: list[str]
-        """
-        return self._available_languages
-
-    @available_languages.setter
-    def available_languages(self, available_languages):
-        """Sets the available_languages of this DatabaseTranslatedString.
-
-            
-
-        :param available_languages: The available_languages of this DatabaseTranslatedString.
-        :type: list[str]
-        """
-
-        self._available_languages = available_languages
-    
-    @property
-    def display_name(self):
-        """Gets the display_name of this DatabaseTranslatedString.
-
-            
-
-        :return: The display_name of this DatabaseTranslatedString.
+        :return: The language of this LocalizedString.
         :rtype: str
         """
-        return self._display_name
+        return self._language
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this DatabaseTranslatedString.
+    @language.setter
+    def language(self, language):
+        """Sets the language of this LocalizedString.
 
-            
+            The term's language.
 
-        :param display_name: The display_name of this DatabaseTranslatedString.
+        :param language: The language of this LocalizedString.
         :type: str
         """
 
-        self._display_name = display_name
+        self._language = language
     
     @property
-    def items(self):
-        """Gets the items of this DatabaseTranslatedString.
+    def string(self):
+        """Gets the string of this LocalizedString.
 
-            
+            The localized term.
 
-        :return: The items of this DatabaseTranslatedString.
-        :rtype: list[DatabaseTranslatedStringItem]
+        :return: The string of this LocalizedString.
+        :rtype: str
         """
-        return self._items
+        return self._string
 
-    @items.setter
-    def items(self, items):
-        """Sets the items of this DatabaseTranslatedString.
+    @string.setter
+    def string(self, string):
+        """Sets the string of this LocalizedString.
 
-            
+            The localized term.
 
-        :param items: The items of this DatabaseTranslatedString.
-        :type: list[DatabaseTranslatedStringItem]
+        :param string: The string of this LocalizedString.
+        :type: str
         """
 
-        self._items = items
+        self._string = string
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -120,27 +94,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(DatabaseTranslatedString, dict):
+        if issubclass(LocalizedString, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, DatabaseTranslatedString):
+        if not isinstance(other, LocalizedString):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/database_translated_string_create.py` & `wallee-4.0.0/wallee/models/transaction_comment_create.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
+from . import AbstractTransactionCommentActive
 
 
-
-class DatabaseTranslatedStringCreate:
+class TransactionCommentCreate(AbstractTransactionCommentActive):
 
     swagger_types = {
     
-        'items': 'list[DatabaseTranslatedStringItemCreate]',
+        'transaction': 'int',
     }
 
     attribute_map = {
-        'items': 'items',
+        'transaction': 'transaction',
     }
 
     
-    _items = None
+    _transaction = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.items = kwargs.get('items', None)
-        
+        self.transaction = kwargs.get('transaction')
+
+        super().__init__(**kwargs)
+        self.swagger_types.update(super().swagger_types)
+        self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def items(self):
-        """Gets the items of this DatabaseTranslatedStringCreate.
+    def transaction(self):
+        """Gets the transaction of this TransactionCommentCreate.
 
             
 
-        :return: The items of this DatabaseTranslatedStringCreate.
-        :rtype: list[DatabaseTranslatedStringItemCreate]
+        :return: The transaction of this TransactionCommentCreate.
+        :rtype: int
         """
-        return self._items
+        return self._transaction
 
-    @items.setter
-    def items(self, items):
-        """Sets the items of this DatabaseTranslatedStringCreate.
+    @transaction.setter
+    def transaction(self, transaction):
+        """Sets the transaction of this TransactionCommentCreate.
 
             
 
-        :param items: The items of this DatabaseTranslatedStringCreate.
-        :type: list[DatabaseTranslatedStringItemCreate]
+        :param transaction: The transaction of this TransactionCommentCreate.
+        :type: int
         """
+        if transaction is None:
+            raise ValueError("Invalid value for `transaction`, must not be `None`")
 
-        self._items = items
+        self._transaction = transaction
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -68,27 +73,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(DatabaseTranslatedStringCreate, dict):
+        if issubclass(TransactionCommentCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, DatabaseTranslatedStringCreate):
+        if not isinstance(other, TransactionCommentCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/database_translated_string_item.py` & `wallee-4.0.0/wallee/models/transaction_aware_entity.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,111 +1,109 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class DatabaseTranslatedStringItem:
+class TransactionAwareEntity:
 
     swagger_types = {
     
-        'language': 'str',
-        'language_code': 'str',
-        'translation': 'str',
+        'id': 'int',
+        'linked_space_id': 'int',
+        'linked_transaction': 'int',
     }
 
     attribute_map = {
-        'language': 'language','language_code': 'languageCode','translation': 'translation',
+        'id': 'id','linked_space_id': 'linkedSpaceId','linked_transaction': 'linkedTransaction',
     }
 
     
-    _language = None
-    _language_code = None
-    _translation = None
+    _id = None
+    _linked_space_id = None
+    _linked_transaction = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.language = kwargs.get('language', None)
-        self.language_code = kwargs.get('language_code', None)
-        self.translation = kwargs.get('translation', None)
+        self.id = kwargs.get('id', None)
+        self.linked_space_id = kwargs.get('linked_space_id', None)
+        self.linked_transaction = kwargs.get('linked_transaction', None)
         
 
     
     @property
-    def language(self):
-        """Gets the language of this DatabaseTranslatedStringItem.
+    def id(self):
+        """Gets the id of this TransactionAwareEntity.
 
-            
+            A unique identifier for the object.
 
-        :return: The language of this DatabaseTranslatedStringItem.
-        :rtype: str
+        :return: The id of this TransactionAwareEntity.
+        :rtype: int
         """
-        return self._language
+        return self._id
 
-    @language.setter
-    def language(self, language):
-        """Sets the language of this DatabaseTranslatedStringItem.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this TransactionAwareEntity.
 
-            
+            A unique identifier for the object.
 
-        :param language: The language of this DatabaseTranslatedStringItem.
-        :type: str
+        :param id: The id of this TransactionAwareEntity.
+        :type: int
         """
 
-        self._language = language
+        self._id = id
     
     @property
-    def language_code(self):
-        """Gets the language_code of this DatabaseTranslatedStringItem.
+    def linked_space_id(self):
+        """Gets the linked_space_id of this TransactionAwareEntity.
 
-            
+            The ID of the space this object belongs to.
 
-        :return: The language_code of this DatabaseTranslatedStringItem.
-        :rtype: str
+        :return: The linked_space_id of this TransactionAwareEntity.
+        :rtype: int
         """
-        return self._language_code
+        return self._linked_space_id
 
-    @language_code.setter
-    def language_code(self, language_code):
-        """Sets the language_code of this DatabaseTranslatedStringItem.
+    @linked_space_id.setter
+    def linked_space_id(self, linked_space_id):
+        """Sets the linked_space_id of this TransactionAwareEntity.
 
-            
+            The ID of the space this object belongs to.
 
-        :param language_code: The language_code of this DatabaseTranslatedStringItem.
-        :type: str
+        :param linked_space_id: The linked_space_id of this TransactionAwareEntity.
+        :type: int
         """
 
-        self._language_code = language_code
+        self._linked_space_id = linked_space_id
     
     @property
-    def translation(self):
-        """Gets the translation of this DatabaseTranslatedStringItem.
+    def linked_transaction(self):
+        """Gets the linked_transaction of this TransactionAwareEntity.
 
             
 
-        :return: The translation of this DatabaseTranslatedStringItem.
-        :rtype: str
+        :return: The linked_transaction of this TransactionAwareEntity.
+        :rtype: int
         """
-        return self._translation
+        return self._linked_transaction
 
-    @translation.setter
-    def translation(self, translation):
-        """Sets the translation of this DatabaseTranslatedStringItem.
+    @linked_transaction.setter
+    def linked_transaction(self, linked_transaction):
+        """Sets the linked_transaction of this TransactionAwareEntity.
 
             
 
-        :param translation: The translation of this DatabaseTranslatedStringItem.
-        :type: str
+        :param linked_transaction: The linked_transaction of this TransactionAwareEntity.
+        :type: int
         """
-        if translation is not None and len(translation) > 16777216:
-            raise ValueError("Invalid value for `translation`, length must be less than or equal to `16777216`")
 
-        self._translation = translation
+        self._linked_transaction = linked_transaction
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -122,27 +120,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(DatabaseTranslatedStringItem, dict):
+        if issubclass(TransactionAwareEntity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, DatabaseTranslatedStringItem):
+        if not isinstance(other, TransactionAwareEntity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/database_translated_string_item_create.py` & `wallee-4.0.0/wallee/models/subscriber_create.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
+from . import AbstractSubscriberUpdate
 
 
-
-class DatabaseTranslatedStringItemCreate:
+class SubscriberCreate(AbstractSubscriberUpdate):
 
     swagger_types = {
     
-        'language': 'str',
-        'translation': 'str',
+        'state': 'CreationEntityState',
+        'external_id': 'str',
     }
 
     attribute_map = {
-        'language': 'language','translation': 'translation',
+        'state': 'state','external_id': 'externalId',
     }
 
     
-    _language = None
-    _translation = None
+    _state = None
+    _external_id = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.language = kwargs.get('language')
+        self.state = kwargs.get('state', None)
+        self.external_id = kwargs.get('external_id')
 
-        self.translation = kwargs.get('translation', None)
-        
+        super().__init__(**kwargs)
+        self.swagger_types.update(super().swagger_types)
+        self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def language(self):
-        """Gets the language of this DatabaseTranslatedStringItemCreate.
+    def state(self):
+        """Gets the state of this SubscriberCreate.
 
-            
+            The object's current state.
 
-        :return: The language of this DatabaseTranslatedStringItemCreate.
-        :rtype: str
+        :return: The state of this SubscriberCreate.
+        :rtype: CreationEntityState
         """
-        return self._language
+        return self._state
 
-    @language.setter
-    def language(self, language):
-        """Sets the language of this DatabaseTranslatedStringItemCreate.
+    @state.setter
+    def state(self, state):
+        """Sets the state of this SubscriberCreate.
 
-            
+            The object's current state.
 
-        :param language: The language of this DatabaseTranslatedStringItemCreate.
-        :type: str
+        :param state: The state of this SubscriberCreate.
+        :type: CreationEntityState
         """
-        if language is None:
-            raise ValueError("Invalid value for `language`, must not be `None`")
 
-        self._language = language
+        self._state = state
     
     @property
-    def translation(self):
-        """Gets the translation of this DatabaseTranslatedStringItemCreate.
+    def external_id(self):
+        """Gets the external_id of this SubscriberCreate.
 
-            
+            A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
 
-        :return: The translation of this DatabaseTranslatedStringItemCreate.
+        :return: The external_id of this SubscriberCreate.
         :rtype: str
         """
-        return self._translation
+        return self._external_id
 
-    @translation.setter
-    def translation(self, translation):
-        """Sets the translation of this DatabaseTranslatedStringItemCreate.
+    @external_id.setter
+    def external_id(self, external_id):
+        """Sets the external_id of this SubscriberCreate.
 
-            
+            A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
 
-        :param translation: The translation of this DatabaseTranslatedStringItemCreate.
+        :param external_id: The external_id of this SubscriberCreate.
         :type: str
         """
-        if translation is not None and len(translation) > 16777216:
-            raise ValueError("Invalid value for `translation`, length must be less than or equal to `16777216`")
+        if external_id is None:
+            raise ValueError("Invalid value for `external_id`, must not be `None`")
 
-        self._translation = translation
+        self._external_id = external_id
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -99,27 +99,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(DatabaseTranslatedStringItemCreate, dict):
+        if issubclass(SubscriberCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, DatabaseTranslatedStringItemCreate):
+        if not isinstance(other, SubscriberCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/debt_collection_case.py` & `wallee-4.0.0/wallee/models/debt_collection_case.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/debt_collection_case_create.py` & `wallee-4.0.0/wallee/models/debt_collection_case_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/debt_collection_case_document.py` & `wallee-4.0.0/wallee/models/debt_collection_case_document.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/debt_collection_case_source.py` & `wallee-4.0.0/wallee/models/debt_collection_case_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this DebtCollectionCaseSource.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this DebtCollectionCaseSource.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this DebtCollectionCaseSource.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this DebtCollectionCaseSource.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this DebtCollectionCaseSource.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this DebtCollectionCaseSource.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this DebtCollectionCaseSource.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this DebtCollectionCaseSource.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/debt_collection_case_update.py` & `wallee-4.0.0/wallee/models/debt_collection_case_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/debt_collection_receipt.py` & `wallee-4.0.0/wallee/models/debt_collection_receipt.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/debt_collection_receipt_source.py` & `wallee-4.0.0/wallee/models/debt_collection_receipt_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this DebtCollectionReceiptSource.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this DebtCollectionReceiptSource.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this DebtCollectionReceiptSource.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this DebtCollectionReceiptSource.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this DebtCollectionReceiptSource.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this DebtCollectionReceiptSource.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this DebtCollectionReceiptSource.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this DebtCollectionReceiptSource.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/debt_collector.py` & `wallee-4.0.0/wallee/models/debt_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this DebtCollector.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this DebtCollector.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this DebtCollector.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this DebtCollector.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this DebtCollector.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this DebtCollector.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this DebtCollector.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this DebtCollector.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/debt_collector_condition.py` & `wallee-4.0.0/wallee/models/debt_collector_condition.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/debt_collector_condition_type.py` & `wallee-4.0.0/wallee/models/debt_collector_condition_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this DebtCollectorConditionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this DebtCollectorConditionType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this DebtCollectorConditionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this DebtCollectorConditionType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this DebtCollectorConditionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this DebtCollectorConditionType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this DebtCollectorConditionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this DebtCollectorConditionType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/debt_collector_configuration.py` & `wallee-4.0.0/wallee/models/debt_collector_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/delivery_indication.py` & `wallee-4.0.0/wallee/models/delivery_indication.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/delivery_indication_decision_reason.py` & `wallee-4.0.0/wallee/models/delivery_indication_decision_reason.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this DeliveryIndicationDecisionReason.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this DeliveryIndicationDecisionReason.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this DeliveryIndicationDecisionReason.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this DeliveryIndicationDecisionReason.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this DeliveryIndicationDecisionReason.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this DeliveryIndicationDecisionReason.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this DeliveryIndicationDecisionReason.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this DeliveryIndicationDecisionReason.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/document_template.py` & `wallee-4.0.0/wallee/models/document_template.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/document_template_type.py` & `wallee-4.0.0/wallee/models/document_template_type.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/document_template_type_group.py` & `wallee-4.0.0/wallee/models/document_template_type_group.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/entity_export_request.py` & `wallee-4.0.0/wallee/models/entity_export_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/entity_query.py` & `wallee-4.0.0/wallee/models/entity_query.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/entity_query_filter.py` & `wallee-4.0.0/wallee/models/entity_query_filter.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/entity_query_order_by.py` & `wallee-4.0.0/wallee/models/entity_query_order_by.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/external_transfer_bank_transaction.py` & `wallee-4.0.0/wallee/models/external_transfer_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/failure_reason.py` & `wallee-4.0.0/wallee/models/failure_reason.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,26 +61,26 @@
 
         self._category = category
     
     @property
     def description(self):
         """Gets the description of this FailureReason.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this FailureReason.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this FailureReason.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this FailureReason.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -130,26 +130,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this FailureReason.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this FailureReason.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this FailureReason.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this FailureReason.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/feature.py` & `wallee-4.0.0/wallee/models/feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,72 +50,72 @@
         
 
     
     @property
     def beta(self):
         """Gets the beta of this Feature.
 
-            
+            Whether the feature is in beta stage and there may still be some issues.
 
         :return: The beta of this Feature.
         :rtype: bool
         """
         return self._beta
 
     @beta.setter
     def beta(self, beta):
         """Sets the beta of this Feature.
 
-            
+            Whether the feature is in beta stage and there may still be some issues.
 
         :param beta: The beta of this Feature.
         :type: bool
         """
 
         self._beta = beta
     
     @property
     def category(self):
         """Gets the category of this Feature.
 
-            
+            The category that the feature belongs to.
 
         :return: The category of this Feature.
         :rtype: FeatureCategory
         """
         return self._category
 
     @category.setter
     def category(self, category):
         """Sets the category of this Feature.
 
-            
+            The category that the feature belongs to.
 
         :param category: The category of this Feature.
         :type: FeatureCategory
         """
 
         self._category = category
     
     @property
     def description(self):
         """Gets the description of this Feature.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this Feature.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this Feature.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this Feature.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -142,95 +142,95 @@
 
         self._id = id
     
     @property
     def logo_path(self):
         """Gets the logo_path of this Feature.
 
-            
+            The path to the feature's logo image.
 
         :return: The logo_path of this Feature.
         :rtype: str
         """
         return self._logo_path
 
     @logo_path.setter
     def logo_path(self, logo_path):
         """Sets the logo_path of this Feature.
 
-            
+            The path to the feature's logo image.
 
         :param logo_path: The logo_path of this Feature.
         :type: str
         """
 
         self._logo_path = logo_path
     
     @property
     def name(self):
         """Gets the name of this Feature.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this Feature.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Feature.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this Feature.
         :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def required_features(self):
         """Gets the required_features of this Feature.
 
-            
+            The features that must be enabled for this feature to work properly.
 
         :return: The required_features of this Feature.
         :rtype: list[int]
         """
         return self._required_features
 
     @required_features.setter
     def required_features(self, required_features):
         """Sets the required_features of this Feature.
 
-            
+            The features that must be enabled for this feature to work properly.
 
         :param required_features: The required_features of this Feature.
         :type: list[int]
         """
 
         self._required_features = required_features
     
     @property
     def sort_order(self):
         """Gets the sort_order of this Feature.
 
-            
+            When listing features, they can be sorted by this number.
 
         :return: The sort_order of this Feature.
         :rtype: int
         """
         return self._sort_order
 
     @sort_order.setter
     def sort_order(self, sort_order):
         """Sets the sort_order of this Feature.
 
-            
+            When listing features, they can be sorted by this number.
 
         :param sort_order: The sort_order of this Feature.
         :type: int
         """
 
         self._sort_order = sort_order
```

### Comparing `wallee-3.4.0/wallee/models/feature_category.py` & `wallee-4.0.0/wallee/models/feature_category.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this FeatureCategory.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this FeatureCategory.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this FeatureCategory.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this FeatureCategory.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -81,49 +81,49 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this FeatureCategory.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this FeatureCategory.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this FeatureCategory.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this FeatureCategory.
         :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def order_weight(self):
         """Gets the order_weight of this FeatureCategory.
 
-            
+            When listing feature categories, they can be sorted by this number.
 
         :return: The order_weight of this FeatureCategory.
         :rtype: int
         """
         return self._order_weight
 
     @order_weight.setter
     def order_weight(self, order_weight):
         """Sets the order_weight of this FeatureCategory.
 
-            
+            When listing feature categories, they can be sorted by this number.
 
         :param order_weight: The order_weight of this FeatureCategory.
         :type: int
         """
 
         self._order_weight = order_weight
```

### Comparing `wallee-3.4.0/wallee/models/human_user.py` & `wallee-4.0.0/wallee/models/human_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         'email_address': 'str',
         'email_address_verified': 'bool',
         'firstname': 'str',
         'language': 'str',
         'lastname': 'str',
         'mobile_phone_number': 'str',
         'mobile_phone_verified': 'bool',
-        'primary_account': 'Account',
-        'scope': 'Scope',
+        'primary_account': 'int',
+        'scope': 'int',
         'time_zone': 'str',
         'two_factor_enabled': 'bool',
         'two_factor_type': 'TwoFactorAuthenticationType',
     }
 
     attribute_map = {
         'email_address': 'emailAddress','email_address_verified': 'emailAddressVerified','firstname': 'firstname','language': 'language','lastname': 'lastname','mobile_phone_number': 'mobilePhoneNumber','mobile_phone_verified': 'mobilePhoneVerified','primary_account': 'primaryAccount','scope': 'scope','time_zone': 'timeZone','two_factor_enabled': 'twoFactorEnabled','two_factor_type': 'twoFactorType',
@@ -59,287 +59,287 @@
         
 
     
     @property
     def email_address(self):
         """Gets the email_address of this HumanUser.
 
-            The email address of the user.
+            The user's email address.
 
         :return: The email_address of this HumanUser.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this HumanUser.
 
-            The email address of the user.
+            The user's email address.
 
         :param email_address: The email_address of this HumanUser.
         :type: str
         """
         if email_address is not None and len(email_address) > 128:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `128`")
 
         self._email_address = email_address
     
     @property
     def email_address_verified(self):
         """Gets the email_address_verified of this HumanUser.
 
-            Defines whether a user is verified or not.
+            Whether the user's email address has been verified.
 
         :return: The email_address_verified of this HumanUser.
         :rtype: bool
         """
         return self._email_address_verified
 
     @email_address_verified.setter
     def email_address_verified(self, email_address_verified):
         """Sets the email_address_verified of this HumanUser.
 
-            Defines whether a user is verified or not.
+            Whether the user's email address has been verified.
 
         :param email_address_verified: The email_address_verified of this HumanUser.
         :type: bool
         """
 
         self._email_address_verified = email_address_verified
     
     @property
     def firstname(self):
         """Gets the firstname of this HumanUser.
 
-            The first name of the user.
+            The user's first name.
 
         :return: The firstname of this HumanUser.
         :rtype: str
         """
         return self._firstname
 
     @firstname.setter
     def firstname(self, firstname):
         """Sets the firstname of this HumanUser.
 
-            The first name of the user.
+            The user's first name.
 
         :param firstname: The firstname of this HumanUser.
         :type: str
         """
         if firstname is not None and len(firstname) > 100:
             raise ValueError("Invalid value for `firstname`, length must be less than or equal to `100`")
 
         self._firstname = firstname
     
     @property
     def language(self):
         """Gets the language of this HumanUser.
 
-            The preferred language of the user.
+            The user's preferred language.
 
         :return: The language of this HumanUser.
         :rtype: str
         """
         return self._language
 
     @language.setter
     def language(self, language):
         """Sets the language of this HumanUser.
 
-            The preferred language of the user.
+            The user's preferred language.
 
         :param language: The language of this HumanUser.
         :type: str
         """
 
         self._language = language
     
     @property
     def lastname(self):
         """Gets the lastname of this HumanUser.
 
-            The last name of the user.
+            The user's last name.
 
         :return: The lastname of this HumanUser.
         :rtype: str
         """
         return self._lastname
 
     @lastname.setter
     def lastname(self, lastname):
         """Sets the lastname of this HumanUser.
 
-            The last name of the user.
+            The user's last name.
 
         :param lastname: The lastname of this HumanUser.
         :type: str
         """
         if lastname is not None and len(lastname) > 100:
             raise ValueError("Invalid value for `lastname`, length must be less than or equal to `100`")
 
         self._lastname = lastname
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this HumanUser.
 
-            
+            The user's mobile phone number.
 
         :return: The mobile_phone_number of this HumanUser.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this HumanUser.
 
-            
+            The user's mobile phone number.
 
         :param mobile_phone_number: The mobile_phone_number of this HumanUser.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 30:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `30`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def mobile_phone_verified(self):
         """Gets the mobile_phone_verified of this HumanUser.
 
-            Defines whether a users mobile phone number is verified or not.
+            Whether the user's mobile phone number has been verified.
 
         :return: The mobile_phone_verified of this HumanUser.
         :rtype: bool
         """
         return self._mobile_phone_verified
 
     @mobile_phone_verified.setter
     def mobile_phone_verified(self, mobile_phone_verified):
         """Sets the mobile_phone_verified of this HumanUser.
 
-            Defines whether a users mobile phone number is verified or not.
+            Whether the user's mobile phone number has been verified.
 
         :param mobile_phone_verified: The mobile_phone_verified of this HumanUser.
         :type: bool
         """
 
         self._mobile_phone_verified = mobile_phone_verified
     
     @property
     def primary_account(self):
         """Gets the primary_account of this HumanUser.
 
-            The primary account links the user to a specific account.
+            The primary account that the user belongs to.
 
         :return: The primary_account of this HumanUser.
-        :rtype: Account
+        :rtype: int
         """
         return self._primary_account
 
     @primary_account.setter
     def primary_account(self, primary_account):
         """Sets the primary_account of this HumanUser.
 
-            The primary account links the user to a specific account.
+            The primary account that the user belongs to.
 
         :param primary_account: The primary_account of this HumanUser.
-        :type: Account
+        :type: int
         """
 
         self._primary_account = primary_account
     
     @property
     def scope(self):
         """Gets the scope of this HumanUser.
 
-            The scope to which the user belongs to.
+            The scope that the user belongs to.
 
         :return: The scope of this HumanUser.
-        :rtype: Scope
+        :rtype: int
         """
         return self._scope
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this HumanUser.
 
-            The scope to which the user belongs to.
+            The scope that the user belongs to.
 
         :param scope: The scope of this HumanUser.
-        :type: Scope
+        :type: int
         """
 
         self._scope = scope
     
     @property
     def time_zone(self):
         """Gets the time_zone of this HumanUser.
 
-            The time zone which is applied for the user. If no timezone is specified the browser is used to determine an appropriate time zone.
+            The user's time zone. If none is specified, the one provided by the browser will be used.
 
         :return: The time_zone of this HumanUser.
         :rtype: str
         """
         return self._time_zone
 
     @time_zone.setter
     def time_zone(self, time_zone):
         """Sets the time_zone of this HumanUser.
 
-            The time zone which is applied for the user. If no timezone is specified the browser is used to determine an appropriate time zone.
+            The user's time zone. If none is specified, the one provided by the browser will be used.
 
         :param time_zone: The time_zone of this HumanUser.
         :type: str
         """
 
         self._time_zone = time_zone
     
     @property
     def two_factor_enabled(self):
         """Gets the two_factor_enabled of this HumanUser.
 
-            Defines whether two-factor authentication is enabled for this user.
+            Whether two-factor authentication is enabled for this user.
 
         :return: The two_factor_enabled of this HumanUser.
         :rtype: bool
         """
         return self._two_factor_enabled
 
     @two_factor_enabled.setter
     def two_factor_enabled(self, two_factor_enabled):
         """Sets the two_factor_enabled of this HumanUser.
 
-            Defines whether two-factor authentication is enabled for this user.
+            Whether two-factor authentication is enabled for this user.
 
         :param two_factor_enabled: The two_factor_enabled of this HumanUser.
         :type: bool
         """
 
         self._two_factor_enabled = two_factor_enabled
     
     @property
     def two_factor_type(self):
         """Gets the two_factor_type of this HumanUser.
 
-            
+            The type of two-factor authentication that is enabled for the user.
 
         :return: The two_factor_type of this HumanUser.
         :rtype: TwoFactorAuthenticationType
         """
         return self._two_factor_type
 
     @two_factor_type.setter
     def two_factor_type(self, two_factor_type):
         """Sets the two_factor_type of this HumanUser.
 
-            
+            The type of two-factor authentication that is enabled for the user.
 
         :param two_factor_type: The two_factor_type of this HumanUser.
         :type: TwoFactorAuthenticationType
         """
 
         self._two_factor_type = two_factor_type
```

### Comparing `wallee-3.4.0/wallee/models/human_user_create.py` & `wallee-4.0.0/wallee/models/human_user_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,26 +28,26 @@
         self.attribute_map.update(super().attribute_map)
 
     
     @property
     def primary_account(self):
         """Gets the primary_account of this HumanUserCreate.
 
-            The primary account links the user to a specific account.
+            The primary account that the user belongs to.
 
         :return: The primary_account of this HumanUserCreate.
         :rtype: int
         """
         return self._primary_account
 
     @primary_account.setter
     def primary_account(self, primary_account):
         """Sets the primary_account of this HumanUserCreate.
 
-            The primary account links the user to a specific account.
+            The primary account that the user belongs to.
 
         :param primary_account: The primary_account of this HumanUserCreate.
         :type: int
         """
 
         self._primary_account = primary_account
```

### Comparing `wallee-3.4.0/wallee/models/human_user_update.py` & `wallee-4.0.0/wallee/models/human_user_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/installment_calculated_plan.py` & `wallee-4.0.0/wallee/models/installment_calculated_plan.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/installment_calculated_slice.py` & `wallee-4.0.0/wallee/models/installment_calculated_slice.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/installment_payment.py` & `wallee-4.0.0/wallee/models/installment_payment.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/installment_payment_slice.py` & `wallee-4.0.0/wallee/models/installment_payment_slice.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/installment_plan_configuration.py` & `wallee-4.0.0/wallee/models/installment_plan_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         'payment_method_configurations': 'list[int]',
         'planned_purge_date': 'datetime',
         'sort_order': 'int',
         'space_reference': 'SpaceReference',
         'state': 'CreationEntityState',
         'tax_class': 'TaxClass',
         'terms_and_conditions': 'ResourcePath',
-        'title': 'DatabaseTranslatedString',
+        'title': 'dict(str, str)',
         'version': 'int',
     }
 
     attribute_map = {
         'base_currency': 'baseCurrency','conditions': 'conditions','id': 'id','installment_fee': 'installmentFee','interest_rate': 'interestRate','linked_space_id': 'linkedSpaceId','minimal_amount': 'minimalAmount','name': 'name','payment_method_configurations': 'paymentMethodConfigurations','planned_purge_date': 'plannedPurgeDate','sort_order': 'sortOrder','space_reference': 'spaceReference','state': 'state','tax_class': 'taxClass','terms_and_conditions': 'termsAndConditions','title': 'title','version': 'version',
     }
 
@@ -424,26 +424,26 @@
     @property
     def title(self):
         """Gets the title of this InstallmentPlanConfiguration.
 
             The title of the installment plan is used within the payment process. The title is visible to the buyer.
 
         :return: The title of this InstallmentPlanConfiguration.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._title
 
     @title.setter
     def title(self, title):
         """Sets the title of this InstallmentPlanConfiguration.
 
             The title of the installment plan is used within the payment process. The title is visible to the buyer.
 
         :param title: The title of this InstallmentPlanConfiguration.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._title = title
     
     @property
     def version(self):
         """Gets the version of this InstallmentPlanConfiguration.
```

### Comparing `wallee-3.4.0/wallee/models/installment_plan_slice_configuration.py` & `wallee-4.0.0/wallee/models/installment_plan_slice_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class InstallmentPlanSliceConfiguration:
 
     swagger_types = {
     
         'id': 'int',
-        'line_item_title': 'DatabaseTranslatedString',
+        'line_item_title': 'dict(str, str)',
         'linked_space_id': 'int',
         'period': 'str',
         'plan': 'InstallmentPlanConfiguration',
         'planned_purge_date': 'datetime',
         'priority': 'int',
         'proportion': 'float',
         'state': 'CreationEntityState',
@@ -79,26 +79,26 @@
     @property
     def line_item_title(self):
         """Gets the line_item_title of this InstallmentPlanSliceConfiguration.
 
             The title of this slices line items. The title is visible to the buyer.
 
         :return: The line_item_title of this InstallmentPlanSliceConfiguration.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._line_item_title
 
     @line_item_title.setter
     def line_item_title(self, line_item_title):
         """Sets the line_item_title of this InstallmentPlanSliceConfiguration.
 
             The title of this slices line items. The title is visible to the buyer.
 
         :param line_item_title: The line_item_title of this InstallmentPlanSliceConfiguration.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._line_item_title = line_item_title
     
     @property
     def linked_space_id(self):
         """Gets the linked_space_id of this InstallmentPlanSliceConfiguration.
```

### Comparing `wallee-3.4.0/wallee/models/internal_transfer_bank_transaction.py` & `wallee-4.0.0/wallee/models/internal_transfer_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/invoice_reconciliation_record.py` & `wallee-4.0.0/wallee/models/invoice_reconciliation_record.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/invoice_reconciliation_record_invoice_link.py` & `wallee-4.0.0/wallee/models/invoice_reconciliation_record_invoice_link.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/invoice_reconciliation_record_type.py` & `wallee-4.0.0/wallee/models/invoice_reconciliation_record_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this InvoiceReconciliationRecordType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this InvoiceReconciliationRecordType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this InvoiceReconciliationRecordType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this InvoiceReconciliationRecordType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this InvoiceReconciliationRecordType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this InvoiceReconciliationRecordType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this InvoiceReconciliationRecordType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this InvoiceReconciliationRecordType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/invoice_reimbursement.py` & `wallee-4.0.0/wallee/models/invoice_reimbursement.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/invoice_reimbursement_with_refund_reference.py` & `wallee-4.0.0/wallee/models/invoice_reimbursement_with_refund_reference.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/label.py` & `wallee-4.0.0/wallee/models/label.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/label_descriptor.py` & `wallee-4.0.0/wallee/models/label_descriptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,95 +47,95 @@
         
 
     
     @property
     def category(self):
         """Gets the category of this LabelDescriptor.
 
-            
+            The label's category.
 
         :return: The category of this LabelDescriptor.
         :rtype: LabelDescriptorCategory
         """
         return self._category
 
     @category.setter
     def category(self, category):
         """Sets the category of this LabelDescriptor.
 
-            
+            The label's category.
 
         :param category: The category of this LabelDescriptor.
         :type: LabelDescriptorCategory
         """
 
         self._category = category
     
     @property
     def description(self):
         """Gets the description of this LabelDescriptor.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this LabelDescriptor.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this LabelDescriptor.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this LabelDescriptor.
         :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def features(self):
         """Gets the features of this LabelDescriptor.
 
-            
+            The features that this label belongs to.
 
         :return: The features of this LabelDescriptor.
         :rtype: list[int]
         """
         return self._features
 
     @features.setter
     def features(self, features):
         """Sets the features of this LabelDescriptor.
 
-            
+            The features that this label belongs to.
 
         :param features: The features of this LabelDescriptor.
         :type: list[int]
         """
 
         self._features = features
     
     @property
     def group(self):
         """Gets the group of this LabelDescriptor.
 
-            
+            The group that this label belongs to.
 
         :return: The group of this LabelDescriptor.
         :rtype: int
         """
         return self._group
 
     @group.setter
     def group(self, group):
         """Sets the group of this LabelDescriptor.
 
-            
+            The group that this label belongs to.
 
         :param group: The group of this LabelDescriptor.
         :type: int
         """
 
         self._group = group
     
@@ -162,72 +162,72 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this LabelDescriptor.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this LabelDescriptor.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this LabelDescriptor.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this LabelDescriptor.
         :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def type(self):
         """Gets the type of this LabelDescriptor.
 
-            
+            The type of the label's value.
 
         :return: The type of this LabelDescriptor.
         :rtype: int
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this LabelDescriptor.
 
-            
+            The type of the label's value.
 
         :param type: The type of this LabelDescriptor.
         :type: int
         """
 
         self._type = type
     
     @property
     def weight(self):
         """Gets the weight of this LabelDescriptor.
 
-            
+            When listing labels, they can be sorted by this number.
 
         :return: The weight of this LabelDescriptor.
         :rtype: int
         """
         return self._weight
 
     @weight.setter
     def weight(self, weight):
         """Sets the weight of this LabelDescriptor.
 
-            
+            When listing labels, they can be sorted by this number.
 
         :param weight: The weight of this LabelDescriptor.
         :type: int
         """
 
         self._weight = weight
```

### Comparing `wallee-3.4.0/wallee/models/label_descriptor_group.py` & `wallee-4.0.0/wallee/models/label_descriptor_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this LabelDescriptorGroup.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this LabelDescriptorGroup.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this LabelDescriptorGroup.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this LabelDescriptorGroup.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -81,49 +81,49 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this LabelDescriptorGroup.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this LabelDescriptorGroup.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this LabelDescriptorGroup.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this LabelDescriptorGroup.
         :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def weight(self):
         """Gets the weight of this LabelDescriptorGroup.
 
-            
+            When listing label groups, they can be sorted by this number.
 
         :return: The weight of this LabelDescriptorGroup.
         :rtype: int
         """
         return self._weight
 
     @weight.setter
     def weight(self, weight):
         """Sets the weight of this LabelDescriptorGroup.
 
-            
+            When listing label groups, they can be sorted by this number.
 
         :param weight: The weight of this LabelDescriptorGroup.
         :type: int
         """
 
         self._weight = weight
```

### Comparing `wallee-3.4.0/wallee/models/label_descriptor_type.py` & `wallee-4.0.0/wallee/models/label_descriptor_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this LabelDescriptorType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this LabelDescriptorType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this LabelDescriptorType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this LabelDescriptorType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -78,26 +78,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this LabelDescriptorType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this LabelDescriptorType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this LabelDescriptorType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this LabelDescriptorType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/legal_organization_form.py` & `wallee-4.0.0/wallee/models/legal_organization_form.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,72 +38,72 @@
         
 
     
     @property
     def country(self):
         """Gets the country of this LegalOrganizationForm.
 
-            
+            The two-letter code of the country the legal organization form is used in (ISO 3166-1 alpha-2 format).
 
         :return: The country of this LegalOrganizationForm.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
         """Sets the country of this LegalOrganizationForm.
 
-            
+            The two-letter code of the country the legal organization form is used in (ISO 3166-1 alpha-2 format).
 
         :param country: The country of this LegalOrganizationForm.
         :type: str
         """
 
         self._country = country
     
     @property
     def description(self):
         """Gets the description of this LegalOrganizationForm.
 
-            
+            The localized descriptions of the legal organization form.
 
         :return: The description of this LegalOrganizationForm.
         :rtype: list[LocalizedString]
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this LegalOrganizationForm.
 
-            
+            The localized descriptions of the legal organization form.
 
         :param description: The description of this LegalOrganizationForm.
         :type: list[LocalizedString]
         """
 
         self._description = description
     
     @property
     def english_description(self):
         """Gets the english_description of this LegalOrganizationForm.
 
-            
+            The English name of the legal organization form.
 
         :return: The english_description of this LegalOrganizationForm.
         :rtype: str
         """
         return self._english_description
 
     @english_description.setter
     def english_description(self, english_description):
         """Sets the english_description of this LegalOrganizationForm.
 
-            
+            The English name of the legal organization form.
 
         :param english_description: The english_description of this LegalOrganizationForm.
         :type: str
         """
 
         self._english_description = english_description
     
@@ -130,26 +130,26 @@
 
         self._id = id
     
     @property
     def shortcut(self):
         """Gets the shortcut of this LegalOrganizationForm.
 
-            
+            The localized shortcuts of the legal organization form.
 
         :return: The shortcut of this LegalOrganizationForm.
         :rtype: list[LocalizedString]
         """
         return self._shortcut
 
     @shortcut.setter
     def shortcut(self, shortcut):
         """Sets the shortcut of this LegalOrganizationForm.
 
-            
+            The localized shortcuts of the legal organization form.
 
         :param shortcut: The shortcut of this LegalOrganizationForm.
         :type: list[LocalizedString]
         """
 
         self._shortcut = shortcut
```

### Comparing `wallee-3.4.0/wallee/models/line_item.py` & `wallee-4.0.0/wallee/models/line_item.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/line_item_attribute.py` & `wallee-4.0.0/wallee/models/line_item_attribute.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/line_item_attribute_create.py` & `wallee-4.0.0/wallee/models/line_item_attribute_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/line_item_create.py` & `wallee-4.0.0/wallee/models/line_item_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/line_item_reduction.py` & `wallee-4.0.0/wallee/models/line_item_reduction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/line_item_reduction_create.py` & `wallee-4.0.0/wallee/models/line_item_reduction_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/localized_string.py` & `wallee-4.0.0/wallee/models/payment_adjustment_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class LocalizedString:
+class PaymentAdjustmentType:
 
     swagger_types = {
     
-        'display_name': 'str',
-        'language': 'str',
-        'string': 'str',
+        'description': 'dict(str, str)',
+        'id': 'int',
+        'name': 'dict(str, str)',
     }
 
     attribute_map = {
-        'display_name': 'displayName','language': 'language','string': 'string',
+        'description': 'description','id': 'id','name': 'name',
     }
 
     
-    _display_name = None
-    _language = None
-    _string = None
+    _description = None
+    _id = None
+    _name = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.display_name = kwargs.get('display_name', None)
-        self.language = kwargs.get('language', None)
-        self.string = kwargs.get('string', None)
+        self.description = kwargs.get('description', None)
+        self.id = kwargs.get('id', None)
+        self.name = kwargs.get('name', None)
         
 
     
     @property
-    def display_name(self):
-        """Gets the display_name of this LocalizedString.
+    def description(self):
+        """Gets the description of this PaymentAdjustmentType.
 
-            
+            The localized description of the object.
 
-        :return: The display_name of this LocalizedString.
-        :rtype: str
+        :return: The description of this PaymentAdjustmentType.
+        :rtype: dict(str, str)
         """
-        return self._display_name
+        return self._description
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this LocalizedString.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this PaymentAdjustmentType.
 
-            
+            The localized description of the object.
 
-        :param display_name: The display_name of this LocalizedString.
-        :type: str
+        :param description: The description of this PaymentAdjustmentType.
+        :type: dict(str, str)
         """
 
-        self._display_name = display_name
+        self._description = description
     
     @property
-    def language(self):
-        """Gets the language of this LocalizedString.
+    def id(self):
+        """Gets the id of this PaymentAdjustmentType.
 
-            
+            A unique identifier for the object.
 
-        :return: The language of this LocalizedString.
-        :rtype: str
+        :return: The id of this PaymentAdjustmentType.
+        :rtype: int
         """
-        return self._language
+        return self._id
 
-    @language.setter
-    def language(self, language):
-        """Sets the language of this LocalizedString.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this PaymentAdjustmentType.
 
-            
+            A unique identifier for the object.
 
-        :param language: The language of this LocalizedString.
-        :type: str
+        :param id: The id of this PaymentAdjustmentType.
+        :type: int
         """
 
-        self._language = language
+        self._id = id
     
     @property
-    def string(self):
-        """Gets the string of this LocalizedString.
+    def name(self):
+        """Gets the name of this PaymentAdjustmentType.
 
-            
+            The localized name of the object.
 
-        :return: The string of this LocalizedString.
-        :rtype: str
+        :return: The name of this PaymentAdjustmentType.
+        :rtype: dict(str, str)
         """
-        return self._string
+        return self._name
 
-    @string.setter
-    def string(self, string):
-        """Sets the string of this LocalizedString.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this PaymentAdjustmentType.
 
-            
+            The localized name of the object.
 
-        :param string: The string of this LocalizedString.
-        :type: str
+        :param name: The name of this PaymentAdjustmentType.
+        :type: dict(str, str)
         """
 
-        self._string = string
+        self._name = name
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -120,27 +120,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(LocalizedString, dict):
+        if issubclass(PaymentAdjustmentType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, LocalizedString):
+        if not isinstance(other, PaymentAdjustmentType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/manual_task.py` & `wallee-4.0.0/wallee/models/manual_task.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,90 +12,87 @@
         'actions': 'list[int]',
         'context_entity_id': 'int',
         'created_on': 'datetime',
         'expires_on': 'datetime',
         'id': 'int',
         'linked_space_id': 'int',
         'planned_purge_date': 'datetime',
-        'space_id': 'int',
         'state': 'ManualTaskState',
         'type': 'int',
     }
 
     attribute_map = {
-        'actions': 'actions','context_entity_id': 'contextEntityId','created_on': 'createdOn','expires_on': 'expiresOn','id': 'id','linked_space_id': 'linkedSpaceId','planned_purge_date': 'plannedPurgeDate','space_id': 'spaceId','state': 'state','type': 'type',
+        'actions': 'actions','context_entity_id': 'contextEntityId','created_on': 'createdOn','expires_on': 'expiresOn','id': 'id','linked_space_id': 'linkedSpaceId','planned_purge_date': 'plannedPurgeDate','state': 'state','type': 'type',
     }
 
     
     _actions = None
     _context_entity_id = None
     _created_on = None
     _expires_on = None
     _id = None
     _linked_space_id = None
     _planned_purge_date = None
-    _space_id = None
     _state = None
     _type = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.actions = kwargs.get('actions', None)
         self.context_entity_id = kwargs.get('context_entity_id', None)
         self.created_on = kwargs.get('created_on', None)
         self.expires_on = kwargs.get('expires_on', None)
         self.id = kwargs.get('id', None)
         self.linked_space_id = kwargs.get('linked_space_id', None)
         self.planned_purge_date = kwargs.get('planned_purge_date', None)
-        self.space_id = kwargs.get('space_id', None)
         self.state = kwargs.get('state', None)
         self.type = kwargs.get('type', None)
         
 
     
     @property
     def actions(self):
         """Gets the actions of this ManualTask.
 
-            
+            The actions that can be triggered to handle the manual task.
 
         :return: The actions of this ManualTask.
         :rtype: list[int]
         """
         return self._actions
 
     @actions.setter
     def actions(self, actions):
         """Sets the actions of this ManualTask.
 
-            
+            The actions that can be triggered to handle the manual task.
 
         :param actions: The actions of this ManualTask.
         :type: list[int]
         """
 
         self._actions = actions
     
     @property
     def context_entity_id(self):
         """Gets the context_entity_id of this ManualTask.
 
-            The context entity ID links the manual task to the entity which caused its creation.
+            The ID of the entity the manual task is linked to.
 
         :return: The context_entity_id of this ManualTask.
         :rtype: int
         """
         return self._context_entity_id
 
     @context_entity_id.setter
     def context_entity_id(self, context_entity_id):
         """Sets the context_entity_id of this ManualTask.
 
-            The context entity ID links the manual task to the entity which caused its creation.
+            The ID of the entity the manual task is linked to.
 
         :param context_entity_id: The context_entity_id of this ManualTask.
         :type: int
         """
 
         self._context_entity_id = context_entity_id
     
@@ -122,26 +119,26 @@
 
         self._created_on = created_on
     
     @property
     def expires_on(self):
         """Gets the expires_on of this ManualTask.
 
-            The expiry date indicates until when the manual task has to be executed.
+            The date and time until when the manual task has to be handled.
 
         :return: The expires_on of this ManualTask.
         :rtype: datetime
         """
         return self._expires_on
 
     @expires_on.setter
     def expires_on(self, expires_on):
         """Sets the expires_on of this ManualTask.
 
-            The expiry date indicates until when the manual task has to be executed.
+            The date and time until when the manual task has to be handled.
 
         :param expires_on: The expires_on of this ManualTask.
         :type: datetime
         """
 
         self._expires_on = expires_on
     
@@ -211,37 +208,14 @@
         :param planned_purge_date: The planned_purge_date of this ManualTask.
         :type: datetime
         """
 
         self._planned_purge_date = planned_purge_date
     
     @property
-    def space_id(self):
-        """Gets the space_id of this ManualTask.
-
-            
-
-        :return: The space_id of this ManualTask.
-        :rtype: int
-        """
-        return self._space_id
-
-    @space_id.setter
-    def space_id(self, space_id):
-        """Sets the space_id of this ManualTask.
-
-            
-
-        :param space_id: The space_id of this ManualTask.
-        :type: int
-        """
-
-        self._space_id = space_id
-    
-    @property
     def state(self):
         """Gets the state of this ManualTask.
 
             The object's current state.
 
         :return: The state of this ManualTask.
         :rtype: ManualTaskState
@@ -260,26 +234,26 @@
 
         self._state = state
     
     @property
     def type(self):
         """Gets the type of this ManualTask.
 
-            The type categorizes the manual task.
+            The manual task's type.
 
         :return: The type of this ManualTask.
         :rtype: int
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this ManualTask.
 
-            The type categorizes the manual task.
+            The manual task's type.
 
         :param type: The type of this ManualTask.
         :type: int
         """
 
         self._type = type
```

### Comparing `wallee-3.4.0/wallee/models/manual_task_action.py` & `wallee-4.0.0/wallee/models/manual_task_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,72 +58,72 @@
 
         self._id = id
     
     @property
     def label(self):
         """Gets the label of this ManualTaskAction.
 
-            
+            The action's label.
 
         :return: The label of this ManualTaskAction.
         :rtype: dict(str, str)
         """
         return self._label
 
     @label.setter
     def label(self, label):
         """Sets the label of this ManualTaskAction.
 
-            
+            The action's label.
 
         :param label: The label of this ManualTaskAction.
         :type: dict(str, str)
         """
 
         self._label = label
     
     @property
     def style(self):
         """Gets the style of this ManualTaskAction.
 
-            
+            The action's style.
 
         :return: The style of this ManualTaskAction.
         :rtype: ManualTaskActionStyle
         """
         return self._style
 
     @style.setter
     def style(self, style):
         """Sets the style of this ManualTaskAction.
 
-            
+            The action's style.
 
         :param style: The style of this ManualTaskAction.
         :type: ManualTaskActionStyle
         """
 
         self._style = style
     
     @property
     def task_type(self):
         """Gets the task_type of this ManualTaskAction.
 
-            
+            The type of manual tasks this action belongs to.
 
         :return: The task_type of this ManualTaskAction.
         :rtype: int
         """
         return self._task_type
 
     @task_type.setter
     def task_type(self, task_type):
         """Sets the task_type of this ManualTaskAction.
 
-            
+            The type of manual tasks this action belongs to.
 
         :param task_type: The task_type of this ManualTaskAction.
         :type: int
         """
 
         self._task_type = task_type
```

### Comparing `wallee-3.4.0/wallee/models/manual_task_type.py` & `wallee-4.0.0/wallee/models/manual_task_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,49 +35,49 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this ManualTaskType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this ManualTaskType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ManualTaskType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this ManualTaskType.
         :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def features(self):
         """Gets the features of this ManualTaskType.
 
-            
+            The features that this type belongs to.
 
         :return: The features of this ManualTaskType.
         :rtype: list[int]
         """
         return self._features
 
     @features.setter
     def features(self, features):
         """Sets the features of this ManualTaskType.
 
-            
+            The features that this type belongs to.
 
         :param features: The features of this ManualTaskType.
         :type: list[int]
         """
 
         self._features = features
     
@@ -104,26 +104,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this ManualTaskType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this ManualTaskType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ManualTaskType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this ManualTaskType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/metric_usage.py` & `wallee-4.0.0/wallee/models/metric_usage.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_adjustment.py` & `wallee-4.0.0/wallee/models/payment_adjustment.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_adjustment_type.py` & `wallee-4.0.0/wallee/models/payment_terminal_receipt_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class PaymentAdjustmentType:
+class PaymentTerminalReceiptType:
 
     swagger_types = {
     
         'description': 'dict(str, str)',
         'id': 'int',
         'name': 'dict(str, str)',
     }
@@ -30,76 +30,76 @@
         self.id = kwargs.get('id', None)
         self.name = kwargs.get('name', None)
         
 
     
     @property
     def description(self):
-        """Gets the description of this PaymentAdjustmentType.
+        """Gets the description of this PaymentTerminalReceiptType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
-        :return: The description of this PaymentAdjustmentType.
+        :return: The description of this PaymentTerminalReceiptType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this PaymentAdjustmentType.
+        """Sets the description of this PaymentTerminalReceiptType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
-        :param description: The description of this PaymentAdjustmentType.
+        :param description: The description of this PaymentTerminalReceiptType.
         :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
-        """Gets the id of this PaymentAdjustmentType.
+        """Gets the id of this PaymentTerminalReceiptType.
 
             A unique identifier for the object.
 
-        :return: The id of this PaymentAdjustmentType.
+        :return: The id of this PaymentTerminalReceiptType.
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this PaymentAdjustmentType.
+        """Sets the id of this PaymentTerminalReceiptType.
 
             A unique identifier for the object.
 
-        :param id: The id of this PaymentAdjustmentType.
+        :param id: The id of this PaymentTerminalReceiptType.
         :type: int
         """
 
         self._id = id
     
     @property
     def name(self):
-        """Gets the name of this PaymentAdjustmentType.
+        """Gets the name of this PaymentTerminalReceiptType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
-        :return: The name of this PaymentAdjustmentType.
+        :return: The name of this PaymentTerminalReceiptType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this PaymentAdjustmentType.
+        """Sets the name of this PaymentTerminalReceiptType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
-        :param name: The name of this PaymentAdjustmentType.
+        :param name: The name of this PaymentTerminalReceiptType.
         :type: dict(str, str)
         """
 
         self._name = name
     
 
     def to_dict(self):
@@ -120,27 +120,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(PaymentAdjustmentType, dict):
+        if issubclass(PaymentTerminalReceiptType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, PaymentAdjustmentType):
+        if not isinstance(other, PaymentTerminalReceiptType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/payment_app_charge_attempt_update_request.py` & `wallee-4.0.0/wallee/models/payment_app_charge_attempt_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_completion_configuration.py` & `wallee-4.0.0/wallee/models/payment_app_completion_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_completion_configuration_create.py` & `wallee-4.0.0/wallee/models/payment_app_completion_configuration_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_completion_update_request.py` & `wallee-4.0.0/wallee/models/payment_app_completion_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_connector.py` & `wallee-4.0.0/wallee/models/payment_app_connector.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_connector_creation_request.py` & `wallee-4.0.0/wallee/models/payment_app_connector_creation_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_processor.py` & `wallee-4.0.0/wallee/models/payment_app_processor.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_processor_creation_request.py` & `wallee-4.0.0/wallee/models/payment_app_processor_creation_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_refund_configuration.py` & `wallee-4.0.0/wallee/models/payment_app_refund_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_refund_configuration_create.py` & `wallee-4.0.0/wallee/models/payment_app_refund_configuration_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_refund_update_request.py` & `wallee-4.0.0/wallee/models/payment_app_refund_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_app_void_update_request.py` & `wallee-4.0.0/wallee/models/payment_app_void_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_connector.py` & `wallee-4.0.0/wallee/models/payment_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,26 +131,26 @@
 
         self._deprecation_reason = deprecation_reason
     
     @property
     def description(self):
         """Gets the description of this PaymentConnector.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this PaymentConnector.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this PaymentConnector.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this PaymentConnector.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -200,26 +200,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this PaymentConnector.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this PaymentConnector.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this PaymentConnector.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this PaymentConnector.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/payment_connector_configuration.py` & `wallee-4.0.0/wallee/models/payment_connector_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_connector_feature.py` & `wallee-4.0.0/wallee/models/payment_connector_feature.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_contract.py` & `wallee-4.0.0/wallee/models/payment_contract.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_contract_type.py` & `wallee-4.0.0/wallee/models/payment_contract_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this PaymentContractType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this PaymentContractType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this PaymentContractType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this PaymentContractType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this PaymentContractType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this PaymentContractType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this PaymentContractType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this PaymentContractType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/payment_information_hash.py` & `wallee-4.0.0/wallee/models/payment_information_hash.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_information_hash_type.py` & `wallee-4.0.0/wallee/models/payment_information_hash_type.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_initiation_advice_file.py` & `wallee-4.0.0/wallee/models/payment_initiation_advice_file.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_link.py` & `wallee-4.0.0/wallee/models/payment_link.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_link_active.py` & `wallee-4.0.0/wallee/models/payment_link_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_link_create.py` & `wallee-4.0.0/wallee/models/payment_link_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_link_update.py` & `wallee-4.0.0/wallee/models/payment_link_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_method.py` & `wallee-4.0.0/wallee/models/payment_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,26 +67,26 @@
 
         self._data_collection_types = data_collection_types
     
     @property
     def description(self):
         """Gets the description of this PaymentMethod.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this PaymentMethod.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this PaymentMethod.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this PaymentMethod.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -159,26 +159,26 @@
 
         self._merchant_description = merchant_description
     
     @property
     def name(self):
         """Gets the name of this PaymentMethod.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this PaymentMethod.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this PaymentMethod.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this PaymentMethod.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/payment_method_brand.py` & `wallee-4.0.0/wallee/models/payment_method_brand.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,26 +41,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this PaymentMethodBrand.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this PaymentMethodBrand.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this PaymentMethodBrand.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this PaymentMethodBrand.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -133,26 +133,26 @@
 
         self._image_path = image_path
     
     @property
     def name(self):
         """Gets the name of this PaymentMethodBrand.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this PaymentMethodBrand.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this PaymentMethodBrand.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this PaymentMethodBrand.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/payment_method_configuration.py` & `wallee-4.0.0/wallee/models/payment_method_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 class PaymentMethodConfiguration:
 
     swagger_types = {
     
         'data_collection_type': 'DataCollectionType',
-        'description': 'DatabaseTranslatedString',
+        'description': 'dict(str, str)',
         'id': 'int',
         'image_resource_path': 'ResourcePath',
         'linked_space_id': 'int',
         'name': 'str',
         'one_click_payment_mode': 'OneClickPaymentMode',
         'payment_method': 'int',
         'planned_purge_date': 'datetime',
         'resolved_description': 'dict(str, str)',
         'resolved_image_url': 'str',
         'resolved_title': 'dict(str, str)',
         'sort_order': 'int',
         'space_id': 'int',
         'state': 'CreationEntityState',
-        'title': 'DatabaseTranslatedString',
+        'title': 'dict(str, str)',
         'version': 'int',
     }
 
     attribute_map = {
         'data_collection_type': 'dataCollectionType','description': 'description','id': 'id','image_resource_path': 'imageResourcePath','linked_space_id': 'linkedSpaceId','name': 'name','one_click_payment_mode': 'oneClickPaymentMode','payment_method': 'paymentMethod','planned_purge_date': 'plannedPurgeDate','resolved_description': 'resolvedDescription','resolved_image_url': 'resolvedImageUrl','resolved_title': 'resolvedTitle','sort_order': 'sortOrder','space_id': 'spaceId','state': 'state','title': 'title','version': 'version',
     }
 
@@ -100,26 +100,26 @@
     @property
     def description(self):
         """Gets the description of this PaymentMethodConfiguration.
 
             The payment method configuration description can be used to show a text during the payment process. Choose an appropriate description as it will be displayed to your customer.
 
         :return: The description of this PaymentMethodConfiguration.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this PaymentMethodConfiguration.
 
             The payment method configuration description can be used to show a text during the payment process. Choose an appropriate description as it will be displayed to your customer.
 
         :param description: The description of this PaymentMethodConfiguration.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
         """Gets the id of this PaymentMethodConfiguration.
@@ -424,26 +424,26 @@
     @property
     def title(self):
         """Gets the title of this PaymentMethodConfiguration.
 
             The title of the payment method configuration is used within the payment process. The title is visible to the customer.
 
         :return: The title of this PaymentMethodConfiguration.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._title
 
     @title.setter
     def title(self, title):
         """Sets the title of this PaymentMethodConfiguration.
 
             The title of the payment method configuration is used within the payment process. The title is visible to the customer.
 
         :param title: The title of this PaymentMethodConfiguration.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._title = title
     
     @property
     def version(self):
         """Gets the version of this PaymentMethodConfiguration.
```

### Comparing `wallee-3.4.0/wallee/models/payment_processor.py` & `wallee-4.0.0/wallee/models/payment_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,26 +70,26 @@
 
         self._company_name = company_name
     
     @property
     def description(self):
         """Gets the description of this PaymentProcessor.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this PaymentProcessor.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this PaymentProcessor.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this PaymentProcessor.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -185,26 +185,26 @@
 
         self._logo_path = logo_path
     
     @property
     def name(self):
         """Gets the name of this PaymentProcessor.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this PaymentProcessor.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this PaymentProcessor.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this PaymentProcessor.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/payment_processor_configuration.py` & `wallee-4.0.0/wallee/models/payment_processor_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal.py` & `wallee-4.0.0/wallee/models/payment_terminal.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,33 +7,35 @@
 
 class PaymentTerminal:
 
     swagger_types = {
     
         'configuration_version': 'PaymentTerminalConfigurationVersion',
         'default_currency': 'str',
+        'device_serial_number': 'str',
         'external_id': 'str',
         'id': 'int',
         'identifier': 'str',
         'linked_space_id': 'int',
         'location_version': 'PaymentTerminalLocationVersion',
         'name': 'str',
         'planned_purge_date': 'datetime',
         'state': 'PaymentTerminalState',
         'type': 'PaymentTerminalType',
         'version': 'int',
     }
 
     attribute_map = {
-        'configuration_version': 'configurationVersion','default_currency': 'defaultCurrency','external_id': 'externalId','id': 'id','identifier': 'identifier','linked_space_id': 'linkedSpaceId','location_version': 'locationVersion','name': 'name','planned_purge_date': 'plannedPurgeDate','state': 'state','type': 'type','version': 'version',
+        'configuration_version': 'configurationVersion','default_currency': 'defaultCurrency','device_serial_number': 'deviceSerialNumber','external_id': 'externalId','id': 'id','identifier': 'identifier','linked_space_id': 'linkedSpaceId','location_version': 'locationVersion','name': 'name','planned_purge_date': 'plannedPurgeDate','state': 'state','type': 'type','version': 'version',
     }
 
     
     _configuration_version = None
     _default_currency = None
+    _device_serial_number = None
     _external_id = None
     _id = None
     _identifier = None
     _linked_space_id = None
     _location_version = None
     _name = None
     _planned_purge_date = None
@@ -42,14 +44,15 @@
     _version = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.configuration_version = kwargs.get('configuration_version', None)
         self.default_currency = kwargs.get('default_currency', None)
+        self.device_serial_number = kwargs.get('device_serial_number', None)
         self.external_id = kwargs.get('external_id', None)
         self.id = kwargs.get('id', None)
         self.identifier = kwargs.get('identifier', None)
         self.linked_space_id = kwargs.get('linked_space_id', None)
         self.location_version = kwargs.get('location_version', None)
         self.name = kwargs.get('name', None)
         self.planned_purge_date = kwargs.get('planned_purge_date', None)
@@ -102,14 +105,37 @@
         :param default_currency: The default_currency of this PaymentTerminal.
         :type: str
         """
 
         self._default_currency = default_currency
     
     @property
+    def device_serial_number(self):
+        """Gets the device_serial_number of this PaymentTerminal.
+
+            
+
+        :return: The device_serial_number of this PaymentTerminal.
+        :rtype: str
+        """
+        return self._device_serial_number
+
+    @device_serial_number.setter
+    def device_serial_number(self, device_serial_number):
+        """Sets the device_serial_number of this PaymentTerminal.
+
+            
+
+        :param device_serial_number: The device_serial_number of this PaymentTerminal.
+        :type: str
+        """
+
+        self._device_serial_number = device_serial_number
+    
+    @property
     def external_id(self):
         """Gets the external_id of this PaymentTerminal.
 
             A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
 
         :return: The external_id of this PaymentTerminal.
         :rtype: str
```

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_address.py` & `wallee-4.0.0/wallee/models/payment_terminal_address.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,335 +65,335 @@
         
 
     
     @property
     def city(self):
         """Gets the city of this PaymentTerminalAddress.
 
-            
+            The city, town or village.
 
         :return: The city of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
         """Sets the city of this PaymentTerminalAddress.
 
-            
+            The city, town or village.
 
         :param city: The city of this PaymentTerminalAddress.
         :type: str
         """
 
         self._city = city
     
     @property
     def country(self):
         """Gets the country of this PaymentTerminalAddress.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :return: The country of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
         """Sets the country of this PaymentTerminalAddress.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :param country: The country of this PaymentTerminalAddress.
         :type: str
         """
 
         self._country = country
     
     @property
     def dependent_locality(self):
         """Gets the dependent_locality of this PaymentTerminalAddress.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :return: The dependent_locality of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
         """Sets the dependent_locality of this PaymentTerminalAddress.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :param dependent_locality: The dependent_locality of this PaymentTerminalAddress.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
         """Gets the email_address of this PaymentTerminalAddress.
 
-            
+            The email address.
 
         :return: The email_address of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this PaymentTerminalAddress.
 
-            
+            The email address.
 
         :param email_address: The email_address of this PaymentTerminalAddress.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this PaymentTerminalAddress.
 
-            
+            The family or last name.
 
         :return: The family_name of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this PaymentTerminalAddress.
 
-            
+            The family or last name.
 
         :param family_name: The family_name of this PaymentTerminalAddress.
         :type: str
         """
 
         self._family_name = family_name
     
     @property
     def given_name(self):
         """Gets the given_name of this PaymentTerminalAddress.
 
-            
+            The given or first name.
 
         :return: The given_name of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this PaymentTerminalAddress.
 
-            
+            The given or first name.
 
         :param given_name: The given_name of this PaymentTerminalAddress.
         :type: str
         """
 
         self._given_name = given_name
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this PaymentTerminalAddress.
 
-            
+            The phone number of a mobile phone.
 
         :return: The mobile_phone_number of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this PaymentTerminalAddress.
 
-            
+            The phone number of a mobile phone.
 
         :param mobile_phone_number: The mobile_phone_number of this PaymentTerminalAddress.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
         """Gets the organization_name of this PaymentTerminalAddress.
 
-            
+            The organization's name.
 
         :return: The organization_name of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
         """Sets the organization_name of this PaymentTerminalAddress.
 
-            
+            The organization's name.
 
         :param organization_name: The organization_name of this PaymentTerminalAddress.
         :type: str
         """
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
         """Gets the phone_number of this PaymentTerminalAddress.
 
-            
+            The phone number.
 
         :return: The phone_number of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
         """Sets the phone_number of this PaymentTerminalAddress.
 
-            
+            The phone number.
 
         :param phone_number: The phone_number of this PaymentTerminalAddress.
         :type: str
         """
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
         """Gets the postal_state of this PaymentTerminalAddress.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :return: The postal_state of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
         """Sets the postal_state of this PaymentTerminalAddress.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :param postal_state: The postal_state of this PaymentTerminalAddress.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
         """Gets the postcode of this PaymentTerminalAddress.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :return: The postcode of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
         """Sets the postcode of this PaymentTerminalAddress.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :param postcode: The postcode of this PaymentTerminalAddress.
         :type: str
         """
 
         self._postcode = postcode
     
     @property
     def salutation(self):
         """Gets the salutation of this PaymentTerminalAddress.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :return: The salutation of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
         """Sets the salutation of this PaymentTerminalAddress.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :param salutation: The salutation of this PaymentTerminalAddress.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
     def sorting_code(self):
         """Gets the sorting_code of this PaymentTerminalAddress.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :return: The sorting_code of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
         """Sets the sorting_code of this PaymentTerminalAddress.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :param sorting_code: The sorting_code of this PaymentTerminalAddress.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
         """Gets the street of this PaymentTerminalAddress.
 
-            
+            The street or PO Box.
 
         :return: The street of this PaymentTerminalAddress.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
         """Sets the street of this PaymentTerminalAddress.
 
-            
+            The street or PO Box.
 
         :param street: The street of this PaymentTerminalAddress.
         :type: str
         """
 
         self._street = street
```

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_configuration.py` & `wallee-4.0.0/wallee/models/payment_terminal_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_configuration_version.py` & `wallee-4.0.0/wallee/models/payment_terminal_configuration_version.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_dcc_transaction_sum.py` & `wallee-4.0.0/wallee/models/payment_terminal_dcc_transaction_sum.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_location.py` & `wallee-4.0.0/wallee/models/payment_terminal_location.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_location_version.py` & `wallee-4.0.0/wallee/models/payment_terminal_location_version.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_receipt_type.py` & `wallee-4.0.0/wallee/models/payment_terminal_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class PaymentTerminalReceiptType:
+class PaymentTerminalType:
 
     swagger_types = {
     
         'description': 'dict(str, str)',
         'id': 'int',
         'name': 'dict(str, str)',
     }
@@ -30,76 +30,76 @@
         self.id = kwargs.get('id', None)
         self.name = kwargs.get('name', None)
         
 
     
     @property
     def description(self):
-        """Gets the description of this PaymentTerminalReceiptType.
+        """Gets the description of this PaymentTerminalType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
-        :return: The description of this PaymentTerminalReceiptType.
+        :return: The description of this PaymentTerminalType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this PaymentTerminalReceiptType.
+        """Sets the description of this PaymentTerminalType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
-        :param description: The description of this PaymentTerminalReceiptType.
+        :param description: The description of this PaymentTerminalType.
         :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
-        """Gets the id of this PaymentTerminalReceiptType.
+        """Gets the id of this PaymentTerminalType.
 
             A unique identifier for the object.
 
-        :return: The id of this PaymentTerminalReceiptType.
+        :return: The id of this PaymentTerminalType.
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this PaymentTerminalReceiptType.
+        """Sets the id of this PaymentTerminalType.
 
             A unique identifier for the object.
 
-        :param id: The id of this PaymentTerminalReceiptType.
+        :param id: The id of this PaymentTerminalType.
         :type: int
         """
 
         self._id = id
     
     @property
     def name(self):
-        """Gets the name of this PaymentTerminalReceiptType.
+        """Gets the name of this PaymentTerminalType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
-        :return: The name of this PaymentTerminalReceiptType.
+        :return: The name of this PaymentTerminalType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this PaymentTerminalReceiptType.
+        """Sets the name of this PaymentTerminalType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
-        :param name: The name of this PaymentTerminalReceiptType.
+        :param name: The name of this PaymentTerminalType.
         :type: dict(str, str)
         """
 
         self._name = name
     
 
     def to_dict(self):
@@ -120,27 +120,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(PaymentTerminalReceiptType, dict):
+        if issubclass(PaymentTerminalType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, PaymentTerminalReceiptType):
+        if not isinstance(other, PaymentTerminalType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_transaction_sum.py` & `wallee-4.0.0/wallee/models/payment_terminal_transaction_sum.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_transaction_summary.py` & `wallee-4.0.0/wallee/models/payment_terminal_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_transaction_summary_fetch_request.py` & `wallee-4.0.0/wallee/models/payment_terminal_transaction_summary_fetch_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/payment_terminal_type.py` & `wallee-4.0.0/wallee/models/subscription_product_active.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,91 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
+from . import AbstractSubscriptionProductActive
 
 
-
-class PaymentTerminalType:
+class SubscriptionProductActive(AbstractSubscriptionProductActive):
 
     swagger_types = {
     
-        'description': 'dict(str, str)',
         'id': 'int',
-        'name': 'dict(str, str)',
+        'version': 'int',
     }
 
     attribute_map = {
-        'description': 'description','id': 'id','name': 'name',
+        'id': 'id','version': 'version',
     }
 
     
-    _description = None
     _id = None
-    _name = None
+    _version = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.description = kwargs.get('description', None)
-        self.id = kwargs.get('id', None)
-        self.name = kwargs.get('name', None)
-        
-
-    
-    @property
-    def description(self):
-        """Gets the description of this PaymentTerminalType.
-
-            The description of the object translated into different languages.
+        self.id = kwargs.get('id')
 
-        :return: The description of this PaymentTerminalType.
-        :rtype: dict(str, str)
-        """
-        return self._description
-
-    @description.setter
-    def description(self, description):
-        """Sets the description of this PaymentTerminalType.
-
-            The description of the object translated into different languages.
+        self.version = kwargs.get('version')
 
-        :param description: The description of this PaymentTerminalType.
-        :type: dict(str, str)
-        """
+        super().__init__(**kwargs)
+        self.swagger_types.update(super().swagger_types)
+        self.attribute_map.update(super().attribute_map)
 
-        self._description = description
     
     @property
     def id(self):
-        """Gets the id of this PaymentTerminalType.
+        """Gets the id of this SubscriptionProductActive.
 
-            A unique identifier for the object.
+            The ID is the primary key of the entity. The ID identifies the entity uniquely.
 
-        :return: The id of this PaymentTerminalType.
+        :return: The id of this SubscriptionProductActive.
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this PaymentTerminalType.
+        """Sets the id of this SubscriptionProductActive.
 
-            A unique identifier for the object.
+            The ID is the primary key of the entity. The ID identifies the entity uniquely.
 
-        :param id: The id of this PaymentTerminalType.
+        :param id: The id of this SubscriptionProductActive.
         :type: int
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
     
     @property
-    def name(self):
-        """Gets the name of this PaymentTerminalType.
+    def version(self):
+        """Gets the version of this SubscriptionProductActive.
 
-            The name of the object translated into different languages.
+            The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :return: The name of this PaymentTerminalType.
-        :rtype: dict(str, str)
+        :return: The version of this SubscriptionProductActive.
+        :rtype: int
         """
-        return self._name
+        return self._version
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this PaymentTerminalType.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this SubscriptionProductActive.
 
-            The name of the object translated into different languages.
+            The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :param name: The name of this PaymentTerminalType.
-        :type: dict(str, str)
+        :param version: The version of this SubscriptionProductActive.
+        :type: int
         """
+        if version is None:
+            raise ValueError("Invalid value for `version`, must not be `None`")
 
-        self._name = name
+        self._version = version
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -120,27 +102,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(PaymentTerminalType, dict):
+        if issubclass(SubscriptionProductActive, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, PaymentTerminalType):
+        if not isinstance(other, SubscriptionProductActive):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/permission.py` & `wallee-4.0.0/wallee/models/permission.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,72 +56,72 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this Permission.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this Permission.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this Permission.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this Permission.
         :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def feature(self):
         """Gets the feature of this Permission.
 
-            
+            The feature that this permission belongs to.
 
         :return: The feature of this Permission.
         :rtype: int
         """
         return self._feature
 
     @feature.setter
     def feature(self, feature):
         """Sets the feature of this Permission.
 
-            
+            The feature that this permission belongs to.
 
         :param feature: The feature of this Permission.
         :type: int
         """
 
         self._feature = feature
     
     @property
     def group(self):
         """Gets the group of this Permission.
 
-            
+            Whether this is a permission group.
 
         :return: The group of this Permission.
         :rtype: bool
         """
         return self._group
 
     @group.setter
     def group(self, group):
         """Sets the group of this Permission.
 
-            
+            Whether this is a permission group.
 
         :param group: The group of this Permission.
         :type: bool
         """
 
         self._group = group
     
@@ -148,141 +148,141 @@
 
         self._id = id
     
     @property
     def leaf(self):
         """Gets the leaf of this Permission.
 
-            
+            Whether this is a leaf in the tree of permissions, and not a group.
 
         :return: The leaf of this Permission.
         :rtype: bool
         """
         return self._leaf
 
     @leaf.setter
     def leaf(self, leaf):
         """Sets the leaf of this Permission.
 
-            
+            Whether this is a leaf in the tree of permissions, and not a group.
 
         :param leaf: The leaf of this Permission.
         :type: bool
         """
 
         self._leaf = leaf
     
     @property
     def name(self):
         """Gets the name of this Permission.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this Permission.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Permission.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this Permission.
         :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def parent(self):
         """Gets the parent of this Permission.
 
-            
+            The group that this permission belongs to.
 
         :return: The parent of this Permission.
         :rtype: int
         """
         return self._parent
 
     @parent.setter
     def parent(self, parent):
         """Sets the parent of this Permission.
 
-            
+            The group that this permission belongs to.
 
         :param parent: The parent of this Permission.
         :type: int
         """
 
         self._parent = parent
     
     @property
     def path_to_root(self):
         """Gets the path_to_root of this Permission.
 
-            
+            All parents of this permission up to the root of the permission tree.
 
         :return: The path_to_root of this Permission.
         :rtype: list[int]
         """
         return self._path_to_root
 
     @path_to_root.setter
     def path_to_root(self, path_to_root):
         """Sets the path_to_root of this Permission.
 
-            
+            All parents of this permission up to the root of the permission tree.
 
         :param path_to_root: The path_to_root of this Permission.
         :type: list[int]
         """
 
         self._path_to_root = path_to_root
     
     @property
     def title(self):
         """Gets the title of this Permission.
 
-            
+            The localized name of the object.
 
         :return: The title of this Permission.
         :rtype: dict(str, str)
         """
         return self._title
 
     @title.setter
     def title(self, title):
         """Sets the title of this Permission.
 
-            
+            The localized name of the object.
 
         :param title: The title of this Permission.
         :type: dict(str, str)
         """
 
         self._title = title
     
     @property
     def two_factor_required(self):
         """Gets the two_factor_required of this Permission.
 
-            
+            Whether users with this permission are required to enable two-factor authentication.
 
         :return: The two_factor_required of this Permission.
         :rtype: bool
         """
         return self._two_factor_required
 
     @two_factor_required.setter
     def two_factor_required(self, two_factor_required):
         """Sets the two_factor_required of this Permission.
 
-            
+            Whether users with this permission are required to enable two-factor authentication.
 
         :param two_factor_required: The two_factor_required of this Permission.
         :type: bool
         """
 
         self._two_factor_required = two_factor_required
```

### Comparing `wallee-3.4.0/wallee/models/persistable_currency_amount.py` & `wallee-4.0.0/wallee/models/persistable_currency_amount.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/persistable_currency_amount_update.py` & `wallee-4.0.0/wallee/models/persistable_currency_amount_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/product_metered_fee.py` & `wallee-4.0.0/wallee/models/product_metered_fee.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 class ProductMeteredFee:
 
     swagger_types = {
     
         'component': 'SubscriptionProductComponent',
-        'description': 'DatabaseTranslatedString',
+        'description': 'dict(str, str)',
         'id': 'int',
         'linked_space_id': 'int',
         'metric': 'SubscriptionMetric',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'tier_pricing': 'ProductMeteredTierPricing',
         'type': 'ProductFeeType',
         'version': 'int',
     }
 
     attribute_map = {
         'component': 'component','description': 'description','id': 'id','linked_space_id': 'linkedSpaceId','metric': 'metric','name': 'name','tier_pricing': 'tierPricing','type': 'type','version': 'version',
@@ -76,26 +76,26 @@
     @property
     def description(self):
         """Gets the description of this ProductMeteredFee.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :return: The description of this ProductMeteredFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ProductMeteredFee.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :param description: The description of this ProductMeteredFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
         """Gets the id of this ProductMeteredFee.
@@ -168,26 +168,26 @@
     @property
     def name(self):
         """Gets the name of this ProductMeteredFee.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :return: The name of this ProductMeteredFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ProductMeteredFee.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :param name: The name of this ProductMeteredFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def tier_pricing(self):
         """Gets the tier_pricing of this ProductMeteredFee.
```

### Comparing `wallee-3.4.0/wallee/models/product_metered_fee_update.py` & `wallee-4.0.0/wallee/models/product_metered_fee_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 class ProductMeteredFeeUpdate:
 
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
         'component': 'int',
-        'description': 'DatabaseTranslatedStringCreate',
+        'description': 'dict(str, str)',
         'metric': 'int',
-        'name': 'DatabaseTranslatedStringCreate',
+        'name': 'dict(str, str)',
         'tier_pricing': 'ProductMeteredTierPricing',
     }
 
     attribute_map = {
         'id': 'id','version': 'version','component': 'component','description': 'description','metric': 'metric','name': 'name','tier_pricing': 'tierPricing',
     }
 
@@ -122,26 +122,26 @@
     @property
     def description(self):
         """Gets the description of this ProductMeteredFeeUpdate.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :return: The description of this ProductMeteredFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ProductMeteredFeeUpdate.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :param description: The description of this ProductMeteredFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def metric(self):
         """Gets the metric of this ProductMeteredFeeUpdate.
@@ -168,26 +168,26 @@
     @property
     def name(self):
         """Gets the name of this ProductMeteredFeeUpdate.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :return: The name of this ProductMeteredFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ProductMeteredFeeUpdate.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :param name: The name of this ProductMeteredFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def tier_pricing(self):
         """Gets the tier_pricing of this ProductMeteredFeeUpdate.
```

### Comparing `wallee-3.4.0/wallee/models/product_metered_tier_fee.py` & `wallee-4.0.0/wallee/models/product_metered_tier_fee.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/product_metered_tier_fee_update.py` & `wallee-4.0.0/wallee/models/product_metered_tier_fee_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/product_period_fee.py` & `wallee-4.0.0/wallee/models/product_period_fee.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 class ProductPeriodFee:
 
     swagger_types = {
     
         'component': 'SubscriptionProductComponent',
-        'description': 'DatabaseTranslatedString',
+        'description': 'dict(str, str)',
         'id': 'int',
-        'ledger_entry_title': 'DatabaseTranslatedString',
+        'ledger_entry_title': 'dict(str, str)',
         'linked_space_id': 'int',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'number_of_free_trial_periods': 'int',
         'period_fee': 'list[PersistableCurrencyAmount]',
         'type': 'ProductFeeType',
         'version': 'int',
     }
 
     attribute_map = {
@@ -79,26 +79,26 @@
     @property
     def description(self):
         """Gets the description of this ProductPeriodFee.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :return: The description of this ProductPeriodFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ProductPeriodFee.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :param description: The description of this ProductPeriodFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
         """Gets the id of this ProductPeriodFee.
@@ -125,26 +125,26 @@
     @property
     def ledger_entry_title(self):
         """Gets the ledger_entry_title of this ProductPeriodFee.
 
             The ledger entry title will be used for the title in the ledger entry and in the invoice.
 
         :return: The ledger_entry_title of this ProductPeriodFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._ledger_entry_title
 
     @ledger_entry_title.setter
     def ledger_entry_title(self, ledger_entry_title):
         """Sets the ledger_entry_title of this ProductPeriodFee.
 
             The ledger entry title will be used for the title in the ledger entry and in the invoice.
 
         :param ledger_entry_title: The ledger_entry_title of this ProductPeriodFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._ledger_entry_title = ledger_entry_title
     
     @property
     def linked_space_id(self):
         """Gets the linked_space_id of this ProductPeriodFee.
@@ -171,26 +171,26 @@
     @property
     def name(self):
         """Gets the name of this ProductPeriodFee.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :return: The name of this ProductPeriodFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ProductPeriodFee.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :param name: The name of this ProductPeriodFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def number_of_free_trial_periods(self):
         """Gets the number_of_free_trial_periods of this ProductPeriodFee.
```

### Comparing `wallee-3.4.0/wallee/models/product_period_fee_update.py` & `wallee-4.0.0/wallee/models/product_period_fee_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 class ProductPeriodFeeUpdate:
 
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
         'component': 'int',
-        'description': 'DatabaseTranslatedStringCreate',
-        'ledger_entry_title': 'DatabaseTranslatedStringCreate',
-        'name': 'DatabaseTranslatedStringCreate',
+        'description': 'dict(str, str)',
+        'ledger_entry_title': 'dict(str, str)',
+        'name': 'dict(str, str)',
         'number_of_free_trial_periods': 'int',
         'period_fee': 'list[PersistableCurrencyAmountUpdate]',
     }
 
     attribute_map = {
         'id': 'id','version': 'version','component': 'component','description': 'description','ledger_entry_title': 'ledgerEntryTitle','name': 'name','number_of_free_trial_periods': 'numberOfFreeTrialPeriods','period_fee': 'periodFee',
     }
@@ -125,72 +125,72 @@
     @property
     def description(self):
         """Gets the description of this ProductPeriodFeeUpdate.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :return: The description of this ProductPeriodFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ProductPeriodFeeUpdate.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :param description: The description of this ProductPeriodFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def ledger_entry_title(self):
         """Gets the ledger_entry_title of this ProductPeriodFeeUpdate.
 
             The ledger entry title will be used for the title in the ledger entry and in the invoice.
 
         :return: The ledger_entry_title of this ProductPeriodFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._ledger_entry_title
 
     @ledger_entry_title.setter
     def ledger_entry_title(self, ledger_entry_title):
         """Sets the ledger_entry_title of this ProductPeriodFeeUpdate.
 
             The ledger entry title will be used for the title in the ledger entry and in the invoice.
 
         :param ledger_entry_title: The ledger_entry_title of this ProductPeriodFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._ledger_entry_title = ledger_entry_title
     
     @property
     def name(self):
         """Gets the name of this ProductPeriodFeeUpdate.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :return: The name of this ProductPeriodFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ProductPeriodFeeUpdate.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :param name: The name of this ProductPeriodFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def number_of_free_trial_periods(self):
         """Gets the number_of_free_trial_periods of this ProductPeriodFeeUpdate.
```

### Comparing `wallee-3.4.0/wallee/models/product_setup_fee.py` & `wallee-4.0.0/wallee/models/product_setup_fee.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 
 class ProductSetupFee:
 
     swagger_types = {
     
         'component': 'SubscriptionProductComponent',
-        'description': 'DatabaseTranslatedString',
+        'description': 'dict(str, str)',
         'id': 'int',
         'linked_space_id': 'int',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'on_downgrade_credited_amount': 'list[PersistableCurrencyAmount]',
         'on_upgrade_credited_amount': 'list[PersistableCurrencyAmount]',
         'setup_fee': 'list[PersistableCurrencyAmount]',
         'type': 'ProductFeeType',
         'version': 'int',
     }
 
@@ -79,26 +79,26 @@
     @property
     def description(self):
         """Gets the description of this ProductSetupFee.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :return: The description of this ProductSetupFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ProductSetupFee.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :param description: The description of this ProductSetupFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
         """Gets the id of this ProductSetupFee.
@@ -148,26 +148,26 @@
     @property
     def name(self):
         """Gets the name of this ProductSetupFee.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :return: The name of this ProductSetupFee.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ProductSetupFee.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :param name: The name of this ProductSetupFee.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def on_downgrade_credited_amount(self):
         """Gets the on_downgrade_credited_amount of this ProductSetupFee.
```

### Comparing `wallee-3.4.0/wallee/models/product_setup_fee_update.py` & `wallee-4.0.0/wallee/models/product_setup_fee_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class ProductSetupFeeUpdate:
 
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
         'component': 'int',
-        'description': 'DatabaseTranslatedStringCreate',
-        'name': 'DatabaseTranslatedStringCreate',
+        'description': 'dict(str, str)',
+        'name': 'dict(str, str)',
         'on_downgrade_credited_amount': 'list[PersistableCurrencyAmountUpdate]',
         'on_upgrade_credited_amount': 'list[PersistableCurrencyAmountUpdate]',
         'setup_fee': 'list[PersistableCurrencyAmountUpdate]',
     }
 
     attribute_map = {
         'id': 'id','version': 'version','component': 'component','description': 'description','name': 'name','on_downgrade_credited_amount': 'onDowngradeCreditedAmount','on_upgrade_credited_amount': 'onUpgradeCreditedAmount','setup_fee': 'setupFee',
@@ -125,49 +125,49 @@
     @property
     def description(self):
         """Gets the description of this ProductSetupFeeUpdate.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :return: The description of this ProductSetupFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this ProductSetupFeeUpdate.
 
             The description of a component fee describes the fee to the subscriber. The description may be shown in documents or on certain user interfaces.
 
         :param description: The description of this ProductSetupFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def name(self):
         """Gets the name of this ProductSetupFeeUpdate.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :return: The name of this ProductSetupFeeUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ProductSetupFeeUpdate.
 
             The name of the fee should describe for the subscriber in few words for what the fee is for.
 
         :param name: The name of this ProductSetupFeeUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def on_downgrade_credited_amount(self):
         """Gets the on_downgrade_credited_amount of this ProductSetupFeeUpdate.
```

### Comparing `wallee-3.4.0/wallee/models/refund.py` & `wallee-4.0.0/wallee/models/refund.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/refund_bank_transaction.py` & `wallee-4.0.0/wallee/models/refund_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/refund_comment.py` & `wallee-4.0.0/wallee/models/refund_comment.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,51 +53,51 @@
         
 
     
     @property
     def content(self):
         """Gets the content of this RefundComment.
 
-            
+            The comment's actual content.
 
         :return: The content of this RefundComment.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
         """Sets the content of this RefundComment.
 
-            
+            The comment's actual content.
 
         :param content: The content of this RefundComment.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
     @property
     def created_by(self):
         """Gets the created_by of this RefundComment.
 
-            
+            The ID of the user the comment was created by.
 
         :return: The created_by of this RefundComment.
         :rtype: int
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this RefundComment.
 
-            
+            The ID of the user the comment was created by.
 
         :param created_by: The created_by of this RefundComment.
         :type: int
         """
 
         self._created_by = created_by
     
@@ -124,49 +124,49 @@
 
         self._created_on = created_on
     
     @property
     def edited_by(self):
         """Gets the edited_by of this RefundComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :return: The edited_by of this RefundComment.
         :rtype: int
         """
         return self._edited_by
 
     @edited_by.setter
     def edited_by(self, edited_by):
         """Sets the edited_by of this RefundComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :param edited_by: The edited_by of this RefundComment.
         :type: int
         """
 
         self._edited_by = edited_by
     
     @property
     def edited_on(self):
         """Gets the edited_on of this RefundComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :return: The edited_on of this RefundComment.
         :rtype: datetime
         """
         return self._edited_on
 
     @edited_on.setter
     def edited_on(self, edited_on):
         """Sets the edited_on of this RefundComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :param edited_on: The edited_on of this RefundComment.
         :type: datetime
         """
 
         self._edited_on = edited_on
     
@@ -216,26 +216,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def pinned(self):
         """Gets the pinned of this RefundComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :return: The pinned of this RefundComment.
         :rtype: bool
         """
         return self._pinned
 
     @pinned.setter
     def pinned(self, pinned):
         """Sets the pinned of this RefundComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :param pinned: The pinned of this RefundComment.
         :type: bool
         """
 
         self._pinned = pinned
```

### Comparing `wallee-3.4.0/wallee/models/refund_comment_active.py` & `wallee-4.0.0/wallee/models/refund_comment_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/refund_comment_create.py` & `wallee-4.0.0/wallee/models/tax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,87 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractRefundCommentActive
 
 
-class RefundCommentCreate(AbstractRefundCommentActive):
+
+class Tax:
 
     swagger_types = {
     
-        'refund': 'int',
+        'rate': 'float',
+        'title': 'str',
     }
 
     attribute_map = {
-        'refund': 'refund',
+        'rate': 'rate','title': 'title',
     }
 
     
-    _refund = None
+    _rate = None
+    _title = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.refund = kwargs.get('refund')
+        self.rate = kwargs.get('rate', None)
+        self.title = kwargs.get('title', None)
+        
+
+    
+    @property
+    def rate(self):
+        """Gets the rate of this Tax.
+
+            
 
-        super().__init__(**kwargs)
-        self.swagger_types.update(super().swagger_types)
-        self.attribute_map.update(super().attribute_map)
+        :return: The rate of this Tax.
+        :rtype: float
+        """
+        return self._rate
+
+    @rate.setter
+    def rate(self, rate):
+        """Sets the rate of this Tax.
+
+            
+
+        :param rate: The rate of this Tax.
+        :type: float
+        """
 
+        self._rate = rate
     
     @property
-    def refund(self):
-        """Gets the refund of this RefundCommentCreate.
+    def title(self):
+        """Gets the title of this Tax.
 
             
 
-        :return: The refund of this RefundCommentCreate.
-        :rtype: int
+        :return: The title of this Tax.
+        :rtype: str
         """
-        return self._refund
+        return self._title
 
-    @refund.setter
-    def refund(self, refund):
-        """Sets the refund of this RefundCommentCreate.
+    @title.setter
+    def title(self, title):
+        """Sets the title of this Tax.
 
             
 
-        :param refund: The refund of this RefundCommentCreate.
-        :type: int
+        :param title: The title of this Tax.
+        :type: str
         """
-        if refund is None:
-            raise ValueError("Invalid value for `refund`, must not be `None`")
+        if title is not None and len(title) > 40:
+            raise ValueError("Invalid value for `title`, length must be less than or equal to `40`")
+        if title is not None and len(title) < 2:
+            raise ValueError("Invalid value for `title`, length must be greater than or equal to `2`")
 
-        self._refund = refund
+        self._title = title
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -73,27 +98,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(RefundCommentCreate, dict):
+        if issubclass(Tax, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, RefundCommentCreate):
+        if not isinstance(other, Tax):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/refund_create.py` & `wallee-4.0.0/wallee/models/refund_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/refund_recovery_bank_transaction.py` & `wallee-4.0.0/wallee/models/refund_recovery_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/rendered_document.py` & `wallee-4.0.0/wallee/models/rendered_document.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/rendered_terminal_receipt.py` & `wallee-4.0.0/wallee/models/rendered_terminal_receipt.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/rendered_terminal_transaction_summary.py` & `wallee-4.0.0/wallee/models/rendered_terminal_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/resource_path.py` & `wallee-4.0.0/wallee/models/resource_path.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/rest_address_format.py` & `wallee-4.0.0/wallee/models/rest_address_format.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,95 +35,95 @@
         
 
     
     @property
     def post_code_examples(self):
         """Gets the post_code_examples of this RestAddressFormat.
 
-            The example post codes allow the user to understand what we expect here.
+            A list of sample post codes.
 
         :return: The post_code_examples of this RestAddressFormat.
         :rtype: list[str]
         """
         return self._post_code_examples
 
     @post_code_examples.setter
     def post_code_examples(self, post_code_examples):
         """Sets the post_code_examples of this RestAddressFormat.
 
-            The example post codes allow the user to understand what we expect here.
+            A list of sample post codes.
 
         :param post_code_examples: The post_code_examples of this RestAddressFormat.
         :type: list[str]
         """
 
         self._post_code_examples = post_code_examples
     
     @property
     def post_code_regex(self):
         """Gets the post_code_regex of this RestAddressFormat.
 
-            The post code regex is a regular expression which can validates the input of the post code.
+            The regular expression to validate post codes.
 
         :return: The post_code_regex of this RestAddressFormat.
         :rtype: str
         """
         return self._post_code_regex
 
     @post_code_regex.setter
     def post_code_regex(self, post_code_regex):
         """Sets the post_code_regex of this RestAddressFormat.
 
-            The post code regex is a regular expression which can validates the input of the post code.
+            The regular expression to validate post codes.
 
         :param post_code_regex: The post_code_regex of this RestAddressFormat.
         :type: str
         """
 
         self._post_code_regex = post_code_regex
     
     @property
     def required_fields(self):
         """Gets the required_fields of this RestAddressFormat.
 
-            The required fields indicate what fields are required within an address to comply with the address format.
+            The fields that are required in the address format.
 
         :return: The required_fields of this RestAddressFormat.
         :rtype: list[RestAddressFormatField]
         """
         return self._required_fields
 
     @required_fields.setter
     def required_fields(self, required_fields):
         """Sets the required_fields of this RestAddressFormat.
 
-            The required fields indicate what fields are required within an address to comply with the address format.
+            The fields that are required in the address format.
 
         :param required_fields: The required_fields of this RestAddressFormat.
         :type: list[RestAddressFormatField]
         """
 
         self._required_fields = required_fields
     
     @property
     def used_fields(self):
         """Gets the used_fields of this RestAddressFormat.
 
-            The used fields indicate what fields are used within this address format.
+            The fields that are used in the address format.
 
         :return: The used_fields of this RestAddressFormat.
         :rtype: list[RestAddressFormatField]
         """
         return self._used_fields
 
     @used_fields.setter
     def used_fields(self, used_fields):
         """Sets the used_fields of this RestAddressFormat.
 
-            The used fields indicate what fields are used within this address format.
+            The fields that are used in the address format.
 
         :param used_fields: The used_fields of this RestAddressFormat.
         :type: list[RestAddressFormatField]
         """
 
         self._used_fields = used_fields
```

### Comparing `wallee-3.4.0/wallee/models/rest_country.py` & `wallee-4.0.0/wallee/models/rest_country.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,141 +41,141 @@
         
 
     
     @property
     def iso_code2_letter(self):
         """Gets the iso_code2_letter of this RestCountry.
 
-            The ISO code 2 letter identifies the country by two chars as defined in ISO 3166-1 (e.g. US, DE, CH).
+            The country's two-letter code (ISO 3166-1 alpha-2 format).
 
         :return: The iso_code2_letter of this RestCountry.
         :rtype: str
         """
         return self._iso_code2_letter
 
     @iso_code2_letter.setter
     def iso_code2_letter(self, iso_code2_letter):
         """Sets the iso_code2_letter of this RestCountry.
 
-            The ISO code 2 letter identifies the country by two chars as defined in ISO 3166-1 (e.g. US, DE, CH).
+            The country's two-letter code (ISO 3166-1 alpha-2 format).
 
         :param iso_code2_letter: The iso_code2_letter of this RestCountry.
         :type: str
         """
 
         self._iso_code2_letter = iso_code2_letter
     
     @property
     def iso_code3_letter(self):
         """Gets the iso_code3_letter of this RestCountry.
 
-            The ISO code 3 letter identifies the country by three chars as defined in ISO 3166-1 (e.g. CHE, USA, GBR).
+            The country's three-letter code (ISO 3166-1 alpha-3 format).
 
         :return: The iso_code3_letter of this RestCountry.
         :rtype: str
         """
         return self._iso_code3_letter
 
     @iso_code3_letter.setter
     def iso_code3_letter(self, iso_code3_letter):
         """Sets the iso_code3_letter of this RestCountry.
 
-            The ISO code 3 letter identifies the country by three chars as defined in ISO 3166-1 (e.g. CHE, USA, GBR).
+            The country's three-letter code (ISO 3166-1 alpha-3 format).
 
         :param iso_code3_letter: The iso_code3_letter of this RestCountry.
         :type: str
         """
 
         self._iso_code3_letter = iso_code3_letter
     
     @property
     def address_format(self):
         """Gets the address_format of this RestCountry.
 
-            The address format of the country indicates how an address has to look like for the country.
+            Specifies the country's way of formatting addresses.
 
         :return: The address_format of this RestCountry.
         :rtype: RestAddressFormat
         """
         return self._address_format
 
     @address_format.setter
     def address_format(self, address_format):
         """Sets the address_format of this RestCountry.
 
-            The address format of the country indicates how an address has to look like for the country.
+            Specifies the country's way of formatting addresses.
 
         :param address_format: The address_format of this RestCountry.
         :type: RestAddressFormat
         """
 
         self._address_format = address_format
     
     @property
     def name(self):
         """Gets the name of this RestCountry.
 
-            The name labels the country by a name in English.
+            The name of the country.
 
         :return: The name of this RestCountry.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this RestCountry.
 
-            The name labels the country by a name in English.
+            The name of the country.
 
         :param name: The name of this RestCountry.
         :type: str
         """
 
         self._name = name
     
     @property
     def numeric_code(self):
         """Gets the numeric_code of this RestCountry.
 
-            The numeric code identifies the country by a three digit number as defined in ISO 3166-1 (e.g. 840, 826, 756).
+            The country's three-digit code (ISO 3166-1 numeric format).
 
         :return: The numeric_code of this RestCountry.
         :rtype: str
         """
         return self._numeric_code
 
     @numeric_code.setter
     def numeric_code(self, numeric_code):
         """Sets the numeric_code of this RestCountry.
 
-            The numeric code identifies the country by a three digit number as defined in ISO 3166-1 (e.g. 840, 826, 756).
+            The country's three-digit code (ISO 3166-1 numeric format).
 
         :param numeric_code: The numeric_code of this RestCountry.
         :type: str
         """
 
         self._numeric_code = numeric_code
     
     @property
     def state_codes(self):
         """Gets the state_codes of this RestCountry.
 
-            The state codes field is a list of all states associated with this country. The list contains the identifiers of the states. The identifiers corresponds to the ISO 3166-2 subdivision identifier.
+            The codes of all regions (e.g. states, provinces) of the country (ISO 3166-2 format).
 
         :return: The state_codes of this RestCountry.
         :rtype: list[str]
         """
         return self._state_codes
 
     @state_codes.setter
     def state_codes(self, state_codes):
         """Sets the state_codes of this RestCountry.
 
-            The state codes field is a list of all states associated with this country. The list contains the identifiers of the states. The identifiers corresponds to the ISO 3166-2 subdivision identifier.
+            The codes of all regions (e.g. states, provinces) of the country (ISO 3166-2 format).
 
         :param state_codes: The state_codes of this RestCountry.
         :type: list[str]
         """
 
         self._state_codes = state_codes
```

### Comparing `wallee-3.4.0/wallee/models/rest_country_state.py` & `wallee-4.0.0/wallee/models/rest_country_state.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,124 +6,150 @@
 
 
 class RestCountryState:
 
     swagger_types = {
     
         'code': 'str',
+        'country': 'str',
         'country_code': 'str',
         'id': 'str',
         'name': 'str',
     }
 
     attribute_map = {
-        'code': 'code','country_code': 'countryCode','id': 'id','name': 'name',
+        'code': 'code','country': 'country','country_code': 'countryCode','id': 'id','name': 'name',
     }
 
     
     _code = None
+    _country = None
     _country_code = None
     _id = None
     _name = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.code = kwargs.get('code', None)
+        self.country = kwargs.get('country', None)
         self.country_code = kwargs.get('country_code', None)
         self.id = kwargs.get('id', None)
         self.name = kwargs.get('name', None)
         
 
     
     @property
     def code(self):
         """Gets the code of this RestCountryState.
 
-            The code of the state identifies the state. The code is typically used within addresses. Some countries may not provide a code. For those the field is null.
+            The state's code used within addresses.
 
         :return: The code of this RestCountryState.
         :rtype: str
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this RestCountryState.
 
-            The code of the state identifies the state. The code is typically used within addresses. Some countries may not provide a code. For those the field is null.
+            The state's code used within addresses.
 
         :param code: The code of this RestCountryState.
         :type: str
         """
 
         self._code = code
     
     @property
+    def country(self):
+        """Gets the country of this RestCountryState.
+
+            
+
+        :return: The country of this RestCountryState.
+        :rtype: str
+        """
+        return self._country
+
+    @country.setter
+    def country(self, country):
+        """Sets the country of this RestCountryState.
+
+            
+
+        :param country: The country of this RestCountryState.
+        :type: str
+        """
+
+        self._country = country
+    
+    @property
     def country_code(self):
         """Gets the country_code of this RestCountryState.
 
-            The country code in ISO two letter format (e.g. UK, DE, CH, US).
+            The two-letter code of the state's country (ISO 3166-1 alpha-2 format).
 
         :return: The country_code of this RestCountryState.
         :rtype: str
         """
         return self._country_code
 
     @country_code.setter
     def country_code(self, country_code):
         """Sets the country_code of this RestCountryState.
 
-            The country code in ISO two letter format (e.g. UK, DE, CH, US).
+            The two-letter code of the state's country (ISO 3166-1 alpha-2 format).
 
         :param country_code: The country_code of this RestCountryState.
         :type: str
         """
 
         self._country_code = country_code
     
     @property
     def id(self):
         """Gets the id of this RestCountryState.
 
-            The ID of the state corresponds to the subdivision identifier defined in ISO 3166-2. The format consists of the country code followed by a dash and a subdivision identifier.
+            The state's code in ISO 3166-2 format.
 
         :return: The id of this RestCountryState.
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this RestCountryState.
 
-            The ID of the state corresponds to the subdivision identifier defined in ISO 3166-2. The format consists of the country code followed by a dash and a subdivision identifier.
+            The state's code in ISO 3166-2 format.
 
         :param id: The id of this RestCountryState.
         :type: str
         """
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this RestCountryState.
 
-            The name is a human readable label of the state in the language of the region.
+            The name of the state.
 
         :return: The name of this RestCountryState.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this RestCountryState.
 
-            The name is a human readable label of the state in the language of the region.
+            The name of the state.
 
         :param name: The name of this RestCountryState.
         :type: str
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/rest_currency.py` & `wallee-4.0.0/wallee/models/rest_currency.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,97 +7,123 @@
 
 class RestCurrency:
 
     swagger_types = {
     
         'currency_code': 'str',
         'fraction_digits': 'int',
+        'name': 'str',
         'numeric_code': 'int',
     }
 
     attribute_map = {
-        'currency_code': 'currencyCode','fraction_digits': 'fractionDigits','numeric_code': 'numericCode',
+        'currency_code': 'currencyCode','fraction_digits': 'fractionDigits','name': 'name','numeric_code': 'numericCode',
     }
 
     
     _currency_code = None
     _fraction_digits = None
+    _name = None
     _numeric_code = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.currency_code = kwargs.get('currency_code', None)
         self.fraction_digits = kwargs.get('fraction_digits', None)
+        self.name = kwargs.get('name', None)
         self.numeric_code = kwargs.get('numeric_code', None)
         
 
     
     @property
     def currency_code(self):
         """Gets the currency_code of this RestCurrency.
 
-            The currency code identifies the currency with the three char long ISO 4217 code (e.g. USD, CHF, EUR).
+            The currency's three-letter code (ISO 4217 format).
 
         :return: The currency_code of this RestCurrency.
         :rtype: str
         """
         return self._currency_code
 
     @currency_code.setter
     def currency_code(self, currency_code):
         """Sets the currency_code of this RestCurrency.
 
-            The currency code identifies the currency with the three char long ISO 4217 code (e.g. USD, CHF, EUR).
+            The currency's three-letter code (ISO 4217 format).
 
         :param currency_code: The currency_code of this RestCurrency.
         :type: str
         """
 
         self._currency_code = currency_code
     
     @property
     def fraction_digits(self):
         """Gets the fraction_digits of this RestCurrency.
 
-            The fraction digits indicates how many places the currency has. This also indicates with which precision we calculate internally when we do calculations with this currency.
+            The currency's number of decimals. When calculating amounts in this currency, the fraction digits determine the accuracy.
 
         :return: The fraction_digits of this RestCurrency.
         :rtype: int
         """
         return self._fraction_digits
 
     @fraction_digits.setter
     def fraction_digits(self, fraction_digits):
         """Sets the fraction_digits of this RestCurrency.
 
-            The fraction digits indicates how many places the currency has. This also indicates with which precision we calculate internally when we do calculations with this currency.
+            The currency's number of decimals. When calculating amounts in this currency, the fraction digits determine the accuracy.
 
         :param fraction_digits: The fraction_digits of this RestCurrency.
         :type: int
         """
 
         self._fraction_digits = fraction_digits
     
     @property
+    def name(self):
+        """Gets the name of this RestCurrency.
+
+            The name of the currency.
+
+        :return: The name of this RestCurrency.
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this RestCurrency.
+
+            The name of the currency.
+
+        :param name: The name of this RestCurrency.
+        :type: str
+        """
+
+        self._name = name
+    
+    @property
     def numeric_code(self):
         """Gets the numeric_code of this RestCurrency.
 
-            The numeric code identifies the currency with the three digit long ISO 4217 code (e.g. 978, 756, 840).
+            The currency's three-digit code (ISO 4217 format).
 
         :return: The numeric_code of this RestCurrency.
         :rtype: int
         """
         return self._numeric_code
 
     @numeric_code.setter
     def numeric_code(self, numeric_code):
         """Sets the numeric_code of this RestCurrency.
 
-            The numeric code identifies the currency with the three digit long ISO 4217 code (e.g. 978, 756, 840).
+            The currency's three-digit code (ISO 4217 format).
 
         :param numeric_code: The numeric_code of this RestCurrency.
         :type: int
         """
 
         self._numeric_code = numeric_code
```

### Comparing `wallee-3.4.0/wallee/models/rest_language.py` & `wallee-4.0.0/wallee/models/rest_language.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,173 +9,199 @@
 
     swagger_types = {
     
         'country_code': 'str',
         'ietf_code': 'str',
         'iso2_code': 'str',
         'iso3_code': 'str',
+        'name': 'str',
         'plural_expression': 'str',
         'primary_of_group': 'bool',
     }
 
     attribute_map = {
-        'country_code': 'countryCode','ietf_code': 'ietfCode','iso2_code': 'iso2Code','iso3_code': 'iso3Code','plural_expression': 'pluralExpression','primary_of_group': 'primaryOfGroup',
+        'country_code': 'countryCode','ietf_code': 'ietfCode','iso2_code': 'iso2Code','iso3_code': 'iso3Code','name': 'name','plural_expression': 'pluralExpression','primary_of_group': 'primaryOfGroup',
     }
 
     
     _country_code = None
     _ietf_code = None
     _iso2_code = None
     _iso3_code = None
+    _name = None
     _plural_expression = None
     _primary_of_group = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
         self.country_code = kwargs.get('country_code', None)
         self.ietf_code = kwargs.get('ietf_code', None)
         self.iso2_code = kwargs.get('iso2_code', None)
         self.iso3_code = kwargs.get('iso3_code', None)
+        self.name = kwargs.get('name', None)
         self.plural_expression = kwargs.get('plural_expression', None)
         self.primary_of_group = kwargs.get('primary_of_group', None)
         
 
     
     @property
     def country_code(self):
         """Gets the country_code of this RestLanguage.
 
-            The country code represents the region of the language as a 2 letter ISO code.
+            The two-letter code of the language's region (ISO 3166-1 alpha-2 format).
 
         :return: The country_code of this RestLanguage.
         :rtype: str
         """
         return self._country_code
 
     @country_code.setter
     def country_code(self, country_code):
         """Sets the country_code of this RestLanguage.
 
-            The country code represents the region of the language as a 2 letter ISO code.
+            The two-letter code of the language's region (ISO 3166-1 alpha-2 format).
 
         :param country_code: The country_code of this RestLanguage.
         :type: str
         """
 
         self._country_code = country_code
     
     @property
     def ietf_code(self):
         """Gets the ietf_code of this RestLanguage.
 
-            The IETF code represents the language as the two letter ISO code including the region (e.g. en-US).
+            The language's IETF tag consisting of the two-letter ISO code and region e.g. en-US, de-CH.
 
         :return: The ietf_code of this RestLanguage.
         :rtype: str
         """
         return self._ietf_code
 
     @ietf_code.setter
     def ietf_code(self, ietf_code):
         """Sets the ietf_code of this RestLanguage.
 
-            The IETF code represents the language as the two letter ISO code including the region (e.g. en-US).
+            The language's IETF tag consisting of the two-letter ISO code and region e.g. en-US, de-CH.
 
         :param ietf_code: The ietf_code of this RestLanguage.
         :type: str
         """
 
         self._ietf_code = ietf_code
     
     @property
     def iso2_code(self):
         """Gets the iso2_code of this RestLanguage.
 
-            The ISO 2 letter code represents the language with two letters.
+            The language's two-letter code (ISO 639-1 format).
 
         :return: The iso2_code of this RestLanguage.
         :rtype: str
         """
         return self._iso2_code
 
     @iso2_code.setter
     def iso2_code(self, iso2_code):
         """Sets the iso2_code of this RestLanguage.
 
-            The ISO 2 letter code represents the language with two letters.
+            The language's two-letter code (ISO 639-1 format).
 
         :param iso2_code: The iso2_code of this RestLanguage.
         :type: str
         """
 
         self._iso2_code = iso2_code
     
     @property
     def iso3_code(self):
         """Gets the iso3_code of this RestLanguage.
 
-            The ISO 3 letter code represents the language with three letters.
+            The language's three-letter code (ISO 639-2/T format).
 
         :return: The iso3_code of this RestLanguage.
         :rtype: str
         """
         return self._iso3_code
 
     @iso3_code.setter
     def iso3_code(self, iso3_code):
         """Sets the iso3_code of this RestLanguage.
 
-            The ISO 3 letter code represents the language with three letters.
+            The language's three-letter code (ISO 639-2/T format).
 
         :param iso3_code: The iso3_code of this RestLanguage.
         :type: str
         """
 
         self._iso3_code = iso3_code
     
     @property
+    def name(self):
+        """Gets the name of this RestLanguage.
+
+            The name of the language.
+
+        :return: The name of this RestLanguage.
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this RestLanguage.
+
+            The name of the language.
+
+        :param name: The name of this RestLanguage.
+        :type: str
+        """
+
+        self._name = name
+    
+    @property
     def plural_expression(self):
         """Gets the plural_expression of this RestLanguage.
 
-            The plural expression defines how to map a plural into the language index. This expression is used to determine the plural form for the translations.
+            The expression to determine the plural index for a given number of items used to find the proper plural form for translations.
 
         :return: The plural_expression of this RestLanguage.
         :rtype: str
         """
         return self._plural_expression
 
     @plural_expression.setter
     def plural_expression(self, plural_expression):
         """Sets the plural_expression of this RestLanguage.
 
-            The plural expression defines how to map a plural into the language index. This expression is used to determine the plural form for the translations.
+            The expression to determine the plural index for a given number of items used to find the proper plural form for translations.
 
         :param plural_expression: The plural_expression of this RestLanguage.
         :type: str
         """
 
         self._plural_expression = plural_expression
     
     @property
     def primary_of_group(self):
         """Gets the primary_of_group of this RestLanguage.
 
-            The primary language of a group indicates whether a language is the primary language of a group of languages. The group is determine by the ISO 2 letter code.
+            Whether this is the primary language in a group of languages.
 
         :return: The primary_of_group of this RestLanguage.
         :rtype: bool
         """
         return self._primary_of_group
 
     @primary_of_group.setter
     def primary_of_group(self, primary_of_group):
         """Sets the primary_of_group of this RestLanguage.
 
-            The primary language of a group indicates whether a language is the primary language of a group of languages. The group is determine by the ISO 2 letter code.
+            Whether this is the primary language in a group of languages.
 
         :param primary_of_group: The primary_of_group of this RestLanguage.
         :type: bool
         """
 
         self._primary_of_group = primary_of_group
```

### Comparing `wallee-3.4.0/wallee/models/role.py` & `wallee-4.0.0/wallee/models/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Role:
 
     swagger_types = {
     
         'account': 'Account',
         'id': 'int',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'permissions': 'list[Permission]',
         'planned_purge_date': 'datetime',
         'state': 'RoleState',
         'two_factor_required': 'bool',
         'version': 'int',
     }
 
@@ -47,26 +47,26 @@
         
 
     
     @property
     def account(self):
         """Gets the account of this Role.
 
-            The account to which this role belongs to. This role can only be assigned within the assigned account and the sub accounts of the assigned account.
+            The account the role belongs to. The role can only be assigned within this account.
 
         :return: The account of this Role.
         :rtype: Account
         """
         return self._account
 
     @account.setter
     def account(self, account):
         """Sets the account of this Role.
 
-            The account to which this role belongs to. This role can only be assigned within the assigned account and the sub accounts of the assigned account.
+            The account the role belongs to. The role can only be assigned within this account.
 
         :param account: The account of this Role.
         :type: Account
         """
 
         self._account = account
     
@@ -93,49 +93,49 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this Role.
 
-            The name of this role is used to identify the role within administrative interfaces.
+            The name used to identify the role.
 
         :return: The name of this Role.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Role.
 
-            The name of this role is used to identify the role within administrative interfaces.
+            The name used to identify the role.
 
         :param name: The name of this Role.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def permissions(self):
         """Gets the permissions of this Role.
 
-            Set of permissions that are granted to this role.
+            The permissions granted to users with this role.
 
         :return: The permissions of this Role.
         :rtype: list[Permission]
         """
         return self._permissions
 
     @permissions.setter
     def permissions(self, permissions):
         """Sets the permissions of this Role.
 
-            Set of permissions that are granted to this role.
+            The permissions granted to users with this role.
 
         :param permissions: The permissions of this Role.
         :type: list[Permission]
         """
 
         self._permissions = permissions
     
@@ -185,26 +185,26 @@
 
         self._state = state
     
     @property
     def two_factor_required(self):
         """Gets the two_factor_required of this Role.
 
-            Defines whether having been granted this role will force a user to use two-factor authentication.
+            Whether users with this role are required to use two-factor authentication.
 
         :return: The two_factor_required of this Role.
         :rtype: bool
         """
         return self._two_factor_required
 
     @two_factor_required.setter
     def two_factor_required(self, two_factor_required):
         """Sets the two_factor_required of this Role.
 
-            Defines whether having been granted this role will force a user to use two-factor authentication.
+            Whether users with this role are required to use two-factor authentication.
 
         :param two_factor_required: The two_factor_required of this Role.
         :type: bool
         """
 
         self._two_factor_required = two_factor_required
```

### Comparing `wallee-3.4.0/wallee/models/sales_channel.py` & `wallee-4.0.0/wallee/models/sales_channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this SalesChannel.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this SalesChannel.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this SalesChannel.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this SalesChannel.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -110,26 +110,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this SalesChannel.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this SalesChannel.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SalesChannel.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this SalesChannel.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/scope.py` & `wallee-4.0.0/wallee/models/scope.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,51 +59,51 @@
         
 
     
     @property
     def domain_name(self):
         """Gets the domain_name of this Scope.
 
-            The domain name to which this scope is mapped to.
+            The domain name that belongs to the scope.
 
         :return: The domain_name of this Scope.
         :rtype: str
         """
         return self._domain_name
 
     @domain_name.setter
     def domain_name(self, domain_name):
         """Sets the domain_name of this Scope.
 
-            The domain name to which this scope is mapped to.
+            The domain name that belongs to the scope.
 
         :param domain_name: The domain_name of this Scope.
         :type: str
         """
         if domain_name is not None and len(domain_name) > 40:
             raise ValueError("Invalid value for `domain_name`, length must be less than or equal to `40`")
 
         self._domain_name = domain_name
     
     @property
     def features(self):
         """Gets the features of this Scope.
 
-            
+            The list of features that are active in the scope.
 
         :return: The features of this Scope.
         :rtype: list[Feature]
         """
         return self._features
 
     @features.setter
     def features(self, features):
         """Sets the features of this Scope.
 
-            
+            The list of features that are active in the scope.
 
         :param features: The features of this Scope.
         :type: list[Feature]
         """
 
         self._features = features
     
@@ -130,51 +130,51 @@
 
         self._id = id
     
     @property
     def machine_name(self):
         """Gets the machine_name of this Scope.
 
-            
+            The name identifying the scope in e.g. URLs.
 
         :return: The machine_name of this Scope.
         :rtype: str
         """
         return self._machine_name
 
     @machine_name.setter
     def machine_name(self, machine_name):
         """Sets the machine_name of this Scope.
 
-            
+            The name identifying the scope in e.g. URLs.
 
         :param machine_name: The machine_name of this Scope.
         :type: str
         """
         if machine_name is not None and len(machine_name) > 50:
             raise ValueError("Invalid value for `machine_name`, length must be less than or equal to `50`")
 
         self._machine_name = machine_name
     
     @property
     def name(self):
         """Gets the name of this Scope.
 
-            The name of the scope is shown to the user where the user should select a scope.
+            The name used to identify the scope.
 
         :return: The name of this Scope.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Scope.
 
-            The name of the scope is shown to the user where the user should select a scope.
+            The name used to identify the scope.
 
         :param name: The name of this Scope.
         :type: str
         """
         if name is not None and len(name) > 50:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")
 
@@ -203,49 +203,49 @@
 
         self._planned_purge_date = planned_purge_date
     
     @property
     def port(self):
         """Gets the port of this Scope.
 
-            The port number to which this scope is mapped to.
+            The port where the scope can be accessed.
 
         :return: The port of this Scope.
         :rtype: int
         """
         return self._port
 
     @port.setter
     def port(self, port):
         """Sets the port of this Scope.
 
-            The port number to which this scope is mapped to.
+            The port where the scope can be accessed.
 
         :param port: The port of this Scope.
         :type: int
         """
 
         self._port = port
     
     @property
     def ssl_active(self):
         """Gets the ssl_active of this Scope.
 
-            Define whether the scope supports SSL.
+            Whether the scope supports SSL.
 
         :return: The ssl_active of this Scope.
         :rtype: bool
         """
         return self._ssl_active
 
     @ssl_active.setter
     def ssl_active(self, ssl_active):
         """Sets the ssl_active of this Scope.
 
-            Define whether the scope supports SSL.
+            Whether the scope supports SSL.
 
         :param ssl_active: The ssl_active of this Scope.
         :type: bool
         """
 
         self._ssl_active = ssl_active
     
@@ -272,49 +272,49 @@
 
         self._state = state
     
     @property
     def themes(self):
         """Gets the themes of this Scope.
 
-            The themes determines how the application layout, look and feel is. By providing multiple themes you can fallback to other themes.
+            The themes that determine the look and feel of the scope's user interface. A fall-through strategy is applied when building the actual theme.
 
         :return: The themes of this Scope.
         :rtype: list[str]
         """
         return self._themes
 
     @themes.setter
     def themes(self, themes):
         """Sets the themes of this Scope.
 
-            The themes determines how the application layout, look and feel is. By providing multiple themes you can fallback to other themes.
+            The themes that determine the look and feel of the scope's user interface. A fall-through strategy is applied when building the actual theme.
 
         :param themes: The themes of this Scope.
         :type: list[str]
         """
 
         self._themes = themes
     
     @property
     def url(self):
         """Gets the url of this Scope.
 
-            
+            The URL where the scope can be accessed.
 
         :return: The url of this Scope.
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """Sets the url of this Scope.
 
-            
+            The URL where the scope can be accessed.
 
         :param url: The url of this Scope.
         :type: str
         """
 
         self._url = url
```

### Comparing `wallee-3.4.0/wallee/models/server_error.py` & `wallee-4.0.0/wallee/models/server_error.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_integration.py` & `wallee-4.0.0/wallee/models/shopify_integration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_recurring_order.py` & `wallee-4.0.0/wallee/models/shopify_recurring_order.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_recurring_order_update_request.py` & `wallee-4.0.0/wallee/models/shopify_recurring_order_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscriber.py` & `wallee-4.0.0/wallee/models/shopify_subscriber.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscriber_active.py` & `wallee-4.0.0/wallee/models/shopify_subscriber_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscriber_creation.py` & `wallee-4.0.0/wallee/models/shopify_subscriber_creation.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription.py` & `wallee-4.0.0/wallee/models/shopify_subscription.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_address.py` & `wallee-4.0.0/wallee/models/shopify_subscription_address.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_address_create.py` & `wallee-4.0.0/wallee/models/shopify_subscription_address_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,485 +83,485 @@
         
 
     
     @property
     def city(self):
         """Gets the city of this ShopifySubscriptionAddressCreate.
 
-            
+            The city, town or village.
 
         :return: The city of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
         """Sets the city of this ShopifySubscriptionAddressCreate.
 
-            
+            The city, town or village.
 
         :param city: The city of this ShopifySubscriptionAddressCreate.
         :type: str
         """
 
         self._city = city
     
     @property
     def commercial_register_number(self):
         """Gets the commercial_register_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The commercial registration number of the organization.
 
         :return: The commercial_register_number of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._commercial_register_number
 
     @commercial_register_number.setter
     def commercial_register_number(self, commercial_register_number):
         """Sets the commercial_register_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The commercial registration number of the organization.
 
         :param commercial_register_number: The commercial_register_number of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if commercial_register_number is not None and len(commercial_register_number) > 100:
             raise ValueError("Invalid value for `commercial_register_number`, length must be less than or equal to `100`")
 
         self._commercial_register_number = commercial_register_number
     
     @property
     def country(self):
         """Gets the country of this ShopifySubscriptionAddressCreate.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :return: The country of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
         """Sets the country of this ShopifySubscriptionAddressCreate.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :param country: The country of this ShopifySubscriptionAddressCreate.
         :type: str
         """
 
         self._country = country
     
     @property
     def date_of_birth(self):
         """Gets the date_of_birth of this ShopifySubscriptionAddressCreate.
 
-            
+            The date of birth.
 
         :return: The date_of_birth of this ShopifySubscriptionAddressCreate.
         :rtype: date
         """
         return self._date_of_birth
 
     @date_of_birth.setter
     def date_of_birth(self, date_of_birth):
         """Sets the date_of_birth of this ShopifySubscriptionAddressCreate.
 
-            
+            The date of birth.
 
         :param date_of_birth: The date_of_birth of this ShopifySubscriptionAddressCreate.
         :type: date
         """
 
         self._date_of_birth = date_of_birth
     
     @property
     def dependent_locality(self):
         """Gets the dependent_locality of this ShopifySubscriptionAddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :return: The dependent_locality of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
         """Sets the dependent_locality of this ShopifySubscriptionAddressCreate.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :param dependent_locality: The dependent_locality of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
         """Gets the email_address of this ShopifySubscriptionAddressCreate.
 
-            
+            The email address.
 
         :return: The email_address of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this ShopifySubscriptionAddressCreate.
 
-            
+            The email address.
 
         :param email_address: The email_address of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if email_address is not None and len(email_address) > 254:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `254`")
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this ShopifySubscriptionAddressCreate.
 
-            
+            The family or last name.
 
         :return: The family_name of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this ShopifySubscriptionAddressCreate.
 
-            
+            The family or last name.
 
         :param family_name: The family_name of this ShopifySubscriptionAddressCreate.
         :type: str
         """
 
         self._family_name = family_name
     
     @property
     def gender(self):
         """Gets the gender of this ShopifySubscriptionAddressCreate.
 
-            
+            The gender.
 
         :return: The gender of this ShopifySubscriptionAddressCreate.
         :rtype: Gender
         """
         return self._gender
 
     @gender.setter
     def gender(self, gender):
         """Sets the gender of this ShopifySubscriptionAddressCreate.
 
-            
+            The gender.
 
         :param gender: The gender of this ShopifySubscriptionAddressCreate.
         :type: Gender
         """
 
         self._gender = gender
     
     @property
     def given_name(self):
         """Gets the given_name of this ShopifySubscriptionAddressCreate.
 
-            
+            The given or first name.
 
         :return: The given_name of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this ShopifySubscriptionAddressCreate.
 
-            
+            The given or first name.
 
         :param given_name: The given_name of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
         self._given_name = given_name
     
     @property
     def legal_organization_form(self):
         """Gets the legal_organization_form of this ShopifySubscriptionAddressCreate.
 
-            
+            The legal form of the organization.
 
         :return: The legal_organization_form of this ShopifySubscriptionAddressCreate.
         :rtype: int
         """
         return self._legal_organization_form
 
     @legal_organization_form.setter
     def legal_organization_form(self, legal_organization_form):
         """Sets the legal_organization_form of this ShopifySubscriptionAddressCreate.
 
-            
+            The legal form of the organization.
 
         :param legal_organization_form: The legal_organization_form of this ShopifySubscriptionAddressCreate.
         :type: int
         """
 
         self._legal_organization_form = legal_organization_form
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The phone number of a mobile phone.
 
         :return: The mobile_phone_number of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The phone number of a mobile phone.
 
         :param mobile_phone_number: The mobile_phone_number of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
         """Gets the organization_name of this ShopifySubscriptionAddressCreate.
 
-            
+            The organization's name.
 
         :return: The organization_name of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
         """Sets the organization_name of this ShopifySubscriptionAddressCreate.
 
-            
+            The organization's name.
 
         :param organization_name: The organization_name of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if organization_name is not None and len(organization_name) > 100:
             raise ValueError("Invalid value for `organization_name`, length must be less than or equal to `100`")
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
         """Gets the phone_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The phone number.
 
         :return: The phone_number of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
         """Sets the phone_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The phone number.
 
         :param phone_number: The phone_number of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if phone_number is not None and len(phone_number) > 100:
             raise ValueError("Invalid value for `phone_number`, length must be less than or equal to `100`")
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
         """Gets the postal_state of this ShopifySubscriptionAddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :return: The postal_state of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
         """Sets the postal_state of this ShopifySubscriptionAddressCreate.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :param postal_state: The postal_state of this ShopifySubscriptionAddressCreate.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
         """Gets the postcode of this ShopifySubscriptionAddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :return: The postcode of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
         """Sets the postcode of this ShopifySubscriptionAddressCreate.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :param postcode: The postcode of this ShopifySubscriptionAddressCreate.
         :type: str
         """
 
         self._postcode = postcode
     
     @property
     def sales_tax_number(self):
         """Gets the sales_tax_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The sales tax number of the organization.
 
         :return: The sales_tax_number of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._sales_tax_number
 
     @sales_tax_number.setter
     def sales_tax_number(self, sales_tax_number):
         """Sets the sales_tax_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The sales tax number of the organization.
 
         :param sales_tax_number: The sales_tax_number of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if sales_tax_number is not None and len(sales_tax_number) > 100:
             raise ValueError("Invalid value for `sales_tax_number`, length must be less than or equal to `100`")
 
         self._sales_tax_number = sales_tax_number
     
     @property
     def salutation(self):
         """Gets the salutation of this ShopifySubscriptionAddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :return: The salutation of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
         """Sets the salutation of this ShopifySubscriptionAddressCreate.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :param salutation: The salutation of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
     def social_security_number(self):
         """Gets the social_security_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The social security number.
 
         :return: The social_security_number of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._social_security_number
 
     @social_security_number.setter
     def social_security_number(self, social_security_number):
         """Sets the social_security_number of this ShopifySubscriptionAddressCreate.
 
-            
+            The social security number.
 
         :param social_security_number: The social_security_number of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if social_security_number is not None and len(social_security_number) > 100:
             raise ValueError("Invalid value for `social_security_number`, length must be less than or equal to `100`")
 
         self._social_security_number = social_security_number
     
     @property
     def sorting_code(self):
         """Gets the sorting_code of this ShopifySubscriptionAddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :return: The sorting_code of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
         """Sets the sorting_code of this ShopifySubscriptionAddressCreate.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :param sorting_code: The sorting_code of this ShopifySubscriptionAddressCreate.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
         """Gets the street of this ShopifySubscriptionAddressCreate.
 
-            
+            The street or PO Box.
 
         :return: The street of this ShopifySubscriptionAddressCreate.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
         """Sets the street of this ShopifySubscriptionAddressCreate.
 
-            
+            The street or PO Box.
 
         :param street: The street of this ShopifySubscriptionAddressCreate.
         :type: str
         """
 
         self._street = street
```

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_creation_request.py` & `wallee-4.0.0/wallee/models/shopify_subscription_creation_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_model_billing_configuration.py` & `wallee-4.0.0/wallee/models/shopify_subscription_model_billing_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_model_item.py` & `wallee-4.0.0/wallee/models/shopify_subscription_model_item.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_model_tax_line.py` & `wallee-4.0.0/wallee/models/shopify_subscription_model_tax_line.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_product.py` & `wallee-4.0.0/wallee/models/shopify_subscription_product.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_product_create.py` & `wallee-4.0.0/wallee/models/shopify_subscription_product_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_product_update.py` & `wallee-4.0.0/wallee/models/shopify_subscription_product_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_suspension.py` & `wallee-4.0.0/wallee/models/shopify_subscription_suspension.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_suspension_create.py` & `wallee-4.0.0/wallee/models/shopify_subscription_suspension_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_update_addresses_request.py` & `wallee-4.0.0/wallee/models/shopify_subscription_update_addresses_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_update_request.py` & `wallee-4.0.0/wallee/models/shopify_subscription_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_version.py` & `wallee-4.0.0/wallee/models/shopify_subscription_version.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_subscription_version_item.py` & `wallee-4.0.0/wallee/models/shopify_subscription_version_item.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_tax_line.py` & `wallee-4.0.0/wallee/models/shopify_tax_line.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/shopify_transaction.py` & `wallee-4.0.0/wallee/models/shopify_transaction.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/space.py` & `wallee-4.0.0/wallee/models/space.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,187 +83,187 @@
         
 
     
     @property
     def account(self):
         """Gets the account of this Space.
 
-            The account to which the space belongs to.
+            The account that the space belongs to.
 
         :return: The account of this Space.
         :rtype: Account
         """
         return self._account
 
     @account.setter
     def account(self, account):
         """Sets the account of this Space.
 
-            The account to which the space belongs to.
+            The account that the space belongs to.
 
         :param account: The account of this Space.
         :type: Account
         """
 
         self._account = account
     
     @property
     def active(self):
         """Gets the active of this Space.
 
-            Active means that this account and all accounts in the hierarchy are active.
+            Whether this space and all its parent accounts are active.
 
         :return: The active of this Space.
         :rtype: bool
         """
         return self._active
 
     @active.setter
     def active(self, active):
         """Sets the active of this Space.
 
-            Active means that this account and all accounts in the hierarchy are active.
+            Whether this space and all its parent accounts are active.
 
         :param active: The active of this Space.
         :type: bool
         """
 
         self._active = active
     
     @property
     def active_or_restricted_active(self):
         """Gets the active_or_restricted_active of this Space.
 
-            This property is true when all accounts in the hierarchy are active or restricted active.
+            Whether this space and all its parent accounts are active or restricted active.
 
         :return: The active_or_restricted_active of this Space.
         :rtype: bool
         """
         return self._active_or_restricted_active
 
     @active_or_restricted_active.setter
     def active_or_restricted_active(self, active_or_restricted_active):
         """Sets the active_or_restricted_active of this Space.
 
-            This property is true when all accounts in the hierarchy are active or restricted active.
+            Whether this space and all its parent accounts are active or restricted active.
 
         :param active_or_restricted_active: The active_or_restricted_active of this Space.
         :type: bool
         """
 
         self._active_or_restricted_active = active_or_restricted_active
     
     @property
     def created_by(self):
         """Gets the created_by of this Space.
 
-            The ID of the user who created this entity.
+            The ID of the user the space was created by.
 
         :return: The created_by of this Space.
         :rtype: int
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this Space.
 
-            The ID of the user who created this entity.
+            The ID of the user the space was created by.
 
         :param created_by: The created_by of this Space.
         :type: int
         """
 
         self._created_by = created_by
     
     @property
     def created_on(self):
         """Gets the created_on of this Space.
 
-            The date and time when this entity was created.
+            The date and time when the space was created.
 
         :return: The created_on of this Space.
         :rtype: datetime
         """
         return self._created_on
 
     @created_on.setter
     def created_on(self, created_on):
         """Sets the created_on of this Space.
 
-            The date and time when this entity was created.
+            The date and time when the space was created.
 
         :param created_on: The created_on of this Space.
         :type: datetime
         """
 
         self._created_on = created_on
     
     @property
     def database(self):
         """Gets the database of this Space.
 
-            The database in which the space's data are stored in.
+            The database the space is connected to and that holds the space's data.
 
         :return: The database of this Space.
         :rtype: TenantDatabase
         """
         return self._database
 
     @database.setter
     def database(self, database):
         """Sets the database of this Space.
 
-            The database in which the space's data are stored in.
+            The database the space is connected to and that holds the space's data.
 
         :param database: The database of this Space.
         :type: TenantDatabase
         """
 
         self._database = database
     
     @property
     def deleted_by(self):
         """Gets the deleted_by of this Space.
 
-            The ID of a user that deleted this entity.
+            The ID of the user the space was deleted by.
 
         :return: The deleted_by of this Space.
         :rtype: int
         """
         return self._deleted_by
 
     @deleted_by.setter
     def deleted_by(self, deleted_by):
         """Sets the deleted_by of this Space.
 
-            The ID of a user that deleted this entity.
+            The ID of the user the space was deleted by.
 
         :param deleted_by: The deleted_by of this Space.
         :type: int
         """
 
         self._deleted_by = deleted_by
     
     @property
     def deleted_on(self):
         """Gets the deleted_on of this Space.
 
-            The date and time when this entity was deleted.
+            The date and time when the space was deleted.
 
         :return: The deleted_on of this Space.
         :rtype: datetime
         """
         return self._deleted_on
 
     @deleted_on.setter
     def deleted_on(self, deleted_on):
         """Sets the deleted_on of this Space.
 
-            The date and time when this entity was deleted.
+            The date and time when the space was deleted.
 
         :param deleted_on: The deleted_on of this Space.
         :type: datetime
         """
 
         self._deleted_on = deleted_on
     
@@ -313,26 +313,26 @@
 
         self._last_modified_date = last_modified_date
     
     @property
     def name(self):
         """Gets the name of this Space.
 
-            The space name is used internally to identify the space in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the space.
 
         :return: The name of this Space.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Space.
 
-            The space name is used internally to identify the space in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the space.
 
         :param name: The name of this Space.
         :type: str
         """
         if name is not None and len(name) > 200:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `200`")
         if name is not None and len(name) < 3:
@@ -363,95 +363,95 @@
 
         self._planned_purge_date = planned_purge_date
     
     @property
     def postal_address(self):
         """Gets the postal_address of this Space.
 
-            The address to use in communication with clients for example in email, documents etc.
+            The address that is used in communication with clients for example in emails, documents, etc.
 
         :return: The postal_address of this Space.
         :rtype: SpaceAddress
         """
         return self._postal_address
 
     @postal_address.setter
     def postal_address(self, postal_address):
         """Sets the postal_address of this Space.
 
-            The address to use in communication with clients for example in email, documents etc.
+            The address that is used in communication with clients for example in emails, documents, etc.
 
         :param postal_address: The postal_address of this Space.
         :type: SpaceAddress
         """
 
         self._postal_address = postal_address
     
     @property
     def primary_currency(self):
         """Gets the primary_currency of this Space.
 
-            This is the currency that is used to display aggregated amounts in the space.
+            The currency that is used to display aggregated amounts in the space.
 
         :return: The primary_currency of this Space.
         :rtype: str
         """
         return self._primary_currency
 
     @primary_currency.setter
     def primary_currency(self, primary_currency):
         """Sets the primary_currency of this Space.
 
-            This is the currency that is used to display aggregated amounts in the space.
+            The currency that is used to display aggregated amounts in the space.
 
         :param primary_currency: The primary_currency of this Space.
         :type: str
         """
 
         self._primary_currency = primary_currency
     
     @property
     def request_limit(self):
         """Gets the request_limit of this Space.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes for this space. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted within two minutes. This limit can only be changed with special privileges.
 
         :return: The request_limit of this Space.
         :rtype: int
         """
         return self._request_limit
 
     @request_limit.setter
     def request_limit(self, request_limit):
         """Sets the request_limit of this Space.
 
-            The request limit defines the maximum number of API request accepted within 2 minutes for this space. This limit can only be changed with special privileges.
+            The maximum number of API requests that are accepted within two minutes. This limit can only be changed with special privileges.
 
         :param request_limit: The request_limit of this Space.
         :type: int
         """
 
         self._request_limit = request_limit
     
     @property
     def restricted_active(self):
         """Gets the restricted_active of this Space.
 
-            Restricted active means that at least one account in the hierarchy is only restricted active, but all are either restricted active or active.
+            Whether this space and all its parent accounts are active or restricted active. There is least one parent account that is restricted active.
 
         :return: The restricted_active of this Space.
         :rtype: bool
         """
         return self._restricted_active
 
     @restricted_active.setter
     def restricted_active(self, restricted_active):
         """Sets the restricted_active of this Space.
 
-            Restricted active means that at least one account in the hierarchy is only restricted active, but all are either restricted active or active.
+            Whether this space and all its parent accounts are active or restricted active. There is least one parent account that is restricted active.
 
         :param restricted_active: The restricted_active of this Space.
         :type: bool
         """
 
         self._restricted_active = restricted_active
     
@@ -478,49 +478,49 @@
 
         self._state = state
     
     @property
     def technical_contact_addresses(self):
         """Gets the technical_contact_addresses of this Space.
 
-            The email address provided as contact addresses will be informed about technical issues or errors triggered by the space.
+            The email address that will receive messages about technical issues and errors that occur in the space.
 
         :return: The technical_contact_addresses of this Space.
         :rtype: list[str]
         """
         return self._technical_contact_addresses
 
     @technical_contact_addresses.setter
     def technical_contact_addresses(self, technical_contact_addresses):
         """Sets the technical_contact_addresses of this Space.
 
-            The email address provided as contact addresses will be informed about technical issues or errors triggered by the space.
+            The email address that will receive messages about technical issues and errors that occur in the space.
 
         :param technical_contact_addresses: The technical_contact_addresses of this Space.
         :type: list[str]
         """
 
         self._technical_contact_addresses = technical_contact_addresses
     
     @property
     def time_zone(self):
         """Gets the time_zone of this Space.
 
-            The time zone assigned to the space determines the time offset for calculating dates within the space. This is typically used for background processed which needs to be triggered on a specific hour within the day. Changing the space time zone will not change the display of dates.
+            The time zone that is used to schedule and run background processes. This does not affect the formatting of dates in the user interface.
 
         :return: The time_zone of this Space.
         :rtype: str
         """
         return self._time_zone
 
     @time_zone.setter
     def time_zone(self, time_zone):
         """Sets the time_zone of this Space.
 
-            The time zone assigned to the space determines the time offset for calculating dates within the space. This is typically used for background processed which needs to be triggered on a specific hour within the day. Changing the space time zone will not change the display of dates.
+            The time zone that is used to schedule and run background processes. This does not affect the formatting of dates in the user interface.
 
         :param time_zone: The time_zone of this Space.
         :type: str
         """
 
         self._time_zone = time_zone
```

### Comparing `wallee-3.4.0/wallee/models/space_address.py` & `wallee-4.0.0/wallee/models/space_address.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,366 +68,366 @@
         
 
     
     @property
     def city(self):
         """Gets the city of this SpaceAddress.
 
-            
+            The city, town or village.
 
         :return: The city of this SpaceAddress.
         :rtype: str
         """
         return self._city
 
     @city.setter
     def city(self, city):
         """Sets the city of this SpaceAddress.
 
-            
+            The city, town or village.
 
         :param city: The city of this SpaceAddress.
         :type: str
         """
 
         self._city = city
     
     @property
     def country(self):
         """Gets the country of this SpaceAddress.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :return: The country of this SpaceAddress.
         :rtype: str
         """
         return self._country
 
     @country.setter
     def country(self, country):
         """Sets the country of this SpaceAddress.
 
-            
+            The two-letter country code (ISO 3166 format).
 
         :param country: The country of this SpaceAddress.
         :type: str
         """
 
         self._country = country
     
     @property
     def dependent_locality(self):
         """Gets the dependent_locality of this SpaceAddress.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :return: The dependent_locality of this SpaceAddress.
         :rtype: str
         """
         return self._dependent_locality
 
     @dependent_locality.setter
     def dependent_locality(self, dependent_locality):
         """Sets the dependent_locality of this SpaceAddress.
 
-            
+            The dependent locality which is a sub-division of the state.
 
         :param dependent_locality: The dependent_locality of this SpaceAddress.
         :type: str
         """
         if dependent_locality is not None and len(dependent_locality) > 100:
             raise ValueError("Invalid value for `dependent_locality`, length must be less than or equal to `100`")
 
         self._dependent_locality = dependent_locality
     
     @property
     def email_address(self):
         """Gets the email_address of this SpaceAddress.
 
-            The email address is used within emails and as reply to address.
+            The email address used for communication with clients.
 
         :return: The email_address of this SpaceAddress.
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this SpaceAddress.
 
-            The email address is used within emails and as reply to address.
+            The email address used for communication with clients.
 
         :param email_address: The email_address of this SpaceAddress.
         :type: str
         """
 
         self._email_address = email_address
     
     @property
     def family_name(self):
         """Gets the family_name of this SpaceAddress.
 
-            
+            The family or last name.
 
         :return: The family_name of this SpaceAddress.
         :rtype: str
         """
         return self._family_name
 
     @family_name.setter
     def family_name(self, family_name):
         """Sets the family_name of this SpaceAddress.
 
-            
+            The family or last name.
 
         :param family_name: The family_name of this SpaceAddress.
         :type: str
         """
         if family_name is not None and len(family_name) > 100:
             raise ValueError("Invalid value for `family_name`, length must be less than or equal to `100`")
 
         self._family_name = family_name
     
     @property
     def given_name(self):
         """Gets the given_name of this SpaceAddress.
 
-            
+            The given or first name.
 
         :return: The given_name of this SpaceAddress.
         :rtype: str
         """
         return self._given_name
 
     @given_name.setter
     def given_name(self, given_name):
         """Sets the given_name of this SpaceAddress.
 
-            
+            The given or first name.
 
         :param given_name: The given_name of this SpaceAddress.
         :type: str
         """
         if given_name is not None and len(given_name) > 100:
             raise ValueError("Invalid value for `given_name`, length must be less than or equal to `100`")
 
         self._given_name = given_name
     
     @property
     def mobile_phone_number(self):
         """Gets the mobile_phone_number of this SpaceAddress.
 
-            
+            The phone number of a mobile phone.
 
         :return: The mobile_phone_number of this SpaceAddress.
         :rtype: str
         """
         return self._mobile_phone_number
 
     @mobile_phone_number.setter
     def mobile_phone_number(self, mobile_phone_number):
         """Sets the mobile_phone_number of this SpaceAddress.
 
-            
+            The phone number of a mobile phone.
 
         :param mobile_phone_number: The mobile_phone_number of this SpaceAddress.
         :type: str
         """
         if mobile_phone_number is not None and len(mobile_phone_number) > 100:
             raise ValueError("Invalid value for `mobile_phone_number`, length must be less than or equal to `100`")
 
         self._mobile_phone_number = mobile_phone_number
     
     @property
     def organization_name(self):
         """Gets the organization_name of this SpaceAddress.
 
-            
+            The organization's name.
 
         :return: The organization_name of this SpaceAddress.
         :rtype: str
         """
         return self._organization_name
 
     @organization_name.setter
     def organization_name(self, organization_name):
         """Sets the organization_name of this SpaceAddress.
 
-            
+            The organization's name.
 
         :param organization_name: The organization_name of this SpaceAddress.
         :type: str
         """
         if organization_name is not None and len(organization_name) > 100:
             raise ValueError("Invalid value for `organization_name`, length must be less than or equal to `100`")
 
         self._organization_name = organization_name
     
     @property
     def phone_number(self):
         """Gets the phone_number of this SpaceAddress.
 
-            
+            The phone number.
 
         :return: The phone_number of this SpaceAddress.
         :rtype: str
         """
         return self._phone_number
 
     @phone_number.setter
     def phone_number(self, phone_number):
         """Sets the phone_number of this SpaceAddress.
 
-            
+            The phone number.
 
         :param phone_number: The phone_number of this SpaceAddress.
         :type: str
         """
         if phone_number is not None and len(phone_number) > 100:
             raise ValueError("Invalid value for `phone_number`, length must be less than or equal to `100`")
 
         self._phone_number = phone_number
     
     @property
     def postal_state(self):
         """Gets the postal_state of this SpaceAddress.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :return: The postal_state of this SpaceAddress.
         :rtype: str
         """
         return self._postal_state
 
     @postal_state.setter
     def postal_state(self, postal_state):
         """Sets the postal_state of this SpaceAddress.
 
-            
+            The name of the region, typically a state, county, province or prefecture.
 
         :param postal_state: The postal_state of this SpaceAddress.
         :type: str
         """
 
         self._postal_state = postal_state
     
     @property
     def postcode(self):
         """Gets the postcode of this SpaceAddress.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :return: The postcode of this SpaceAddress.
         :rtype: str
         """
         return self._postcode
 
     @postcode.setter
     def postcode(self, postcode):
         """Sets the postcode of this SpaceAddress.
 
-            
+            The postal code, also known as ZIP, postcode, etc.
 
         :param postcode: The postcode of this SpaceAddress.
         :type: str
         """
 
         self._postcode = postcode
     
     @property
     def sales_tax_number(self):
         """Gets the sales_tax_number of this SpaceAddress.
 
-            
+            The sales tax number of the organization.
 
         :return: The sales_tax_number of this SpaceAddress.
         :rtype: str
         """
         return self._sales_tax_number
 
     @sales_tax_number.setter
     def sales_tax_number(self, sales_tax_number):
         """Sets the sales_tax_number of this SpaceAddress.
 
-            
+            The sales tax number of the organization.
 
         :param sales_tax_number: The sales_tax_number of this SpaceAddress.
         :type: str
         """
         if sales_tax_number is not None and len(sales_tax_number) > 100:
             raise ValueError("Invalid value for `sales_tax_number`, length must be less than or equal to `100`")
 
         self._sales_tax_number = sales_tax_number
     
     @property
     def salutation(self):
         """Gets the salutation of this SpaceAddress.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :return: The salutation of this SpaceAddress.
         :rtype: str
         """
         return self._salutation
 
     @salutation.setter
     def salutation(self, salutation):
         """Sets the salutation of this SpaceAddress.
 
-            
+            The salutation e.g. Mrs, Mr, Dr.
 
         :param salutation: The salutation of this SpaceAddress.
         :type: str
         """
         if salutation is not None and len(salutation) > 20:
             raise ValueError("Invalid value for `salutation`, length must be less than or equal to `20`")
 
         self._salutation = salutation
     
     @property
     def sorting_code(self):
         """Gets the sorting_code of this SpaceAddress.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :return: The sorting_code of this SpaceAddress.
         :rtype: str
         """
         return self._sorting_code
 
     @sorting_code.setter
     def sorting_code(self, sorting_code):
         """Sets the sorting_code of this SpaceAddress.
 
-            The sorting code identifies the post office at which the post box is located in.
+            The sorting code identifying the post office where the PO Box is located.
 
         :param sorting_code: The sorting_code of this SpaceAddress.
         :type: str
         """
         if sorting_code is not None and len(sorting_code) > 100:
             raise ValueError("Invalid value for `sorting_code`, length must be less than or equal to `100`")
 
         self._sorting_code = sorting_code
     
     @property
     def street(self):
         """Gets the street of this SpaceAddress.
 
-            
+            The street or PO Box.
 
         :return: The street of this SpaceAddress.
         :rtype: str
         """
         return self._street
 
     @street.setter
     def street(self, street):
         """Sets the street of this SpaceAddress.
 
-            
+            The street or PO Box.
 
         :param street: The street of this SpaceAddress.
         :type: str
         """
 
         self._street = street
```

### Comparing `wallee-3.4.0/wallee/models/space_create.py` & `wallee-4.0.0/wallee/models/webhook_url_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,91 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractSpaceUpdate
+from . import AbstractWebhookUrlUpdate
 
 
-class SpaceCreate(AbstractSpaceUpdate):
+class WebhookUrlUpdate(AbstractWebhookUrlUpdate):
 
     swagger_types = {
     
-        'account': 'int',
+        'id': 'int',
+        'version': 'int',
     }
 
     attribute_map = {
-        'account': 'account',
+        'id': 'id','version': 'version',
     }
 
     
-    _account = None
+    _id = None
+    _version = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.account = kwargs.get('account')
+        self.id = kwargs.get('id')
+
+        self.version = kwargs.get('version')
 
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def account(self):
-        """Gets the account of this SpaceCreate.
+    def id(self):
+        """Gets the id of this WebhookUrlUpdate.
+
+            The ID is the primary key of the entity. The ID identifies the entity uniquely.
+
+        :return: The id of this WebhookUrlUpdate.
+        :rtype: int
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this WebhookUrlUpdate.
+
+            The ID is the primary key of the entity. The ID identifies the entity uniquely.
+
+        :param id: The id of this WebhookUrlUpdate.
+        :type: int
+        """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")
+
+        self._id = id
+    
+    @property
+    def version(self):
+        """Gets the version of this WebhookUrlUpdate.
 
-            The account to which the space belongs to.
+            The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :return: The account of this SpaceCreate.
+        :return: The version of this WebhookUrlUpdate.
         :rtype: int
         """
-        return self._account
+        return self._version
 
-    @account.setter
-    def account(self, account):
-        """Sets the account of this SpaceCreate.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this WebhookUrlUpdate.
 
-            The account to which the space belongs to.
+            The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :param account: The account of this SpaceCreate.
+        :param version: The version of this WebhookUrlUpdate.
         :type: int
         """
-        if account is None:
-            raise ValueError("Invalid value for `account`, must not be `None`")
+        if version is None:
+            raise ValueError("Invalid value for `version`, must not be `None`")
 
-        self._account = account
+        self._version = version
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -73,27 +102,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(SpaceCreate, dict):
+        if issubclass(WebhookUrlUpdate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, SpaceCreate):
+        if not isinstance(other, WebhookUrlUpdate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/space_reference.py` & `wallee-4.0.0/wallee/models/space_reference.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/space_update.py` & `wallee-4.0.0/wallee/models/space_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/space_view.py` & `wallee-4.0.0/wallee/models/space_view.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/static_value.py` & `wallee-4.0.0/wallee/models/static_value.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this StaticValue.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this StaticValue.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this StaticValue.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this StaticValue.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this StaticValue.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this StaticValue.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this StaticValue.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this StaticValue.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/subscriber.py` & `wallee-4.0.0/wallee/models/subscriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,26 +279,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def meta_data(self):
         """Gets the meta_data of this Subscriber.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this Subscriber.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this Subscriber.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this Subscriber.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/subscriber_active.py` & `wallee-4.0.0/wallee/models/subscriber_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscriber_create.py` & `wallee-4.0.0/wallee/models/token_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractSubscriberUpdate
+from . import AbstractTokenUpdate
 
 
-class SubscriberCreate(AbstractSubscriberUpdate):
+class TokenCreate(AbstractTokenUpdate):
 
     swagger_types = {
     
-        'state': 'CreationEntityState',
         'external_id': 'str',
+        'state': 'CreationEntityState',
     }
 
     attribute_map = {
-        'state': 'state','external_id': 'externalId',
+        'external_id': 'externalId','state': 'state',
     }
 
     
-    _state = None
     _external_id = None
+    _state = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.state = kwargs.get('state', None)
         self.external_id = kwargs.get('external_id')
 
+        self.state = kwargs.get('state', None)
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def state(self):
-        """Gets the state of this SubscriberCreate.
-
-            The object's current state.
-
-        :return: The state of this SubscriberCreate.
-        :rtype: CreationEntityState
-        """
-        return self._state
-
-    @state.setter
-    def state(self, state):
-        """Sets the state of this SubscriberCreate.
-
-            The object's current state.
-
-        :param state: The state of this SubscriberCreate.
-        :type: CreationEntityState
-        """
-
-        self._state = state
-    
-    @property
     def external_id(self):
-        """Gets the external_id of this SubscriberCreate.
+        """Gets the external_id of this TokenCreate.
 
             A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
 
-        :return: The external_id of this SubscriberCreate.
+        :return: The external_id of this TokenCreate.
         :rtype: str
         """
         return self._external_id
 
     @external_id.setter
     def external_id(self, external_id):
-        """Sets the external_id of this SubscriberCreate.
+        """Sets the external_id of this TokenCreate.
 
             A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
 
-        :param external_id: The external_id of this SubscriberCreate.
+        :param external_id: The external_id of this TokenCreate.
         :type: str
         """
         if external_id is None:
             raise ValueError("Invalid value for `external_id`, must not be `None`")
 
         self._external_id = external_id
     
+    @property
+    def state(self):
+        """Gets the state of this TokenCreate.
+
+            The object's current state.
+
+        :return: The state of this TokenCreate.
+        :rtype: CreationEntityState
+        """
+        return self._state
+
+    @state.setter
+    def state(self, state):
+        """Sets the state of this TokenCreate.
+
+            The object's current state.
+
+        :param state: The state of this TokenCreate.
+        :type: CreationEntityState
+        """
+
+        self._state = state
+    
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -99,27 +99,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(SubscriberCreate, dict):
+        if issubclass(TokenCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, SubscriberCreate):
+        if not isinstance(other, TokenCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/subscriber_update.py` & `wallee-4.0.0/wallee/models/subscriber_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,26 +250,26 @@
 
         self._language = language
     
     @property
     def meta_data(self):
         """Gets the meta_data of this SubscriberUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this SubscriberUpdate.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this SubscriberUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this SubscriberUpdate.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/subscription.py` & `wallee-4.0.0/wallee/models/subscription.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_affiliate.py` & `wallee-4.0.0/wallee/models/subscription_affiliate.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,26 +145,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def meta_data(self):
         """Gets the meta_data of this SubscriptionAffiliate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this SubscriptionAffiliate.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this SubscriptionAffiliate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this SubscriptionAffiliate.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/subscription_affiliate_create.py` & `wallee-4.0.0/wallee/models/subscription_affiliate_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_affiliate_deleted.py` & `wallee-4.0.0/wallee/models/subscription_affiliate_deleted.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_affiliate_deleting.py` & `wallee-4.0.0/wallee/models/subscription_affiliate_deleting.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_affiliate_inactive.py` & `wallee-4.0.0/wallee/models/subscription_affiliate_inactive.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_affiliate_update.py` & `wallee-4.0.0/wallee/models/subscription_affiliate_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,26 +116,26 @@
 
         self._language = language
     
     @property
     def meta_data(self):
         """Gets the meta_data of this SubscriptionAffiliateUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this SubscriptionAffiliateUpdate.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this SubscriptionAffiliateUpdate.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this SubscriptionAffiliateUpdate.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/subscription_change_request.py` & `wallee-4.0.0/wallee/models/subscription_change_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_charge.py` & `wallee-4.0.0/wallee/models/subscription_charge.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_charge_create.py` & `wallee-4.0.0/wallee/models/subscription_charge_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_component_configuration.py` & `wallee-4.0.0/wallee/models/subscription_component_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_component_reference_configuration.py` & `wallee-4.0.0/wallee/models/subscription_component_reference_configuration.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_create_request.py` & `wallee-4.0.0/wallee/models/subscription_create_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_ledger_entry.py` & `wallee-4.0.0/wallee/models/subscription_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_ledger_entry_create.py` & `wallee-4.0.0/wallee/models/subscription_ledger_entry_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_metric.py` & `wallee-4.0.0/wallee/models/subscription_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 
 
 class SubscriptionMetric:
 
     swagger_types = {
     
-        'description': 'DatabaseTranslatedString',
+        'description': 'dict(str, str)',
         'id': 'int',
         'linked_space_id': 'int',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'planned_purge_date': 'datetime',
         'state': 'CreationEntityState',
         'type': 'SubscriptionMetricType',
         'version': 'int',
     }
 
     attribute_map = {
@@ -50,26 +50,26 @@
     @property
     def description(self):
         """Gets the description of this SubscriptionMetric.
 
             
 
         :return: The description of this SubscriptionMetric.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this SubscriptionMetric.
 
             
 
         :param description: The description of this SubscriptionMetric.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
         """Gets the id of this SubscriptionMetric.
@@ -119,26 +119,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionMetric.
 
             
 
         :return: The name of this SubscriptionMetric.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionMetric.
 
             
 
         :param name: The name of this SubscriptionMetric.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def planned_purge_date(self):
         """Gets the planned_purge_date of this SubscriptionMetric.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_metric_active.py` & `wallee-4.0.0/wallee/models/subscription_metric_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_metric_create.py` & `wallee-4.0.0/wallee/models/subscription_metric_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_metric_type.py` & `wallee-4.0.0/wallee/models/subscription_metric_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this SubscriptionMetricType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this SubscriptionMetricType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this SubscriptionMetricType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this SubscriptionMetricType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this SubscriptionMetricType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this SubscriptionMetricType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionMetricType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this SubscriptionMetricType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/subscription_metric_update.py` & `wallee-4.0.0/wallee/models/subscription_metric_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class SubscriptionMetricUpdate:
 
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
-        'description': 'DatabaseTranslatedStringCreate',
-        'name': 'DatabaseTranslatedStringCreate',
+        'description': 'dict(str, str)',
+        'name': 'dict(str, str)',
     }
 
     attribute_map = {
         'id': 'id','version': 'version','description': 'description','name': 'name',
     }
 
     
@@ -90,49 +90,49 @@
     @property
     def description(self):
         """Gets the description of this SubscriptionMetricUpdate.
 
             
 
         :return: The description of this SubscriptionMetricUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this SubscriptionMetricUpdate.
 
             
 
         :param description: The description of this SubscriptionMetricUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def name(self):
         """Gets the name of this SubscriptionMetricUpdate.
 
             
 
         :return: The name of this SubscriptionMetricUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionMetricUpdate.
 
             
 
         :param name: The name of this SubscriptionMetricUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
 
     def to_dict(self):
         result = {}
```

### Comparing `wallee-3.4.0/wallee/models/subscription_metric_usage_report.py` & `wallee-4.0.0/wallee/models/subscription_metric_usage_report.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_metric_usage_report_create.py` & `wallee-4.0.0/wallee/models/subscription_metric_usage_report_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_pending.py` & `wallee-4.0.0/wallee/models/subscription_pending.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_period_bill.py` & `wallee-4.0.0/wallee/models/subscription_period_bill.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product.py` & `wallee-4.0.0/wallee/models/subscription_product.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product_active.py` & `wallee-4.0.0/wallee/models/webhook_listener_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractSubscriptionProductActive
+from . import AbstractWebhookListenerUpdate
 
 
-class SubscriptionProductActive(AbstractSubscriptionProductActive):
+class WebhookListenerUpdate(AbstractWebhookListenerUpdate):
 
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
     }
 
@@ -31,55 +31,55 @@
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
     def id(self):
-        """Gets the id of this SubscriptionProductActive.
+        """Gets the id of this WebhookListenerUpdate.
 
             The ID is the primary key of the entity. The ID identifies the entity uniquely.
 
-        :return: The id of this SubscriptionProductActive.
+        :return: The id of this WebhookListenerUpdate.
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this SubscriptionProductActive.
+        """Sets the id of this WebhookListenerUpdate.
 
             The ID is the primary key of the entity. The ID identifies the entity uniquely.
 
-        :param id: The id of this SubscriptionProductActive.
+        :param id: The id of this WebhookListenerUpdate.
         :type: int
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
     
     @property
     def version(self):
-        """Gets the version of this SubscriptionProductActive.
+        """Gets the version of this WebhookListenerUpdate.
 
             The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :return: The version of this SubscriptionProductActive.
+        :return: The version of this WebhookListenerUpdate.
         :rtype: int
         """
         return self._version
 
     @version.setter
     def version(self, version):
-        """Sets the version of this SubscriptionProductActive.
+        """Sets the version of this WebhookListenerUpdate.
 
             The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :param version: The version of this SubscriptionProductActive.
+        :param version: The version of this WebhookListenerUpdate.
         :type: int
         """
         if version is None:
             raise ValueError("Invalid value for `version`, must not be `None`")
 
         self._version = version
     
@@ -102,27 +102,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(SubscriptionProductActive, dict):
+        if issubclass(WebhookListenerUpdate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, SubscriptionProductActive):
+        if not isinstance(other, WebhookListenerUpdate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_component.py` & `wallee-4.0.0/wallee/models/subscription_product_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 class SubscriptionProductComponent:
 
     swagger_types = {
     
         'component_change_weight': 'int',
         'component_group': 'SubscriptionProductComponentGroup',
         'default_component': 'bool',
-        'description': 'DatabaseTranslatedString',
+        'description': 'dict(str, str)',
         'id': 'int',
         'linked_space_id': 'int',
         'maximal_quantity': 'float',
         'minimal_quantity': 'float',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'quantity_step': 'float',
         'reference': 'SubscriptionProductComponentReference',
         'sort_order': 'int',
         'tax_class': 'TaxClass',
         'version': 'int',
     }
 
@@ -137,26 +137,26 @@
     @property
     def description(self):
         """Gets the description of this SubscriptionProductComponent.
 
             The component description may contain a longer description which gives the subscriber a better understanding of what the component contains.
 
         :return: The description of this SubscriptionProductComponent.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this SubscriptionProductComponent.
 
             The component description may contain a longer description which gives the subscriber a better understanding of what the component contains.
 
         :param description: The description of this SubscriptionProductComponent.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def id(self):
         """Gets the id of this SubscriptionProductComponent.
@@ -252,26 +252,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionProductComponent.
 
             The component name is shown to the subscriber. It should describe in few words what the component does contain.
 
         :return: The name of this SubscriptionProductComponent.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionProductComponent.
 
             The component name is shown to the subscriber. It should describe in few words what the component does contain.
 
         :param name: The name of this SubscriptionProductComponent.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def quantity_step(self):
         """Gets the quantity_step of this SubscriptionProductComponent.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_component_group.py` & `wallee-4.0.0/wallee/models/subscription_product_component_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class SubscriptionProductComponentGroup:
 
     swagger_types = {
     
         'id': 'int',
         'linked_space_id': 'int',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'optional': 'bool',
         'product_version': 'SubscriptionProductVersion',
         'sort_order': 'int',
         'version': 'int',
     }
 
     attribute_map = {
@@ -93,26 +93,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionProductComponentGroup.
 
             The component group name will be shown when the components are selected. This can be visible to the subscriber.
 
         :return: The name of this SubscriptionProductComponentGroup.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionProductComponentGroup.
 
             The component group name will be shown when the components are selected. This can be visible to the subscriber.
 
         :param name: The name of this SubscriptionProductComponentGroup.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def optional(self):
         """Gets the optional of this SubscriptionProductComponentGroup.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_component_group_update.py` & `wallee-4.0.0/wallee/models/subscription_product_component_group_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class SubscriptionProductComponentGroupUpdate:
 
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
-        'name': 'DatabaseTranslatedStringCreate',
+        'name': 'dict(str, str)',
         'optional': 'bool',
         'product_version': 'int',
         'sort_order': 'int',
     }
 
     attribute_map = {
         'id': 'id','version': 'version','name': 'name','optional': 'optional','product_version': 'productVersion','sort_order': 'sortOrder',
@@ -96,26 +96,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionProductComponentGroupUpdate.
 
             The component group name will be shown when the components are selected. This can be visible to the subscriber.
 
         :return: The name of this SubscriptionProductComponentGroupUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionProductComponentGroupUpdate.
 
             The component group name will be shown when the components are selected. This can be visible to the subscriber.
 
         :param name: The name of this SubscriptionProductComponentGroupUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def optional(self):
         """Gets the optional of this SubscriptionProductComponentGroupUpdate.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_component_reference.py` & `wallee-4.0.0/wallee/models/subscription_product_component_reference.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product_component_update.py` & `wallee-4.0.0/wallee/models/subscription_product_component_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     swagger_types = {
     
         'id': 'int',
         'version': 'int',
         'component_change_weight': 'int',
         'component_group': 'int',
         'default_component': 'bool',
-        'description': 'DatabaseTranslatedStringCreate',
+        'description': 'dict(str, str)',
         'maximal_quantity': 'float',
         'minimal_quantity': 'float',
-        'name': 'DatabaseTranslatedStringCreate',
+        'name': 'dict(str, str)',
         'quantity_step': 'float',
         'reference': 'int',
         'sort_order': 'int',
         'tax_class': 'int',
     }
 
     attribute_map = {
@@ -186,26 +186,26 @@
     @property
     def description(self):
         """Gets the description of this SubscriptionProductComponentUpdate.
 
             The component description may contain a longer description which gives the subscriber a better understanding of what the component contains.
 
         :return: The description of this SubscriptionProductComponentUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this SubscriptionProductComponentUpdate.
 
             The component description may contain a longer description which gives the subscriber a better understanding of what the component contains.
 
         :param description: The description of this SubscriptionProductComponentUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def maximal_quantity(self):
         """Gets the maximal_quantity of this SubscriptionProductComponentUpdate.
@@ -255,26 +255,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionProductComponentUpdate.
 
             The component name is shown to the subscriber. It should describe in few words what the component does contain.
 
         :return: The name of this SubscriptionProductComponentUpdate.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionProductComponentUpdate.
 
             The component name is shown to the subscriber. It should describe in few words what the component does contain.
 
         :param name: The name of this SubscriptionProductComponentUpdate.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def quantity_step(self):
         """Gets the quantity_step of this SubscriptionProductComponentUpdate.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_create.py` & `wallee-4.0.0/wallee/models/subscription_product_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product_retirement.py` & `wallee-4.0.0/wallee/models/subscription_product_retirement.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product_retirement_create.py` & `wallee-4.0.0/wallee/models/subscription_product_retirement_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product_version.py` & `wallee-4.0.0/wallee/models/subscription_product_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         'created_on': 'datetime',
         'default_currency': 'str',
         'enabled_currencies': 'list[str]',
         'id': 'int',
         'increment_number': 'int',
         'linked_space_id': 'int',
         'minimal_number_of_periods': 'int',
-        'name': 'DatabaseTranslatedString',
+        'name': 'dict(str, str)',
         'number_of_notice_periods': 'int',
         'obsoleted_on': 'datetime',
         'planned_purge_date': 'datetime',
         'product': 'SubscriptionProduct',
         'reference': 'str',
         'retiring_finished_on': 'datetime',
         'retiring_started_on': 'datetime',
@@ -319,26 +319,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionProductVersion.
 
             The product version name is the name of the product which is shown to the user for the version. When the visible product name should be changed for a particular product a new version has to be created which contains the new name of the product.
 
         :return: The name of this SubscriptionProductVersion.
-        :rtype: DatabaseTranslatedString
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionProductVersion.
 
             The product version name is the name of the product which is shown to the user for the version. When the visible product name should be changed for a particular product a new version has to be created which contains the new name of the product.
 
         :param name: The name of this SubscriptionProductVersion.
-        :type: DatabaseTranslatedString
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def number_of_notice_periods(self):
         """Gets the number_of_notice_periods of this SubscriptionProductVersion.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_version_pending.py` & `wallee-4.0.0/wallee/models/subscription_product_version_pending.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         'id': 'int',
         'version': 'int',
         'billing_cycle': 'str',
         'comment': 'str',
         'default_currency': 'str',
         'enabled_currencies': 'list[str]',
         'minimal_number_of_periods': 'int',
-        'name': 'DatabaseTranslatedStringCreate',
+        'name': 'dict(str, str)',
         'number_of_notice_periods': 'int',
         'product': 'int',
         'state': 'SubscriptionProductVersionState',
         'tax_calculation': 'TaxCalculation',
     }
 
     attribute_map = {
@@ -229,26 +229,26 @@
     @property
     def name(self):
         """Gets the name of this SubscriptionProductVersionPending.
 
             The product version name is the name of the product which is shown to the user for the version. When the visible product name should be changed for a particular product a new version has to be created which contains the new name of the product.
 
         :return: The name of this SubscriptionProductVersionPending.
-        :rtype: DatabaseTranslatedStringCreate
+        :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this SubscriptionProductVersionPending.
 
             The product version name is the name of the product which is shown to the user for the version. When the visible product name should be changed for a particular product a new version has to be created which contains the new name of the product.
 
         :param name: The name of this SubscriptionProductVersionPending.
-        :type: DatabaseTranslatedStringCreate
+        :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def number_of_notice_periods(self):
         """Gets the number_of_notice_periods of this SubscriptionProductVersionPending.
```

### Comparing `wallee-3.4.0/wallee/models/subscription_product_version_retirement.py` & `wallee-4.0.0/wallee/models/subscription_product_version_retirement.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_product_version_retirement_create.py` & `wallee-4.0.0/wallee/models/subscription_product_version_retirement_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_suspension.py` & `wallee-4.0.0/wallee/models/subscription_suspension.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_suspension_create.py` & `wallee-4.0.0/wallee/models/subscription_suspension_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_suspension_running.py` & `wallee-4.0.0/wallee/models/subscription_suspension_running.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_update.py` & `wallee-4.0.0/wallee/models/subscription_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_update_request.py` & `wallee-4.0.0/wallee/models/subscription_update_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/subscription_version.py` & `wallee-4.0.0/wallee/models/subscription_version.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/tax.py` & `wallee-4.0.0/wallee/models/tax_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
 
 
 
-class Tax:
+class TaxCreate:
 
     swagger_types = {
     
         'rate': 'float',
         'title': 'str',
     }
 
@@ -20,62 +20,68 @@
     
     _rate = None
     _title = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.rate = kwargs.get('rate', None)
-        self.title = kwargs.get('title', None)
+        self.rate = kwargs.get('rate')
+
+        self.title = kwargs.get('title')
+
         
 
     
     @property
     def rate(self):
-        """Gets the rate of this Tax.
+        """Gets the rate of this TaxCreate.
 
             
 
-        :return: The rate of this Tax.
+        :return: The rate of this TaxCreate.
         :rtype: float
         """
         return self._rate
 
     @rate.setter
     def rate(self, rate):
-        """Sets the rate of this Tax.
+        """Sets the rate of this TaxCreate.
 
             
 
-        :param rate: The rate of this Tax.
+        :param rate: The rate of this TaxCreate.
         :type: float
         """
+        if rate is None:
+            raise ValueError("Invalid value for `rate`, must not be `None`")
 
         self._rate = rate
     
     @property
     def title(self):
-        """Gets the title of this Tax.
+        """Gets the title of this TaxCreate.
 
             
 
-        :return: The title of this Tax.
+        :return: The title of this TaxCreate.
         :rtype: str
         """
         return self._title
 
     @title.setter
     def title(self, title):
-        """Sets the title of this Tax.
+        """Sets the title of this TaxCreate.
 
             
 
-        :param title: The title of this Tax.
+        :param title: The title of this TaxCreate.
         :type: str
         """
+        if title is None:
+            raise ValueError("Invalid value for `title`, must not be `None`")
         if title is not None and len(title) > 40:
             raise ValueError("Invalid value for `title`, length must be less than or equal to `40`")
         if title is not None and len(title) < 2:
             raise ValueError("Invalid value for `title`, length must be greater than or equal to `2`")
 
         self._title = title
     
@@ -98,27 +104,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(Tax, dict):
+        if issubclass(TaxCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, Tax):
+        if not isinstance(other, TaxCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/tax_class.py` & `wallee-4.0.0/wallee/models/tax_class.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/tenant_database.py` & `wallee-4.0.0/wallee/models/tenant_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this TenantDatabase.
 
-            The name of the database.
+            The name used to identify the database.
 
         :return: The name of this TenantDatabase.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this TenantDatabase.
 
-            The name of the database.
+            The name used to identify the database.
 
         :param name: The name of this TenantDatabase.
         :type: str
         """
         if name is not None and len(name) > 200:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `200`")
```

### Comparing `wallee-3.4.0/wallee/models/terminal_receipt_fetch_request.py` & `wallee-4.0.0/wallee/models/terminal_receipt_fetch_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/token.py` & `wallee-4.0.0/wallee/models/token.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/token_create.py` & `wallee-4.0.0/wallee/models/webhook_listener_create.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,117 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractTokenUpdate
+from . import AbstractWebhookListenerUpdate
 
 
-class TokenCreate(AbstractTokenUpdate):
+class WebhookListenerCreate(AbstractWebhookListenerUpdate):
 
     swagger_types = {
     
-        'external_id': 'str',
-        'state': 'CreationEntityState',
+        'entity': 'int',
+        'identity': 'int',
+        'url': 'int',
     }
 
     attribute_map = {
-        'external_id': 'externalId','state': 'state',
+        'entity': 'entity','identity': 'identity','url': 'url',
     }
 
     
-    _external_id = None
-    _state = None
+    _entity = None
+    _identity = None
+    _url = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.external_id = kwargs.get('external_id')
+        self.entity = kwargs.get('entity')
+
+        self.identity = kwargs.get('identity', None)
+        self.url = kwargs.get('url')
 
-        self.state = kwargs.get('state', None)
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def external_id(self):
-        """Gets the external_id of this TokenCreate.
+    def entity(self):
+        """Gets the entity of this WebhookListenerCreate.
+
+            The entity that is to be monitored.
+
+        :return: The entity of this WebhookListenerCreate.
+        :rtype: int
+        """
+        return self._entity
+
+    @entity.setter
+    def entity(self, entity):
+        """Sets the entity of this WebhookListenerCreate.
+
+            The entity that is to be monitored.
+
+        :param entity: The entity of this WebhookListenerCreate.
+        :type: int
+        """
+        if entity is None:
+            raise ValueError("Invalid value for `entity`, must not be `None`")
+
+        self._entity = entity
+    
+    @property
+    def identity(self):
+        """Gets the identity of this WebhookListenerCreate.
 
-            A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
+            The identity used to sign messages.
 
-        :return: The external_id of this TokenCreate.
-        :rtype: str
+        :return: The identity of this WebhookListenerCreate.
+        :rtype: int
         """
-        return self._external_id
+        return self._identity
 
-    @external_id.setter
-    def external_id(self, external_id):
-        """Sets the external_id of this TokenCreate.
+    @identity.setter
+    def identity(self, identity):
+        """Sets the identity of this WebhookListenerCreate.
 
-            A client generated nonce which identifies the entity to be created. Subsequent creation requests with the same external ID will not create new entities but return the initially created entity instead.
+            The identity used to sign messages.
 
-        :param external_id: The external_id of this TokenCreate.
-        :type: str
+        :param identity: The identity of this WebhookListenerCreate.
+        :type: int
         """
-        if external_id is None:
-            raise ValueError("Invalid value for `external_id`, must not be `None`")
 
-        self._external_id = external_id
+        self._identity = identity
     
     @property
-    def state(self):
-        """Gets the state of this TokenCreate.
+    def url(self):
+        """Gets the url of this WebhookListenerCreate.
 
-            The object's current state.
+            The URL where notifications about entity changes are sent to.
 
-        :return: The state of this TokenCreate.
-        :rtype: CreationEntityState
+        :return: The url of this WebhookListenerCreate.
+        :rtype: int
         """
-        return self._state
+        return self._url
 
-    @state.setter
-    def state(self, state):
-        """Sets the state of this TokenCreate.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this WebhookListenerCreate.
 
-            The object's current state.
+            The URL where notifications about entity changes are sent to.
 
-        :param state: The state of this TokenCreate.
-        :type: CreationEntityState
+        :param url: The url of this WebhookListenerCreate.
+        :type: int
         """
+        if url is None:
+            raise ValueError("Invalid value for `url`, must not be `None`")
 
-        self._state = state
+        self._url = url
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -99,27 +128,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(TokenCreate, dict):
+        if issubclass(WebhookListenerCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, TokenCreate):
+        if not isinstance(other, WebhookListenerCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/token_update.py` & `wallee-4.0.0/wallee/models/token_update.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/token_version.py` & `wallee-4.0.0/wallee/models/token_version.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/token_version_type.py` & `wallee-4.0.0/wallee/models/token_version_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this TokenVersionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this TokenVersionType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this TokenVersionType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this TokenVersionType.
         :type: dict(str, str)
         """
 
         self._description = description
     
@@ -104,26 +104,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this TokenVersionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this TokenVersionType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this TokenVersionType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this TokenVersionType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/tokenized_card_data.py` & `wallee-4.0.0/wallee/models/tokenized_card_data.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/tokenized_card_data_create.py` & `wallee-4.0.0/wallee/models/tokenized_card_data_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction.py` & `wallee-4.0.0/wallee/models/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1236,26 +1236,26 @@
 
         self._merchant_reference = merchant_reference
     
     @property
     def meta_data(self):
         """Gets the meta_data of this Transaction.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :return: The meta_data of this Transaction.
         :rtype: dict(str, str)
         """
         return self._meta_data
 
     @meta_data.setter
     def meta_data(self, meta_data):
         """Sets the meta_data of this Transaction.
 
-            Meta data allow to store additional data along the object.
+            Allow to store additional information about the object.
 
         :param meta_data: The meta_data of this Transaction.
         :type: dict(str, str)
         """
 
         self._meta_data = meta_data
```

### Comparing `wallee-3.4.0/wallee/models/transaction_aware_entity.py` & `wallee-4.0.0/wallee/models/transaction_pending.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,91 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
+from . import AbstractTransactionPending
 
 
-
-class TransactionAwareEntity:
+class TransactionPending(AbstractTransactionPending):
 
     swagger_types = {
     
         'id': 'int',
-        'linked_space_id': 'int',
-        'linked_transaction': 'int',
+        'version': 'int',
     }
 
     attribute_map = {
-        'id': 'id','linked_space_id': 'linkedSpaceId','linked_transaction': 'linkedTransaction',
+        'id': 'id','version': 'version',
     }
 
     
     _id = None
-    _linked_space_id = None
-    _linked_transaction = None
+    _version = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.id = kwargs.get('id', None)
-        self.linked_space_id = kwargs.get('linked_space_id', None)
-        self.linked_transaction = kwargs.get('linked_transaction', None)
-        
+        self.id = kwargs.get('id')
+
+        self.version = kwargs.get('version')
+
+        super().__init__(**kwargs)
+        self.swagger_types.update(super().swagger_types)
+        self.attribute_map.update(super().attribute_map)
 
     
     @property
     def id(self):
-        """Gets the id of this TransactionAwareEntity.
+        """Gets the id of this TransactionPending.
 
-            A unique identifier for the object.
+            The ID is the primary key of the entity. The ID identifies the entity uniquely.
 
-        :return: The id of this TransactionAwareEntity.
+        :return: The id of this TransactionPending.
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this TransactionAwareEntity.
+        """Sets the id of this TransactionPending.
 
-            A unique identifier for the object.
+            The ID is the primary key of the entity. The ID identifies the entity uniquely.
 
-        :param id: The id of this TransactionAwareEntity.
+        :param id: The id of this TransactionPending.
         :type: int
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
     
     @property
-    def linked_space_id(self):
-        """Gets the linked_space_id of this TransactionAwareEntity.
-
-            The ID of the space this object belongs to.
-
-        :return: The linked_space_id of this TransactionAwareEntity.
-        :rtype: int
-        """
-        return self._linked_space_id
-
-    @linked_space_id.setter
-    def linked_space_id(self, linked_space_id):
-        """Sets the linked_space_id of this TransactionAwareEntity.
-
-            The ID of the space this object belongs to.
-
-        :param linked_space_id: The linked_space_id of this TransactionAwareEntity.
-        :type: int
-        """
-
-        self._linked_space_id = linked_space_id
-    
-    @property
-    def linked_transaction(self):
-        """Gets the linked_transaction of this TransactionAwareEntity.
+    def version(self):
+        """Gets the version of this TransactionPending.
 
-            
+            The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :return: The linked_transaction of this TransactionAwareEntity.
+        :return: The version of this TransactionPending.
         :rtype: int
         """
-        return self._linked_transaction
+        return self._version
 
-    @linked_transaction.setter
-    def linked_transaction(self, linked_transaction):
-        """Sets the linked_transaction of this TransactionAwareEntity.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this TransactionPending.
 
-            
+            The version number indicates the version of the entity. The version is incremented whenever the entity is changed.
 
-        :param linked_transaction: The linked_transaction of this TransactionAwareEntity.
+        :param version: The version of this TransactionPending.
         :type: int
         """
+        if version is None:
+            raise ValueError("Invalid value for `version`, must not be `None`")
 
-        self._linked_transaction = linked_transaction
+        self._version = version
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -120,27 +102,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(TransactionAwareEntity, dict):
+        if issubclass(TransactionPending, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, TransactionAwareEntity):
+        if not isinstance(other, TransactionPending):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/transaction_comment.py` & `wallee-4.0.0/wallee/models/transaction_comment.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,51 +53,51 @@
         
 
     
     @property
     def content(self):
         """Gets the content of this TransactionComment.
 
-            
+            The comment's actual content.
 
         :return: The content of this TransactionComment.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
         """Sets the content of this TransactionComment.
 
-            
+            The comment's actual content.
 
         :param content: The content of this TransactionComment.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
     @property
     def created_by(self):
         """Gets the created_by of this TransactionComment.
 
-            
+            The ID of the user the comment was created by.
 
         :return: The created_by of this TransactionComment.
         :rtype: int
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this TransactionComment.
 
-            
+            The ID of the user the comment was created by.
 
         :param created_by: The created_by of this TransactionComment.
         :type: int
         """
 
         self._created_by = created_by
     
@@ -124,49 +124,49 @@
 
         self._created_on = created_on
     
     @property
     def edited_by(self):
         """Gets the edited_by of this TransactionComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :return: The edited_by of this TransactionComment.
         :rtype: int
         """
         return self._edited_by
 
     @edited_by.setter
     def edited_by(self, edited_by):
         """Sets the edited_by of this TransactionComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :param edited_by: The edited_by of this TransactionComment.
         :type: int
         """
 
         self._edited_by = edited_by
     
     @property
     def edited_on(self):
         """Gets the edited_on of this TransactionComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :return: The edited_on of this TransactionComment.
         :rtype: datetime
         """
         return self._edited_on
 
     @edited_on.setter
     def edited_on(self, edited_on):
         """Sets the edited_on of this TransactionComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :param edited_on: The edited_on of this TransactionComment.
         :type: datetime
         """
 
         self._edited_on = edited_on
     
@@ -216,26 +216,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def pinned(self):
         """Gets the pinned of this TransactionComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :return: The pinned of this TransactionComment.
         :rtype: bool
         """
         return self._pinned
 
     @pinned.setter
     def pinned(self, pinned):
         """Sets the pinned of this TransactionComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :param pinned: The pinned of this TransactionComment.
         :type: bool
         """
 
         self._pinned = pinned
```

### Comparing `wallee-3.4.0/wallee/models/transaction_comment_active.py` & `wallee-4.0.0/wallee/models/transaction_comment_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_comment_create.py` & `wallee-4.0.0/wallee/models/account_create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,88 @@
 # coding: utf-8
 import pprint
 import six
 from enum import Enum
-from . import AbstractTransactionCommentActive
+from . import AbstractAccountUpdate
 
 
-class TransactionCommentCreate(AbstractTransactionCommentActive):
+class AccountCreate(AbstractAccountUpdate):
 
     swagger_types = {
     
-        'transaction': 'int',
+        'parent_account': 'int',
+        'scope': 'int',
     }
 
     attribute_map = {
-        'transaction': 'transaction',
+        'parent_account': 'parentAccount','scope': 'scope',
     }
 
     
-    _transaction = None
+    _parent_account = None
+    _scope = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
-        self.transaction = kwargs.get('transaction')
+        self.parent_account = kwargs.get('parent_account', None)
+        self.scope = kwargs.get('scope')
 
         super().__init__(**kwargs)
         self.swagger_types.update(super().swagger_types)
         self.attribute_map.update(super().attribute_map)
 
     
     @property
-    def transaction(self):
-        """Gets the transaction of this TransactionCommentCreate.
+    def parent_account(self):
+        """Gets the parent_account of this AccountCreate.
 
-            
+            The parent account responsible for administering this account.
 
-        :return: The transaction of this TransactionCommentCreate.
+        :return: The parent_account of this AccountCreate.
         :rtype: int
         """
-        return self._transaction
+        return self._parent_account
 
-    @transaction.setter
-    def transaction(self, transaction):
-        """Sets the transaction of this TransactionCommentCreate.
+    @parent_account.setter
+    def parent_account(self, parent_account):
+        """Sets the parent_account of this AccountCreate.
 
-            
+            The parent account responsible for administering this account.
 
-        :param transaction: The transaction of this TransactionCommentCreate.
+        :param parent_account: The parent_account of this AccountCreate.
         :type: int
         """
-        if transaction is None:
-            raise ValueError("Invalid value for `transaction`, must not be `None`")
 
-        self._transaction = transaction
+        self._parent_account = parent_account
+    
+    @property
+    def scope(self):
+        """Gets the scope of this AccountCreate.
+
+            The scope that the account belongs to.
+
+        :return: The scope of this AccountCreate.
+        :rtype: int
+        """
+        return self._scope
+
+    @scope.setter
+    def scope(self, scope):
+        """Sets the scope of this AccountCreate.
+
+            The scope that the account belongs to.
+
+        :param scope: The scope of this AccountCreate.
+        :type: int
+        """
+        if scope is None:
+            raise ValueError("Invalid value for `scope`, must not be `None`")
+
+        self._scope = scope
     
 
     def to_dict(self):
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -73,27 +99,27 @@
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             elif isinstance(value, Enum):
                 result[attr] = value.value
             else:
                 result[attr] = value
-        if issubclass(TransactionCommentCreate, dict):
+        if issubclass(AccountCreate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         return self.to_str()
 
     def __eq__(self, other):
-        if not isinstance(other, TransactionCommentCreate):
+        if not isinstance(other, AccountCreate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `wallee-3.4.0/wallee/models/transaction_completion.py` & `wallee-4.0.0/wallee/models/transaction_completion.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_completion_request.py` & `wallee-4.0.0/wallee/models/transaction_completion_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_create.py` & `wallee-4.0.0/wallee/models/transaction_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_group.py` & `wallee-4.0.0/wallee/models/transaction_group.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_invoice.py` & `wallee-4.0.0/wallee/models/transaction_invoice.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_invoice_comment.py` & `wallee-4.0.0/wallee/models/transaction_invoice_comment.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,51 +53,51 @@
         
 
     
     @property
     def content(self):
         """Gets the content of this TransactionInvoiceComment.
 
-            
+            The comment's actual content.
 
         :return: The content of this TransactionInvoiceComment.
         :rtype: str
         """
         return self._content
 
     @content.setter
     def content(self, content):
         """Sets the content of this TransactionInvoiceComment.
 
-            
+            The comment's actual content.
 
         :param content: The content of this TransactionInvoiceComment.
         :type: str
         """
         if content is not None and len(content) > 262144:
             raise ValueError("Invalid value for `content`, length must be less than or equal to `262144`")
 
         self._content = content
     
     @property
     def created_by(self):
         """Gets the created_by of this TransactionInvoiceComment.
 
-            
+            The ID of the user the comment was created by.
 
         :return: The created_by of this TransactionInvoiceComment.
         :rtype: int
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this TransactionInvoiceComment.
 
-            
+            The ID of the user the comment was created by.
 
         :param created_by: The created_by of this TransactionInvoiceComment.
         :type: int
         """
 
         self._created_by = created_by
     
@@ -124,49 +124,49 @@
 
         self._created_on = created_on
     
     @property
     def edited_by(self):
         """Gets the edited_by of this TransactionInvoiceComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :return: The edited_by of this TransactionInvoiceComment.
         :rtype: int
         """
         return self._edited_by
 
     @edited_by.setter
     def edited_by(self, edited_by):
         """Sets the edited_by of this TransactionInvoiceComment.
 
-            
+            The ID of the user the comment was last updated by.
 
         :param edited_by: The edited_by of this TransactionInvoiceComment.
         :type: int
         """
 
         self._edited_by = edited_by
     
     @property
     def edited_on(self):
         """Gets the edited_on of this TransactionInvoiceComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :return: The edited_on of this TransactionInvoiceComment.
         :rtype: datetime
         """
         return self._edited_on
 
     @edited_on.setter
     def edited_on(self, edited_on):
         """Sets the edited_on of this TransactionInvoiceComment.
 
-            The date on which the comment was last edited.
+            The date and time when the comment was last updated.
 
         :param edited_on: The edited_on of this TransactionInvoiceComment.
         :type: datetime
         """
 
         self._edited_on = edited_on
     
@@ -216,26 +216,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def pinned(self):
         """Gets the pinned of this TransactionInvoiceComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :return: The pinned of this TransactionInvoiceComment.
         :rtype: bool
         """
         return self._pinned
 
     @pinned.setter
     def pinned(self, pinned):
         """Sets the pinned of this TransactionInvoiceComment.
 
-            
+            Whether the comment is pinned to the top.
 
         :param pinned: The pinned of this TransactionInvoiceComment.
         :type: bool
         """
 
         self._pinned = pinned
```

### Comparing `wallee-3.4.0/wallee/models/transaction_invoice_comment_active.py` & `wallee-4.0.0/wallee/models/transaction_invoice_comment_active.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_invoice_comment_create.py` & `wallee-4.0.0/wallee/models/transaction_invoice_comment_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_invoice_replacement.py` & `wallee-4.0.0/wallee/models/transaction_invoice_replacement.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_line_item_version.py` & `wallee-4.0.0/wallee/models/transaction_line_item_version.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_line_item_version_create.py` & `wallee-4.0.0/wallee/models/transaction_line_item_version_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/transaction_void.py` & `wallee-4.0.0/wallee/models/transaction_void.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/two_factor_authentication_type.py` & `wallee-4.0.0/wallee/models/two_factor_authentication_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,72 +38,72 @@
         
 
     
     @property
     def description(self):
         """Gets the description of this TwoFactorAuthenticationType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :return: The description of this TwoFactorAuthenticationType.
         :rtype: dict(str, str)
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this TwoFactorAuthenticationType.
 
-            The description of the object translated into different languages.
+            The localized description of the object.
 
         :param description: The description of this TwoFactorAuthenticationType.
         :type: dict(str, str)
         """
 
         self._description = description
     
     @property
     def feature(self):
         """Gets the feature of this TwoFactorAuthenticationType.
 
-            
+            The feature that this type belongs to.
 
         :return: The feature of this TwoFactorAuthenticationType.
         :rtype: int
         """
         return self._feature
 
     @feature.setter
     def feature(self, feature):
         """Sets the feature of this TwoFactorAuthenticationType.
 
-            
+            The feature that this type belongs to.
 
         :param feature: The feature of this TwoFactorAuthenticationType.
         :type: int
         """
 
         self._feature = feature
     
     @property
     def icon(self):
         """Gets the icon of this TwoFactorAuthenticationType.
 
-            
+            The identifier of the icon representing this type.
 
         :return: The icon of this TwoFactorAuthenticationType.
         :rtype: str
         """
         return self._icon
 
     @icon.setter
     def icon(self, icon):
         """Sets the icon of this TwoFactorAuthenticationType.
 
-            
+            The identifier of the icon representing this type.
 
         :param icon: The icon of this TwoFactorAuthenticationType.
         :type: str
         """
 
         self._icon = icon
     
@@ -130,26 +130,26 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this TwoFactorAuthenticationType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :return: The name of this TwoFactorAuthenticationType.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this TwoFactorAuthenticationType.
 
-            The name of the object translated into different languages.
+            The localized name of the object.
 
         :param name: The name of this TwoFactorAuthenticationType.
         :type: dict(str, str)
         """
 
         self._name = name
```

### Comparing `wallee-3.4.0/wallee/models/user.py` & `wallee-4.0.0/wallee/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class User:
 
     swagger_types = {
     
         'id': 'int',
         'planned_purge_date': 'datetime',
-        'scope': 'Scope',
+        'scope': 'int',
         'state': 'CreationEntityState',
         'user_type': 'UserType',
         'version': 'int',
     }
 
     attribute_map = {
         'id': 'id','planned_purge_date': 'plannedPurgeDate','scope': 'scope','state': 'state','user_type': 'userType','version': 'version',
@@ -87,29 +87,29 @@
 
         self._planned_purge_date = planned_purge_date
     
     @property
     def scope(self):
         """Gets the scope of this User.
 
-            
+            The scope that the user belongs to.
 
         :return: The scope of this User.
-        :rtype: Scope
+        :rtype: int
         """
         return self._scope
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this User.
 
-            
+            The scope that the user belongs to.
 
         :param scope: The scope of this User.
-        :type: Scope
+        :type: int
         """
 
         self._scope = scope
     
     @property
     def state(self):
         """Gets the state of this User.
@@ -133,26 +133,26 @@
 
         self._state = state
     
     @property
     def user_type(self):
         """Gets the user_type of this User.
 
-            
+            The user's type which defines its role and capabilities.
 
         :return: The user_type of this User.
         :rtype: UserType
         """
         return self._user_type
 
     @user_type.setter
     def user_type(self, user_type):
         """Sets the user_type of this User.
 
-            
+            The user's type which defines its role and capabilities.
 
         :param user_type: The user_type of this User.
         :type: UserType
         """
 
         self._user_type = user_type
```

### Comparing `wallee-3.4.0/wallee/models/user_account_role.py` & `wallee-4.0.0/wallee/models/user_account_role.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/user_space_role.py` & `wallee-4.0.0/wallee/models/user_space_role.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/web_app_confirmation_request.py` & `wallee-4.0.0/wallee/models/web_app_confirmation_request.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/web_app_confirmation_response.py` & `wallee-4.0.0/wallee/models/web_app_confirmation_response.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/models/webhook_identity.py` & `wallee-4.0.0/wallee/models/webhook_identity.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,26 +87,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def name(self):
         """Gets the name of this WebhookIdentity.
 
-            The identity name is used internally to identify the webhook identity in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook identity.
 
         :return: The name of this WebhookIdentity.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this WebhookIdentity.
 
-            The identity name is used internally to identify the webhook identity in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook identity.
 
         :param name: The name of this WebhookIdentity.
         :type: str
         """
         if name is not None and len(name) > 50:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")
```

### Comparing `wallee-3.4.0/wallee/models/webhook_listener.py` & `wallee-4.0.0/wallee/models/webhook_listener.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,49 +56,49 @@
         
 
     
     @property
     def entity(self):
         """Gets the entity of this WebhookListener.
 
-            The listener listens on state changes of the entity linked with the listener.
+            The entity that is to be monitored.
 
         :return: The entity of this WebhookListener.
         :rtype: int
         """
         return self._entity
 
     @entity.setter
     def entity(self, entity):
         """Sets the entity of this WebhookListener.
 
-            The listener listens on state changes of the entity linked with the listener.
+            The entity that is to be monitored.
 
         :param entity: The entity of this WebhookListener.
         :type: int
         """
 
         self._entity = entity
     
     @property
     def entity_states(self):
         """Gets the entity_states of this WebhookListener.
 
-            The target state identifies the state into which entities need to move into to trigger the webhook listener.
+            The entity's target states that are to be monitored.
 
         :return: The entity_states of this WebhookListener.
         :rtype: list[str]
         """
         return self._entity_states
 
     @entity_states.setter
     def entity_states(self, entity_states):
         """Sets the entity_states of this WebhookListener.
 
-            The target state identifies the state into which entities need to move into to trigger the webhook listener.
+            The entity's target states that are to be monitored.
 
         :param entity_states: The entity_states of this WebhookListener.
         :type: list[str]
         """
 
         self._entity_states = entity_states
     
@@ -125,26 +125,26 @@
 
         self._id = id
     
     @property
     def identity(self):
         """Gets the identity of this WebhookListener.
 
-            The identity which will be used to sign messages sent by this listener.
+            The identity used to sign messages.
 
         :return: The identity of this WebhookListener.
         :rtype: WebhookIdentity
         """
         return self._identity
 
     @identity.setter
     def identity(self, identity):
         """Sets the identity of this WebhookListener.
 
-            The identity which will be used to sign messages sent by this listener.
+            The identity used to sign messages.
 
         :param identity: The identity of this WebhookListener.
         :type: WebhookIdentity
         """
 
         self._identity = identity
     
@@ -171,51 +171,51 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def name(self):
         """Gets the name of this WebhookListener.
 
-            The webhook listener name is used internally to identify the webhook listener in administrative interfaces.For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook listener.
 
         :return: The name of this WebhookListener.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this WebhookListener.
 
-            The webhook listener name is used internally to identify the webhook listener in administrative interfaces.For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook listener.
 
         :param name: The name of this WebhookListener.
         :type: str
         """
         if name is not None and len(name) > 50:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")
 
         self._name = name
     
     @property
     def notify_every_change(self):
         """Gets the notify_every_change of this WebhookListener.
 
-            Defines whether the webhook listener is to be informed about every change made to the entity in contrast to state transitions only.
+            Whether every update of the entity or only state changes are to be monitored.
 
         :return: The notify_every_change of this WebhookListener.
         :rtype: bool
         """
         return self._notify_every_change
 
     @notify_every_change.setter
     def notify_every_change(self, notify_every_change):
         """Sets the notify_every_change of this WebhookListener.
 
-            Defines whether the webhook listener is to be informed about every change made to the entity in contrast to state transitions only.
+            Whether every update of the entity or only state changes are to be monitored.
 
         :param notify_every_change: The notify_every_change of this WebhookListener.
         :type: bool
         """
 
         self._notify_every_change = notify_every_change
     
@@ -265,26 +265,26 @@
 
         self._state = state
     
     @property
     def url(self):
         """Gets the url of this WebhookListener.
 
-            The URL which is invoked by the listener to notify the application about the event.
+            The URL where notifications about entity changes are sent to.
 
         :return: The url of this WebhookListener.
         :rtype: WebhookUrl
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """Sets the url of this WebhookListener.
 
-            The URL which is invoked by the listener to notify the application about the event.
+            The URL where notifications about entity changes are sent to.
 
         :param url: The url of this WebhookListener.
         :type: WebhookUrl
         """
 
         self._url = url
```

### Comparing `wallee-3.4.0/wallee/models/webhook_listener_entity.py` & `wallee-4.0.0/wallee/models/webhook_listener_entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,49 +55,49 @@
 
         self._id = id
     
     @property
     def name(self):
         """Gets the name of this WebhookListenerEntity.
 
-            
+            The name used to identify the webhook listener entity.
 
         :return: The name of this WebhookListenerEntity.
         :rtype: dict(str, str)
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this WebhookListenerEntity.
 
-            
+            The name used to identify the webhook listener entity.
 
         :param name: The name of this WebhookListenerEntity.
         :type: dict(str, str)
         """
 
         self._name = name
     
     @property
     def technical_name(self):
         """Gets the technical_name of this WebhookListenerEntity.
 
-            
+            The name used to programmatically identify the webhook listener entity.
 
         :return: The technical_name of this WebhookListenerEntity.
         :rtype: str
         """
         return self._technical_name
 
     @technical_name.setter
     def technical_name(self, technical_name):
         """Sets the technical_name of this WebhookListenerEntity.
 
-            
+            The name used to programmatically identify the webhook listener entity.
 
         :param technical_name: The technical_name of this WebhookListenerEntity.
         :type: str
         """
 
         self._technical_name = technical_name
```

### Comparing `wallee-3.4.0/wallee/models/webhook_url.py` & `wallee-4.0.0/wallee/models/webhook_url.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,26 +47,26 @@
         
 
     
     @property
     def application_managed(self):
         """Gets the application_managed of this WebhookUrl.
 
-            The webhook URL is managed by the application and cannot be changed via the user interface.
+            Whether the webhook URL is managed by the application, and therefore cannot be changed via the user interface.
 
         :return: The application_managed of this WebhookUrl.
         :rtype: bool
         """
         return self._application_managed
 
     @application_managed.setter
     def application_managed(self, application_managed):
         """Sets the application_managed of this WebhookUrl.
 
-            The webhook URL is managed by the application and cannot be changed via the user interface.
+            Whether the webhook URL is managed by the application, and therefore cannot be changed via the user interface.
 
         :param application_managed: The application_managed of this WebhookUrl.
         :type: bool
         """
 
         self._application_managed = application_managed
     
@@ -116,26 +116,26 @@
 
         self._linked_space_id = linked_space_id
     
     @property
     def name(self):
         """Gets the name of this WebhookUrl.
 
-            The URL name is used internally to identify the URL in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook URL.
 
         :return: The name of this WebhookUrl.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this WebhookUrl.
 
-            The URL name is used internally to identify the URL in administrative interfaces. For example it is used within search fields and hence it should be distinct and descriptive.
+            The name used to identify the webhook URL.
 
         :param name: The name of this WebhookUrl.
         :type: str
         """
         if name is not None and len(name) > 50:
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")
 
@@ -187,26 +187,26 @@
 
         self._state = state
     
     @property
     def url(self):
         """Gets the url of this WebhookUrl.
 
-            The URL to which the HTTP requests are sent to. An example URL could look like https://www.example.com/some/path?some-query-parameter=value.
+            The actual URL where notifications about entity changes are sent to.
 
         :return: The url of this WebhookUrl.
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """Sets the url of this WebhookUrl.
 
-            The URL to which the HTTP requests are sent to. An example URL could look like https://www.example.com/some/path?some-query-parameter=value.
+            The actual URL where notifications about entity changes are sent to.
 
         :param url: The url of this WebhookUrl.
         :type: str
         """
         if url is not None and len(url) > 500:
             raise ValueError("Invalid value for `url`, length must be less than or equal to `500`")
         if url is not None and len(url) < 9:
```

### Comparing `wallee-3.4.0/wallee/models/webhook_url_create.py` & `wallee-4.0.0/wallee/models/webhook_url_create.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee/rest.py` & `wallee-4.0.0/wallee/rest.py`

 * *Files identical despite different names*

### Comparing `wallee-3.4.0/wallee.egg-info/PKG-INFO` & `wallee-4.0.0/wallee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallee
-Version: 3.4.0
+Version: 4.0.0
 Summary: SDK that allows you to access wallee
 Author: Wallee AG
 License: Apache-2.0
 Keywords: wallee,Payment,Payment Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `wallee-3.4.0/wallee.egg-info/SOURCES.txt` & `wallee-4.0.0/wallee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -209,18 +209,14 @@
 wallee/models/customer_comment_active.py
 wallee/models/customer_comment_create.py
 wallee/models/customer_create.py
 wallee/models/customer_postal_address.py
 wallee/models/customer_postal_address_create.py
 wallee/models/customers_presence.py
 wallee/models/data_collection_type.py
-wallee/models/database_translated_string.py
-wallee/models/database_translated_string_create.py
-wallee/models/database_translated_string_item.py
-wallee/models/database_translated_string_item_create.py
 wallee/models/debt_collection_case.py
 wallee/models/debt_collection_case_create.py
 wallee/models/debt_collection_case_document.py
 wallee/models/debt_collection_case_source.py
 wallee/models/debt_collection_case_state.py
 wallee/models/debt_collection_case_update.py
 wallee/models/debt_collection_environment.py
```

