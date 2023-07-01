# Comparing `tmp/autobean-refactor-0.2.3.tar.gz` & `tmp/autobean-refactor-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobean-refactor-0.2.3.tar", last modified: Sat Apr  1 15:34:58 2023, max compression
+gzip compressed data, was "autobean-refactor-0.2.4.tar", last modified: Sat Jul  1 13:45:40 2023, max compression
```

## Comparing `autobean-refactor-0.2.3.tar` & `autobean-refactor-0.2.4.tar`

### file list

```diff
@@ -1,118 +1,119 @@
--rw-r--r--   0        0        0     1065 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/LICENSE
--rw-r--r--   0        0        0      822 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/__init__.py
--rw-r--r--   0        0        0     8351 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/beancount.lark
--rw-r--r--   0        0        0     1397 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/__init__.py
--rw-r--r--   0        0        0      124 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/account.py
--rw-r--r--   0        0        0       32 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/amount.py
--rw-r--r--   0        0        0       33 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/balance.py
--rw-r--r--   0        0        0     5963 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/base.py
--rw-r--r--   0        0        0     2837 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/block_comment.py
--rw-r--r--   0        0        0      377 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/bool.py
--rw-r--r--   0        0        0       31 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/close.py
--rw-r--r--   0        0        0       35 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/commodity.py
--rw-r--r--   0        0        0       41 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/compound_amount.py
--rw-r--r--   0        0        0     1047 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/cost.py
--rw-r--r--   0        0        0      336 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/cost_component.py
--rw-r--r--   0        0        0    11341 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/cost_spec.py
--rw-r--r--   0        0        0      126 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/currency.py
--rw-r--r--   0        0        0     4904 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/custom.py
--rw-r--r--   0        0        0      440 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/date.py
--rw-r--r--   0        0        0     1971 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/document.py
--rw-r--r--   0        0        0     1405 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/escaped_string.py
--rw-r--r--   0        0        0       31 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/event.py
--rw-r--r--   0        0        0      433 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/file.py
--rw-r--r--   0        0        0        0 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/__init__.py
--rw-r--r--   0        0        0     3340 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/amount.py
--rw-r--r--   0        0        0    14739 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/balance.py
--rw-r--r--   0        0        0    11601 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/close.py
--rw-r--r--   0        0        0    11671 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/commodity.py
--rw-r--r--   0        0        0     5720 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/compound_amount.py
--rw-r--r--   0        0        0     2083 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/cost_spec.py
--rw-r--r--   0        0        0    11583 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/custom.py
--rw-r--r--   0        0        0    12495 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/document.py
--rw-r--r--   0        0        0    12590 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/event.py
--rw-r--r--   0        0        0     3693 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/file.py
--rw-r--r--   0        0        0     5297 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/ignored_line.py
--rw-r--r--   0        0        0     8103 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/include.py
--rw-r--r--   0        0        0     9244 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/meta_item.py
--rw-r--r--   0        0        0    12434 2023-04-01 15:34:41.845196 autobean-refactor-0.2.3/autobean_refactor/models/generated/note.py
--rw-r--r--   0        0        0     2356 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/number_expr.py
--rw-r--r--   0        0        0     3764 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/number_paren_expr.py
--rw-r--r--   0        0        0     2975 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/number_unary_expr.py
--rw-r--r--   0        0        0    14123 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/open.py
--rw-r--r--   0        0        0     8823 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/option.py
--rw-r--r--   0        0        0    12676 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/pad.py
--rw-r--r--   0        0        0     9133 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/plugin.py
--rw-r--r--   0        0        0     7927 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/popmeta.py
--rw-r--r--   0        0        0     7893 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/poptag.py
--rw-r--r--   0        0        0    15859 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/posting.py
--rw-r--r--   0        0        0    12477 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/price.py
--rw-r--r--   0        0        0     9133 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/pushmeta.py
--rw-r--r--   0        0        0     7902 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/pushtag.py
--rw-r--r--   0        0        0    12618 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/query.py
--rw-r--r--   0        0        0     3105 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/tolerance.py
--rw-r--r--   0        0        0     4206 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/total_cost.py
--rw-r--r--   0        0        0     4613 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/total_price.py
--rw-r--r--   0        0        0    15355 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/transaction.py
--rw-r--r--   0        0        0     4017 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/unit_cost.py
--rw-r--r--   0        0        0     4599 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/generated/unit_price.py
--rw-r--r--   0        0        0      113 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/ignored.py
--rw-r--r--   0        0        0       38 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/ignored_line.py
--rw-r--r--   0        0        0       33 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/include.py
--rw-r--r--   0        0        0      368 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/inline_comment.py
--rw-r--r--   0        0        0      318 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/__init__.py
--rw-r--r--   0        0        0      892 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/base_property.py
--rw-r--r--   0        0        0     2190 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/base_token_models.py
--rw-r--r--   0        0        0     7991 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/fields.py
--rw-r--r--   0        0        0      441 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/indexes.py
--rw-r--r--   0        0        0     7841 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/interleaving_comments.py
--rw-r--r--   0        0        0      250 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/placeholder.py
--rw-r--r--   0        0        0    13029 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/properties.py
--rw-r--r--   0        0        0      435 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/registry.py
--rw-r--r--   0        0        0     2781 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/repeated.py
--rw-r--r--   0        0        0     3163 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/spacing_accessors.py
--rw-r--r--   0        0        0     3180 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/surrounding_comments.py
--rw-r--r--   0        0        0      825 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/token_models.py
--rw-r--r--   0        0        0    11519 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/internal/value_properties.py
--rw-r--r--   0        0        0      304 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/link.py
--rw-r--r--   0        0        0       35 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/meta_item.py
--rw-r--r--   0        0        0    10447 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/meta_item_internal.py
--rw-r--r--   0        0        0      312 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/meta_key.py
--rw-r--r--   0        0        0      603 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/meta_value.py
--rw-r--r--   0        0        0     2074 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/meta_value_internal.py
--rw-r--r--   0        0        0     1929 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/note.py
--rw-r--r--   0        0        0      135 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/null.py
--rw-r--r--   0        0        0      392 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number.py
--rw-r--r--   0        0        0     3841 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number_add_expr.py
--rw-r--r--   0        0        0      326 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number_atom_expr.py
--rw-r--r--   0        0        0    10072 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number_expr.py
--rw-r--r--   0        0        0     3848 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number_mul_expr.py
--rw-r--r--   0        0        0      315 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number_paren_expr.py
--rw-r--r--   0        0        0      469 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/number_unary_expr.py
--rw-r--r--   0        0        0       30 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/open.py
--rw-r--r--   0        0        0       32 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/option.py
--rw-r--r--   0        0        0       29 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/pad.py
--rw-r--r--   0        0        0       32 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/plugin.py
--rw-r--r--   0        0        0       33 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/popmeta.py
--rw-r--r--   0        0        0       32 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/poptag.py
--rw-r--r--   0        0        0       33 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/posting.py
--rw-r--r--   0        0        0      133 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/posting_flag.py
--rw-r--r--   0        0        0       31 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/price.py
--rw-r--r--   0        0        0      631 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/punctuation.py
--rw-r--r--   0        0        0       34 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/pushmeta.py
--rw-r--r--   0        0        0       33 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/pushtag.py
--rw-r--r--   0        0        0       31 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/query.py
--rw-r--r--   0        0        0      366 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/spacing.py
--rw-r--r--   0        0        0      302 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/tag.py
--rw-r--r--   0        0        0      581 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/tolerance.py
--rw-r--r--   0        0        0       37 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/total_price.py
--rw-r--r--   0        0        0     4897 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/transaction.py
--rw-r--r--   0        0        0      370 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/transaction_flag.py
--rw-r--r--   0        0        0       36 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/models/unit_price.py
--rw-r--r--   0        0        0    10000 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/parser.py
--rw-r--r--   0        0        0      256 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/printer.py
--rw-r--r--   0        0        0        0 2023-04-01 15:34:41.849196 autobean-refactor-0.2.3/autobean_refactor/py.typed
--rw-r--r--   0        0        0     6814 2023-04-01 15:34:41.853196 autobean-refactor-0.2.3/autobean_refactor/token_store.py
--rw-r--r--   0        0        0      760 2023-04-01 15:34:41.853196 autobean-refactor-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 autobean-refactor-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/LICENSE
+-rw-r--r--   0        0        0      865 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/__init__.py
+-rw-r--r--   0        0        0     8351 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/beancount.lark
+-rw-r--r--   0        0        0     2328 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/editor.py
+-rw-r--r--   0        0        0     1397 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/account.py
+-rw-r--r--   0        0        0       32 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/amount.py
+-rw-r--r--   0        0        0       33 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/balance.py
+-rw-r--r--   0        0        0     6114 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/base.py
+-rw-r--r--   0        0        0     2923 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/block_comment.py
+-rw-r--r--   0        0        0      438 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/bool.py
+-rw-r--r--   0        0        0       31 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/close.py
+-rw-r--r--   0        0        0       35 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/commodity.py
+-rw-r--r--   0        0        0       41 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/compound_amount.py
+-rw-r--r--   0        0        0     1047 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/cost.py
+-rw-r--r--   0        0        0      336 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/cost_component.py
+-rw-r--r--   0        0        0    11370 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/cost_spec.py
+-rw-r--r--   0        0        0      159 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/currency.py
+-rw-r--r--   0        0        0     4933 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/custom.py
+-rw-r--r--   0        0        0      476 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/date.py
+-rw-r--r--   0        0        0     2000 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/document.py
+-rw-r--r--   0        0        0     1438 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/escaped_string.py
+-rw-r--r--   0        0        0       31 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/event.py
+-rw-r--r--   0        0        0      433 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/file.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/__init__.py
+-rw-r--r--   0        0        0     3407 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/amount.py
+-rw-r--r--   0        0        0    14881 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/balance.py
+-rw-r--r--   0        0        0    11726 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/close.py
+-rw-r--r--   0        0        0    11801 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/commodity.py
+-rw-r--r--   0        0        0     5834 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/compound_amount.py
+-rw-r--r--   0        0        0     2147 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/cost_spec.py
+-rw-r--r--   0        0        0    11712 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/custom.py
+-rw-r--r--   0        0        0    12638 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/document.py
+-rw-r--r--   0        0        0    12716 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/event.py
+-rw-r--r--   0        0        0     3763 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/file.py
+-rw-r--r--   0        0        0     5480 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/ignored_line.py
+-rw-r--r--   0        0        0     8227 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/include.py
+-rw-r--r--   0        0        0     9314 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/meta_item.py
+-rw-r--r--   0        0        0    12562 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/note.py
+-rw-r--r--   0        0        0     2414 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/number_expr.py
+-rw-r--r--   0        0        0     3924 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/number_paren_expr.py
+-rw-r--r--   0        0        0     3055 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/number_unary_expr.py
+-rw-r--r--   0        0        0    14245 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/open.py
+-rw-r--r--   0        0        0     8947 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/option.py
+-rw-r--r--   0        0        0    12819 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/pad.py
+-rw-r--r--   0        0        0     9249 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/plugin.py
+-rw-r--r--   0        0        0     8045 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/popmeta.py
+-rw-r--r--   0        0        0     8008 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/poptag.py
+-rw-r--r--   0        0        0    15938 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/posting.py
+-rw-r--r--   0        0        0    12604 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/price.py
+-rw-r--r--   0        0        0     9260 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/pushmeta.py
+-rw-r--r--   0        0        0     8020 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/pushtag.py
+-rw-r--r--   0        0        0    12744 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/query.py
+-rw-r--r--   0        0        0     3203 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/tolerance.py
+-rw-r--r--   0        0        0     4346 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/total_cost.py
+-rw-r--r--   0        0        0     4720 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/total_price.py
+-rw-r--r--   0        0        0    15435 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/transaction.py
+-rw-r--r--   0        0        0     4152 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_cost.py
+-rw-r--r--   0        0        0     4703 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_price.py
+-rw-r--r--   0        0        0      162 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/ignored.py
+-rw-r--r--   0        0        0       38 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/ignored_line.py
+-rw-r--r--   0        0        0       33 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/include.py
+-rw-r--r--   0        0        0      423 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/inline_comment.py
+-rw-r--r--   0        0        0      318 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/base_property.py
+-rw-r--r--   0        0        0     2213 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/base_token_models.py
+-rw-r--r--   0        0        0     7991 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/fields.py
+-rw-r--r--   0        0        0      441 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/indexes.py
+-rw-r--r--   0        0        0     8020 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/interleaving_comments.py
+-rw-r--r--   0        0        0      250 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/placeholder.py
+-rw-r--r--   0        0        0    14206 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/properties.py
+-rw-r--r--   0        0        0      435 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/registry.py
+-rw-r--r--   0        0        0     2810 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/repeated.py
+-rw-r--r--   0        0        0     3159 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/spacing_accessors.py
+-rw-r--r--   0        0        0     3180 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/surrounding_comments.py
+-rw-r--r--   0        0        0      825 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/token_models.py
+-rw-r--r--   0        0        0    12620 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/value_properties.py
+-rw-r--r--   0        0        0      334 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/link.py
+-rw-r--r--   0        0        0       35 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_item.py
+-rw-r--r--   0        0        0    10447 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_item_internal.py
+-rw-r--r--   0        0        0      346 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_key.py
+-rw-r--r--   0        0        0      603 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_value.py
+-rw-r--r--   0        0        0     2074 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_value_internal.py
+-rw-r--r--   0        0        0     1958 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/note.py
+-rw-r--r--   0        0        0      170 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/null.py
+-rw-r--r--   0        0        0      425 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number.py
+-rw-r--r--   0        0        0     3870 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_add_expr.py
+-rw-r--r--   0        0        0      326 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_atom_expr.py
+-rw-r--r--   0        0        0     9384 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_expr.py
+-rw-r--r--   0        0        0     3877 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_mul_expr.py
+-rw-r--r--   0        0        0      315 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_paren_expr.py
+-rw-r--r--   0        0        0      469 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_unary_expr.py
+-rw-r--r--   0        0        0       30 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/open.py
+-rw-r--r--   0        0        0       32 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/option.py
+-rw-r--r--   0        0        0       29 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/pad.py
+-rw-r--r--   0        0        0       32 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/plugin.py
+-rw-r--r--   0        0        0       33 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/popmeta.py
+-rw-r--r--   0        0        0       32 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/poptag.py
+-rw-r--r--   0        0        0       33 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/posting.py
+-rw-r--r--   0        0        0      168 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/posting_flag.py
+-rw-r--r--   0        0        0       31 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/price.py
+-rw-r--r--   0        0        0      831 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/punctuation.py
+-rw-r--r--   0        0        0       34 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/pushmeta.py
+-rw-r--r--   0        0        0       33 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/pushtag.py
+-rw-r--r--   0        0        0       31 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/query.py
+-rw-r--r--   0        0        0      420 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/spacing.py
+-rw-r--r--   0        0        0      331 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/tag.py
+-rw-r--r--   0        0        0      592 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/tolerance.py
+-rw-r--r--   0        0        0       37 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/total_price.py
+-rw-r--r--   0        0        0     4926 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/transaction.py
+-rw-r--r--   0        0        0      409 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/transaction_flag.py
+-rw-r--r--   0        0        0       36 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/unit_price.py
+-rw-r--r--   0        0        0     9046 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/parser.py
+-rw-r--r--   0        0        0      256 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/printer.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/py.typed
+-rw-r--r--   0        0        0    13605 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/token_store.py
+-rw-r--r--   0        0        0      923 2023-07-01 13:45:22.522656 autobean-refactor-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 autobean-refactor-0.2.4/PKG-INFO
```

### Comparing `autobean-refactor-0.2.3/LICENSE` & `autobean-refactor-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/README.md` & `autobean-refactor-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,7 +2,9 @@
 [![build](https://github.com/SEIAROTg/autobean-refactor/actions/workflows/build.yml/badge.svg)](https://github.com/SEIAROTg/autobean-refactor/actions/workflows/build.yml)
 [![pypi](https://img.shields.io/pypi/v/autobean-refactor)](https://pypi.org/project/autobean-refactor/)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/8acbf50474596bc201ab/test_coverage)](https://codeclimate.com/github/SEIAROTg/autobean-refactor/test_coverage)
 [![Maintainability](https://api.codeclimate.com/v1/badges/8acbf50474596bc201ab/maintainability)](https://codeclimate.com/github/SEIAROTg/autobean-refactor/maintainability)
 [![license](https://img.shields.io/github/license/SEIAROTg/autobean-refactor.svg)](https://github.com/SEIAROTg/autobean-refactor)
 
 An ergonomic and lossless beancount manipulation library.
+
+https://autobean-refactor.readthedocs.io/
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/beancount.lark` & `autobean-refactor-0.2.4/autobean_refactor/beancount.lark`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/__init__.py` & `autobean-refactor-0.2.4/autobean_refactor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/base.py` & `autobean-refactor-0.2.4/autobean_refactor/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 import copy
-from typing import Any, ClassVar, Iterator, Optional, Protocol, Self, Type, TypeVar, cast
+from typing import Any, ClassVar, Iterator, Optional, Protocol, TypeVar, cast
+from typing_extensions import Self
 from autobean_refactor import token_store as token_store_lib
 
 _T = TypeVar('_T', bound='RawTokenModel')
 TokenStore = token_store_lib.TokenStore['RawTokenModel']
 
 
 # This could technically be replaced with map.__getitem__ but that didn't work well with mypy.
@@ -33,14 +34,15 @@
 
 class Formatter(Protocol):
     def __call__(self, model: 'RawModel', *, indent: int) -> None:
         pass
 
 
 class RawModel(abc.ABC):
+    """Base class for all models."""
     RULE: ClassVar[str]
 
     @property
     @abc.abstractmethod
     def token_store(self) -> Optional[TokenStore]:
         ...
 
@@ -94,24 +96,25 @@
 
     @abc.abstractmethod
     def auto_claim_comments(self) -> None:
         ...
 
 
 class RawTokenModel(token_store_lib.Token, RawModel):
+    """Base class for all token models."""
     def __init__(self, raw_text: str) -> None:
         super().__init__(raw_text)
 
     @classmethod
     def from_raw_text(cls, raw_text: str) -> Self:
         return cls(raw_text)
 
     @property
     def token_store(self) -> Optional[TokenStore]:
-        return self.store_handle.store if self.store_handle else None
+        return self.store_handle.block.store if self.store_handle else None
 
     @property
     def first_token(self) -> 'RawTokenModel':
         return self
 
     @property
     def last_token(self) -> 'RawTokenModel':
@@ -150,14 +153,15 @@
         pass
 
     def __hash__(self) -> int:
         return hash((type(self).RULE, self.raw_text))
 
 
 class RawTreeModel(RawModel):
+    """Base class for all tree models."""
     INLINE: ClassVar[bool] = False  # True iif this model contains no EOL
 
     def __init__(self, token_store: TokenStore) -> None:
         super().__init__()
         self._token_store = token_store
 
     @classmethod
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/block_comment.py` & `autobean-refactor-0.2.4/autobean_refactor/models/block_comment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Self, final
+from typing import final
+from typing_extensions import Self
 from . import base
 from .internal import registry as _registry
 from .internal import spacing_accessors as _spacing_accessors
 from .internal import value_properties as _value_properties
 
 
 def _splitlines(s: str) -> list[str]:
@@ -10,14 +11,15 @@
     if not lines or lines[-1].endswith('\n'):
         lines.append('')
     return lines
 
 
 @_registry.token_model
 class BlockComment(base.RawTokenModel, _value_properties.RWValueWithIndent[str], _spacing_accessors.SpacingAccessorsMixin):
+    """Comment that occupies one or more whole lines."""
     RULE = 'BLOCK_COMMENT'
 
     @final
     def __init__(self, raw_text: str, indent: str, value: str, *, claimed: bool = True) -> None:
         super().__init__(raw_text)
         self._value = value
         self._indent = indent
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/cost.py` & `autobean-refactor-0.2.4/autobean_refactor/models/cost.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/cost_spec.py` & `autobean-refactor-0.2.4/autobean_refactor/models/cost_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import datetime
 import decimal
-from typing import MutableSequence, Optional, Self, Type
+from typing import MutableSequence, Optional, Type
+from typing_extensions import Self
 from .generated import cost_spec
 from .cost_component import CostComponent
 from . import internal
 from .date import Date
 from .punctuation import Asterisk
 from .escaped_string import EscapedString
 from .currency import Currency
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/custom.py` & `autobean-refactor-0.2.4/autobean_refactor/models/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import decimal
-from typing import Iterable, Iterator, Mapping, Optional, Self, Union, get_args
+from typing import Iterable, Iterator, Mapping, Optional, Union, get_args
+from typing_extensions import Self
 
 from . import internal, meta_item_internal
 from .generated import custom
 from .generated.custom import CustomLabel, CustomRawValue
 from .block_comment import BlockComment
 from .escaped_string import EscapedString
 from .date import Date
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/document.py` & `autobean-refactor-0.2.4/autobean_refactor/models/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import itertools
-from typing import Iterable, Mapping, Optional, Self
+from typing import Iterable, Mapping, Optional
+from typing_extensions import Self
 from . import internal, meta_item_internal
 from .date import Date
 from .account import Account
 from .block_comment import BlockComment
 from .escaped_string import EscapedString
 from .inline_comment import InlineComment
 from .link import Link
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/escaped_string.py` & `autobean-refactor-0.2.4/autobean_refactor/models/escaped_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from . import internal
 
 
 @internal.token_model
 class EscapedString(internal.SingleValueRawTokenModel[str]):
+    """String (e.g. `"foo"`)."""
     RULE = 'ESCAPED_STRING'
     # See: https://github.com/beancount/beancount/blob/d841487ccdda04c159de86b1186e7c2ea997a3e2/beancount/parser/tokens.c#L102
     __ESCAPE_MAP = {
         '\n': 'n',
         '\t': 't',
         '\r': 'r',
         '\f': 'f',
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/amount.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/amount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import decimal
-from typing import Iterator, Self, final
+from typing import Iterator, final
+from typing_extensions import Self
 from .. import base, internal
 from ..currency import Currency
 from ..number_expr import NumberExpr
 from ..spacing import Whitespace
 
 
 @internal.tree_model
 class Amount(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Amount (e.g. `100.00 USD`)."""
     RULE = 'amount'
     INLINE = True
 
     _number = internal.required_field[NumberExpr]()
     _currency = internal.required_field[Currency]()
 
     raw_number = internal.required_node_property(_number)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/balance.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
 import decimal
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..currency import Currency
 from ..date import Date
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
@@ -16,20 +17,22 @@
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 from ..tolerance import Tolerance
 
 
 @internal.token_model
 class BalanceLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `balance`."""
     RULE = 'BALANCE'
     DEFAULT = 'balance'
 
 
 @internal.tree_model
 class Balance(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Balance entry (e.g. `2000-01-01 balance Assets:Foo 100.00 USD`)."""
     RULE = 'balance'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[BalanceLabel]()
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/close.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/close.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..date import Date
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class CloseLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `close`."""
     RULE = 'CLOSE'
     DEFAULT = 'close'
 
 
 @internal.tree_model
 class Close(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Close entry (e.g. `2000-01-01 close Assets:Foo`)."""
     RULE = 'close'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[CloseLabel]()
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/commodity.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/commodity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..block_comment import BlockComment
 from ..currency import Currency
 from ..date import Date
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class CommodityLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `commodity`."""
     RULE = 'COMMODITY'
     DEFAULT = 'commodity'
 
 
 @internal.tree_model
 class Commodity(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Commodity entry (e.g. `2000-01-01 commodity USD`)."""
     RULE = 'commodity'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[CommodityLabel]()
     _currency = internal.required_field[Currency]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/compound_amount.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/compound_amount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import decimal
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..currency import Currency
 from ..number_expr import NumberExpr
 from ..spacing import Whitespace
 
 
 @internal.token_model
 class Hash(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `#`."""
     RULE = 'HASH'
     DEFAULT = '#'
 
 
 @internal.tree_model
 class CompoundAmount(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Compound amount (e.g. `1.00 # 10.00 USD`)."""
     RULE = 'compound_amount'
     INLINE = True
 
     _number_per = internal.optional_right_field[NumberExpr](separators=(Whitespace.from_default(),))
     _hash = internal.required_field[Hash]()
     _number_total = internal.optional_left_field[NumberExpr](separators=(Whitespace.from_default(),))
     _currency = internal.required_field[Currency]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/cost_spec.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/cost_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Self, final
+from typing import Iterator, final
+from typing_extensions import Self
 from .. import base, internal
 from ..cost import TotalCost, UnitCost
 
 
 @internal.tree_model
 class CostSpec(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Unit cost or total cost."""
     RULE = 'cost_spec'
     INLINE = True
 
     _cost = internal.required_field[TotalCost | UnitCost]()
 
     raw_cost = internal.required_node_property[TotalCost | UnitCost](_cost)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/custom.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Optional, Self, final
+from typing import Iterable, Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..amount import Amount
 from ..block_comment import BlockComment
 from ..bool import Bool
 from ..date import Date
 from ..escaped_string import EscapedString
@@ -16,20 +17,22 @@
 from ..spacing import Newline, Whitespace
 
 CustomRawValue = Account | Amount | Bool | Date | EscapedString | NumberExpr
 
 
 @internal.token_model
 class CustomLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `custom`."""
     RULE = 'CUSTOM'
     DEFAULT = 'custom'
 
 
 @internal.tree_model
 class Custom(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Custom entry (e.g. `2000-01-01 custom "foo" "bar"`)."""
     RULE = 'custom'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[CustomLabel]()
     _type = internal.required_field[EscapedString]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/document.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Optional, Self, final
+from typing import Iterable, Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..date import Date
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..link import Link
@@ -13,20 +14,22 @@
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 from ..tag import Tag
 
 
 @internal.token_model
 class DocumentLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `document`."""
     RULE = 'DOCUMENT'
     DEFAULT = 'document'
 
 
 @internal.tree_model
 class Document(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Document entry (e.g. `2000-01-01 balance Assets:Foo "foo.pdf"`)."""
     RULE = 'document'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[DocumentLabel]()
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/event.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..block_comment import BlockComment
 from ..date import Date
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class EventLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `event`."""
     RULE = 'EVENT'
     DEFAULT = 'event'
 
 
 @internal.tree_model
 class Event(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Event entry (e.g. `2000-01-01 event "foo" "bar"`)."""
     RULE = 'event'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[EventLabel]()
     _type = internal.required_field[EscapedString]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/file.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Self, final, get_args
+from typing import Iterable, Iterator, final, get_args
+from typing_extensions import Self
 from .. import base, internal
 from ..balance import Balance
 from ..block_comment import BlockComment
 from ..close import Close
 from ..commodity import Commodity
 from ..custom import Custom
 from ..document import Document
@@ -27,14 +28,15 @@
 from ..transaction import Transaction
 
 Directive = Balance | Close | Commodity | Custom | Document | Event | IgnoredLine | Include | Note | Open | Option | Pad | Plugin | Popmeta | Poptag | Price | Pushmeta | Pushtag | Query | Transaction
 
 
 @internal.tree_model
 class File(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Contains everything in a file."""
     RULE = 'file'
 
     _directives = internal.repeated_field[Directive | BlockComment](separators=(Newline.from_default(), Newline.from_default()), separators_before=())
 
     raw_directives_with_comments = internal.repeated_node_with_interleaving_comments_property[Directive | BlockComment](_directives)
     raw_directives = internal.repeated_filtered_node_property[Directive](raw_directives_with_comments, get_args(Directive))
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/ignored_line.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/ignored_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..ignored import Ignored
 from ..punctuation import Eol
 from ..spacing import Newline
 
 
 @internal.tree_model
 class IgnoredLine(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Ignored line (e.g. `* title`).
+    
+    Lines starting with certain characters are ignored in beancount. This models captures those lines.
+    """
     RULE = 'ignored_line'
 
     _ignored = internal.required_field[Ignored]()
     _eol = internal.required_field[Eol]()
 
     @internal.custom_property
     def _leading_comment_pivot(self) -> base.RawTokenModel:
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/include.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/include.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class IncludeLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `include`."""
     RULE = 'INCLUDE'
     DEFAULT = 'include'
 
 
 @internal.tree_model
 class Include(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Include directive (e.g. `include "foo.bean"`)."""
     RULE = 'include'
 
     _label = internal.required_field[IncludeLabel]()
     _filename = internal.required_field[EscapedString]()
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/meta_item.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/meta_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_value_internal
 from ..block_comment import BlockComment
 from ..inline_comment import InlineComment
 from ..meta_key import MetaKey
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import Eol, Indent
 from ..spacing import Newline, Whitespace
 
 
 @internal.tree_model
 class MetaItem(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Meta item (e.g. `foo: "bar"`)."""
     RULE = 'meta_item'
 
     _indent = internal.required_field[Indent]()
     _key = internal.required_field[MetaKey]()
     _value = internal.optional_left_field[MetaRawValue](separators=(Whitespace.from_default(),))
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/note.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/note.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Optional, Self, final
+from typing import Iterable, Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..date import Date
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..link import Link
@@ -13,20 +14,22 @@
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 from ..tag import Tag
 
 
 @internal.token_model
 class NoteLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `note`."""
     RULE = 'NOTE'
     DEFAULT = 'note'
 
 
 @internal.tree_model
 class Note(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Note entry (e.g. `2000-01-01 note Assets:Foo "foo"`)."""
     RULE = 'note'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[NoteLabel]()
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/number_expr.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/number_expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Self, TYPE_CHECKING, final
+from typing import Iterator, TYPE_CHECKING, final
+from typing_extensions import Self
 from .. import base, internal
 if TYPE_CHECKING:
   from ..number_add_expr import NumberAddExpr
 
 
 @internal.tree_model
 class NumberExpr(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Number expression."""
     RULE = 'number_expr'
     INLINE = True
 
     _number_add_expr = internal.required_field['NumberAddExpr']()
 
     raw_number_add_expr = internal.required_node_property(_number_add_expr)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/number_paren_expr.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/number_paren_expr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Self, TYPE_CHECKING, final
+from typing import Iterator, TYPE_CHECKING, final
+from typing_extensions import Self
 from .. import base, internal
 if TYPE_CHECKING:
   from ..number_add_expr import NumberAddExpr
 
 
 @internal.token_model
 class LeftParen(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `(`."""
     RULE = 'LEFT_PAREN'
     DEFAULT = '('
 
 
 @internal.token_model
 class RightParen(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `)`."""
     RULE = 'RIGHT_PAREN'
     DEFAULT = ')'
 
 
 @internal.tree_model
 class NumberParenExpr(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Parentheses-enclosed number expression (e.g. `(42.00)`)."""
     RULE = 'number_paren_expr'
     INLINE = True
 
     _left_paren = internal.required_field[LeftParen]()
     _inner_expr = internal.required_field['NumberAddExpr']()
     _right_paren = internal.required_field[RightParen]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/number_unary_expr.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/number_unary_expr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Self, TYPE_CHECKING, final
+from typing import Iterator, TYPE_CHECKING, final
+from typing_extensions import Self
 from .. import base, internal
 if TYPE_CHECKING:
   from ..number_atom_expr import NumberAtomExpr
 
 
 @internal.token_model
 class UnaryOp(internal.SimpleRawTokenModel):
     RULE = 'UNARY_OP'
 
 
 @internal.tree_model
 class NumberUnaryExpr(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Unary number expression (e.g. `-42.00`)."""
     RULE = 'number_unary_expr'
     INLINE = True
 
     _unary_op = internal.required_field[UnaryOp]()
     _operand = internal.required_field['NumberAtomExpr']()
 
     raw_unary_op = internal.required_node_property(_unary_op)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/open.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/open.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..currency import Currency
 from ..date import Date
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
@@ -14,20 +15,22 @@
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import Comma, DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class OpenLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `open`."""
     RULE = 'OPEN'
     DEFAULT = 'open'
 
 
 @internal.tree_model
 class Open(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Open entry (e.g. `2000-01-01 open Assets:Foo`)."""
     RULE = 'open'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[OpenLabel]()
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/option.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class OptionLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `option`."""
     RULE = 'OPTION'
     DEFAULT = 'option'
 
 
 @internal.tree_model
 class Option(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Option directive (e.g. `option "title" "foo"`)."""
     RULE = 'option'
 
     _label = internal.required_field[OptionLabel]()
     _key = internal.required_field[EscapedString]()
     _value = internal.required_field[EscapedString]()
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/pad.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/pad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..date import Date
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class PadLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `pad`."""
     RULE = 'PAD'
     DEFAULT = 'pad'
 
 
 @internal.tree_model
 class Pad(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Pad entry (e.g. `2000-01-01 pad Assets:Foo Equity:Opening-Balances`)."""
     RULE = 'pad'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[PadLabel]()
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/plugin.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class PluginLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `plugin`."""
     RULE = 'PLUGIN'
     DEFAULT = 'plugin'
 
 
 @internal.tree_model
 class Plugin(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Plugin directive (e.g. `plugin "foo"`)."""
     RULE = 'plugin'
 
     _label = internal.required_field[PluginLabel]()
     _name = internal.required_field[EscapedString]()
     _config = internal.optional_left_field[EscapedString](separators=(Whitespace.from_default(),))
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/popmeta.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/popmeta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..inline_comment import InlineComment
 from ..meta_key import MetaKey
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class PopmetaLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `popmeta`."""
     RULE = 'POPMETA'
     DEFAULT = 'popmeta'
 
 
 @internal.tree_model
 class Popmeta(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Popmeta directive (e.g. `popmeta foo:`)."""
     RULE = 'popmeta'
 
     _label = internal.required_field[PopmetaLabel]()
     _key = internal.required_field[MetaKey]()
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/poptag.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/poptag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..inline_comment import InlineComment
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 from ..tag import Tag
 
 
 @internal.token_model
 class PoptagLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `poptag`."""
     RULE = 'POPTAG'
     DEFAULT = 'poptag'
 
 
 @internal.tree_model
 class Poptag(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Poptag directive (e.g. `poptag #foo`)."""
     RULE = 'poptag'
 
     _label = internal.required_field[PoptagLabel]()
     _tag = internal.required_field[Tag]()
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/posting.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/posting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import decimal
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..account import Account
 from ..block_comment import BlockComment
 from ..cost_spec import CostSpec
 from ..currency import Currency
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
@@ -19,14 +20,15 @@
 from ..unit_price import UnitPrice
 
 PriceAnnotation = TotalPrice | UnitPrice
 
 
 @internal.tree_model
 class Posting(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Posting (e.g. `Assets:Foo -10.00 USD`)."""
     RULE = 'posting'
 
     indent_by = internal.data_field[str]()
 
     _indent = internal.required_field[Indent]()
     _flag = internal.optional_right_field[PostingFlag](separators=(Whitespace.from_default(),))
     _account = internal.required_field[Account]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/price.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/price.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..amount import Amount
 from ..block_comment import BlockComment
 from ..currency import Currency
 from ..date import Date
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class PriceLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `price`."""
     RULE = 'PRICE'
     DEFAULT = 'price'
 
 
 @internal.tree_model
 class Price(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Price entry (e.g. `2000-01-01 price GBP 2.00 USD`)."""
     RULE = 'price'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[PriceLabel]()
     _currency = internal.required_field[Currency]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/pushmeta.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/pushmeta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_value_internal
 from ..block_comment import BlockComment
 from ..inline_comment import InlineComment
 from ..meta_key import MetaKey
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class PushmetaLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `pushmeta`."""
     RULE = 'PUSHMETA'
     DEFAULT = 'pushmeta'
 
 
 @internal.tree_model
 class Pushmeta(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Pushmeta directive (e.g. `pushmeta foo: "bar"`)."""
     RULE = 'pushmeta'
 
     _label = internal.required_field[PushmetaLabel]()
     _key = internal.required_field[MetaKey]()
     _value = internal.optional_left_field[MetaRawValue](separators=(Whitespace.from_default(),))
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/pushtag.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/pushtag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..block_comment import BlockComment
 from ..inline_comment import InlineComment
 from ..punctuation import Eol
 from ..spacing import Newline, Whitespace
 from ..tag import Tag
 
 
 @internal.token_model
 class PushtagLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `pushtag`."""
     RULE = 'PUSHTAG'
     DEFAULT = 'pushtag'
 
 
 @internal.tree_model
 class Pushtag(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Pushtag directive (e.g. `pushtag #foo`)."""
     RULE = 'pushtag'
 
     _label = internal.required_field[PushtagLabel]()
     _tag = internal.required_field[Tag]()
     _inline_comment = internal.optional_left_field[InlineComment](separators=(Whitespace.from_default(),))
     _eol = internal.required_field[Eol]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/query.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import datetime
-from typing import Iterable, Iterator, Mapping, Optional, Self, final
+from typing import Iterable, Iterator, Mapping, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..block_comment import BlockComment
 from ..date import Date
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..meta_item import MetaItem
 from ..meta_value import MetaRawValue, MetaValue
 from ..punctuation import DedentMark, Eol
 from ..spacing import Newline, Whitespace
 
 
 @internal.token_model
 class QueryLabel(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `query`."""
     RULE = 'QUERY'
     DEFAULT = 'query'
 
 
 @internal.tree_model
 class Query(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Query entry (e.g. `2000-01-01 query "foo" "..."`)."""
     RULE = 'query'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _label = internal.required_field[QueryLabel]()
     _name = internal.required_field[EscapedString]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/tolerance.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/tolerance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import decimal
-from typing import Iterator, Self, final
+from typing import Iterator, final
+from typing_extensions import Self
 from .. import base, internal
 from ..number_expr import NumberExpr
 from ..spacing import Whitespace
 
 
 @internal.token_model
 class Tilde(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `~`."""
     RULE = 'TILDE'
     DEFAULT = '~'
 
 
 @internal.tree_model
 class Tolerance(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Tolerance (e.g. `~ 0.01`)."""
     RULE = 'tolerance'
     INLINE = True
 
     _tilde = internal.required_field[Tilde]()
     _number = internal.required_field[NumberExpr]()
 
     raw_number = internal.required_node_property(_number)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/total_cost.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/total_cost.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Self, final
+from typing import Iterable, Iterator, final
+from typing_extensions import Self
 from .. import base, internal
 from ..cost_component import CostComponent
 from ..punctuation import Comma
 from ..spacing import Whitespace
 
 
 @internal.token_model
 class DblLeftBrace(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `{{`."""
     RULE = 'DBL_LEFT_BRACE'
     DEFAULT = '{{'
 
 
 @internal.token_model
 class DblRightBrace(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `}}`."""
     RULE = 'DBL_RIGHT_BRACE'
     DEFAULT = '}}'
 
 
 @internal.tree_model
 class TotalCost(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Total cost (e.g. `{{10.00 USD}}`)."""
     RULE = 'total_cost'
     INLINE = True
 
     _dbl_left_brace = internal.required_field[DblLeftBrace]()
     _components = internal.repeated_field[CostComponent](separators=(Comma.from_default(), Whitespace.from_default()), separators_before=())
     _dbl_right_brace = internal.required_field[DblRightBrace]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/total_price.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/total_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import decimal
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..currency import Currency
 from ..number_expr import NumberExpr
 from ..spacing import Whitespace
 
 
 @internal.token_model
 class AtAt(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `@@`."""
     RULE = 'ATAT'
     DEFAULT = '@@'
 
 
 @internal.tree_model
 class TotalPrice(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Total price (e.g. `@@ 10.00 USD`)."""
     RULE = 'total_price'
     INLINE = True
 
     _label = internal.required_field[AtAt]()
     _number = internal.optional_left_field[NumberExpr](separators=(Whitespace.from_default(),))
     _currency = internal.optional_left_field[Currency](separators=(Whitespace.from_default(),))
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/transaction.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Optional, Self, final
+from typing import Iterable, Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal, meta_item_internal
 from ..block_comment import BlockComment
 from ..date import Date
 from ..escaped_string import EscapedString
 from ..inline_comment import InlineComment
 from ..link import Link
 from ..meta_item import MetaItem
@@ -14,14 +15,15 @@
 from ..spacing import Newline, Whitespace
 from ..tag import Tag
 from ..transaction_flag import TransactionFlag
 
 
 @internal.tree_model
 class Transaction(internal.SurroundingCommentsMixin, base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Transaction entry (e.g. `2000-01-01 *`)."""
     RULE = 'transaction'
 
     indent_by = internal.data_field[str]()
 
     _date = internal.required_field[Date]()
     _flag = internal.required_field[TransactionFlag]()
     _string0 = internal.optional_left_field[EscapedString](separators=(Whitespace.from_default(),))
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/unit_cost.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_cost.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
-from typing import Iterable, Iterator, Self, final
+from typing import Iterable, Iterator, final
+from typing_extensions import Self
 from .. import base, internal
 from ..cost_component import CostComponent
 from ..punctuation import Comma
 from ..spacing import Whitespace
 
 
 @internal.token_model
 class LeftBrace(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `{`."""
     RULE = 'LEFT_BRACE'
     DEFAULT = '{'
 
 
 @internal.token_model
 class RightBrace(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `}`."""
     RULE = 'RIGHT_BRACE'
     DEFAULT = '}'
 
 
 @internal.tree_model
 class UnitCost(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Unit cost (e.g. `{10.00 USD}`)."""
     RULE = 'unit_cost'
     INLINE = True
 
     _left_brace = internal.required_field[LeftBrace]()
     _components = internal.repeated_field[CostComponent](separators=(Comma.from_default(), Whitespace.from_default()), separators_before=())
     _right_brace = internal.required_field[RightBrace]()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/generated/unit_price.py` & `autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # DO NOT EDIT
 # This file is automatically generated by autobean_refactor.modelgen.
 
 import decimal
-from typing import Iterator, Optional, Self, final
+from typing import Iterator, Optional, final
+from typing_extensions import Self
 from .. import base, internal
 from ..currency import Currency
 from ..number_expr import NumberExpr
 from ..spacing import Whitespace
 
 
 @internal.token_model
 class At(internal.SimpleDefaultRawTokenModel):
+    """Contains literal `@`."""
     RULE = 'AT'
     DEFAULT = '@'
 
 
 @internal.tree_model
 class UnitPrice(base.RawTreeModel, internal.SpacingAccessorsMixin):
+    """Unit price (e.g. `@ 10.00 USD`)."""
     RULE = 'unit_price'
     INLINE = True
 
     _label = internal.required_field[At]()
     _number = internal.optional_left_field[NumberExpr](separators=(Whitespace.from_default(),))
     _currency = internal.optional_left_field[Currency](separators=(Whitespace.from_default(),))
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/base_property.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/base_property.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
-from typing import Generic, Optional, Self, Type, TypeVar, overload
+from typing import Generic, Optional, Type, TypeVar, overload
+from typing_extensions import Self
 from .. import base
 
 _U = TypeVar('_U', bound=base.RawTreeModel)
 _V = TypeVar('_V')
 _V_cov = TypeVar('_V_cov', covariant=True)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/base_token_models.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/base_token_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import abc
-from typing import Self, Type, TypeVar, final
+from typing import TypeVar, final
+from typing_extensions import Self
 from .. import base
 from .value_properties import RWValue
 
 _V = TypeVar('_V')
 
 
 class SimpleRawTokenModel(base.RawTokenModel):
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/fields.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/fields.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/interleaving_comments.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/interleaving_comments.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,19 @@
         token_store.splice(others + ignored, first, last)
 
 
 class _CommentClaimer(Generic[_M]):
     def __init__(
             self,
             repeated: repeated.Repeated[_M | BlockComment],
+            notify: Callable[[], None],
             model: base.RawTreeModel,
             comments: Optional[Iterable[BlockComment]]):
         self._repeated = repeated
+        self._notify = notify
         self._model = model
         self._comments_to_claim = (
             {id(comment) for comment in comments} if comments is not None else _Universe())
 
     def _find_inner(self) -> Iterator[_M | BlockComment]:
         token_store = self._repeated.token_store
         # inclusive
@@ -133,14 +135,15 @@
         items = list(itertools.chain(comments_before, items_inner, comments_after))
         comments = []
         for item in items:
             if isinstance(item, BlockComment):
                 comments.append(item)
                 item.claimed = True
         self._repeated.items[:] = items
+        self._notify()
         return comments
 
 
 class RepeatedNodeWithInterleavingCommentsWrapper(properties.RepeatedNodeWrapper[_M | BlockComment]):
 
     def __init__(
             self,
@@ -151,15 +154,19 @@
         super().__init__(repeated, field)
         self._model = model
 
     def claim_interleaving_comments(
             self,
             comments: Optional[Iterable[BlockComment]] = None,
     ) -> tuple[BlockComment, ...]:
-        return tuple(_CommentClaimer(self._repeated, self._model, comments).claim())
+        return tuple(_CommentClaimer(
+            self._repeated,
+            self._notify,
+            self._model,
+            comments).claim())
 
     def unclaim_interleaving_comments(
             self,
             comments: Optional[Iterable[BlockComment]] = None,
     ) -> tuple[BlockComment, ...]:
         unclaimed_comments = []
         comment_set = (
@@ -175,14 +182,15 @@
             if comment_set is not None:
                 comment_set.discard(id(item))
             item.claimed = False
             unclaimed_comments.append(item)
         if comment_set:
             raise ValueError(f'{len(comment_set)} comment(s) not found.')
         self._repeated.items[:] = items
+        self._notify()
         return tuple(unclaimed_comments)
 
     def auto_claim_comments(self) -> None:
         super().auto_claim_comments()
         self.claim_interleaving_comments()
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/properties.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import abc
 import copy
 import functools
 import itertools
 from typing import Any, Callable, Collection, Iterable, MutableSequence, Optional, Type, TypeVar, overload
 from .base_property import base_ro_property, base_rw_property
 from .fields import required_field, optional_field, repeated_field
 from .repeated import Repeated
@@ -61,18 +62,30 @@
             pivot = self._pivot_property.__get__(instance)
             self._inner_field._remove_node(instance.token_store, pivot, current)
         elif current is not None and value is not None:
             replace_node(current, value)
         self._inner_field.__set__(instance, value)
 
 
+class RepeatedNodeWrapperUpdateHandler(abc.ABC):
+
+    @abc.abstractmethod
+    def handle(self) -> None:
+        ...
+
+    @abc.abstractmethod
+    def handle_splice(self, l: int, r: int, value: list[Any]) -> None:
+        ...
+
+
 class RepeatedNodeWrapper(MutableSequence[_M]):
     def __init__(self, repeated: Repeated[_M], field: repeated_field) -> None:
         self._repeated = repeated
         self._field = field
+        self._update_handlers = list[RepeatedNodeWrapperUpdateHandler]()
 
     @property
     def repeated(self) -> Repeated[_M]:
         return self._repeated
 
     @functools.cached_property
     def _separators(self) -> tuple[base.RawTokenModel, ...]:
@@ -80,14 +93,25 @@
 
     @functools.cached_property
     def _separators_before(self) -> tuple[base.RawTokenModel, ...]:
         return (
             self._field.separators_before
             if self._field.separators_before is not None else self._field.separators)
 
+    def register_update_handler(self, handler: RepeatedNodeWrapperUpdateHandler) -> None:
+        self._update_handlers.append(handler)
+
+    def _notify(self) -> None:
+        for handler in self._update_handlers:
+            handler.handle()
+
+    def _notify_splice(self, l: int, r: int, values: list[_M]) -> None:
+        for handler in self._update_handlers:
+            handler.handle_splice(l, r, values)
+
     def __len__(self) -> int:
         return len(self._repeated.items)
 
     @overload
     def __getitem__(self, index: int) -> _M:
         ...
     @overload
@@ -162,65 +186,76 @@
     def __setitem__(self, index: int | slice, value: _M | Iterable[_M]) -> None:
         if isinstance(index, int):
             assert not isinstance(value, Iterable)
             item = self._repeated.items[index]
             self._repeated.token_store.splice(value.detach(), item.first_token, item.last_token)
             value.reattach(self._repeated.token_store)
             self._repeated.items[index] = value
+            self._notify_splice(index, index + 1, [value])
             return
         assert isinstance(value, Iterable)
         values = list(value)
         r = indexes.range_from_index(index, len(self._repeated.items))
         separators_before_last = (
             self._repeated.token_store.get_prev(self._repeated.items[0].first_token)
             if self._repeated.items else None)
         if r.step == 1:
             self._del_tokens(r.start, r.stop)
             self._insert_tokens(
                 r.start, values, len(self._repeated.items) - len(r), separators_before_last)
             self._repeated.items[indexes.slice_from_range(r)] = values
             for value in values:
                 value.reattach(self._repeated.token_store)
+            self._notify_splice(r.start, r.stop, values)
         else:
             if len(r) != len(values):
                 raise ValueError(f'attempt to assign sequence of size {len(values)} to extended slice of size {len(r)}')
             for i, value in zip(r, values):
                 self._del_tokens(i, i + 1)
                 self._insert_tokens(i, [value], len(self._repeated.items) - 1, separators_before_last)
                 value.reattach(self._repeated.token_store)
                 self._repeated.items[i] = value
+            self._notify()
 
     def insert(self, index: int, value: _M) -> None:
         index = min(index, len(self._repeated.items))
         self._insert_tokens(index, [value])
         value.reattach(self._repeated.token_store)
         self._repeated.items.insert(index, value)
+        self._notify_splice(index, index, [value])
 
     def append(self, value: _M) -> None:
-        self._insert_tokens(len(self._repeated.items), [value])
+        index = len(self._repeated.items)
+        self._insert_tokens(index, [value])
         value.reattach(self._repeated.token_store)
         self._repeated.items.append(value)
+        self._notify_splice(index, index, [value])
 
     def clear(self) -> None:
-        self._del_tokens(0, len(self._repeated.items))
+        index = len(self._repeated.items)
+        self._del_tokens(0, index)
         self._repeated.items.clear()
+        self._notify()
 
     def extend(self, values: Iterable[_M]) -> None:
         values = list(values)
-        self._insert_tokens(len(self._repeated.items), values)
+        index = len(self._repeated.items)
+        self._insert_tokens(index, values)
         self._repeated.items.extend(values)
+        self._notify_splice(index, index, values)
 
     def pop(self, index: int = -1) -> _M:
         value = self._repeated.items[index]
         tokens = value.tokens
         r = indexes.range_from_index(index, len(self._repeated.items))
         self._del_tokens(r.start, r.stop)
         token_store = base.TokenStore.from_tokens(tokens)
         value.reattach(token_store)
         self._repeated.items.pop(index)
+        self._notify_splice(r.start, r.stop, [])
         return value
 
     def __deepcopy__(self, memo: dict[int, Any]) -> 'RepeatedNodeWrapper':
         repeated = copy.deepcopy(self._repeated, memo)
         return RepeatedNodeWrapper(repeated, self._field)
 
     def drop_many(self, indexes: Iterable[int]) -> None:
@@ -230,14 +265,15 @@
             list(r) for _, r in itertools.groupby(indexes, key=lambda i: i + next(count))
         )
         for r in ranges:
             self._del_tokens(r[-1], r[0] + 1)
         self._repeated.items[:] = (
             item for i, item in enumerate(self._repeated.items) if i not in indexes
         )
+        self._notify()
 
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, Collection) and
             all(a == b for a, b in itertools.zip_longest(self, other)))
 
     def auto_claim_comments(self) -> None:
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/repeated.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/repeated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
-from typing import Generic, Iterable, Iterator, Optional, Self, TypeVar
+from typing import Generic, Iterable, Iterator, Optional, TypeVar
+from typing_extensions import Self
 from .. import base
 from .placeholder import Placeholder
 
 _M = TypeVar('_M', bound=base.RawModel)
 
 class Repeated(base.RawTreeModel, Generic[_M]):
     def __init__(
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/spacing_accessors.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/spacing_accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,23 @@
         token = succ(token)
     return tokens
 
 
 class SpacingAccessorsMixin(base.RawModel):
 
     @property
-    def raw_spacing_before(self) -> tuple[base.RawTokenModel, ...]:
+    def raw_spacing_before(self) -> Sequence[base.RawTokenModel]:
         if self.token_store is None:
             return ()
         return tuple(reversed(_find_spacing(
                 self.token_store.get_prev(self.first_token),
                 self.token_store.get_prev)))
 
     @raw_spacing_before.setter
-    def raw_spacing_before(self, tokens: tuple[base.RawTokenModel, ...]) -> None:
+    def raw_spacing_before(self, tokens: Sequence[base.RawTokenModel]) -> None:
         if self.token_store is None:
             raise ValueError('Cannot set spacing without a token store.')
         current_tokens = self.raw_spacing_before
         if current_tokens:
             self.token_store.splice(tokens, current_tokens[0], current_tokens[-1])
         else:
             self.token_store.insert_before(self.first_token, tokens)
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/surrounding_comments.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/surrounding_comments.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/token_models.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/token_models.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/internal/value_properties.py` & `autobean-refactor-0.2.4/autobean_refactor/models/internal/value_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import bisect
 import datetime
 import decimal
 import abc
 import itertools
-from typing import Any, Callable, Collection, Generic, Iterable, Iterator, MutableSequence, Optional, Self, Type, TypeGuard, TypeVar, cast, overload
+from typing import Any, Callable, Collection, Generic, Iterable, Iterator, MutableSequence, Optional, Type, TypeGuard, TypeVar, cast, overload
+from typing_extensions import Self
 from .. import base
 from . import indexes, base_property, properties
 
 
 _V = TypeVar('_V')
 _M = TypeVar('_M', bound=base.RawModel)
 _M2 = TypeVar('_M2', bound=base.RawModel)
@@ -43,211 +45,235 @@
 
     @classmethod
     @abc.abstractmethod
     def from_value(cls, value: _V, *, indent: str = '') -> Self:
         raise NotImplementedError()
 
 
-class required_value_property(Generic[_V, _U]):
+class required_value_property(properties.base_rw_property[_V, _U]):
     def __init__(self, inner_property: base_property.base_ro_property[RWValue[_V], _U]):
         self._inner_property = inner_property
 
-    def __get__(self, instance: _U, owner: Optional[Type[_U]] = None) -> _V:
-        return self._inner_property.__get__(instance, owner).value
+    def _get(self, instance: _U) -> _V:
+        return self._inner_property.__get__(instance).value
     
     def __set__(self, instance: _U, value: _V) -> None:
         self._inner_property.__get__(instance).value = value
 
 
-class optional_string_property(Generic[_SV]):
+class optional_string_property(properties.base_rw_property[Optional[str], _U]):
     def __init__(self, inner_property: base_property.base_rw_property[Optional[_SV], _U], inner_type: Type[_SV]):
         self._inner_property = inner_property
         self._inner_type = inner_type
 
-    def __get__(self, instance: _U, owner: Optional[Type[_U]] = None) -> Optional[str]:
-        s = self._inner_property.__get__(instance, owner)
+    def _get(self, instance: _U) -> Optional[str]:
+        s = self._inner_property.__get__(instance)
         return s.value if s is not None else None
     
     def __set__(self, instance: _U, value: Optional[str]) -> None:
         current = self._inner_property.__get__(instance)
         if current is not None and value is not None:
             current.value = value
         else:
             s = self._inner_type.from_value(value) if value is not None else None
             self._inner_property.__set__(instance, s)
 
 
-class optional_indented_string_property(Generic[_ISV]):
+class optional_indented_string_property(properties.base_rw_property[Optional[str], _U]):
     def __init__(
             self,
             inner_property: base_property.base_rw_property[Optional[_ISV], _U],
             inner_type: Type[_ISV],
             indent_property: base_property.base_ro_property[_SV, base.RawTreeModel]):
         self._inner_property = inner_property
         self._inner_type = inner_type
         self._indent_property = indent_property
 
-    def __get__(self, instance: _U, owner: Optional[Type[_U]] = None) -> Optional[str]:
-        s = self._inner_property.__get__(instance, owner)
+    def _get(self, instance: _U) -> Optional[str]:
+        s = self._inner_property.__get__(instance)
         return s.value if s is not None else None
     
     def __set__(self, instance: _U, value: Optional[str]) -> None:
         current = self._inner_property.__get__(instance)
         if current is not None and value is not None:
             current.value = value
         else:
             indent = self._indent_property.__get__(instance).value
             s = self._inner_type.from_value(value, indent=indent) if value is not None else None
             self._inner_property.__set__(instance, s)
 
 
-class optional_decimal_property(Generic[_U]):
+class optional_decimal_property(properties.base_rw_property[Optional[decimal.Decimal], _U]):
     def __init__(self, inner_property: base_property.base_rw_property[Optional[_DV], _U], inner_type: Type[_DV]):
         self._inner_property = inner_property
         self._inner_type = inner_type
 
-    def __get__(self, instance: _U, owner: Optional[Type[_U]] = None) -> Optional[decimal.Decimal]:
-        s = self._inner_property.__get__(instance, owner)
+    def _get(self, instance: _U) -> Optional[decimal.Decimal]:
+        s = self._inner_property.__get__(instance)
         return s.value if s is not None else None
     
     def __set__(self, instance: _U, value: Optional[decimal.Decimal]) -> None:
         current = self._inner_property.__get__(instance)
         if current is not None and value is not None:
             current.value = value
         else:
             s = self._inner_type.from_value(value) if value is not None else None
             self._inner_property.__set__(instance, s)
 
 
-class optional_date_property(Generic[_U]):
+class optional_date_property(properties.base_rw_property[Optional[datetime.date], _U]):
     def __init__(self, inner_property: base_property.base_rw_property[Optional[_DateV], _U], inner_type: Type[_DateV]):
         self._inner_property = inner_property
         self._inner_type = inner_type
 
-    def __get__(self, instance: _U, owner: Optional[Type[_U]] = None) -> Optional[datetime.date]:
-        s = self._inner_property.__get__(instance, owner)
+    def _get(self, instance: _U) -> Optional[datetime.date]:
+        s = self._inner_property.__get__(instance)
         return s.value if s is not None else None
     
     def __set__(self, instance: _U, value: Optional[datetime.date]) -> None:
         current = self._inner_property.__get__(instance)
         if current is not None and value is not None:
             current.value = value
         else:
             s = self._inner_type.from_value(value) if value is not None else None
             self._inner_property.__set__(instance, s)
 
 
+class _RepeatedValueWrapperUpdateHandler(properties.RepeatedNodeWrapperUpdateHandler):
+    def __init__(
+            self,
+            raw_wrapper: properties.RepeatedNodeWrapper[Any],
+            raw_type: Type[_M] | tuple[Type[_M], ...],
+            raw_indexes: list[int],
+    ) -> None:
+        self._raw_wrapper = raw_wrapper
+        self._raw_type = raw_type
+        self._raw_indexes = raw_indexes
+
+    def handle(self) -> None:
+        self._raw_indexes[:] = [
+            i for i, model in enumerate(self._raw_wrapper)
+            if isinstance(model, self._raw_type)]
+
+    def handle_splice(self, l: int, r: int, values: list[Any]) -> None:
+        filtered_indexes = [
+            l + i
+            for i, value in enumerate(values)
+            if isinstance(value, self._raw_type)
+        ]
+        ll = bisect.bisect_left(self._raw_indexes, l)
+        rr = bisect.bisect_left(self._raw_indexes, r)
+        diff = len(values) - r + l
+        self._raw_indexes[ll:rr] = filtered_indexes
+        if diff:
+            for i in range(ll + len(filtered_indexes), len(self._raw_indexes)):
+                self._raw_indexes[i] += diff
+
+
 class RepeatedValueWrapper(MutableSequence[_V], Generic[_M, _V]):
     def __init__(
             self,
             raw_wrapper: properties.RepeatedNodeWrapper[_M | Any],
             raw_type: Type[_M] | tuple[Type[_M], ...],
             from_raw_type: Callable[[_M], _V],
             to_raw_type: Callable[[_V], _M],
             update_raw: Callable[[_M, _V], bool],
     ):
         self._raw_wrapper = raw_wrapper
         self._raw_type = raw_type
         self._from_raw_type = from_raw_type
         self._to_raw_type = to_raw_type
         self._update_raw = update_raw
+        self._raw_indexes = [
+            i for i, item in enumerate(self._raw_wrapper) if isinstance(item, self._raw_type)]
+        self._raw_wrapper.register_update_handler(
+            _RepeatedValueWrapperUpdateHandler(raw_wrapper, raw_type, self._raw_indexes))
 
     def _check_type(self, v: Any) -> TypeGuard[_M]:
         return isinstance(v, self._raw_type)
 
     def __len__(self) -> int:
-        return sum(1 for _ in self)
+        return len(self._raw_indexes)
 
     def __iter__(self) -> Iterator[_V]:
         return (
-            self._from_raw_type(item) for item in self._raw_wrapper if self._check_type(item))
-
-    def _filtered_items(self) -> list[tuple[int, _M]]:
-        return [(i, item) for i, item in enumerate(self._raw_wrapper) if isinstance(item, self._raw_type)]
+            self._from_raw_type(self._raw_wrapper[i]) for i in self._raw_indexes)
 
     @overload
     def __getitem__(self, index: int) -> _V:
         ...
     @overload
     def __getitem__(self, index: slice) -> list[_V]:
         ...
     def __getitem__(self, index: int | slice) -> _V | list[_V]:
-        items = self._filtered_items()
         if isinstance(index, int):
-            return self._from_raw_type(items[index][1])
-        return [self._from_raw_type(item[1]) for item in items[index]]
+            return self._from_raw_type(self._raw_wrapper[self._raw_indexes[index]])
+        return [self._from_raw_type(self._raw_wrapper[i]) for i in self._raw_indexes[index]]
 
     def __delitem__(self, index: int | slice) -> None:
-        items = self._filtered_items()
-        r = indexes.range_from_index(index, len(items))
-        self._raw_wrapper.drop_many(items[i][0] for i in r)
+        r = indexes.range_from_index(index, len(self._raw_indexes))
+        self._raw_wrapper.drop_many(self._raw_indexes[i] for i in r)
 
     @overload
     def __setitem__(self, index: int, value: _V) -> None:
         ...
     @overload
     def __setitem__(self, index: slice, value: Iterable[_V]) -> None:
         ...
     def __setitem__(self, index: int | slice, value: _V | Iterable[_V]) -> None:
-        items = self._filtered_items()
         if isinstance(index, int):
             values = [cast(_V, value)]
         else:
             assert isinstance(value, Iterable)
             values = list(value)
-        r = indexes.range_from_index(index, len(items))
-        items_to_update = items[indexes.slice_from_range(r)]
+        r = indexes.range_from_index(index, len(self._raw_indexes))
+        raw_indexes_to_update = self._raw_indexes[indexes.slice_from_range(r)]
         # We don't allow assignment with distinct length here because the underlying models may not be consecutive.
-        if len(items_to_update) != len(values):
-            raise ValueError(f'attempt to assign sequence of size {len(values)} to extended slice of size {len(items_to_update)}')
-        for item, value in zip(items_to_update, values):
-            if not self._update_raw(item[1], value):
-                self._raw_wrapper[item[0]] = self._to_raw_type(value)
+        if len(raw_indexes_to_update) != len(values):
+            raise ValueError(
+                f'attempt to assign sequence of size {len(values)} to extended slice of size '
+                f'{len(raw_indexes_to_update)}')
+        for raw_index, value in zip(raw_indexes_to_update, values):
+            if not self._update_raw(self._raw_wrapper[raw_index], value):
+                self._raw_wrapper[raw_index] = self._to_raw_type(value)
 
     def insert(self, index: int, value: _V) -> None:
-        items = self._filtered_items()
-        if index >= len(items):
-            underlying_index = len(self._raw_wrapper)
-        elif index < -len(items):
-            underlying_index = 0
+        if index >= len(self._raw_indexes):
+            raw_index = len(self._raw_wrapper)
+        elif index < -len(self._raw_indexes):
+            raw_index = 0
         else:
-            underlying_index = items[index][0]
-        self._raw_wrapper.insert(underlying_index, self._to_raw_type(value))
+            raw_index = self._raw_indexes[index]
+        self._raw_wrapper.insert(raw_index, self._to_raw_type(value))
 
     def append(self, value: _V) -> None:
         self._raw_wrapper.append(self._to_raw_type(value))
 
     def clear(self) -> None:
-        items = self._filtered_items()
-        self._raw_wrapper.drop_many(item[0] for item in items)
+        self._raw_wrapper.drop_many(self._raw_indexes)
 
     def extend(self, values: Iterable[_V]) -> None:
         self._raw_wrapper.extend(self._to_raw_type(value) for value in values)
 
     def pop(self, index: int = -1) -> _V:
-        items = self._filtered_items()
-        if not items:
-            raise IndexError('pop from empty list')
-        if not -len(items) <= index < len(items):
+        if not -len(self._raw_indexes) <= index < len(self._raw_indexes):
             raise IndexError('pop index out of range')
-        underlying_index = items[index][0]
-        self._raw_wrapper.pop(underlying_index)
-        return self._from_raw_type(items[index][1])
+        raw_index = self._raw_indexes[index]
+        return self._from_raw_type(self._raw_wrapper.pop(raw_index))
 
     def remove(self, value: _V) -> None:
-        items = self._filtered_items()
-        for i, item in items:
-            if self._from_raw_type(item) == value:
-                self._raw_wrapper.pop(i)
+        for raw_index in self._raw_indexes:
+            if self._from_raw_type(self._raw_wrapper[raw_index]) == value:
+                self._raw_wrapper.pop(raw_index)
                 return
         raise ValueError(f'{value!r} not found in list')
 
     def discard(self, value: _V) -> None:
-        items = self._filtered_items()
-        self._raw_wrapper.drop_many(item[0] for item in items if self._from_raw_type(item[1]) == value)
+        self._raw_wrapper.drop_many(
+            i for i in self._raw_indexes if self._from_raw_type(self._raw_wrapper[i]) == value)
 
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, Collection) and
             all(a == b for a, b in itertools.zip_longest(self, other)))
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/meta_item_internal.py` & `autobean-refactor-0.2.4/autobean_refactor/models/meta_item_internal.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/meta_value.py` & `autobean-refactor-0.2.4/autobean_refactor/models/meta_value.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/meta_value_internal.py` & `autobean-refactor-0.2.4/autobean_refactor/models/meta_value_internal.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/note.py` & `autobean-refactor-0.2.4/autobean_refactor/models/note.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import itertools
-from typing import Iterable, Mapping, Optional, Self
+from typing import Iterable, Mapping, Optional
+from typing_extensions import Self
 from . import internal, meta_item_internal
 from .date import Date
 from .account import Account
 from .block_comment import BlockComment
 from .escaped_string import EscapedString
 from .inline_comment import InlineComment
 from .link import Link
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/number_add_expr.py` & `autobean-refactor-0.2.4/autobean_refactor/models/number_add_expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import decimal
-from typing import Any, Iterator, Optional, Self, cast, final, TYPE_CHECKING
+from typing import Any, Iterator, Optional, cast, final, TYPE_CHECKING
+from typing_extensions import Self
 from . import base
 from . import internal
 from .spacing import Whitespace
 if TYPE_CHECKING:
     from .number_mul_expr import NumberMulExpr
 else:
     NumberMulExpr = Any
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/number_expr.py` & `autobean-refactor-0.2.4/autobean_refactor/models/number_expr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,24 @@
 import copy
 import decimal
-from typing import Any, Callable, Literal, NoReturn, Union, overload
+from typing import Callable, Literal, NoReturn, Union, overload
 from . import base
 from . import internal
 from . import number
 from .number_add_expr import NumberAddExpr, AddOp
 from .number_mul_expr import NumberMulExpr, MulOp
 from .number_atom_expr import NumberAtomExpr
 from .number_unary_expr import NumberUnaryExpr
 from .number_paren_expr import NumberParenExpr
 from .spacing import Whitespace
 from .generated.number_paren_expr import LeftParen, RightParen
 from .generated.number_unary_expr import UnaryOp
 from .generated import number_expr
 
 _AnyNumber = Union[int, decimal.Decimal, 'NumberExpr']
-_OP_INFO = {
-    '__iadd__': ('+=', False),
-    '__isub__': ('-=', False),
-    '__imul__': ('*=', False),
-    '__itruediv__': ('/=', False),
-    '__add__': ('+', False),
-    '__sub__': ('-', False),
-    '__mul__': ('*', False),
-    '__truediv__': ('/', False),
-    '__radd__': ('+', True),
-    '__rsub__': ('-', True),
-    '__rmul__': ('*', True),
-    '__rtruediv__': ('/', True),
-}
 
 
 def _add_expr_from_value(value: decimal.Decimal) -> NumberAddExpr:
     number_token = number.Number.from_value(abs(value))
     token_store = base.TokenStore.from_tokens([number_token])
     atom_expr: NumberAtomExpr
     if value < 0:
@@ -51,24 +37,15 @@
     def wrapped_op(self: 'NumberExpr', other: object) -> 'NumberExpr':
         if isinstance(other, int):
             other = NumberExpr.from_value(decimal.Decimal(other))
         elif isinstance(other, decimal.Decimal):
             other = NumberExpr.from_value(other)
         if isinstance(other, NumberExpr):
             return op(self, other)
-        op_name, rev = _OP_INFO[op.__name__]
-        lhs: Any
-        rhs: Any
-        if rev:
-            lhs, rhs = other, self
-        else:
-            lhs, rhs = self, other
-        raise TypeError(
-            f'unsupported operand type(s) for {op_name}: '
-            f'{type(lhs).__name__!r} and {type(rhs).__name__!r}.')
+        return NotImplemented
     return wrapped_op
 
 
 def _wrap_paren(add_expr: NumberAddExpr) -> NumberParenExpr:
     left_paren = LeftParen.from_default()
     right_paren = RightParen.from_default()
     add_expr.token_store.insert_before(add_expr.first_token, [left_paren])
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/number_mul_expr.py` & `autobean-refactor-0.2.4/autobean_refactor/models/number_mul_expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import decimal
-from typing import Any, Iterator, Optional, Self, cast, final, TYPE_CHECKING
+from typing import Any, Iterator, Optional, cast, final, TYPE_CHECKING
+from typing_extensions import Self
 from . import base
 from . import internal
 from .spacing import Whitespace
 if TYPE_CHECKING:
     from .number_atom_expr import NumberAtomExpr
 else:
     NumberAtomExpr = Any
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/tolerance.py` & `autobean-refactor-0.2.4/autobean_refactor/models/tolerance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import decimal
-from typing import Self
+from typing_extensions import Self
 from . import internal
 from .generated import tolerance
 from .generated.tolerance import Tilde
 
 
 @internal.tree_model
 class Tolerance(tolerance.Tolerance, internal.RWValue[decimal.Decimal]):
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/models/transaction.py` & `autobean-refactor-0.2.4/autobean_refactor/models/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import itertools
-from typing import Iterable, Mapping, Optional, Self
+from typing import Iterable, Mapping, Optional
+from typing_extensions import Self
 from . import base, internal, meta_item_internal
 from .block_comment import BlockComment
 from .date import Date
 from .escaped_string import EscapedString
 from .inline_comment import InlineComment
 from .link import Link
 from .meta_value import MetaRawValue, MetaValue
```

### Comparing `autobean-refactor-0.2.3/autobean_refactor/parser.py` & `autobean-refactor-0.2.4/autobean_refactor/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import collections
 import copy
 import enum
-import glob
-import os.path
 import pathlib
 import re
 from typing import Iterable, Iterator, Optional, Type, TypeVar
 import lark
 from lark import exceptions
 from lark import lexer
 from lark import load_grammar
@@ -81,26 +78,14 @@
 
 
 class _Floating(enum.Enum):
     LEFT = enum.auto()
     RIGHT = enum.auto()
 
 
-def _get_include_paths(path: str, file: models.File) -> Iterable[str]:
-    for directive in file.raw_directives:
-        if not isinstance(directive, models.Include):
-            continue
-        matches = glob.glob(os.path.join(os.path.dirname(path), directive.filename), recursive=True)
-        if not matches:
-            lineno = directive.token_store.get_position(directive.first_token).line
-            raise ValueError(f'No files match {directive.filename!r} ({path}:{lineno})')
-        for match in matches:
-            yield os.path.normpath(match)
-
-
 class Parser:
     _lark: lark.Lark
     _token_models: dict[str, Type[models.RawTokenModel]]
     _tree_models: dict[str, Type[models.RawTreeModel]]
 
     def __init__(self) -> None:
         start = list(models.TREE_MODELS.keys())
@@ -124,35 +109,22 @@
                 lark.Token('$END', '', 0, 1, 1), {target.RULE})
         if tokens[0].type != target.RULE:
             raise exceptions.UnexpectedToken(tokens[0], {target.RULE})
         if len(tokens) > 1:
             raise exceptions.UnexpectedToken(tokens[1], {'$END'})
         return target.from_raw_text(tokens[0].value)
 
-    def parse(self, text: str, target: Type[_U]) -> _U:
+    def parse(self, text: str, target: Type[_U], *, auto_claim_comments: bool = True) -> _U:
         if target.INLINE:
-            return self._parse(text, target, self._lark_inline)
+            model = self._parse(text, target, self._lark_inline)
         else:
-            return self._parse(text, target, self._lark)
-
-    def parse_file_recursive(self, path: str) -> dict[str, models.File]:
-        files = {}
-        queue = collections.deque([path])
-
-        while queue:
-            path = queue.popleft()
-            if path in files:
-                continue
-            with open(path) as f:
-                text = f.read()
-            file = self.parse(text, models.File)
-            files[path] = file
-            queue.extend(_get_include_paths(path, file))
-        
-        return files
+            model = self._parse(text, target, self._lark)
+        if auto_claim_comments:
+            model.auto_claim_comments()
+        return model
 
     def _parse(self, text: str, target: Type[_U], lark_instance: lark.Lark) -> _U:
         parser = lark_instance.parse_interactive(text=text, start=target.RULE)
         tokens = []
         for token in parser.lexer_thread.lex(parser.parser_state):
             tokens.append(token)
             if token.type not in _IGNORED_TOKENS or token.type in parser.choices():
```

### Comparing `autobean-refactor-0.2.3/pyproject.toml` & `autobean-refactor-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "autobean-refactor"
-version = "0.2.3"
+version = "0.2.4"
 description = "An ergonomic and losess beancount manipulation library"
 authors = [
     { name = "SEIAROTg", email = "seiarotg@gmail.com" },
 ]
 dependencies = [
     "lark>=1.1.5",
+    "typing-extensions>=4.4.0",
 ]
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
@@ -34,8 +35,12 @@
 dev = [
     "mypy>=0.991",
     "pytest>=7.2.0",
     "pytest-cov>=4.0.0",
     "pytest-benchmark>=4.0.0",
     "mako>=1.2.4",
     "stringcase>=1.2.0",
+    "sphinx-book-theme>=0.3.3,<1.0.0",
+    "jupyter-book>=0.14.0,<0.15.0",
+    "docutils>=0.18.1",
+    "types-docutils>=0.20.0.1",
 ]
```

### Comparing `autobean-refactor-0.2.3/PKG-INFO` & `autobean-refactor-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: autobean-refactor
-Version: 0.2.3
+Version: 0.2.4
 Summary: An ergonomic and losess beancount manipulation library
 License: MIT
 Author-email: SEIAROTg <seiarotg@gmail.com>
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # autobean-refactor
 [![build](https://github.com/SEIAROTg/autobean-refactor/actions/workflows/build.yml/badge.svg)](https://github.com/SEIAROTg/autobean-refactor/actions/workflows/build.yml)
 [![pypi](https://img.shields.io/pypi/v/autobean-refactor)](https://pypi.org/project/autobean-refactor/)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/8acbf50474596bc201ab/test_coverage)](https://codeclimate.com/github/SEIAROTg/autobean-refactor/test_coverage)
 [![Maintainability](https://api.codeclimate.com/v1/badges/8acbf50474596bc201ab/maintainability)](https://codeclimate.com/github/SEIAROTg/autobean-refactor/maintainability)
 [![license](https://img.shields.io/github/license/SEIAROTg/autobean-refactor.svg)](https://github.com/SEIAROTg/autobean-refactor)
 
 An ergonomic and lossless beancount manipulation library.
 
+https://autobean-refactor.readthedocs.io/
+
```

