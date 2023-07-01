# Comparing `tmp/increase-0.8.0.tar.gz` & `tmp/increase-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increase-0.8.0.tar", max compression
+gzip compressed data, was "increase-0.8.1.tar", max compression
```

## Comparing `increase-0.8.0.tar` & `increase-0.8.1.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0    11338 2023-06-29 12:24:52.608649 increase-0.8.0/LICENSE
--rw-r--r--   0        0        0     8418 2023-06-29 12:24:52.608649 increase-0.8.0/README.md
--rw-r--r--   0        0        0     1883 2023-06-29 12:24:52.608649 increase-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/__init__.py
--rw-r--r--   0        0        0    46808 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_base_exceptions.py
--rw-r--r--   0        0        0    26762 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_client.py
--rw-r--r--   0        0        0    10875 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_models.py
--rw-r--r--   0        0        0     4846 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_qs.py
--rw-r--r--   0        0        0      890 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_resource.py
--rw-r--r--   0        0        0     5884 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_streaming.py
--rw-r--r--   0        0        0     4229 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_types.py
--rw-r--r--   0        0        0     1277 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/_utils/_utils.py
--rw-r--r--   0        0        0      127 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/_version.py
--rw-r--r--   0        0        0     1109 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/pagination.py
--rw-r--r--   0        0        0        0 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/py.typed
--rw-r--r--   0        0        0     4478 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/__init__.py
--rw-r--r--   0        0        0    15065 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/account_numbers.py
--rw-r--r--   0        0        0     7400 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/account_statements.py
--rw-r--r--   0        0        0    18102 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/account_transfers.py
--rw-r--r--   0        0        0    18476 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/accounts.py
--rw-r--r--   0        0        0    15600 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/ach_prenotifications.py
--rw-r--r--   0        0        0    26071 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/ach_transfers.py
--rw-r--r--   0        0        0     4285 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/balance_lookups.py
--rw-r--r--   0        0        0     8651 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/bookkeeping_accounts.py
--rw-r--r--   0        0        0     4122 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/bookkeeping_entries.py
--rw-r--r--   0        0        0     4842 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/bookkeeping_entry_sets.py
--rw-r--r--   0        0        0    10707 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/card_disputes.py
--rw-r--r--   0        0        0    10597 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/card_profiles.py
--rw-r--r--   0        0        0    19120 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/cards.py
--rw-r--r--   0        0        0    11757 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/check_deposits.py
--rw-r--r--   0        0        0    23188 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/check_transfers.py
--rw-r--r--   0        0        0     7771 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/declined_transactions.py
--rw-r--r--   0        0        0     7353 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/digital_wallet_tokens.py
--rw-r--r--   0        0        0     7177 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/documents.py
--rw-r--r--   0        0        0      282 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/entities/__init__.py
--rw-r--r--   0        0        0    14010 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/entities/entities.py
--rw-r--r--   0        0        0     8071 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/entities/supplemental_documents.py
--rw-r--r--   0        0        0    18799 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/event_subscriptions.py
--rw-r--r--   0        0        0     7154 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/events.py
--rw-r--r--   0        0        0    10548 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/exports.py
--rw-r--r--   0        0        0    15315 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/external_accounts.py
--rw-r--r--   0        0        0    12929 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/files.py
--rw-r--r--   0        0        0     2040 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/groups.py
--rw-r--r--   0        0        0    12035 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/inbound_ach_transfer_returns.py
--rw-r--r--   0        0        0     7075 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0    14231 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/limits.py
--rw-r--r--   0        0        0     6593 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/oauth_connections.py
--rw-r--r--   0        0        0     8344 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/pending_transactions.py
--rw-r--r--   0        0        0     6300 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/programs.py
--rw-r--r--   0        0        0     8536 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/real_time_decisions.py
--rw-r--r--   0        0        0    14968 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4951 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/routing_numbers.py
--rw-r--r--   0        0        0     1989 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/account_statements.py
--rw-r--r--   0        0        0     4024 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/account_transfers.py
--rw-r--r--   0        0        0    21871 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/ach_transfers.py
--rw-r--r--   0        0        0     5051 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/card_disputes.py
--rw-r--r--   0        0        0     3967 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/card_refunds.py
--rw-r--r--   0        0        0    11463 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/cards.py
--rw-r--r--   0        0        0    10125 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/check_deposits.py
--rw-r--r--   0        0        0    11013 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/check_transfers.py
--rw-r--r--   0        0        0     4085 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/digital_wallet_token_requests.py
--rw-r--r--   0        0        0     3639 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/documents.py
--rw-r--r--   0        0        0    13466 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0     4411 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/interest_payments.py
--rw-r--r--   0        0        0     3919 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/programs.py
--rw-r--r--   0        0        0    11257 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4588 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/simulations.py
--rw-r--r--   0        0        0    12351 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/wire_transfers.py
--rw-r--r--   0        0        0     7800 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/transactions.py
--rw-r--r--   0        0        0    13338 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/wire_drawdown_requests.py
--rw-r--r--   0        0        0    27583 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/resources/wire_transfers.py
--rw-r--r--   0        0        0     8739 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/__init__.py
--rw-r--r--   0        0        0     1666 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account.py
--rw-r--r--   0        0        0      747 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_create_params.py
--rw-r--r--   0        0        0     1693 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_list_params.py
--rw-r--r--   0        0        0     1026 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number.py
--rw-r--r--   0        0        0      408 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number_create_params.py
--rw-r--r--   0        0        0     1598 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number_list_params.py
--rw-r--r--   0        0        0      435 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number_update_params.py
--rw-r--r--   0        0        0     1347 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_statement.py
--rw-r--r--   0        0        0     1534 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_statement_list_params.py
--rw-r--r--   0        0        0     2648 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_transfer.py
--rw-r--r--   0        0        0      814 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_transfer_create_params.py
--rw-r--r--   0        0        0     1494 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_transfer_list_params.py
--rw-r--r--   0        0        0      271 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_update_params.py
--rw-r--r--   0        0        0     2152 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_prenotification.py
--rw-r--r--   0        0        0     1847 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_prenotification_create_params.py
--rw-r--r--   0        0        0     1391 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_prenotification_list_params.py
--rw-r--r--   0        0        0     8882 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_transfer.py
--rw-r--r--   0        0        0     3388 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_transfer_create_params.py
--rw-r--r--   0        0        0     1592 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_transfer_list_params.py
--rw-r--r--   0        0        0      585 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/balance_lookup_lookup_params.py
--rw-r--r--   0        0        0      780 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/balance_lookup_lookup_response.py
--rw-r--r--   0        0        0      823 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_account.py
--rw-r--r--   0        0        0      626 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_account_create_params.py
--rw-r--r--   0        0        0      428 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_account_list_params.py
--rw-r--r--   0        0        0      698 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry.py
--rw-r--r--   0        0        0      424 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry_list_params.py
--rw-r--r--   0        0        0      895 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry_set.py
--rw-r--r--   0        0        0     1133 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry_set_create_params.py
--rw-r--r--   0        0        0     2342 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card.py
--rw-r--r--   0        0        0     1767 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_create_params.py
--rw-r--r--   0        0        0      907 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_details.py
--rw-r--r--   0        0        0     2011 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_dispute.py
--rw-r--r--   0        0        0      483 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_dispute_create_params.py
--rw-r--r--   0        0        0     1661 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_dispute_list_params.py
--rw-r--r--   0        0        0     1451 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_list_params.py
--rw-r--r--   0        0        0     2186 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_profile.py
--rw-r--r--   0        0        0     1820 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_profile_create_params.py
--rw-r--r--   0        0        0      716 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_profile_list_params.py
--rw-r--r--   0        0        0     1611 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_update_params.py
--rw-r--r--   0        0        0     4894 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_deposit.py
--rw-r--r--   0        0        0      748 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_deposit_create_params.py
--rw-r--r--   0        0        0     1477 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_deposit_list_params.py
--rw-r--r--   0        0        0     6750 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_transfer.py
--rw-r--r--   0        0        0     1939 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_transfer_create_params.py
--rw-r--r--   0        0        0     1488 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_transfer_list_params.py
--rw-r--r--   0        0        0    13068 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/declined_transaction.py
--rw-r--r--   0        0        0     1598 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/declined_transaction_list_params.py
--rw-r--r--   0        0        0      950 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/digital_wallet_token.py
--rw-r--r--   0        0        0     1489 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/digital_wallet_token_list_params.py
--rw-r--r--   0        0        0      883 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/document.py
--rw-r--r--   0        0        0     1780 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/document_list_params.py
--rw-r--r--   0        0        0      418 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/__init__.py
--rw-r--r--   0        0        0      634 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/supplemental_document.py
--rw-r--r--   0        0        0      343 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/supplemental_document_create_params.py
--rw-r--r--   0        0        0      547 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/supplemental_document_list_params.py
--rw-r--r--   0        0        0    11893 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entity.py
--rw-r--r--   0        0        0    25685 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entity_create_params.py
--rw-r--r--   0        0        0     1367 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entity_list_params.py
--rw-r--r--   0        0        0     2724 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event.py
--rw-r--r--   0        0        0     4044 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_list_params.py
--rw-r--r--   0        0        0     3124 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription.py
--rw-r--r--   0        0        0     2526 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription_create_params.py
--rw-r--r--   0        0        0      426 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription_list_params.py
--rw-r--r--   0        0        0      360 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription_update_params.py
--rw-r--r--   0        0        0     1147 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/export.py
--rw-r--r--   0        0        0     2946 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/export_create_params.py
--rw-r--r--   0        0        0      404 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/export_list_params.py
--rw-r--r--   0        0        0     1205 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account.py
--rw-r--r--   0        0        0      706 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account_create_params.py
--rw-r--r--   0        0        0      701 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account_list_params.py
--rw-r--r--   0        0        0      420 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account_update_params.py
--rw-r--r--   0        0        0     1612 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/file.py
--rw-r--r--   0        0        0     1115 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/file_create_params.py
--rw-r--r--   0        0        0     2202 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/file_list_params.py
--rw-r--r--   0        0        0      738 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/group.py
--rw-r--r--   0        0        0     1693 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_ach_transfer_return.py
--rw-r--r--   0        0        0     1109 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_ach_transfer_return_create_params.py
--rw-r--r--   0        0        0      440 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_ach_transfer_return_list_params.py
--rw-r--r--   0        0        0     2916 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_wire_drawdown_request.py
--rw-r--r--   0        0        0      444 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     1041 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit.py
--rw-r--r--   0        0        0      696 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit_create_params.py
--rw-r--r--   0        0        0      527 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit_list_params.py
--rw-r--r--   0        0        0      332 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit_update_params.py
--rw-r--r--   0        0        0      779 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/oauth_connection.py
--rw-r--r--   0        0        0      422 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/oauth_connection_list_params.py
--rw-r--r--   0        0        0    12078 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/pending_transaction.py
--rw-r--r--   0        0        0     1956 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/pending_transaction_list_params.py
--rw-r--r--   0        0        0      735 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/program.py
--rw-r--r--   0        0        0      406 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/program_list_params.py
--rw-r--r--   0        0        0     6113 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_decision.py
--rw-r--r--   0        0        0     2451 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_decision_action_params.py
--rw-r--r--   0        0        0     5096 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_payments_transfer.py
--rw-r--r--   0        0        0     1283 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_payments_transfer_create_params.py
--rw-r--r--   0        0        0     1664 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_payments_transfer_list_params.py
--rw-r--r--   0        0        0      895 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/routing_number.py
--rw-r--r--   0        0        0      522 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/routing_number_list_params.py
--rw-r--r--   0        0        0      155 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared/__init__.py
--rw-r--r--   0        0        0      489 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared/point_of_service_entry_mode.py
--rw-r--r--   0        0        0      155 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared_params/__init__.py
--rw-r--r--   0        0        0      525 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared_params/point_of_service_entry_mode.py
--rw-r--r--   0        0        0     2608 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/__init__.py
--rw-r--r--   0        0        0      338 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/account_statement_create_params.py
--rw-r--r--   0        0        0     1027 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     3303 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/ach_transfer_return_params.py
--rw-r--r--   0        0        0    51481 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/ach_transfer_simulation.py
--rw-r--r--   0        0        0    26885 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_authorization_simulation.py
--rw-r--r--   0        0        0      823 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_authorize_params.py
--rw-r--r--   0        0        0      443 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_dispute_action_params.py
--rw-r--r--   0        0        0      400 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_refund_create_params.py
--rw-r--r--   0        0        0      610 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_settlement_params.py
--rw-r--r--   0        0        0      425 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/check_transfer_return_params.py
--rw-r--r--   0        0        0      346 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
--rw-r--r--   0        0        0      953 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
--rw-r--r--   0        0        0      325 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/document_create_params.py
--rw-r--r--   0        0        0    51652 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
--rw-r--r--   0        0        0     2648 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      435 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/interest_payment_create_params.py
--rw-r--r--   0        0        0    37747 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/interest_payment_simulation_result.py
--rw-r--r--   0        0        0      299 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/program_create_params.py
--rw-r--r--   0        0        0     1362 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
--rw-r--r--   0        0        0     1020 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     2591 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
--rw-r--r--   0        0        0    37791 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/wire_transfer_simulation.py
--rw-r--r--   0        0        0    36238 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/transaction.py
--rw-r--r--   0        0        0     3293 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/transaction_list_params.py
--rw-r--r--   0        0        0     2239 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_drawdown_request.py
--rw-r--r--   0        0        0     1148 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      430 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     5343 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_transfer.py
--rw-r--r--   0        0        0     1367 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_transfer_create_params.py
--rw-r--r--   0        0        0     1588 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_transfer_list_params.py
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 increase-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-07-01 00:24:38.031246 increase-0.8.1/LICENSE
+-rw-r--r--   0        0        0     8418 2023-07-01 00:24:38.031246 increase-0.8.1/README.md
+-rw-r--r--   0        0        0     1881 2023-07-01 00:24:38.031246 increase-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-07-01 00:24:38.031246 increase-0.8.1/src/increase/__init__.py
+-rw-r--r--   0        0        0    46808 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_base_exceptions.py
+-rw-r--r--   0        0        0    26762 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_client.py
+-rw-r--r--   0        0        0    10875 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_models.py
+-rw-r--r--   0        0        0     4846 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_qs.py
+-rw-r--r--   0        0        0      890 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_resource.py
+-rw-r--r--   0        0        0     5884 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_streaming.py
+-rw-r--r--   0        0        0     4229 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_types.py
+-rw-r--r--   0        0        0     1277 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_utils/_utils.py
+-rw-r--r--   0        0        0      127 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/_version.py
+-rw-r--r--   0        0        0     1109 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/pagination.py
+-rw-r--r--   0        0        0        0 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/py.typed
+-rw-r--r--   0        0        0     4478 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/__init__.py
+-rw-r--r--   0        0        0    15065 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/account_numbers.py
+-rw-r--r--   0        0        0     7400 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/account_statements.py
+-rw-r--r--   0        0        0    18102 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/account_transfers.py
+-rw-r--r--   0        0        0    18476 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/accounts.py
+-rw-r--r--   0        0        0    15600 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/ach_prenotifications.py
+-rw-r--r--   0        0        0    26071 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/ach_transfers.py
+-rw-r--r--   0        0        0     4285 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/balance_lookups.py
+-rw-r--r--   0        0        0     8651 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/bookkeeping_accounts.py
+-rw-r--r--   0        0        0     4122 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/bookkeeping_entries.py
+-rw-r--r--   0        0        0     4842 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/bookkeeping_entry_sets.py
+-rw-r--r--   0        0        0    10707 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/card_disputes.py
+-rw-r--r--   0        0        0    10597 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/card_profiles.py
+-rw-r--r--   0        0        0    19120 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/cards.py
+-rw-r--r--   0        0        0    11757 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/check_deposits.py
+-rw-r--r--   0        0        0    23188 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/check_transfers.py
+-rw-r--r--   0        0        0     7771 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/declined_transactions.py
+-rw-r--r--   0        0        0     7353 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/digital_wallet_tokens.py
+-rw-r--r--   0        0        0     7177 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/documents.py
+-rw-r--r--   0        0        0      282 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/entities/__init__.py
+-rw-r--r--   0        0        0    14010 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/entities/entities.py
+-rw-r--r--   0        0        0     8071 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/entities/supplemental_documents.py
+-rw-r--r--   0        0        0    18799 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/event_subscriptions.py
+-rw-r--r--   0        0        0     7154 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/events.py
+-rw-r--r--   0        0        0    10548 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/exports.py
+-rw-r--r--   0        0        0    15315 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/external_accounts.py
+-rw-r--r--   0        0        0    12929 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/files.py
+-rw-r--r--   0        0        0     2040 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/groups.py
+-rw-r--r--   0        0        0    12035 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/inbound_ach_transfer_returns.py
+-rw-r--r--   0        0        0     7075 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0    14231 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/limits.py
+-rw-r--r--   0        0        0     6593 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/oauth_connections.py
+-rw-r--r--   0        0        0     8344 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/pending_transactions.py
+-rw-r--r--   0        0        0     6300 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/programs.py
+-rw-r--r--   0        0        0     8536 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/real_time_decisions.py
+-rw-r--r--   0        0        0    14968 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4951 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/routing_numbers.py
+-rw-r--r--   0        0        0     1989 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/__init__.py
+-rw-r--r--   0        0        0     4026 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/account_statements.py
+-rw-r--r--   0        0        0     4024 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/account_transfers.py
+-rw-r--r--   0        0        0    21871 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/ach_transfers.py
+-rw-r--r--   0        0        0     5051 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/card_disputes.py
+-rw-r--r--   0        0        0     3967 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/card_refunds.py
+-rw-r--r--   0        0        0    11463 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/cards.py
+-rw-r--r--   0        0        0    10125 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/check_deposits.py
+-rw-r--r--   0        0        0    11013 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/check_transfers.py
+-rw-r--r--   0        0        0     4085 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/digital_wallet_token_requests.py
+-rw-r--r--   0        0        0     3639 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/documents.py
+-rw-r--r--   0        0        0    13466 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0     4411 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/interest_payments.py
+-rw-r--r--   0        0        0     3919 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/programs.py
+-rw-r--r--   0        0        0    11257 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4588 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/simulations.py
+-rw-r--r--   0        0        0    12351 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/simulations/wire_transfers.py
+-rw-r--r--   0        0        0     7800 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/transactions.py
+-rw-r--r--   0        0        0    13338 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/wire_drawdown_requests.py
+-rw-r--r--   0        0        0    27583 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/resources/wire_transfers.py
+-rw-r--r--   0        0        0     8739 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/types/__init__.py
+-rw-r--r--   0        0        0     1666 2023-07-01 00:24:38.035246 increase-0.8.1/src/increase/types/account.py
+-rw-r--r--   0        0        0      747 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_create_params.py
+-rw-r--r--   0        0        0     1693 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_list_params.py
+-rw-r--r--   0        0        0     1026 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number.py
+-rw-r--r--   0        0        0      408 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number_create_params.py
+-rw-r--r--   0        0        0     1598 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number_list_params.py
+-rw-r--r--   0        0        0      435 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_number_update_params.py
+-rw-r--r--   0        0        0     1347 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_statement.py
+-rw-r--r--   0        0        0     1534 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_statement_list_params.py
+-rw-r--r--   0        0        0     2648 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_transfer.py
+-rw-r--r--   0        0        0      814 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_transfer_create_params.py
+-rw-r--r--   0        0        0     1494 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_transfer_list_params.py
+-rw-r--r--   0        0        0      271 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/account_update_params.py
+-rw-r--r--   0        0        0     2152 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_prenotification.py
+-rw-r--r--   0        0        0     1847 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_prenotification_create_params.py
+-rw-r--r--   0        0        0     1391 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_prenotification_list_params.py
+-rw-r--r--   0        0        0     8882 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_transfer.py
+-rw-r--r--   0        0        0     3388 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_transfer_create_params.py
+-rw-r--r--   0        0        0     1592 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/ach_transfer_list_params.py
+-rw-r--r--   0        0        0      585 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/balance_lookup_lookup_params.py
+-rw-r--r--   0        0        0      780 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/balance_lookup_lookup_response.py
+-rw-r--r--   0        0        0      823 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_account.py
+-rw-r--r--   0        0        0      626 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_account_create_params.py
+-rw-r--r--   0        0        0      428 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_account_list_params.py
+-rw-r--r--   0        0        0      698 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry.py
+-rw-r--r--   0        0        0      424 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry_list_params.py
+-rw-r--r--   0        0        0      895 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry_set.py
+-rw-r--r--   0        0        0     1133 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/bookkeeping_entry_set_create_params.py
+-rw-r--r--   0        0        0     2342 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card.py
+-rw-r--r--   0        0        0     1767 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_create_params.py
+-rw-r--r--   0        0        0      907 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_details.py
+-rw-r--r--   0        0        0     2011 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_dispute.py
+-rw-r--r--   0        0        0      483 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_dispute_create_params.py
+-rw-r--r--   0        0        0     1661 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_dispute_list_params.py
+-rw-r--r--   0        0        0     1451 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_list_params.py
+-rw-r--r--   0        0        0     2186 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_profile.py
+-rw-r--r--   0        0        0     1820 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_profile_create_params.py
+-rw-r--r--   0        0        0      716 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_profile_list_params.py
+-rw-r--r--   0        0        0     1611 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/card_update_params.py
+-rw-r--r--   0        0        0     4894 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_deposit.py
+-rw-r--r--   0        0        0      748 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_deposit_create_params.py
+-rw-r--r--   0        0        0     1477 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_deposit_list_params.py
+-rw-r--r--   0        0        0     6750 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_transfer.py
+-rw-r--r--   0        0        0     1939 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_transfer_create_params.py
+-rw-r--r--   0        0        0     1488 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/check_transfer_list_params.py
+-rw-r--r--   0        0        0    13068 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/declined_transaction.py
+-rw-r--r--   0        0        0     1598 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/declined_transaction_list_params.py
+-rw-r--r--   0        0        0      950 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/digital_wallet_token.py
+-rw-r--r--   0        0        0     1489 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/digital_wallet_token_list_params.py
+-rw-r--r--   0        0        0      883 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/document.py
+-rw-r--r--   0        0        0     1780 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/document_list_params.py
+-rw-r--r--   0        0        0      418 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/supplemental_document.py
+-rw-r--r--   0        0        0      343 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/supplemental_document_create_params.py
+-rw-r--r--   0        0        0      547 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entities/supplemental_document_list_params.py
+-rw-r--r--   0        0        0    11893 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entity.py
+-rw-r--r--   0        0        0    25685 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entity_create_params.py
+-rw-r--r--   0        0        0     1367 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/entity_list_params.py
+-rw-r--r--   0        0        0     2724 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event.py
+-rw-r--r--   0        0        0     4044 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_list_params.py
+-rw-r--r--   0        0        0     3124 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription.py
+-rw-r--r--   0        0        0     2526 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription_create_params.py
+-rw-r--r--   0        0        0      426 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription_list_params.py
+-rw-r--r--   0        0        0      360 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/event_subscription_update_params.py
+-rw-r--r--   0        0        0     1147 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/export.py
+-rw-r--r--   0        0        0     2946 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/export_create_params.py
+-rw-r--r--   0        0        0      404 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/export_list_params.py
+-rw-r--r--   0        0        0     1205 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account.py
+-rw-r--r--   0        0        0      706 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account_create_params.py
+-rw-r--r--   0        0        0      701 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account_list_params.py
+-rw-r--r--   0        0        0      420 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/external_account_update_params.py
+-rw-r--r--   0        0        0     1612 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/file.py
+-rw-r--r--   0        0        0     1115 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/file_create_params.py
+-rw-r--r--   0        0        0     2202 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/file_list_params.py
+-rw-r--r--   0        0        0      738 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/group.py
+-rw-r--r--   0        0        0     1693 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_ach_transfer_return.py
+-rw-r--r--   0        0        0     1109 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_ach_transfer_return_create_params.py
+-rw-r--r--   0        0        0      440 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_ach_transfer_return_list_params.py
+-rw-r--r--   0        0        0     2916 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_wire_drawdown_request.py
+-rw-r--r--   0        0        0      444 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/inbound_wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     1041 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit.py
+-rw-r--r--   0        0        0      696 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit_create_params.py
+-rw-r--r--   0        0        0      527 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit_list_params.py
+-rw-r--r--   0        0        0      332 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/limit_update_params.py
+-rw-r--r--   0        0        0      779 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/oauth_connection.py
+-rw-r--r--   0        0        0      422 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/oauth_connection_list_params.py
+-rw-r--r--   0        0        0    12078 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/pending_transaction.py
+-rw-r--r--   0        0        0     1956 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/pending_transaction_list_params.py
+-rw-r--r--   0        0        0      735 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/program.py
+-rw-r--r--   0        0        0      406 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/program_list_params.py
+-rw-r--r--   0        0        0     6113 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_decision.py
+-rw-r--r--   0        0        0     2451 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_decision_action_params.py
+-rw-r--r--   0        0        0     5096 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_payments_transfer.py
+-rw-r--r--   0        0        0     1283 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_payments_transfer_create_params.py
+-rw-r--r--   0        0        0     1664 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/real_time_payments_transfer_list_params.py
+-rw-r--r--   0        0        0      895 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/routing_number.py
+-rw-r--r--   0        0        0      522 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/routing_number_list_params.py
+-rw-r--r--   0        0        0      155 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0      155 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/shared_params/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0     2608 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/account_statement_create_params.py
+-rw-r--r--   0        0        0     1027 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     3303 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/ach_transfer_return_params.py
+-rw-r--r--   0        0        0    51481 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/ach_transfer_simulation.py
+-rw-r--r--   0        0        0    26885 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_authorization_simulation.py
+-rw-r--r--   0        0        0      823 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_authorize_params.py
+-rw-r--r--   0        0        0      443 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_dispute_action_params.py
+-rw-r--r--   0        0        0      400 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_refund_create_params.py
+-rw-r--r--   0        0        0      610 2023-07-01 00:24:38.039247 increase-0.8.1/src/increase/types/simulations/card_settlement_params.py
+-rw-r--r--   0        0        0      425 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/check_transfer_return_params.py
+-rw-r--r--   0        0        0      346 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/digital_wallet_token_request_create_params.py
+-rw-r--r--   0        0        0      953 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py
+-rw-r--r--   0        0        0      325 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/document_create_params.py
+-rw-r--r--   0        0        0    51652 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
+-rw-r--r--   0        0        0     2648 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      435 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/interest_payment_create_params.py
+-rw-r--r--   0        0        0    37747 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/interest_payment_simulation_result.py
+-rw-r--r--   0        0        0      299 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/program_create_params.py
+-rw-r--r--   0        0        0     1362 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
+-rw-r--r--   0        0        0     1020 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     2591 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    37791 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/simulations/wire_transfer_simulation.py
+-rw-r--r--   0        0        0    36238 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/transaction.py
+-rw-r--r--   0        0        0     3293 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2239 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_drawdown_request.py
+-rw-r--r--   0        0        0     1148 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      430 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     5343 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_transfer.py
+-rw-r--r--   0        0        0     1367 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_transfer_create_params.py
+-rw-r--r--   0        0        0     1588 2023-07-01 00:24:38.043247 increase-0.8.1/src/increase/types/wire_transfer_list_params.py
+-rw-r--r--   0        0        0     9328 1970-01-01 00:00:00.000000 increase-0.8.1/PKG-INFO
```

### Comparing `increase-0.8.0/LICENSE` & `increase-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/README.md` & `increase-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/pyproject.toml` & `increase-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "increase"
-version = "0.8.0"
+version = "0.8.1"
 description = "Client library for the increase API"
 readme = "README.md"
 authors = ["Increase <dev-feedback@increase.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/increase/increase-python"
 packages = [
   { include = "increase", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = ">= 0.23.0"
-pydantic = ">= 1.9.0"
+pydantic = "^1.9.0"
 typing-extensions = ">= 4.1.1"
 anyio = ">= 3.5.0"
 distro = ">= 1.7.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "1.1.297"
```

### Comparing `increase-0.8.0/src/increase/__init__.py` & `increase-0.8.1/src/increase/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_base_client.py` & `increase-0.8.1/src/increase/_base_client.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_base_exceptions.py` & `increase-0.8.1/src/increase/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_client.py` & `increase-0.8.1/src/increase/_client.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_exceptions.py` & `increase-0.8.1/src/increase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_models.py` & `increase-0.8.1/src/increase/_models.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_qs.py` & `increase-0.8.1/src/increase/_qs.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_resource.py` & `increase-0.8.1/src/increase/_resource.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_streaming.py` & `increase-0.8.1/src/increase/_streaming.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_types.py` & `increase-0.8.1/src/increase/_types.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_utils/__init__.py` & `increase-0.8.1/src/increase/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_utils/_transform.py` & `increase-0.8.1/src/increase/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/_utils/_utils.py` & `increase-0.8.1/src/increase/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/pagination.py` & `increase-0.8.1/src/increase/pagination.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/__init__.py` & `increase-0.8.1/src/increase/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/account_numbers.py` & `increase-0.8.1/src/increase/resources/account_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/account_statements.py` & `increase-0.8.1/src/increase/resources/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/account_transfers.py` & `increase-0.8.1/src/increase/resources/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/accounts.py` & `increase-0.8.1/src/increase/resources/accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/ach_prenotifications.py` & `increase-0.8.1/src/increase/resources/ach_prenotifications.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/ach_transfers.py` & `increase-0.8.1/src/increase/resources/ach_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/balance_lookups.py` & `increase-0.8.1/src/increase/resources/balance_lookups.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/bookkeeping_accounts.py` & `increase-0.8.1/src/increase/resources/bookkeeping_accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/bookkeeping_entries.py` & `increase-0.8.1/src/increase/resources/bookkeeping_entries.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/bookkeeping_entry_sets.py` & `increase-0.8.1/src/increase/resources/bookkeeping_entry_sets.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/card_disputes.py` & `increase-0.8.1/src/increase/resources/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/card_profiles.py` & `increase-0.8.1/src/increase/resources/card_profiles.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/cards.py` & `increase-0.8.1/src/increase/resources/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/check_deposits.py` & `increase-0.8.1/src/increase/resources/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/check_transfers.py` & `increase-0.8.1/src/increase/resources/check_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/declined_transactions.py` & `increase-0.8.1/src/increase/resources/declined_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/digital_wallet_tokens.py` & `increase-0.8.1/src/increase/resources/digital_wallet_tokens.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/documents.py` & `increase-0.8.1/src/increase/resources/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/entities/entities.py` & `increase-0.8.1/src/increase/resources/entities/entities.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/entities/supplemental_documents.py` & `increase-0.8.1/src/increase/resources/entities/supplemental_documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/event_subscriptions.py` & `increase-0.8.1/src/increase/resources/event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/events.py` & `increase-0.8.1/src/increase/resources/events.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/exports.py` & `increase-0.8.1/src/increase/resources/exports.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/external_accounts.py` & `increase-0.8.1/src/increase/resources/external_accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/files.py` & `increase-0.8.1/src/increase/resources/files.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/groups.py` & `increase-0.8.1/src/increase/resources/groups.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/inbound_ach_transfer_returns.py` & `increase-0.8.1/src/increase/resources/inbound_ach_transfer_returns.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/inbound_wire_drawdown_requests.py` & `increase-0.8.1/src/increase/resources/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/limits.py` & `increase-0.8.1/src/increase/resources/limits.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/oauth_connections.py` & `increase-0.8.1/src/increase/resources/oauth_connections.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/pending_transactions.py` & `increase-0.8.1/src/increase/resources/pending_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/programs.py` & `increase-0.8.1/src/increase/resources/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/real_time_decisions.py` & `increase-0.8.1/src/increase/resources/real_time_decisions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/real_time_payments_transfers.py` & `increase-0.8.1/src/increase/resources/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/routing_numbers.py` & `increase-0.8.1/src/increase/resources/routing_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/__init__.py` & `increase-0.8.1/src/increase/resources/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/account_statements.py` & `increase-0.8.1/src/increase/resources/simulations/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/account_transfers.py` & `increase-0.8.1/src/increase/resources/simulations/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/ach_transfers.py` & `increase-0.8.1/src/increase/resources/simulations/ach_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/card_disputes.py` & `increase-0.8.1/src/increase/resources/simulations/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/card_refunds.py` & `increase-0.8.1/src/increase/resources/simulations/card_refunds.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/cards.py` & `increase-0.8.1/src/increase/resources/simulations/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/check_deposits.py` & `increase-0.8.1/src/increase/resources/simulations/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/check_transfers.py` & `increase-0.8.1/src/increase/resources/simulations/check_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/digital_wallet_token_requests.py` & `increase-0.8.1/src/increase/resources/simulations/digital_wallet_token_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/documents.py` & `increase-0.8.1/src/increase/resources/simulations/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py` & `increase-0.8.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/interest_payments.py` & `increase-0.8.1/src/increase/resources/simulations/interest_payments.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/programs.py` & `increase-0.8.1/src/increase/resources/simulations/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/real_time_payments_transfers.py` & `increase-0.8.1/src/increase/resources/simulations/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/simulations.py` & `increase-0.8.1/src/increase/resources/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/simulations/wire_transfers.py` & `increase-0.8.1/src/increase/resources/simulations/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/transactions.py` & `increase-0.8.1/src/increase/resources/transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/wire_drawdown_requests.py` & `increase-0.8.1/src/increase/resources/wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/resources/wire_transfers.py` & `increase-0.8.1/src/increase/resources/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/__init__.py` & `increase-0.8.1/src/increase/types/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account.py` & `increase-0.8.1/src/increase/types/account.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_create_params.py` & `increase-0.8.1/src/increase/types/account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_list_params.py` & `increase-0.8.1/src/increase/types/account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_number.py` & `increase-0.8.1/src/increase/types/account_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_number_list_params.py` & `increase-0.8.1/src/increase/types/account_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_statement.py` & `increase-0.8.1/src/increase/types/account_statement.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_statement_list_params.py` & `increase-0.8.1/src/increase/types/account_statement_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_transfer.py` & `increase-0.8.1/src/increase/types/account_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_transfer_create_params.py` & `increase-0.8.1/src/increase/types/account_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/account_transfer_list_params.py` & `increase-0.8.1/src/increase/types/account_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/ach_prenotification.py` & `increase-0.8.1/src/increase/types/ach_prenotification.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/ach_prenotification_create_params.py` & `increase-0.8.1/src/increase/types/ach_prenotification_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/ach_prenotification_list_params.py` & `increase-0.8.1/src/increase/types/ach_prenotification_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/ach_transfer.py` & `increase-0.8.1/src/increase/types/ach_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/ach_transfer_create_params.py` & `increase-0.8.1/src/increase/types/ach_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/ach_transfer_list_params.py` & `increase-0.8.1/src/increase/types/ach_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/balance_lookup_lookup_params.py` & `increase-0.8.1/src/increase/types/balance_lookup_lookup_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/balance_lookup_lookup_response.py` & `increase-0.8.1/src/increase/types/balance_lookup_lookup_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/bookkeeping_account.py` & `increase-0.8.1/src/increase/types/bookkeeping_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/bookkeeping_account_create_params.py` & `increase-0.8.1/src/increase/types/bookkeeping_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/bookkeeping_entry.py` & `increase-0.8.1/src/increase/types/bookkeeping_entry.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/bookkeeping_entry_set.py` & `increase-0.8.1/src/increase/types/bookkeeping_entry_set.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/bookkeeping_entry_set_create_params.py` & `increase-0.8.1/src/increase/types/bookkeeping_entry_set_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card.py` & `increase-0.8.1/src/increase/types/card.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_create_params.py` & `increase-0.8.1/src/increase/types/card_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_details.py` & `increase-0.8.1/src/increase/types/card_details.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_dispute.py` & `increase-0.8.1/src/increase/types/card_dispute.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_dispute_list_params.py` & `increase-0.8.1/src/increase/types/card_dispute_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_list_params.py` & `increase-0.8.1/src/increase/types/card_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_profile.py` & `increase-0.8.1/src/increase/types/card_profile.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_profile_create_params.py` & `increase-0.8.1/src/increase/types/card_profile_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_profile_list_params.py` & `increase-0.8.1/src/increase/types/card_profile_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/card_update_params.py` & `increase-0.8.1/src/increase/types/card_update_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/check_deposit.py` & `increase-0.8.1/src/increase/types/check_deposit.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/check_deposit_create_params.py` & `increase-0.8.1/src/increase/types/check_deposit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/check_deposit_list_params.py` & `increase-0.8.1/src/increase/types/check_deposit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/check_transfer.py` & `increase-0.8.1/src/increase/types/check_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/check_transfer_create_params.py` & `increase-0.8.1/src/increase/types/check_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/check_transfer_list_params.py` & `increase-0.8.1/src/increase/types/check_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/declined_transaction.py` & `increase-0.8.1/src/increase/types/declined_transaction.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/declined_transaction_list_params.py` & `increase-0.8.1/src/increase/types/declined_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/digital_wallet_token.py` & `increase-0.8.1/src/increase/types/digital_wallet_token.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/digital_wallet_token_list_params.py` & `increase-0.8.1/src/increase/types/digital_wallet_token_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/document.py` & `increase-0.8.1/src/increase/types/document.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/document_list_params.py` & `increase-0.8.1/src/increase/types/document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/entities/supplemental_document.py` & `increase-0.8.1/src/increase/types/entities/supplemental_document.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/entities/supplemental_document_list_params.py` & `increase-0.8.1/src/increase/types/entities/supplemental_document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/entity.py` & `increase-0.8.1/src/increase/types/entity.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/entity_create_params.py` & `increase-0.8.1/src/increase/types/entity_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/entity_list_params.py` & `increase-0.8.1/src/increase/types/entity_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/event.py` & `increase-0.8.1/src/increase/types/event.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/event_list_params.py` & `increase-0.8.1/src/increase/types/event_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/event_subscription.py` & `increase-0.8.1/src/increase/types/event_subscription.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/event_subscription_create_params.py` & `increase-0.8.1/src/increase/types/event_subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/export.py` & `increase-0.8.1/src/increase/types/export.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/export_create_params.py` & `increase-0.8.1/src/increase/types/export_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/external_account.py` & `increase-0.8.1/src/increase/types/external_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/external_account_create_params.py` & `increase-0.8.1/src/increase/types/external_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/external_account_list_params.py` & `increase-0.8.1/src/increase/types/external_account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/file.py` & `increase-0.8.1/src/increase/types/file.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/file_create_params.py` & `increase-0.8.1/src/increase/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/file_list_params.py` & `increase-0.8.1/src/increase/types/file_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/group.py` & `increase-0.8.1/src/increase/types/group.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/inbound_ach_transfer_return.py` & `increase-0.8.1/src/increase/types/inbound_ach_transfer_return.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/inbound_ach_transfer_return_create_params.py` & `increase-0.8.1/src/increase/types/inbound_ach_transfer_return_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/inbound_wire_drawdown_request.py` & `increase-0.8.1/src/increase/types/inbound_wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/limit.py` & `increase-0.8.1/src/increase/types/limit.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/limit_create_params.py` & `increase-0.8.1/src/increase/types/limit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/limit_list_params.py` & `increase-0.8.1/src/increase/types/limit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/oauth_connection.py` & `increase-0.8.1/src/increase/types/oauth_connection.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/pending_transaction.py` & `increase-0.8.1/src/increase/types/pending_transaction.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/pending_transaction_list_params.py` & `increase-0.8.1/src/increase/types/pending_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/program.py` & `increase-0.8.1/src/increase/types/program.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/real_time_decision.py` & `increase-0.8.1/src/increase/types/real_time_decision.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/real_time_decision_action_params.py` & `increase-0.8.1/src/increase/types/real_time_decision_action_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/real_time_payments_transfer.py` & `increase-0.8.1/src/increase/types/real_time_payments_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/real_time_payments_transfer_create_params.py` & `increase-0.8.1/src/increase/types/real_time_payments_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/real_time_payments_transfer_list_params.py` & `increase-0.8.1/src/increase/types/real_time_payments_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/routing_number.py` & `increase-0.8.1/src/increase/types/routing_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/routing_number_list_params.py` & `increase-0.8.1/src/increase/types/routing_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/shared_params/point_of_service_entry_mode.py` & `increase-0.8.1/src/increase/types/shared_params/point_of_service_entry_mode.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/__init__.py` & `increase-0.8.1/src/increase/types/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py` & `increase-0.8.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/ach_transfer_return_params.py` & `increase-0.8.1/src/increase/types/simulations/ach_transfer_return_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/ach_transfer_simulation.py` & `increase-0.8.1/src/increase/types/simulations/ach_transfer_simulation.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/card_authorization_simulation.py` & `increase-0.8.1/src/increase/types/simulations/card_authorization_simulation.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/card_authorize_params.py` & `increase-0.8.1/src/increase/types/simulations/card_authorize_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/card_settlement_params.py` & `increase-0.8.1/src/increase/types/simulations/card_settlement_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py` & `increase-0.8.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py` & `increase-0.8.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py` & `increase-0.8.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/interest_payment_simulation_result.py` & `increase-0.8.1/src/increase/types/simulations/interest_payment_simulation_result.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py` & `increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py` & `increase-0.8.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py` & `increase-0.8.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/simulations/wire_transfer_simulation.py` & `increase-0.8.1/src/increase/types/simulations/wire_transfer_simulation.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/transaction.py` & `increase-0.8.1/src/increase/types/transaction.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/transaction_list_params.py` & `increase-0.8.1/src/increase/types/transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/wire_drawdown_request.py` & `increase-0.8.1/src/increase/types/wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/wire_drawdown_request_create_params.py` & `increase-0.8.1/src/increase/types/wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/wire_transfer.py` & `increase-0.8.1/src/increase/types/wire_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/wire_transfer_create_params.py` & `increase-0.8.1/src/increase/types/wire_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/src/increase/types/wire_transfer_list_params.py` & `increase-0.8.1/src/increase/types/wire_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.8.0/PKG-INFO` & `increase-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increase
-Version: 0.8.0
+Version: 0.8.1
 Summary: Client library for the increase API
 Home-page: https://github.com/increase/increase-python
 License: Apache-2.0
 Author: Increase
 Author-email: dev-feedback@increase.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.5.0)
 Requires-Dist: distro (>=1.7.0)
 Requires-Dist: httpx (>=0.23.0)
-Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.1.1)
 Project-URL: Repository, https://github.com/increase/increase-python
 Description-Content-Type: text/markdown
 
 # Increase Python API Library
 
 [![PyPI version](https://img.shields.io/pypi/v/increase.svg)](https://pypi.org/project/increase/)
```

